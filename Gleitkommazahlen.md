# Definition 
Im Dezimalsystem werden Zahlen So definiert;
$$123.45 = 1*10^2+2*10^1+3*10^0+4*10^{-1}+5*10^{-2}$$
$$= 1*10^2(1*10^{0}+2*10^{-1}+3*10^{-2}+4*10^{-3}+5*10^{-4})$$
die Binaerzahl $10010.1$ kan dementsprechend auch als:
$$2^4(1*2^0+0*2^{-1}+0*2^{-2}+1*2^{-3}+0*2^{-4}+1*2^{-5}$$
und algemein kann man definieren:
$$\pm \left( \sum^{\inf}_{j=1}d_jb^{-j}\right)\times b^e$$
Dar hierfuer unedlich speicher gebraucht ist kann man beschraenken auf 
$$\pm \left( \sum^{m}_{j=1}d_jb^{-j}\right)\times b^e$$
wobei
![[Pasted image 20220105231332.png]]
gilt


## Maschinenzahlen
Dar die Gleitpunktdarstellung nicht mehr bei Festgeseztem Speicher alle Zahlen Darstellen kann wird ein Zahlenbereich festgelegt mithilfe der parameter der oberen Funktion
$$\text{Maschinen Zahlen:  } \mathbb{M}(b,\ m,\ r,\ R)$$
Hierfuehr muss man von den Reelen Zahlen auf die Maschinen Zahlen abbilden
$$fl:\mathbb{R} \rightarrow \mathbb{M}$$
Diese Abbildung nent man die Reduktionsabbildung
![[Pasted image 20220110134310.png]]

Hierdurch erfolgt das ein [[Fehleranalyse|Gleitkomma fehler]] entsteht. Der Absolute Fehler ist hierbei maximal wenn sich $x$ genau zwischen zwei Zahlen aus der Zielmenge befindet. Der Relative Fehler wiederum ist immer $\leq \frac{1}{2}b^{1-m}$  Deswegen nennt man diesen Wert die **Relative Maschinengenauigkeit**. Mithilfe dieser Zahl kann man auch genau bestimmen was die naechste Zahl der Reihe ist.

Die Zahlen die Teil der Maschinenzahlen sind nent man den Bildbereich also den teil der durch den exponenten $e$ beschraenkt wird:
$$\mathbb{D}\ :=\ [-x_{max},-x_{min}]\ \cup \ [x_{min},x_{max}]$$


### Min Max
Die Grenzen der Maschinenzahlen koennen durch 2 gleichungen bestimmt werden:
$$x_{min} = (0,\ 1000..0)\times b^r= b^{r-1}$$
$$x_{max} = (0,\ aa...a)\times b^R\ \text{ mit }a=b-1$$
umgerechnet mithilfe der Geometrischen Reihe:
$$x_{max}= (1-b^{-m})b^R$$

## Rundungsfehler
![[Pasted image 20221025124054.png]]
der [[Konditionen|relative Fehler]] der Rundung:
$$

\left|\frac{fl(x)-x}{x}\right| \le \frac{\frac{b^-m}{2}b^e}{b^{-1}b^e} = \frac{b^{1-m}}{2}
$$$$
\Rightarrow eps  := \frac{b^{1-m}}{2}
$$
## Arithmetikfehler

![[Pasted image 20221025124426.png]]
![[Pasted image 20221025125139.png]]