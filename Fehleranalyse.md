# Definition 
Bei Umsetzen eines [[Algorithmus]] koenen fehler entstehen welche einige Ursachen haben koennen.  Formal kann man sich ein solches [[Problem]] als funktion vorstellen: $y=f(x)$ die Sowohl einen Eingabefehler ($\Delta x$) wie auch einen Ausgabefehler ($\Delta y$) haben kann. Oft muss das verhaeltnis dieser beiden zueinander ermittelt werden.

# Ursachen 
## Fehlerquellen
Es ibt mehrere Fehlerquellen bei Numerischen Loesungen:

- **Modellfehler**: Das Modell ist eine Idealisierung er Realitaet
- **Datenfehler**: z.B. Materialparameter im Modell nicht exakt bekannt
- **Verfahrensfehler**: Numersiche verfahren bieten nur Naeherungsweise Loesungen
- **Rundungsfehler**: Durchuerung eines [[Algorithmus]] auf Computer
