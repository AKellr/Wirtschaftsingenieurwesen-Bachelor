## Gebrochen rationale Funktionen in der Anwendung
Gebrochen rationale Funktionen werden in der **Regelungstechnik** zur **Beschreibung von Systemen** (wie z.B. Filtern) durch eine **Übertragungsfunktion $G$** genutzt.
- Die Übertragungsfunktion $G$ wird als Quotient aus Eingangsgröße $U_1$ und Ausgangsgröße $U_2$ in Abhängigkeit vom Parameter $s$ dargestellt: $$G(s) = \frac{U_2(s)}{U_1(s)}.$$
- Da $U_1(s)$ und $U_2(s)$ oft Polynome sind, ist $G$ der **Quotient zweier Polynome**.
- In der Regelungstechnik sind nur **echt gebrochen rationale Übertragungsfunktionen realisierbar**.
## Definition der gebrochen rationalen Funktion
Eine Funktion $f$ heißt **gebrochen rational**, wenn sie als **Quotient zweier ganzrationaler Funktionen** dargestellt werden kann:

$$f(x) = \frac{g(x)}{h(x)} = \frac{a_n x^n + a_{n-1} x^{n-1} + \cdots + a_1 x + a_0}{b_m x^m + b_{m-1} x^{m-1} + \cdots + b_1 x + b_0}$$

- **Echt gebrochen rational:** Wenn der Grad des Nennerpolynoms $m$ größer ist als der Grad des Zählerpolynoms $n$ ($m > n$). Die Namensgebung ist analog zu Brüchen, bei denen der Nenner größer ist als der Zähler.
- **Unecht gebrochen rational:** Wenn der Grad des Nennerpolynoms $m$ kleiner oder gleich dem Grad des Zählerpolynoms $n$ ist ($m \le n$). Die Namensgebung ist analog zu Brüchen, bei denen der Nenner kleiner oder gleich dem Zähler ist.
## Nullstellen gebrochen rationaler Funktionen
Eine gebrochen rationale Funktion $f(x) = \frac{g(x)}{h(x)}$ hat eine **Nullstelle bei $x_0$**, wenn die folgenden Bedingungen erfüllt sind:
- Das **Zählerpolynom $g$ ist an der Stelle $x_0$ Null** ($g(x_0) = 0$).
- Das **Nennerpolynom $h$ ist an der Stelle $x_0$ nicht Null** ($h(x_0) \ne 0$).
$$\text{Wenn } g(x_0) = 0 \text{ und } h(x_0) \ne 0 \implies f(x_0) = 0.$$
- An **gemeinsamen Nullstellen** von $g$ und $h$ liegen **keine Nullstellen** von $f$, da $f$ dort nicht definiert ist.

## Polstellen gebrochen rationaler Funktionen
Eine gebrochen rationale Funktion $f(x) = \frac{g(x)}{h(x)}$ hat eine **Polstelle bei $x_0$**, wenn die folgenden Bedingungen erfüllt sind:
- Das **Nennerpolynom $h$ ist an der Stelle $x_0$ Null** ($h(x_0) = 0$).
- Das **Zählerpolynom $g$ ist an der Stelle $x_0$ nicht Null** ($g(x_0) \ne 0$).$$\text{Wenn } h(x_0) = 0 \text{ und } g(x_0) \ne 0 \implies x_0 \text{ ist Polstelle von } f.$$
- An Polstellen wachsen bzw. fallen die Funktionswerte **über alle Grenzen**.
- Die Funktion ist an Polstellen **nicht definiert**.
- In der Regelungstechnik bestimmen die **Polstellen der Übertragungsfunktion $G$ das Zeitverhalten und die Stabilität des Systems**.
- Die Umkehrung der Polstellenregel gilt nicht immer: Polstellen von $f$ können (müssen aber nicht) auch an gemeinsamen Nullstellen von $g$ und $h$ liegen.
## Asymptoten einer gebrochen rationale Funktion
**Asymptoten** sind Kurven, denen sich der Graph einer Funktion $f$ **für große $|x|$** oder **in der Nähe einer Polstelle** annähert.
1. **Senkrechte Asymptote:** Zu jeder Polstelle $x_0$ von $f$ gehört die senkrechte Asymptote $$x = x_0.$$
2. **Asymptoten für große $|x|$:**
    - **Echt gebrochen rationale Funktionen ($m > n$):** Die **$x$-Achse** (Gerade $y=0$) ist die Asymptote.
    - **Unecht gebrochen rationale Funktionen mit Zählergrad = Nennergrad ($m = n$):** Die Gerade $$y = \frac{a_n}{b_n}$$ ist die Asymptote.
    - **Unecht gebrochen rationale Funktionen mit Zählergrad > Nennergrad ($n > m$):** Die Asymptote ist eine **ganzrationale Funktion $y = p(x)$**.

## Definitionslücken
Wenn $x_0$ eine **gemeinsame Nullstelle** sowohl des Zählerpolynoms $g$ als auch des Nennerpolynoms $h$ ist ($g(x_0) = 0$ und $h(x_0) = 0$), liegt bei $x_0$ eine Definitionslücke vor.
- **Behebbare Definitionslücke:** Liegt vor, wenn sich der Faktor $(x - x_0)$ aus der Linearfaktorzerlegung von $g$ und $h$ **vollständig kürzen lässt**.
- **Polstelle:** Bleibt der Faktor $(x - x_0)$ im Nenner übrig, liegt eine Polstelle vor.
	- **Keine Nullstelle:** Bleibt der Faktor $(x - x_0)$ im Zähler übrig, liegt dort keine Nullstelle von $f$, da $f$ bei $x_0$ nicht definiert ist.