
# Definition 
Eine Abbildung (oder Funktion) benoetigt 2 nicht leere [[Mengen]] und weist jeden ellement aus der ersten einem ellement aus der zweiten zu.  
$$f:A\rightarrow B$$
A heist Definitionsbereich und B Ziel. Die Menge 
![[Pasted image 20211014131824.png]]
nennt man den Graph von f.

Eine Funktion ist Auserdem eine Teilmenge des Kreuzprodukts des Definitionsbereichs mit der Zielmenge. Hierbei muss gelten das jedes Ellement aus x genau einen y wert hat mit $(x, y) \in f$.Alternativ wenn $(x, y_1) \in f$ und $(x, y_2) \in f$  dann $y_1 = y_2$

## sd
![[Pasted image 20211014133009.png]]

## Injektiv, Surjektiv, Bijektiv
![[Pasted image 20211014133658.png]]
Wenn man von der Komposition von 2 bijektiven Funktionen, die immer weiter bijektiv bleibt, das inverse nimmt ist dies gleich der Komposition der Umkehrabbildung.  
$$(g\circ f)^{-1} = f^{-1} \circ g^{-1}$$
Ausserdem gelten noch:
$$(f^{-1})^{-1} = f$$
$$id_M^{-1}=id_M$$
## Bild, Urbild und Faser
Das Bild eines Ellementes des Definitionsbereichs unter einer Abbildung ist das Eindeutig zu. Ein Bild ist Definiert als die Abbildung des Wertes.

Das Urbild ist das gegenteil: Fuer ein ellement der Zielmenge kriegt man ein Ellement der Definitionsmenge welches auf dieses Zielellement Abbildet. Ein Urbild ist der Ursprungswert vor der Abbildung. $f^{-1}(x)$

Gibt es nur ein Ellement dessen Urbild man ermittelt nennt man dies die Faser der Abbildung. Jedes Ellement liegt in genau einer Faser.

Ein Bild ist hoechstens so Maechtig wie die Definitionsmenge.

## Gleichheit von Abbildungen
Zwei Abbildungen sind gleich wenn der Definitionsbereich und das Ziel  das selbe sind und die [[Abbildungsvorschrift]] die selbe ist fuer alle eingaben.

Alternativ kann auch die funktionsgleichheit durch folgendes bestimmt werden.
![[Pasted image 20211025090509.png]]![[Pasted image 20211028142959.png]]

## Komposition von Abbildungen
Ist der Ziel bereich einer Abbildung gleich dem Definitionsbereich einer Anderen so kann eine Komposition gebildet werden. 
$$f:M \rightarrow N,\ g: N \rightarrow L$$
$$f\circ g:\ M \rightarrow L \mapsto g(f(x))$$ 
Fuer die Komposition von Abbildungen gilt das Assoziativgesetz:
$$f:M \rightarrow N,\ g: N \rightarrow L,\ h:L \rightarrow K$$
$$h\circ (f\circ g) =(h\circ f) \circ g$$ 
Die Identitaet wird nicht bei einer Komposition veraendert. Die Identitaet ist der Ursprungswert.

## Umkehrabbildung
Falls die Komposition von 2 Abbildungen die Identitaet der Ersten ergibt so ist die 2te eine Umkehrabbildung:
$$f:M \rightarrow N,\ g: N \rightarrow L$$
$$g\circ f=id_m\Rightarrow \text{g ist linksseitige Umkehrabbildung von f}$$ 
$$f\circ g=id_N\Rightarrow \text{g ist rechtsseitige Umkehrabbildung von f}$$ 
Sind beide Richtungen Wahr ist $g$ die Umkehrabbildung von $f$. Man Sagt auch $g$ ist zu $f$ invers. 

Eine Abbildung besitzt Umkehrabbildungen nur in bestimten faellen:
- bei injektivitaet besitzt eine Abbildung eine linksseitige Umkehrabbildung
- bei surjektivitaet besitzt eine Abbildung eine rechtsseitige Umkehrabbildung
- bei bijektivitaet besitzt eine Abbildung ein Inverses

Umkehrabbildungen werden mit $f^{-1}$ bezeichnet. $f$ heist invertierbar wenn eine funktion existiert die bei beidseitig bei der Komposition die Identitaet ergibt.

## In sich Abbildungen
Besitzt man 2 Abbildungen dessen Definitionsbereich = Zielbereich gilt so lassen sich die Kompositionen in beide Richtungen bilden. Man kann auch weiter definieren:
$$f^n := \underbrace{f\circ...\circ f}_{\text{n mal}}, \ f^0 := id_M$$
Falls $f$ bijektiv ist:
$$f^{-n}:=(f^{-1})^n$$