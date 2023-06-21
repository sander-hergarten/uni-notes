# Definition
Eine Relation zwischen zwei Mengen ist eine Teilmenge des Kreuzproduktes der Beiden Mengen. Sind beide Mengen gleich so sagt man die Realtion auf die menge.

Eine Relation kann als x R y geschrieben werden

Eine [[Abbildung]] ist auch eine Relation nur das es keine Regeln zu den Paaren gibt.

## Eigenschaften
**Reflexiv:**
Fuer alle $x \in M:\ x\ R\ x$

**Symetrisch:**
Fuer alle $x,y \in M:\ x\ R\ y\Rightarrow y\ R\ x$

**Antisymetrisch**
Fuer alle $x,y \in M:\ x\ R\ y \text{ und }y\ R\ x \Rightarrow x=y$

**Transitiv**
Fuer alle $x,y,z \in M:\ x\ R\ y \text{ und } y\ R\ z\ \Rightarrow x\ R\ z$

**Vollstaendig**
Fuer alle $x,y\in M:\ x\ R\ y \text{ oder }y\ R\ x$

## Abschluss
Ein Transitiver Abschluss ist definiert als eine Teilmenge einer Relation auf einer Menge

## Äquivalenzrelation
sind Relationen die sowohl Reflexiv als auch Symetrisch und Transitiv sind. Es existiert eine Bijektion von einer Aequivalenzrelation und einer Partition einer Menge.

### Äquivalenz klassen:
Hat mann eine Aequivalenzrelation C auf einer Menge M und ein ellement x aus dieser Menge so ist die Aequivalenzklasse von x alle ellemente die zu x Aequivalent sind laut relation.
$$[x]=[x]_C:=\{ !x\in M |!xCx \}$$
Ein Representatnt dieser Klasse ist jedes ellement das in der Klasse liegt.

Zwei Aequivalenzklassen zu zwei ellementen sind gleich wenn die eine in der Anderen enthalten ist. Also genau wenn das eine Ellement in Relation zum anderen steht.

### Quotienten Menge:
Die Quotienten Menge einer Menge mit einer Relation wird Quotientenmenge von *Menge* modulo *Relation* genannt. Das ist die Menge an Aequivalenzklassen.
$$M/C \ :=\{\ [x]_C\ |\ x\in M\ \}$$
Die Quotienten abbildung ist die abbildung die einem Ellement aus einer Menge seine Aequivalenzklassen Zuweist. 

Die Quotientenmenge ist eine [[Mengen#Mengenpartitionen| Partition]] von der Ursprungsmenge.

## Ordnungen
### Präordnung
sind Realtionen die Sowohl Reflexiv als auch Transitiv sind. 
### Partielle Ordnung
sind Präordnungen die Antisymetrisch sind

### Totalordnung
Eine Totalordnung ist eine Partielle Ordnung die vollstaendig ist.

## Striktordnung
Eine Striktordnung ist keine Ordnung. Es ist definiert als eine Ordnung auf zwei ellementen die nicht gleich sind.

Prae/Total/partiell geordnete Mengen sind Mengen auf denen die entsprechende Ordnung definiert ist. Eine praegeordnete Teilmenge ist eine Teilmenge einer geordneten Menge die die Ordnungsrelation von der Ursprungsmenge kopiert.

### Minimal/Maximale Ellemente
Bei einer Praegeordneten Menge ist ein Ellement minimal wenn es kein echtkleineres anderes ellement aus der Menge gibt. Maximale Ellemente sind ellemente wo es keine Echtgroesseres Ellement gibt
$$x,y \in M,\ \ y\leq x \Rightarrow x\leq y$$
$$x,y \in M,\ \ y\geq x \Rightarrow x\geq y$$
Bei einer Geordneten Menge:
$$x,y \in M,\ \ y\leq x \Rightarrow x = y$$
$$x,y \in M,\ \ y\geq x \Rightarrow x = y$$

### Größte und Kleinste Elemente
Bei einer Praegeordneten Menge ist eine Element das Kleinste element falls es $\leq$ als alle anderen ist. Es ist das groeste falls es $\geq$ ist. Bei Praegeordneten Mengen ist das Kleinste/Groeste Element auch immer das Minimale/Maximale. Diese Bedingung ist nicht beidseitig. Falls man eine Ordnung hat gibt es hoechstens nur ein kleinstes/groestes Element. Bei einer Totalordnung ist ein Minimales Element auch ein kleinstes Element