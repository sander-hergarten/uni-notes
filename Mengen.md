# Definition 
Eine Menge ist jede Zussamenfassung von bestimmten wohlunterscheidbaren Objekten. Zwei Mengen sind gleich wenn Beide eine Teilmenge von einander sind.

## Teilmenge
Eine Teilmenge X von Menge Y ist geschrieben als:
$$X \subseteq Y$$
bzw fuer die verneinung
$$X \nsubseteq Y$$

## Maechtigkeit 
Die Maechtigkeit ist die Anzahl an Ellementen in einer Menge und wird | X | geschrieben. Zwei Mengen heisen gleichmaechtig wenn eine bijektive [[Abbildung]] $M\rightarrow N$ existiert

### Satz von Cantor
Fuer jede Menge M sind M und Pot(M) nicht gleichmaechtig.

### Endlichkeit von Mengen
Eine Menge $M$ ist endlich wenn es ein eine Natuerliche Zahl gibt welche den selben wert hat wie die Maechtigkeit. Wenn M endlich ist, ist eine Abzaehlung von M eine Bijektion von den Natuerlichen Zahlen nach M

## Aussondern
Mengen koennnen durch eine [[Aussageform]] definiert werden:
$$\{x\in M | A(X)=True\}$$
wenn A(x) eine Aussageform ist. 

## Bild 
Das Bild einer Menge ist definiert als 
$$f(M) := \{f(x)|x\in M \}$$

das Urbild ist
$$f^{-1}(N):=\{x \in A|f(x)\in N \}$$

## Indexmenge
Indexmengen sind Mengen die durchnummeriert sind. Die Objekte einer Indexmenge sind paarweise verschieden wenn 2 Objekte nur gleich sind wenn sie den gleichen Index haben.

 Zwei Mengen heisen disjunkt, wenn sie nicht die gleichen Objekte haben also $A \cap B = \emptyset$
 
 Mengen sind Parweise disjunkt wenn es $n$ Mengen gibt und jedes paar disjunkt ist auser wenn beide den selben Index haben 
 
 ## Mengenpartitionen
Eine Partition von einer Menge M ist eine Menge aus Teilmengen von M. dabei sind diese Teilmengen paarweise disjunkt, nicht leer und die vereinigung aller dieser Mengen ist die Menge M. Ein Ellement einer Partition wird ein Teil der Partition gennant

## Homomorphiesatz für Mengen
Dar nichtleere [[Abbildung#Bild Urbild und Faser| Fasern]] einer Abbildung eine Partition bilden, ist es moeglich eine Äquivalenzrelation zu ermitteln, mithilfe der [[Relation#Quotienten Menge| Quotienten Menge]]. Die Aequivalenzrelationist zeigt die Bildgleichheit: $x_0Rx_1\Leftrightarrow f(x_0)=f(x_1)$

Mithilfe einer Quotienten Abbildung kann man die entsprechende Aequivalenzklasse determinieren, also die Menge an ellementen die das selbe bild wie x haben. Nun heist das dass es eine Wohldefinierte Abbildung von der Aequivalenzklasse auf das Ziel $f(x)$ gibt.
![[Pasted image 20211123061301.png]]
Diese Funktion nennen wir $\bar{f}$ und ist injektiv. Das Bild von $\bar{f}$ ist gleich dem Bild von $f$
