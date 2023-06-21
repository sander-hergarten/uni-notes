# Definition
Die LOOP und WHILE sprachen sind entwickelt worden um die [[Entscheidbarkeit von Sprachen]] zu determinieren

## LOOP
Das Programm enthaelt:
* Variablen $x_0,...,x_n$ 
* Konstanten $0,1$
* Symbole $:=,\ +,\ ;$
* Schluesselwoerter $\text{LOOP DO ENDLOOP}$

Die eingabe ist in den Variablen enthalten und die restlichen variablen werden mit 0 initialisiert. Das Ergebniss ist am Ende in der Variablen $x_0$

Die syntax kann induktiv erzeugt werden. Ein loop programm kann definiert werden durch:
$$x_i\ :=\ x_j+c,\ c\in \{0,\ 1\}$$
deshalb koennen auch zwei loop Programme zusammengefuehrt werden:
$$P_1;P_2$$
um ein neues zu bilden. Zusaetzlich ist auch moeglich:
$$\text{LOOP } x_i \text{ DO } P \text{ ENDLOOP}$$
Dies heist $P$ wird $x_i$-mal ausgefuehrt. Aendert sich der Wert von $x_i$ bei ausfuehrung der Schleife ist das egal.

**Formal:**
Ein Loop Programm $P$ mit $k$ Variablen berechnet eine k-stellige Funktion der Form: 
$$[P]:\mathbb{N}^k\rightarrow\mathbb{N}^k$$
Nun ist eine Zuweisung:
![[Pasted image 20211210125852.png]]
und eine Hintereinanderausfuehrung:
![[Pasted image 20211210125913.png]]
ein Loop:
![[Pasted image 20211210130009.png]]
If statement:
![[Pasted image 20211210131249.png]]

## WHILE
Die While Programme sind sehr Aehnlich zu den Loop programmen. Das Programm enthaelt:
* Variablen $x_0,...,x_n$ 
* Konstanten $0,1$
* Symbole $:=,\ +,\ ;,\ \neq$
* Schluesselwoerter $\text{WHILE DO ENDWHILE}$

While Konstrukt:
$$\text{WHILE } x_i \neq 0 \text{ DO }P\text{ ENDWHILE}$$

Nun ist die entsprechende Funktion nur eine Partielle Funktion dar sie an manchen Stellen undefiniert ist wenn eine Endlosschleife erzeugt wird. Trozdem kann man definieren:

Ein WHILE Programm $P$ mit $k$ Variablen berechnet eine k-stellige Funktion der Form: 
$$[P]:\mathbb{N}^k\rightarrow\mathbb{N}^k$$
 ![[Pasted image 20211210132131.png]]
 
 ----
 While Programm sind Turing volstaendig waehrend Loop Programme es nicht sind.