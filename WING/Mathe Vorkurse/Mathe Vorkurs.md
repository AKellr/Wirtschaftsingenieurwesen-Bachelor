	
Eine **Aussage**: entweder **wahr** oder **falsch**
**Implikation**: $A \implies B$ ("aus A folgt B") ist wahr, wenn A und B beide wahr sind, und wenn A falsch ist (unabhängig von B)

**Äquivalenz**: $A \Leftrightarrow B$ ("A ist äquivalent zu B") ist wahr, wenn A und B denselben Wahrheitswert haben, sonst falsch.

**Menge**: eine Zusammenfassung unterscheidbarer Objekte, den Elementen der Menge, zu einer Gesamtheit
	- **Reihenfolge** der Elemente ist **beliebig**. 
	- **Duplikation** kommt **nicht vor**

$M = \{ x \mid A(x) \}$  lies: "M ist gleich der Menge aller x, für die gilt: A(x)" 

**Potenzgesetze**:
$$a^n \cdot b^n = (a \cdot b)^n \qquad \frac{a^n}{b^n} = \left(\frac{a}{b}\right)^n \quad (b \neq 0)$$
$$a^m \cdot a^n = a^{m+n} \qquad \frac{a^m}{a^n} = a^{m-n} = \frac{1}{a^{n-m}} \quad (a \neq 0)$$
$$(a^m)^n = a^{m \cdot n}$$

**Wurzelgesetze**:
 $$\sqrt[n]{a} \cdot \sqrt[n]{b} = \sqrt[n]{a \cdot b} \qquad \frac{\sqrt[n]{a}}{\sqrt[n]{b}} = \sqrt[n]{\frac{a}{b}} \quad (b \neq 0)$$
$$\sqrt[m]{a} \cdot \sqrt[n]{a} = \sqrt[m \cdot n]{a^{m+n}} \qquad \frac{\sqrt[m]{a}}{\sqrt[n]{a}} = \sqrt[m \cdot n]{a^{n-m}} \quad (a \neq 0)$$
$$\sqrt[m]{\sqrt[n]{a}} = \sqrt[m \cdot n]{a}$$

**Zweiter Fall beim Rationalmachen des Nenners**:
$$\frac{Z}{N} = \frac{Z}{\sqrt[s]{a^r}} = \frac{Z}{\sqrt[s]{a^r}} \cdot \frac{\sqrt[s]{a^{s-r}}}{\sqrt[s]{a^{s-r}}} = \frac{Z \cdot \sqrt[s]{a^{s-r}}}{\sqrt[s]{a^r \cdot a^{s-r}}} = \frac{Z \cdot \sqrt[s]{a^{s-r}}}{\sqrt[s]{a^{r+s-r}}} = \frac{Z \cdot \sqrt[s]{a^{s-r}}}{\sqrt[s]{a^s}} = \frac{Z \cdot \sqrt[s]{a^{s-r}}}{a}$$

Der **Logarithmus** von **a** zur **Basis** **b** ist also **diejenige reelle Zahl**, mit der man **b potenzieren** muss, um **a** zu erhalten:
$$\log_b a = c \iff a = b^c \quad (a>0, b>0, b \neq 1)$$
**Logarithmieren** ist die **zweite Umkehrung** des **Potenzierens** (erste ist **Wurzeln**).

**Basiswechsel**: Man kann einen Logarithmus einer beliebigen Basis b in einen Logarithmus zu einer beliebigen zulässigen anderen Basis d umrechnen und umgekehrt.
$$\log_b x = {\log_d b}\cdot{\log_d x} $$
$$\log_d x = \frac{\log_b x}{\log_b d}$$

**Äquivalente Umformungen von Gleichungen:**
- Vertauschen beider Seiten
- Addition oder Subtraktion desselben Terms auf beiden Seiten
- Multiplikation oder Division mit derselben von 0 verschiedenen Zahl auf beiden Seiten

**Nichtäquivalente Umformungen von Gleichungen (Änderung der Lösungsmenge einer Gleichung):**
- Multiplikation beider Seiten mit einem Term, der die Variable enthält
- Division beider Seiten mit einem Term, der die Variable enthält
- Quadrieren (Allgemeiner: Potenzieren) der beiden Seiten
- Radizieren der beiden Seiten

