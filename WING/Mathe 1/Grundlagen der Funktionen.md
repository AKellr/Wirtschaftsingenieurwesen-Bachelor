### 1.1 Darstellung und Eigenschaften von Funktionen
#### Funktionsbegriff
- **Definition**: Eine Funktion ist eine **eindeutige Zuordnung** von Elementen $x$ aus einem Definitionsbereich $D$ (Argumente) zu Elementen $y$ aus einem Bild- oder Wertebereich $B$.
    - $D$ ist die Menge aller erlaubten $x$-Werte.
    - $B$ ist die Menge aller möglichen $y$-Werte.
- **Eindeutigkeit**: Jedem Argument $x$ wird **genau ein Funktionswert** $y$ zugeordnet.
- **Reelle Funktionen**: Bilden Argumente $x \in D$ mit $D \subseteq \mathbb{R}$ auf Funktionswerte $y \in B$ mit $B \subseteq \mathbb{R}$ ab.
#### Darstellung von Funktionen
Es gibt verschiedene Arten, eine Funktion darzustellen:
1. **Wertetabelle**: Besonders für Messwerte geeignet.
2. **Funktionsgleichung (explizit)**: $y = f(x)$.
3. **Funktionsgraph**: Visuelle Darstellung im Koordinatensystem.
4. **Implizite Darstellung**: Eine Gleichung $F(x, y) = 0$, die von Wertepaaren $(x, y)$ erfüllt wird.
5. **Parametrische Darstellung**: Wertepaare $(x, y)$ werden durch einen Parameter $t$ ausgedrückt: $x = f(t)$ und $y = g(t)$.
#### Funktionseigenschaften
**1. Symmetrie**
- **Gerade Funktion**: Eine Funktion $f$ ist gerade, wenn für alle $x \in D$ gilt: **$f(-x) = f(x)$**.
    - Der Graph ist **achsensymmetrisch zur y-Achse**.
    - Beispiel: $y=x^n$ mit geradem Exponenten $n$.
- **Ungerade Funktion**: Eine Funktion $f$ ist ungerade, wenn für alle $x \in D$ gilt: **$f(-x) = -f(x)$**.
    - Der Graph ist **punktsymmetrisch zum Ursprung**.
    - Beispiel: $y=x^n$ mit ungeradem Exponenten $n$.
**2. Monotonie (Wachstumsverhalten)** Eine Funktion $f$ heißt:
- **monoton wachsend**, wenn $f(x_2) \geq f(x_1)$ für $x_2 > x_1$ gilt.
- **streng monoton wachsend**, wenn $f(x_2) > f(x_1)$ für $x_2 > x_1$ gilt.
- **monoton fallend**, wenn $f(x_2) \leq f(x_1)$ für $x_2 > x_1$ gilt.
- **streng monoton fallend**, wenn $f(x_2) < f(x_1)$ für $x_2 > x_1$ gilt.
- Streng monotone Funktionen sind immer umkehrbar.
#### Umkehrbarkeit und Umkehrfunktion
- **Umkehrbarkeit**: Eine Funktion $f$ ist umkehrbar, wenn es zu jedem Funktionswert $y$ genau ein Argument $x$ gibt. Das bedeutet: $x_1 \neq x_2 \implies f(x_1) \neq f(x_2)$.
- **Umkehrfunktion**: Ordnet jedem Funktionswert $y \in B$ das ursprüngliche Argument $x \in D$ zu.
    - Schreibweise: $x = f^{-1}(y)$.
    - **Bestimmung**: Die Funktionsgleichung $y=f(x)$ wird nach $x$ aufgelöst.
    - **Graph**: Der Graph der Umkehrfunktion $f^{-1}$ entsteht durch Spiegelung des Graphen von $f$ an der Winkelhalbierenden ($y=x$).
#### Verkettung von Funktionen
- **Definition**: Die Verkettung der Funktionen $f$ und $g$ ist definiert als $(g \circ f)(x) = g(f(x))$.
    - Man spricht dies als "g verkettet mit f" oder "g Kringel f".
    - Zuerst wird die **innere Funktion** ($f$) angewendet, dann die **äußere Funktion** ($g$).
- **Wichtige Eigenschaften**:
    - Die Reihenfolge ist im Allgemeinen **nicht vertauschbar**: $g(f(x)) \neq f(g(x))$.
    - Für eine Funktion $f$ und ihre Umkehrfunktion $f^{-1}$ gilt jedoch: $f^{-1}(f(x)) = x = f(f^{-1}(x))$.
### 1.2 Potenzfunktionen
#### Potenzfunktion mit natürlichem Exponenten
- **Definition**: Eine Funktion vom Typ $y = f(x) = x^n$ mit einem natürlichen Exponenten $n \in \mathbb{N}$.
- Sie dienen als Bausteine für ganzrationale Funktionen.
- **Symmetrie**:
    - Gerade Exponenten $\implies$ gerade Funktion.
    - Ungerade Exponenten $\implies$ ungerade Funktion.
#### Nullstellen
- **Definition**: Ein Wert $x_0 \in D$ heißt Nullstelle einer Funktion $f$, wenn $f(x_0)=0$ gilt.
- Nullstellen werden durch das Lösen der Gleichung $f(x)=0$ bestimmt.
- Jede Potenzfunktion $y=x^n$ hat bei $x=0$ eine Nullstelle.
#### Potenzfunktion mit negativem Exponenten
- Definiert für $x \neq 0$: $f(x) = x^{-n} = \frac{1}{x^n}$ mit $n \in \mathbb{N}$.
- Bei $x=0$ haben diese Funktionen eine **Polstelle**, an der die Funktionswerte über alle Grenzen wachsen oder fallen.
#### Umkehrfunktion der Potenzfunktionen
- Die Umkehrfunktion von $f(x) = x^n$ (für $x \geq 0$) ist die **Wurzelfunktion** $f^{-1}(x) = \sqrt[n]{x} = x^{\frac{1}{n}}$.
#### Potenzgesetze
Für beliebige Potenzen $x^n$ mit $n \in \mathbb{R}$ gelten folgende Gesetze:
1. **Multiplikation**: $x^n \cdot x^m = x^{n+m}$.
2. **Division**: $\frac{x^n}{x^m} = x^{n-m}$.
3. **Potenzierung**: $(x^n)^m = x^{n \cdot m}$.