## 1.2 Potenzfunktionen
Definition und Eigenschaften
Eine Funktion vom Typ $y = f(x) = x^n$ mit natürlichem Exponenten $n \in \mathbb{N}$ wird als **Potenzfunktion** bezeichnet.

Potenzfunktionen sind wichtig als „Bausteine“ der ganzrationalen Funktionen (Abschnitt 1.3).

|   |   |   |
|---|---|---|
|Exponent $n$|Symmetrie (Eigenschaft)|Graph ist symmetrisch zu|
|Gerade|Gerade Funktion ($f(-x) = f(x)$)|$y$-Achse|
|Ungerade|Ungerade Funktion ($f(-x) = -f(x)$)|Ursprung|

Nullstellen
Ein $x_0 \in D$ ist eine **Nullstelle** einer Funktion $f$, wenn $f(x_0) = 0$ gilt.
• Der Graph jeder Potenzfunktion schneidet oder berührt die waagerechte Achse bei $x = 0$.
• Die Nullstellen werden durch Lösen der Gleichung $f(x) = 0$ bestimmt.

Potenzfunktionen mit negativem Exponenten

Potenzfunktionen können für $x \neq 0$ auch mit negativen Exponenten definiert werden: $$f(x) = x^{-n} = \frac{1}{x^n} \quad \text{mit } n \in \mathbb{N}$$

• Bei $x = 0$ wachsen bzw. fallen die Funktionswerte über bzw. unter alle Grenzen.
• Die Funktionen haben an dieser Stelle eine **Polstelle**.

Umkehrfunktion (Wurzelfunktion)
Die Umkehrfunktionen von Potenzfunktionen $f(x) = x^n$ (üblicherweise für $x \geq 0$ definiert) sind die **Wurzelfunktionen**: $$f^{-1}(x) = \sqrt[n]{x} = x^{\frac{1}{n}}$$

Potenzfunktionen mit rationalem Exponenten $\frac{m}{n} \in \mathbb{Q}$ sind gegeben durch: $$y = f(x) = x^{\frac{m}{n}} = \sqrt[n]{x^m}$$

Potenzgesetze
Für beliebige Potenzen $x^n$ mit $n \in \mathbb{R}$ gelten die folgenden Potenzgesetze
1. **Multiplikation von Potenzen** $\rightarrow$ Addition der Exponenten: $$x^n \cdot x^m = x^{n+m}$$
2. **Division von Potenzen** $\rightarrow$ Subtraktion der Exponenten: $$\frac{x^n}{x^m} = x^{n-m}$$
3. **Potenzierung von Potenzen** $\rightarrow$ Multiplikation der Exponenten: $$(x^n)^m = x^{n \cdot m}$$

## 1.3 Ganzrationale Funktionen (Polynomfunktionen)

Definition
Eine Funktion vom Typ **ganzrationale Funktion** (oder Polynomfunktion) ist definiert als: $$y = f(x) = a_n x^n + a_{n-1} x^{n-1} + \cdots + a_1 x + a_0$$ Hierbei ist $n \in \mathbb{N}_0$.

• Die reellen Zahlenwerte $a_0, a_1, \ldots, a_n$ heißen **Koeffizienten**.
• Der höchste auftretende Exponent $n$ ist der **Grad** der Funktion.

**Anwendung**
Ganzrationale Funktionen finden Anwendung in verschiedenen Bereichen:
• **Werkstoffkunde**: Temperaturabhängigkeit des elektrischen Widerstands.
• **Betriebswirtschaft**: Beschreibung von Erlösfunktionen.
• **Technische** Mechanik: Beschreibung der Biegung von Balken.
• **Vorteil**: einfaches Rechnen! Nullstellen

**Nullstellensatz:** Ganzrationale Funktionen mit ungeradem Grad haben immer **mindestens eine Nullstelle**.
• Ganzrationale Funktionen mit ungeradem Grad sind punktsymmetrisch.
• **Fundamentalsatz der Algebra:** Eine ganzrationale Funktion vom Grad $n$ hat **höchstens $n$ Nullstellen**.

**Berechnung der Nullstellen:**
• Für $n=1$ und $n=2$ existieren einfache Lösungsformeln.
• Für $n=3$ und $n=4$ gibt es komplizierte Lösungsformeln.
• Für $n \geq 5$ sind keine Lösungsformeln möglich.
• Ab $n=3$ wird die Verwendung numerischer Verfahren, wie das Newton-Verfahren ($\rightarrow$ Abschnitt 3.5), empfohlen.

**Linearfaktorzerlegung**
Wenn eine ganzrationale Funktion vom Grad $n$ die $n$ Nullstellen $x_1, x_2, \ldots, x_n$ besitzt, kann sie in **Linearfaktoren** zerlegt werden: $$f(x) = a_n(x - x_1) \cdot (x - x_2) \cdot \ldots \cdot (x - x_n)$$Dies ist gleichbedeutend mit der Definitionsgleichung: $$f(x) = a_n x^n + a_{n-1} x^{n-1} + \cdots + a_1 x + a_0$$

• Die Nullstellen müssen nicht alle verschieden sein; ist $x_i$ eine mehrfache Nullstelle, kommt der entsprechende Linearfaktor mehrfach vor.
    ◦ _Beispiel:_ $f(x) = x^3 + x^2 - 8x - 12$ hat $x_1 = -2$ (doppelt) und $x_2 = 3$ (einfach). Die Zerlegung ist $f(x) = (x + 2)^2 \cdot (x - 3)$.
    ◦ _Beispiel:_ $f(x) = x^3 - 2x^2 - 5x + 6$ hat die Nullstellen $x_1 = -2, x_2 = 1$ und $x_3 = 3$. Die Zerlegung ist $f(x) = (x + 2) \cdot (x - 1) \cdot (x - 3)$.