**Achtung!** Durch nichtäquivalente Umformungen können zur Lösungsmenge der ursprünglichen Gleichung weitere Lösungen hinzukommen, die bisher nicht vorhanden waren, oder Lösungen der ursprünglichen Gleichung verloren gehen.

Für **Lineare Gleichungssystem** gibt es drei Möglichkeiten zur Lösung:
- **Einsetzungsverfahren**
- **Gleichsetzungsverfahren**
- **Additionsverfahren**

**Der Absolutbetrag**: $|x|$ 

![[licensed-image.jpg|320]]![[licensed-image (1).jpg|320]]![[Gemini_Generated_Image_6rdlee6rdlee6rdl.png|320]]

Man kann bemerken, dass Gleichungen **zweiten oder vierten Grades** hätten **keine reelle Lösungen.** Aufgrund des Verlaufs **muss** der Graph (**dritten Grades**) die x-Achse mindestens einmal schneiden. 
- Der Graph dritten Grades kommt immer von einem Extrem und bewegt sich zum anderen Extrem, oder umgekehrt. Deswegen muss der Graph die x-Achse mindestens einmal schneiden.

**Rechenregeln für Summenzeichen**:
$$\sum_{i=1}^{n} (a_i \pm b_i) = \sum_{i=1}^{n} a_i \pm \sum_{i=1}^{n} b_i$$
$$\sum_{i=1}^{n} c a_i = c \sum_{i=1}^{n} a_i$$
$$\sum_{i=1}^{m} a_i + \sum_{i=m+1}^{n} a_i = \sum_{i=1}^{n} a_i$$
$$\sum_{i=m}^{n} c = c \cdot (n-m+1)$$
$$\sum_{i=m}^{n} a_i = \sum_{k=m+c}^{n+c} a_{k-c}$$
**Rechenregeln für Produktzeichen**:
$$\prod_{i=1}^{n} (a_i \cdot b_i) = \prod_{i=1}^{n} a_i \cdot \prod_{i=1}^{n} b_i$$
$$\prod_{i=1}^{n} (c \cdot a_i) = c^n \cdot \prod_{i=1}^{n} a_i$$
$$\prod_{i=1}^{m} a_i \cdot \prod_{i=m+1}^{n} a_i = \prod_{i=1}^{n} a_i$$
$$\prod_{i=m}^{n} c = c^{n-m+1}$$
$$\prod_{i=m}^{n} a_i = \prod_{j=m-k}^{n-k} a_{j+k}$$
**Analytische Darstellung**
Hier ist die Zuordnungsvorschrift in Form einer Gleichung (Funktionsgleichung) gegeben. Man unterscheidet zwei Arten:
$$y = f(x): \textbf{Explizite Darstellung:}$$ $$\text{Die Funktion ist nach einer Variablen aufgelöst (hier $y$).}$$
$$F(x,y) = 0: \textbf{Implizite Darstellung:}$$$$\text{Die Funktion ist nicht nach einer Variablen aufgelöst}$$ $$F(x,y) = x^2 + y^2 - r^2 = 0 \text{ (Kreisgleichung)}$$
Hierfür gibt es auch eine **explizite Darstellung**. Auflösung nach $y$ liefert $y = \pm \sqrt{r^2 - x^2}$. Die **positive bzw. negative** Wurzel beschreibt jeweils **den oberen bzw. unteren Halbkreis**.

**Parameterdarstellung**
Oft ist es bei der mathematischen **Beschreibung** von **Vorgängen in Natur und Technik** zweckmäßig, die augenblickliche Lage eines Körpers durch kartesische Koordinaten zu beschreiben, die sich mit der Zeit $t$ verändern. Die kartesischen Koordinaten sind also Funktionen der Zeit: $$  x=x(t), y=y(t), t_1 \le t \le t_2. $$Eine solche Darstellung mit der **Hilfsvariablen** $t$ als Parameter heißt **Parameterdarstellung** einer Funktion. In **Naturwissenschaft und Technik** **bezeichnet** der Parameter $t$ meist die **Zeit** oder einen **Winkel**. Für jeden Wert des Parameters $t$ aus dem Intervall $t_1 \le t \le t_2$ erhalten wir genau einen Punkt der Kurve.

**Eigenschaften von Funktionen**
In einer **Nullstelle** **schneidet** oder **berührt** der **Graph** der Funktion die **x-Achse**.

