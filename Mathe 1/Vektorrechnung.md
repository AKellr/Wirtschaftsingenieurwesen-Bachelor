[[Math]]

## 7.1 Eigenschaften von Vektoren (Eigenschaften von Vektoren)

### Vektoren und Skalare
In der Physik und bei technischen Anwendungen unterscheidet man zwischen Größen:
- **Skalar:** Eine Größe, die durch die Angabe einer Maßzahl vollständig bestimmt ist (z.B. Temperatur, Spannung, Zeit, Widerstand).
- **Vektor:** Eine Größe, die durch die Angabe einer Maßzahl und einer Richtung vollständig bestimmt ist (z.B. Geschwindigkeit, Kraft, elektrische und magnetische Feldstärke).

**Schreibweise:** Vektoren werden symbolisch durch Pfeile dargestellt ($\vec{a}, \vec{x}, \ldots$). Die Maßzahl entspricht der Länge des Pfeils und die Richtung der Pfeilspitze. Skalare werden mit $\lambda, \mu, \ldots$ bezeichnet. Der Anfangspunkt $A$ und der Endpunkt $E$ eines Vektors sind beliebig.
### Koordinaten und Ortsvektor
Vektoren können in einem Koordinatensystem in der Ebene oder im Raum durch ihre Komponenten beschrieben werden.
- **Ortsvektor** (vom Ursprung $O$ zum Punkt $P(x; y)$ in der Ebene): $$\vec{r}(P) = \vec{OP} = \begin{pmatrix} x \ y \end{pmatrix}.$$
- **Ortsvektor** im Raum zum Punkt $P(x; y; z)$: $$\vec{r}(P) = \vec{OP} = \begin{pmatrix} x \ y \ z \end{pmatrix}.$$
### Spaltenvektoren
Ein Vektor $\vec{a} = \vec{AE}$ mit Anfangspunkt $A(a_x; a_y)$ und Endpunkt $E(e_x; e_y)$ in der Ebene wird als Spaltenvektor geschrieben als: $$\vec{a} = \vec{AE} = \begin{pmatrix} e_x - a_x \ e_y - a_y \end{pmatrix}$$ Dies gilt analog im Raum und kann auf beliebige Dimension $n$ verallgemeinert werden.
### Betrag eines Vektors
Der **Betrag** $|\vec{a}|$ eines Vektors entspricht der Länge des Pfeils und wird mittels des Satzes des Pythagoras berechnet:
- Ebene: $$|\vec{a}| = \sqrt{a_x^2 + a_y^2}.$$
- Raum: $$|\vec{a}| = \sqrt{a_x^2 + a_y^2 + a_z^2}.$$
### Vektoreigenschaften
1. Zwei Vektoren sind **gleich**, wenn sie in Maßzahl (Betrag) und Richtung übereinstimmen.
2. Zwei Vektoren sind **parallel**, wenn sie dieselbe Richtung haben.
3. Zwei Vektoren sind **antiparallel**, wenn sie entgegengesetzte Richtungen haben.
4. Der Vektor $\vec{b}$ heißt **Gegenvektor** zum Vektor $\vec{a}$, wenn die Beträge gleich und die Richtungen entgegengesetzt sind.
5. Zwei Vektoren heißen **orthogonal**, wenn sie senkrecht aufeinander stehen.
### Spezielle Vektoren
- **Nullvektor** $\vec{0}$: Hat den Betrag Null.
- **Einheitsvektoren** $\vec{e}$: Haben den Betrag eins.
- Die Einheitsvektoren in x-, y- (und z-) Richtung definieren das Koordinatensystem. Als Spaltenvektoren (im Raum) sind sie: $$\vec{e}_x = \begin{pmatrix} 1 \ 0 \ 0 \end{pmatrix}, \quad \vec{e}_y = \begin{pmatrix} 0 \ 1 \ 0 \end{pmatrix}, \quad \vec{e}_z = \begin{pmatrix} 0 \ 0 \ 1 \end{pmatrix}.$$
## 7.2 Vektoroperationen (Vektoroperationen)
### 7.2.1 Grundrechenarten (Grundrechenarten)
#### Vektoraddition
- **Graphisch:** Erfolgt nach der Parallelogrammregel. Die Summe $\vec{a} + \vec{b}$ ist der Verbindungsvektor vom Anfangspunkt von $\vec{a}$ zum Endpunkt von $\vec{b}$, oder die Diagonale im Parallelogramm.
- **Rechnerisch (Komponentenweise):** $$\vec{a} + \vec{b} = \begin{pmatrix} a_x \ a_y \ a_z \end{pmatrix} + \begin{pmatrix} b_x \ b_y \ b_z \end{pmatrix} = \begin{pmatrix} a_x + b_x \ a_y + b_y \ a_z + b_z \end{pmatrix}.$$Dies ist für beliebige Spaltenvektoren verallgemeinerbar.
#### Vektorsubtraktion
- **Graphisch:** Die Differenz $\vec{a} - \vec{b}$ ist die Nebendiagonale im Parallelogramm, genauer der Verbindungsvektor vom Anfangspunkt von $\vec{a}$ zum Anfangspunkt von $\vec{b}$, wenn die Endpunkte von $\vec{a}$ und $\vec{b}$ übereinander liegen.
- **Rechnerisch (Komponentenweise):** $$\vec{a} - \vec{b} = \begin{pmatrix} a_x \ a_y \ a_z \end{pmatrix} - \begin{pmatrix} b_x \ b_y \ b_z \end{pmatrix} = \begin{pmatrix} a_x - b_x \ a_y - b_y \ a_z - b_z \end{pmatrix}.$$
#### Skalarenmultiplikation
Die Multiplikation eines Vektors $\vec{a}$ mit einem Skalar $\lambda$ ergibt einen Vektor $\vec{b} = \lambda \cdot \vec{a}$. Diese Operation wird als „Strecken“ oder „Stauchen“ von Vektoren interpretiert.
- $\vec{b}$ ist parallel zu $\vec{a}$, wenn $\lambda > 0$.
- $\vec{b}$ ist antiparallel zu $\vec{a}$, wenn $\lambda < 0$.
- **Distributivgesetz:** $\lambda \cdot (\vec{a} + \vec{b}) = \lambda \cdot \vec{a} + \lambda \cdot \vec{b}$.
- **Rechnerisch (Komponentenweise):** $$\lambda \cdot \vec{a} = \lambda \cdot \begin{pmatrix} a_x \ a_y \ a_z \end{pmatrix} = \begin{pmatrix} \lambda \cdot a_x \ \lambda \cdot a_y \ \lambda \cdot a_z \end{pmatrix}.$$
#### Linearkombination von Einheitsvektoren
Jeder Vektor $\vec{a}$ kann als Linearkombination der Einheitsvektoren dargestellt werden: $$\vec{a} = \begin{pmatrix} a_x \ a_y \ a_z \end{pmatrix} = a_x \cdot \vec{e}_x + a_y \cdot \vec{e}_y + a_z \cdot \vec{e}_z.$$
### 7.2.2 Skalarprodukt (Skalarprodukt)
Das Skalarprodukt zweier Vektoren $\vec{a}$ und $\vec{b}$ ist eine **skalare Größe**.
- **Definition:** $$\vec{a} \cdot \vec{b} = |\vec{a}| \cdot |\vec{b}| \cdot \cos \phi$$ wobei $0^\circ \leq \phi \leq 180^\circ$ der von $\vec{a}$ und $\vec{b}$ eingeschlossene Winkel ist.
- **Anwendung:** In der Physik ist die Arbeit gleich Kraft in Wegrichtung mal Weg, also dem Anteil von $\vec{F}$ in Richtung des Weges $\vec{s}$ ($\vec{F}_{\parallel}$) mal $\vec{s}$.
- **Skalarprodukt von Spaltenvektoren (Komponentenweise):** $$\vec{a} \cdot \vec{b} = \begin{pmatrix} a_x \ a_y \ a_z \end{pmatrix} \cdot \begin{pmatrix} b_x \ b_y \ b_z \end{pmatrix} = a_x \cdot b_x + a_y \cdot b_y + a_z \cdot b_z.$$
**Wichtige Eigenschaften:**
1. **Kommutativgesetz:** $\vec{a} \cdot \vec{b} = \vec{b} \cdot \vec{a}$.
2. Wenn $\vec{a}$ und $\vec{b}$ senkrecht aufeinander stehen (orthogonal), gilt $\vec{a} \cdot \vec{b} = 0$.
3. Das Skalarprodukt eines Vektors mit sich selbst ist gleich dem quadrierten Betrag: $\vec{a} \cdot \vec{a} = |\vec{a}|^2$.
4. **Distributivgesetz:** $\vec{a} \cdot (\vec{b} + \vec{c}) = \vec{a} \cdot \vec{b} + \vec{a} \cdot \vec{c}$.

