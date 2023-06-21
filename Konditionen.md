# Definition 
die Kondition ist die eigenschaft eines problems. Sie misst die empfindlicheit eines Problems im falle von fehlern. Eine as verhaeltniss von inputfehler zu outputfehler bei der Bearbeitung eines [[Problem]]. Eine hilfe bei der [[Fehleranalyse]] 

um algemein  Konditionen zu erstellen muss e

Eine Kondition wird Ermittelt:
![[Pasted image 20211025210713.png]]

hierbei ist $\Delta _x$ der unterschied zwischen der Wahren Eingabe und $\Delta _y$ der unterschied zwischen der Wahren Ausgabe. 

## Absolute Kondition
Das Verhaeltniss des Absoluten Fehlers:
$$\frac{\lVert \Delta y\rVert Y}{\lVert \Delta x\rVert X}$$

Um Algemein die Kondition eines Problems zu ermitteln nimmt man das [[Taylor Serie|Taylorpolynom]] 1ster ordnung um den Punkt x. Nun ist der Fehler $f'(x)* \Delta x$. 

Hierdurch kann man aproximiren
$$f(\widetilde{x}) \dot{=}f(x)+f'(x)(\widetilde{x}-x)$$

und den aproximierten Fehler erhalten durch die Umstellung
$$f(\widetilde{x})- f(x) \dot{=}f'(x)(\widetilde{x}-x)$$

Mann sieht das $f(\widetilde{x})- f(x)$ der Ausgabe Fehler $\Delta y$ ist und $(\widetilde{x}-x)$ der Eingabe Fehler $\Delta x$ ist. Das heist $f'(x)$ ist die Absolute Konditionzahl.

Jeh Groesser die Steigung umso mehr werden Fehler in der Eingabe Herausgehoben. 

Die Vektoriesierte Kondition funktioniert genauso nur muss die Ableitung von f auf die Partiele Ableitung aller komponennten in f summiert sein:
$$f(\widetilde{x}) \dot{=}f(x)+\sum_{j=1}^n \frac{\delta f(x)}{dx_j}(\widetilde{x}-x)$$
Dementsprechend: 
$$f(\widetilde{x})-f(x) \dot{=}\sum_{j=1}^n \frac{\delta f(x)}{dx_j}(\widetilde{x}-x)$$
## Relative Kondition
Mit der relativen Kondition wird das Verheltnis
$$\frac{\delta _y}{\delta _x}$$
des relativen Ausgabefehlers zum relativen Eingabefehler Betrachtet. Ein Problem ist umso besser kondititioniert je kleiner die Schranken sind

Der Prozess zur ermitelung der Relativen Kondition ist eine weiterfuerung des Absoluten. Mann stellt jedoch um zu der Form des Relativen Fehlers:

$$\frac{f(\widetilde{x})- f(x)}{f(x)} \dot{=}f'(x)\frac{1}{f(x)}(\widetilde{x}-x)$$
Mann Multipliziert um es anschaulicher zu machen mit $\frac{x}{x}$
$$\frac{f(\widetilde{x})- f(x)}{f(x)} \dot{=}f'(x)\frac{x}{f(x)}\frac{(\widetilde{x}-x)}{x}$$

Mann sieht nun die Fehler in der Ein-/Ausgabe $\frac{f(\widetilde{x})- f(x)}{f(x)}$ und $\frac{(\widetilde{x}-x)}{x}$ und die relative Konditionszahl $f'(x)\frac{x}{f(x)}$