Eine Funktion $f$ heißt auf der Menge $M \subseteq D_f$ **nach unten**$ bzw. **nach oben** **beschränkt**, wenn es eine endliche Konstante $C_1$ bzw. $C_2$ gibt, so dass $C_1 \le f(x)$ für alle $x \in M$ bzw. $f(x) \le C_2$ für alle $x \in M$ gilt. Dabei werden $C_1$ bzw. $C_2$ **untere** bzw. **obere Schranke** von $f$ auf $M$ genannt.

Eine Funktion $f$ heißt **gerade** $\iff f(-x) = f(x)$ für alle $x \in D_f$.
Die Kurve einer geraden Funktion ist **spiegelsymmetrisch** (**achsensymmetrisch**) zur **y-Achse**.
($cos(x)$ is only trig function that is gerade)

Eine Funktion $f$ heißt **ungerade** $\iff f(-x) = -f(x)$ für alle $x \in D_f$.
Die Kurve einer ungeraden Funktion ist **punktsymmetrisch** oder **zentralsymmetrisch** zum **Ursprung**.

**Monotonie einer Funktion**
$f$ heißt **monoton wachsend**, falls für alle $x_1, x_2 \in D_f$ gilt: $$ x_1 < x_2 \Rightarrow f(x_1) \le f(x_2). $$ $f$ heißt **monoton fallend**, falls für alle $x_1, x_2 \in D_f$ gilt: $$ x_1 < x_2 \Rightarrow f(x_1) \ge f(x_2). $$ Man spricht von **strenger Monotonie**, wenn aus $x_1 < x_2$ die Beziehungen $f(x_1) < f(x_2)$ bzw. $f(x_1) > f(x_2)$ folgen.

Konstante Funktionen sind sowohl monoton wachsend als auch monoton fallend (aber **nicht streng**).

**Beispiel**: Welches Monotonieverhalten besitzt die Funktion $y = \frac{x+1}{x-3}$?