### 7.2.3 Vektorprodukt (Vektorprodukt / Kreuzprodukt)
Das Vektorprodukt ist **nur für Vektoren im Raum definiert**. Es ergibt einen **Vektor** $\vec{c} = \vec{a} \times \vec{b}$.
- **Eigenschaften von $\vec{c}$:**
    1. $\vec{c}$ steht senkrecht auf $\vec{a}$ und $\vec{b}$.
    2. Der Betrag ist $|\vec{c}| = |\vec{a}| \cdot |\vec{b}| \cdot \sin \phi$, wobei $\phi$ der Winkel zwischen $\vec{a}$ und $\vec{b}$ ist.
    3. $\vec{a}, \vec{b}$ und $\vec{c}$ bilden ein Rechtssystem; die Richtung ergibt sich aus der **Rechte-Hand-Regel**.
- **Geometrische Bedeutung:** Der Betrag des Vektorprodukts entspricht der **Fläche** des von $\vec{a}$ und $\vec{b}$ aufgespannten Parallelogramms.
- **Anwendung:** Z.B. zur Berechnung des Drehmoments $\vec{M}$.
- **Vektorprodukt von Spaltenvektoren:** $$\begin{pmatrix} a_x \ a_y \ a_z \end{pmatrix} \times \begin{pmatrix} b_x \ b_y \ b_z \end{pmatrix} = \begin{pmatrix} a_y b_z - a_z b_y \ a_z b_x - a_x b_z \ a_x b_y - a_y b_x \end{pmatrix}.$$

