# Definition
Beweisprinzipien geben eine hilfestellung um [[Aussagen]] zu beweisen. Das Ziel wird definiert als:
$$A \Rightarrow B$$
Aequivalenzen koennen auf gleichem weg definiert werden, dar:
$$(A \Leftrightarrow B) \Leftrightarrow ((A \Rightarrow B) \wedge (B \Rightarrow A))$$

## Direkter Beweis
Bei dem Direkten beweis fuer die Implikation kann man grundsetzlich annehmen das $A$ Wahr ist. Das ziel ist eine Kette von implikationen zu finden wobei die letzte Ausage dieser kette $B$ ist.

## Kontraposition
statt zu zeigen das $A \rightarrow B$ gilt zeigt man stattdessen: 
$$\neg B \Rightarrow \neg A$$
Dies Beruht auf der [[Tautologie]]: 
$$(A \Rightarrow B) \Leftrightarrow (\neg B \Rightarrow \neg A)$$

## Widerspruch
Zeige das A wahr ist ist nun das Ziel. Man nimmt stattdessen eine definitiv falsche Aussage $(B\wedge \neg B)$ von der Negation von A impliziert wird

## Induktion
![[Pasted image 20211018083706.png]]
Man kann das Induktionsprinzip auf Rekursion verwenden:
![[Pasted image 20211018085650.png]]