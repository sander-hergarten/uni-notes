# Definition
Es gibt einen NAT Router der mit dem Internet verbunden ist. Alle dahinter kriegen private addressen. Er leitet mit einer eigenen Öffentlichen addresse die packete an private weiter
![[Pasted image 20220512093328.png]]


Dar Nicht Genug [[IP-Addressen]] existieren wird NAT angewendet

## Privaten Adressen 
Standardisierte Adressblöcker die jeder frei benutzen kann. Diese werden nicht im internet geroutet

## Absendungs Tabelle
Ein NAT Router hält eine lockale Tabelle die auf die privaten addressen mapped. Um die Packete zurück zu wenden wird ein Port für die Addressen festgelegt. 

Der Sendende private rechner entscheidet aber den Port, weshalb es wichtig ist kollisionen zu vermeiden. Um das zu vermeiden ändert der NAT Router bei Collisionen den Port zu den nächsten freien Port.

**Beispiel:**
![[Pasted image 20220512094243.png]]
