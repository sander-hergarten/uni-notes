# Definition
dieser Automat ist anders als eine [[Turingmaschine | Mehrspur TM]] dar sich n baender existieren und man sich auf jeden band unabhaengig bewegen. 
![[Pasted image 20211019090027.png]]

Sieh hat aber immer noch die gleiche Beschreibende Faehigkeit denn man kann eine Mehrband TM mit einer Einspurigen TM Simulieren
![[Pasted image 20211019091050.png]]
Hierbei wird 1 schritt in $O(t(n))$ wenn $t(n)$ die Laufzeit des Mehrspur TM verwandelt. Das heist insgesamt $O(t(n)^2)$