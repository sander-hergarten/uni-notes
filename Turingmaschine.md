# Definition
Eine turing maschine ist ein versuch alles berechenbares in einer machine zu berechnen

es best aus:
![[Pasted image 20211013165958.png]]
Es besteht aus einem Band das an einem [[Automat]] angeschlossen ist. Die Turingmaschine ist definiert durch das 7-Tupel aus diesen Zeichen

## Vorgang
Der Anfangszustand ist $q_0$ auf dem band ist die Eingabe. Geht man nach rechts ist die man Positiv links Negativ.
![[Pasted image 20211013170430.png]]
Die Turing machine folgt den generellen regeln eines Automatens. Am ende kann das wort vom band gelesen werden oder der Wahrheitswert.

## Performance
Es gibt TMs die nie terminieren. Man misst Leistung:
![[Pasted image 20211013170943.png]]

## Konfiguration
Eine Konfiguration ermoeglicht das kopieren der TM. Der Bandinhalt wird als string geschrieben und der kopf wird einfach reingeschrieben. Der Kopf ist auf dem zeichen direkt rechts von sich.

## Programmierung
![[Pasted image 20211013174843.png]]

## Universelle  Turingmaschine
Die Universelle Turingmaschine simuliert eine andere Turingmaschine. Dabei ist $U$die Kodierung einer beliebigen TM M. Mann bezeichnet auch $<M>$ als die Kodierung
### Kodierung
Mann nennt auch $<M>$ die Gödelnummer. Diese Erhaelt man durch Kodierung der Uebergaenge. Mann Bildet eine Binaer zahl 
![[Pasted image 20211019093450.png]]
und haengt alle aneinander
![[Pasted image 20211019093441.png]] 
ie Kodierung des t-ten Ueberganges nennet man $code(t)$

Die UTM erhaelt ein wort welches eine Telmenge von der Goedelnummer eines Automats ist.

## Nicht Deterministische TM
Der Unterschied zu einer normalen TM ist das anstatt eines deterministischen Automatens der in den naechsten Zustand fuehrt benutzt man einen NFA. Der Einzige Unterschied ist das die Zustandueberfuehrung nicht durch eine Funktion sondern eine Relation gemacht wird.
![[Pasted image 20220114110421.png]]
Ein Beispiel fuer eine Ueberfuehrungstabelle waere :
![[Pasted image 20220114110506.png]]
solange ein Moeglicher Pfad akzeptiert akzeptiert auch das Programm.

Der Rechenweg einer NTM ist eine Konfigurationsfolge, die mit Startkonfiguration beginnt und mit Nachfolgekonfiguration fortgesetzt wird bis ein endzustand ereicht wird. Die moeglichen Rechenwege einer NTM koennen in einem Berechnungsbaum zusammengefasst werden. Die Knoten sind die Konfigurationen, die Wurzel die Startkonfiguration und die Kinder alle moeglichen Nachfolgekonfigurationen: ![[Pasted image 20220114111313.png]]
Der maximale Verzweigungsgrad ist hierbei:
![[Pasted image 20220114111900.png]]
### Laufzeit von NTM
Die Laufzeit definiert bei einer NTM $M$ und einer Eingabe $x$ als die Laufzeit die Laenge des kuerzesten akzeptierenden Rechenwegs von $M$ auf $x$. Wird $x$ nicht akzeptiert so ist die Laufzeit = 0. Die Worstcase Laufzeit ist deshalb auf einer Eingabe der Laenge $n$  die Maximale baumtiefe die es in der NTM $M$ gibt. Formal ist sie definiert als: ![[Pasted image 20220114112740.png]]