**Wichtige Eigenschaften:**
1. **Kein Kommutativgesetz:** $\vec{a} \times \vec{b} = -\vec{b} \times \vec{a}$.
2. Wenn $\vec{a}$ und $\vec{b}$ parallel sind, gilt $\vec{a} \times \vec{b} = \vec{0}$.
3. **Distributivgesetz:** $\vec{a} \times (\vec{b} + \vec{c}) = \vec{a} \times \vec{b} + \vec{a} \times \vec{c}$.

### 7.2.4 Spatprodukt (Spatprodukt)
Das Spatprodukt ist eine **skalare Größe** von drei Vektoren $\vec{a}, \vec{b}, \vec{c}$ und ist **nur für Vektoren im Raum definiert**.
- **Definition:** $$[\vec{a}\vec{b}\vec{c}] = \vec{a} \cdot (\vec{b} \times \vec{c}).$$
- **Geometrische Bedeutung:** Der Betrag des Spatprodukts entspricht dem **Volumen** des von $\vec{a}, \vec{b}$ und $\vec{c}$ aufgespannten Parallelepipeds.

**Eigenschaften:**
1. Bei einer **zyklischen Vertauschung** der Vektoren bleibt das Spatprodukt unverändert: $[\vec{a}\vec{b}\vec{c}] = [\vec{b}\vec{c}\vec{a}] = [\vec{c}\vec{a}\vec{b}]$.
2. Bei jeder anderen Vertauschung ändert das Spatprodukt das Vorzeichen: $[\vec{a}\vec{b}\vec{c}] = - [\vec{a}\vec{c}\vec{b}]$.
3. Wenn $\vec{a}, \vec{b}$ und $\vec{c}$ in einer Ebene liegen, ist $[\vec{a}\vec{b}\vec{c}] = 0$.