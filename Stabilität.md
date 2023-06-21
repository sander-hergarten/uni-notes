> Ein Algorithmus heißt **gutartig** oder **stabil** wenn die durch ihn im laufe der Rechnung erzeugten Fehler in der Größenordnung des durch die Kondition des Problems bedingten unvermeidbaren Fehler bleiben.

Wenn ein Problem schlecht Konditioniert ist kann mann nicht erwarten das ein stabiler algorithmus gute Ergebnisse Liefert. Dementsprechend sind Numerische methoden nicht anwendbar in solchen fällen.

Man versucht die auswertung $f: X\rightarrow Y$ zu erhalten aber erhält statdessen ein abgewandeltes $\tilde{f}: X\rightarrow Y$ welches wegen Fehlern wie Rundungsfehler und Gleitpunkt arithmetik nicht $f$ ist.

Das ziel ist also den fehler zwischen den beiden funktionen auf die kondition des problems zu reduzieren:
$$\frac{\lVert \tilde{f}(x) -f(x) \rVert}{\lVert f(x)\rVert} = O(\textbf{eps})$$
<h3 align=center>Rückwärts stabilität</h3>
ein verfahren gilt als rückwerts stabil wenn:
$$
\begin{align}
\tilde{f}(x) &= f(\tilde{x}) \\
\Rightarrow\frac{\lVert x-\tilde{x} \rVert}{\lVert x \rVert} &= O(\textbf{eps})
\end{align}$$
dies heist das ein Algorithmus ist Rückwärts stabil wenn er die exakte Lösung des Problems mit fast richtiget eingabe liefert:
$$x\rightarrow\tilde{x}=x(1+\epsilon),\ \ \lvert\epsilon\rvert \le \textbf{eps}$$
und das wenn ein rückwärts stabiler Algorithmus für ein Problem $f$ mit Kondition $\kappa (x)$ angewendet wird gilt:
$$\frac{\lVert \tilde{f}(x) -f(x) \rVert}{\lVert f(x)\rVert} = O(\kappa(x)\textbf{eps})$$