Sei $x_1 < x_2$. Dann gilt: $$ f(x_2) - f(x_1) = \frac{x_2+1}{x_2-3} - \frac{x_1+1}{x_1-3} = \frac{(x_2+1)(x_1-3) - (x_1+1)(x_2-3)}{(x_2-3)(x_1-3)}$$
$$= \frac{x_1x_2 - 3x_2 + x_1 - 3 - (x_1x_2 - 3x_1 + x_2 - 3)}{(x_2-3)(x_1-3)} = \frac{4(x_1 - x_2)}{(x_2-3)(x_1-3)} $$ Der Definitionsbereich wird an der Unstetigkeitsstelle $x=3$ in die beiden Teilintervalle $I_1 = ]-\infty;3[$ und $I_2 = ]3;+\infty[$ zerlegt. Beide müssen nun auch getrennt untersucht werden. Im Teilintervall $I_1$ gilt $x < 3$. Dann ist $x_2-3 < 0$ und $x_1-3 < 0$. Die Voraussetzung $x_1 < x_2$ ist äquivalent zu $x_1-x_2 < 0$. Eingesetzt in die letzte Gleichung folgt sofort $f(x_2) - f(x_1) < 0$, d.h. $f(x_2) < f(x_1)$. Das bedeutet, dass die Funktion im Teilintervall $I_1$ streng monoton fallend ist. Im Teilintervall $I_2$ gilt entsprechend $x > 3$. Daraus folgt $x_2-3 > 0$ und $x_1-3 > 0$. Wegen der Voraussetzung $x_1 < x_2$ gilt wiederum $x_1-x_2 < 0$. Somit gilt auch in $I_2$, $f(x_2) - f(x_1) < 0$, d.h. $f(x_2) < f(x_1)$. Die Funktion ist also auch im Teilintervall $I_2$ streng monoton fallend. Damit ist gezeigt, dass sich die gegebene Funktion im gesamten Definitionsbereich streng monoton fallend verhält.

**Umkehrfunktion**
Die Funktion $f: D_f \to W_f$ sei **bijektiv**, d. h.
$$\text{Zu jedem Element }y \in W_f \text{ gibt es ein }x \in D_f \text{ mit } y = f(x)$$$$\text{Derselbe Funktionswert wird nicht zwei verschiedenen Argumenten zugeordnet, d. h. }$$$$x_1 < x_2 \Rightarrow f(x_1) \neq f(x_2).x$$

Die Punkte $P = (a,b)$ und $P' = (b,a)$ liegen im kartesischen Koordinatensystem **symmetrisch zur Geraden $y = x$** (der Winkelhalbierenden des 1. und 3. Quadranten).
![[Pasted image 20250926081021.png]]

![[Pasted image 20250923162038.png]]

**Jede streng monoton** wachsende **oder** fallende Funktion **besitzt eine Umkehrfunktion.**

**Verschiebung in y-Richtung**
Eine gegebene Funktion $y = f(x)$ soll um eine reelle Zahl $b$ in $y$-Richtung verschoben werden. Dies wird erreicht durch Addition der Zahl $b$ zu jedem Funktionswert, also durch die Funktion $y = f(x) + b$.

Ist $b > 0$, so erfolgt die Verschiebung in positiver $y$-Richtung, bei $b < 0$ in negativer $y$-Richtung.

**Verschiebung in $x$-Richtung**
Jetzt soll die Funktion $y = f(x)$ um eine reelle Zahl $a$ in $x$-Richtung verschoben werden. Die Funktion $y = f(x - a)$ leistet das Gewünschte. 

Ist $a > 0$, so erfolgt die Verschiebung in positiver $x$-Richtung, bei $a < 0$ in negativer $x$-Richtung.

![[Pasted image 20250926081330.png]]

Wir werden jetzt einen Kreis in Mittelpunktslage (d. h. Mittelpunkt $(0|0)$) mit dem Radius $r$ mit der Gleichung $x^2 + y^2 = r^2$ um $a$ Einheiten nach rechts und um $b$ Einheiten nach oben verschieben (Fig. 3). Die beiden oben angegebenen Verschiebungen $x \to x-a$ und $y \to y-b$ finden Anwendung und es ergibt sich sofort die Gleichung des vom Koordinatenursprung zum Mittelpunkt $(a|b)$ verschobenen gleichgroßen Kreises
$$(x-a)^2 + (y-b)^2 = r^2.$$
**Spiegelung an der y-Achse**
Zu einer gegebenen Funktion $y = f(x)$ ist $y = f(-x)$ diejenige, die $f(x)$ an der $y$-Achse spiegelt. Anders ausgedrückt, man muss in der Funktionsgleichung der Originalkurve jedes $x$ durch $-x$ ersetzen, um die zur Originalkurve an der $y$-Achse gespiegelte Bildkurve zu erhalten.

![[Pasted image 20250926081621.png]]

**Spiegelung an der x-Achse**
Um einen Punkt an der $x$-Achse zu spiegeln, muss die $y$-Koordinate des Punktes das jeweils andere Vorzeichen erhalten.

Besteht die zu spiegelnde Funktion aus mehr als einem Punkt (die bisher betrachteten Funktionen hatten sogar unendlich viele Punkte), ist für jedes Element des Wertebereiches der Originalfunktion dieser Vorzeichenwechsel vorzunehmen.
Damit ist $y = -f(x)$ diejenige Funktion, die $f(x)$ an der $x$-Achse spiegelt (nach oben/unten geöffnet)

![[Pasted image 20250926081738.png]]

**Streckungen/Stauchungen in y-Richtung**
Das Bild der Funktion $g(x) = c \cdot f(x)$ entsteht, indem man alle Funktionswerte der Originalfunktion $y = f(x)$ durch ihren $c$-fachen Wert ersetzt. Geometrisch heißt das, alle Funktionswerte werden auf den $c$-fachen Wert gestreckt, wenn $|c| > 1$ ist. Falls $|c| < 1$, werden alle Funktionswerte auf den $c$-fachen Wert gestaucht.

Bei negativem $c$ tritt zusätzlich noch eine Spiegelung an der $x$-Achse auf.

![[Pasted image 20250926081941.png]]

**Streckungen/Stauchungen in x-Richtung**
Das Bild der Funktion $g(x) = f(cx)$ entsteht durch Stauchung oder Streckung der Funktion $y = f(x)$ in $x$-Richtung. Wenn $|c| > 1$ ist, tritt eine Stauchung ein, falls $|c| < 1$, eine Streckung.

Bei negativem $c$ tritt zusätzlich noch eine Spiegelung an der $y$-Achse auf.

![[Pasted image 20250926082038.png]]

Ist umgekehrt $g(x)$ gegeben, so kann $f(x)$ wie folgt bestimmt werden: $f(x) = g\left(\frac{x}{c}\right)$.