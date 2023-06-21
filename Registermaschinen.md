# Definition
Registermaschinen sind ein alternativer Weg zur [[Turingmaschine]] die Berechenbarkeit bestimmter Probleme zu Ermitteln. Um zu zeigen das Registermaschinen genau die selben Probleme wie eine TM loesen koenen muss man nachweisen dass:
1. Registermaschinen TM simulieren Koennen
2. TMs Registermaschinen simulieren Koennen

## Funktionsweise
Eine Registermaschine enthaelt einen Speicher welcher aus Zellen besteht. Es gibt auserdem einen Akkumulator welcher das Ergebnis abspeichert. Auserdem gibt es befehle welche auf den Akkumulator ausgefuert werden. Der Akku kann in den Speicher schreiben oder aus dem Speicher lesen.

Hierbei ist dies die vollstaendige Liste an Befehlen:
![[Pasted image 20211026005612.png]]
![[Pasted image 20211026005649.png]]

| Syntax       | Bewirkte Veraenderung | Befehlszaehler |
| ------------ | --------------------- | -------------- |
| LOAD $i$     | $c(0):=c(1)$          | $b:=b+1$       |
| CLOAD $i$    | $c(0):=i$             | $b:=b+1$       |
| INLOAD $i$   | $c(0):=c(c(i))$       | $b:=b+1$       |
| STORE $i$    | $c(i):=c(0)$          | $b:=b+1$       |
| INDSTORE $i$ | $c(c(i)):=c(0)$       | $b:=b+1$       |
| ADD $i$      | $c(0) := c(0)+c(i)$   | $b:=b+1$       |
|              |                       |                |

## Simulation von RAM durch TM 
**Aussage:**
Fuer jede im logorithmischen Kostenmass t(n)-zeitbeschraenkte RAM gibt es ein Poynom q unde eine q(n+t(n))-zeitbeschraenkte TM die den RAM simuliert.

**Beweis:**
Man nehme eine 2 Band Turingmaschine dar q ein Polynom ist macht es keinen Unterschied zur Aussage ($q^2$ ist weiterhin ein Polynom)

Auf Band 1 werden einzelne Befehle simuliert und auf Band 2 wird der Inhalt des speichers gelegt. 

Der Speicher wird auf dem TM Band durch einen binaeren index markiert
```
##0#bin(0)##...##bin(i)#bin(c(i))###
```
Hiermit ist der Platzbedarf auf Band 2 durch O(n+t(n)) beschraenkt, weil die RAM fuer hedes neue Bit, das sie erzeugt, mindestens eine Zeiteinheit benoetigt

## Simulation von TM durch RAM
**Aussage:**
In gleicher zeit sollte es moeglich sein eine TM zu Simulieren

**Beweis:**
Man nimmt an das es ein Band TM ist welche einseitig beschraenkt ist

Hier sind Zellen drauf die man mit 0-n durchnummeriert. Die Zustaende unb Bandalphabet sind durchnumeriert.

Das Register 1 Speichert den Index an der Kopfposition. Register 2 den Zustand. Register 3 - n die Inhalte der Bandzellen.

Die Zustaende werden iterativ abgefragt und ausprobiert bis ein passender gefunden wird. 