# Definition
Anhand von einer routing tabelle wird in jedem sytem die [[IP-Addressen]] zu den Hosts zurück gefürt.
![[Pasted image 20220512090936.png]]
## Direct route
über das selbe netzwerk

## Indirect route
muss durch mehrere router geleitet werden

# Beispiel
![[Pasted image 20220512091625.png]]
Die [[Subnetz Maske]] ist auch aufgeschrieben für jede addresse. Die Flags geben das verhalten des eintrags an:
- **G**: Gateway
- **H**: Host
- **S**: Static

# Classless Inter Domain Routing
![[Pasted image 20220512092416.png]]
# Ablauf
## Longest Prefix Match
![[Pasted image 20220512092648.png]]
Der Router geht bit für bit durch die addressen und versucht den nächstennachbarn zu finden. wenn ein 32bit eintrag getroffen wird hat man einen host gefunden  
**Beispiel:**
![[Pasted image 20220512092908.png]]
**Route #1**: ist die passendse umleitung
