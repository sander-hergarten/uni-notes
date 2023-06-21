# Definition
P und NP sind Komplexitaetsklassen

**P** steht fuer Polynomielle Algorithmenund **NP**. non deterministisch Polynomiel Probleme die unter P fallen sind in endlicher zeit loesbar waehrend die die in np sind es nicht sind. Um zu ermitteln ob ein Problem in endlicher zeitloesbar ist kann man konzepte aus der Berechenbarkeit borgen. Z.B kann die Laufzeit mithilfe einer [[Registermaschinen]] determinieren.

## Polynomiell
Die Klasse **P** enthaelt auschlieslich Entscheidungsprobleme die durch eine TM entschieden werden koennen. Statt der RAM koennte man auch genauso gut eine TM hier benutzen

## Non deterministisch Polynomiell
Hier Benuzen wir eine Nicht deterministishe [[Turingmaschine]]. Diese Komplexitaetsklasse enthaelt alle Entscheidungsprobleme die durch eine NTM erkannt werden, deren Worstcase Laufzeit poynomiell beschraenkt ist. 

Es ist moeglich an der Problemstellung ein NP problem zu entdecken. Eine Sprache Liegt genau dann in NP wenn es eine polynomiellen deterministischen Algorithmus $V$ une ein Polynom $p$ mit der folgenden Eigenschaft gibt:![[Pasted image 20220114113854.png]]
Das Funktioniert weil der Algorithus in endlicher zeit lauft und der einfach ueber alle eingaben laufen kann bis er akzeptiert. Es gibt immer ein Polynom und einen Verifizierer. Wenn  $y$ durch das Polynom beschraenkt ist dann wird xy fuer mindestens ein x akzeptiert solange x in der Sprache ist. Das $y$ wird deshbalb zertifikat genant.

Ein Problem heist NP-Schwer wenn es moeglich ist jedes problem in NP auf dieses Problem zu reduzieren. Es heist NP-Vollstaendig wenn es NP Schwer ist und in NP Liegt.

### NP Vollstaendigkeit
um NP Vollstaendigkeit zu zeigen:
![[Pasted image 20220121100803.png]]

## Polynomielle Reduktion
Die Polynomielle Reduktion funktioniert sehr aehnlich zur regulaeren [[Entscheidbarkeit von Sprachen#Reduktionen|Reduktion]]. Der Unterschied besteht wenn man zeigen kann das ein Problem $L_1$ Reduzierbar ist mit einem Problem $L_2$ und $L_2 \in P$ dann folgt $L_1\in P$  

### Satz von Cook und Levin
Jedes Problem in NP kann in polynomieller Zeit als Spezialfall von SAT formuliert werden. 