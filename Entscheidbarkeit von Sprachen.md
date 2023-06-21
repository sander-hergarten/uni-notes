 # Punkte

- Eine Sprache ist unentscheidbar wenn ihr Komplement unentscheidbar ist und andersrum


# Techniken
## Unterprogrammtechnik
Bei der Unterprogramm technik versucht man eine Neue Tm mithilfe eines Bereits als unentscheidbar bewiesenen Programms zu loesen. Schafft man dies ist auch das betrachtete Programm unentscheidbar, sonst waere es moeglich die eingabe umzukeheren auf das Unentscheidbare Problem.
### Diagonalsprache
$$D= \{ w\in \{ 0,1\}^*|w=w_i\ und\ M_i\ akzeptiert\ w\ nicht\}$$
Das i-te Wort $w_i$ in kanonischer Reihenfolge) ist genau dann in der Diagonalsprache D, wenn die i-te TM $M_i$ nicht $w_i$ akzeptiert
## Satz von Rice
Eine Tm kann nicht auf jeder Eingabe halten weshalb sie nur Partielle Funktionen berechnen. Der Satz sagt aus Das Alle nicht trivialen Aussagen uebere edie von einer Tm berechneten Funktion unentscheidbar sind.

Formal geschrieben:

$$\emptyset \subsetneq S \subsetneq R$$
$$L(S) = \{\langle M\rangle |M \text{ berechnet eine Funktion aus }S \}$$

Hierbei ist $L(S)$ nicht entscheidbar und $R$ die Menge alle Entscheidbaren Funktionen.  Einfach erklaert ist es unmoeglich eine Menge an goedelnummern zu finden bei der die entsprechende [[Turingmaschine | TM]] eine die Funktionen aus $S$ berechnet auser wenn $S$ alle Funktionen sind, wobei die Menge dann alle Goedelnummern enthaelt, oder $S$ die leere Menge ist wobei keine Goedelnummer die Richtige Antwort ist. 

## Reduktionen
Eine Reduktion ist ein Algorithmus der Instanzen eines Startproblems als Spezialfaelle eines Zielprbalems modelliert

### Postsche correspondenzproblem
![[Pasted image 20211126122315.png]]
um mit dem PCP entscheidbarkeit zu prueffen muss das PCP zu den anderen Programm umgewandelt werden.

# Semi-Entscheidbarkeit
Eine Sprache wird entschieden wenn eine Tm auf jeder Eingabe Haelt und genau die Woerter der Sprache erhaelt.

Eine Sprache wird erkannt wenn jedes Wort akzeptiert wird und die selbe TM kein Wort akzeptiert was nicht in der Sprache ist.
Wenn eine TM existiert die die Sprache erkennt sop wird diese als semi-entscheidbar bezeichnet. Semi-entscheidbare sprachen sind auchrekursiv abzaehlbar

Semi-EntEntscheidbare Sprachen sind abgeschlossen in der Vereinigung, im Schnitt aber nicht im Komoplement.

# Rekursive Aufzählung
Es gibt eine Tm die ewig auf ein Ausgabeband alle woerter einer sprache schreibt. Eine Sprache ist aufzaehlbar wenn es solch eine Tm gibt, aka jedes Wort der Sprache ist uergendwann auf dem Band. 

Ist dies der Fall so ist eine Sprache auch semi-entscheidbar wenn eine Sprache abzählbar ist und ihr Komplement auch so ist diese Sprache Entschiedbar.

## Satz von Richardson
Eine Funktion heisst elementar, wenn sie durch Kombination von Addition, Subtraktion, Multiplikation, Division, Potenzieren, Wurzel ziehen, Logarithmieren, Betragsfunktion und den trigonometrischen Funktionen konstruiert werden kann. 

Es ist unentscheidbar ob eine elementare funktion eine elementare Stammfunktion besitzt