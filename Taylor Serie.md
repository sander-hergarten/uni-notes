# Definition 
Mithilfe der Taylor serie koennen andere Funktionen mithilfe eines Polynoms ermittelt werden. Dieses Polynom nennt man Taylor Polynom.

Die idee hinter der Taylor serie ist die Approximation einer Funktion durch gleichsetzen der Ableitungen des Taylor polynoms zu den der Ziel Funktion. Hierbei bildet sich eine Relativ eindeutige Struktur:
$$P(X) = f(0) + \frac{df}{dx}(0)\frac{x^1}{1!} + \frac{d^2f}{dx^2}(0)\frac{x^2}{2!} + \frac{d^3f}{dx^3}(0)\frac{x^3}{3!} \text{ ...}$$
Wobei P(x) die Approximation ist und f(x) die Zielfunktion

## Fehler der Taylorserie 
Der  Fehler des Taylor Polynoms ist einfach ermittelt durch:
$$r(x, x_0) = f(x) - p_n(x, x_0)$$
wobei $p_n$ das Taylor Polynom ist

## Taylorformel
Stellt man den Fehler um erhaelt man die taylorformel:
$$ f(x)= p_n(x, x_0) + r(x, x_0)$$
Dementsprechend ist es sinvoll die Restglied Darstellung zu ermittelen. hierbei gibt es zwei beliebte kandidaten 
1. Nach Lagrange: $$r(x, x_0)=\frac{f^{(n+1)}(z)}{(n+1)!}(x-x_0)^{n+1}$$
2. Nach Cauchy (nicht so relevant)

## Taylorreihe 
ist die unendliche Reihe Definiert als:
$$\sum_{h+0} ^\infty \frac{f^{(h)}(x_0)}{h!}(x-x_0)^k$$