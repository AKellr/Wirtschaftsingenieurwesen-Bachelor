[[GDE]]
# Notizen zu Kapitel 3: Grundgesetze (Notes on Chapter 3: Basic Laws)

## Einführung (Introduction)

Die vom deutschen Physiker Gustav Robert Kirchhoff (1824–1887) formulierten Gesetze sind zentral für die Analyse elektrischer Netzwerke. Sie beschreiben die Abhängigkeiten der Ströme in einem Knoten (node) und der Spannungen in einer Masche (mesh). Daraus lassen sich Regeln für die Reihen- (series) und Parallelschaltung (parallel connection) von Widerständen sowie die Spannungs- und Stromteilerformeln ableiten.

---

## 3.1 Knotenregel (1. Kirchhoffsches Gesetz) (Node Rule / 1st Kirchhoff's Law)

- Ein **Knoten** (node) ist ein Punkt in einer Schaltung, an dem mehrere Leitungen verbunden sind.
- In einem Knoten werden keine Ladungen gespeichert (no charges are stored).
- **1. Kirchhoffsches Gesetz:** In einem Knoten ist die **Summe der zufliessenden Ströme** (sum of inflowing currents) gleich der **Summe der abfliessenden Ströme** (sum of outflowing currents).
- Beispielhafte Darstellung: $$I_1 + I_2 + I_3 = I_4 + I_5$$
- Alternativ kann das Gesetz so formuliert werden, dass die **Summe aller vorzeichenbehafteten Ströme** (sum of all signed currents) eines Knotens null ist. $$I_1 + I_2 + I_3 - I_4 - I_5 = 0$$

---

## 3.2 Maschenregel (2. Kirchhoffsches Gesetz) (Mesh Rule / 2nd Kirchhoff's Law)

- Eine **Masche** (mesh) ist ein geschlossener Weg (closed path) in einem Netzwerk.
- **2. Kirchhoffsches Gesetz:** Die **Summe aller Spannungen** (sum of all voltages), die entlang eines geschlossenen Weges auftreten, ist null.
- Spannungen in Umlaufrichtung werden positiv, entgegengesetzt negativ gezählt (Voltages in the path direction are counted positive, counter direction negative).
- Beispielhafte Darstellung: $$U_1 + U_2 - U_3 - U_4 + U_5 = 0$$
- In einem Netzwerk können mehrere Maschengleichungen aufgestellt werden, jedoch enthält die Gleichung für die grosse Masche oft keine neue Information, wenn sie die Summe der kleineren, unabhängigen Maschen darstellt.

---

## 3.3 Reihenschaltung von Widerständen (Series Connection of Resistors)

- Bei einer Reihenschaltung (series connection) sind Bauelemente hintereinander geschaltet.
- Der **gleiche Strom** (same current) fliesst in allen Bauelementen einer Reihenschaltung.
- Die Gesamtspannung $U$ ist die Summe der Teilspannungen $U_k$ (The total voltage $U$ is the sum of the partial voltages $U_k$): $$U = U_1 + U_2 + U_3$$
- Unter Anwendung des Ohmschen Gesetzes ($U_k = R_k \cdot I$) ergibt sich: $$U = (R_1 + R_2 + R_3) \cdot I$$
- Der Widerstandswert $R$ der Reihenschaltung ist gleich der **Summe der Teilwiderstände** (sum of the partial resistances): $$R = \sum_{i=1}^{n} R_i = R_1 + R_2 + \cdots + R_n$$

---

## 3.4 Spannungsteiler (Voltage Divider)

- Der Spannungsteiler wird verwendet, um aus einer Spannung $U$ eine kleinere Spannung $U_2$ zu erzeugen.
- Die Spannung über dem Widerstand $R_2$ berechnet sich durch die **Spannungsteilerformel** (voltage divider formula): $$U_2 = \frac{R_2}{R_1 + R_2} \cdot U$$
- **Wichtig:** Diese Formel ist nur gültig, falls der Spannungsteiler **unbelastet** (unloaded) ist, d. h. wenn der Laststrom $I_L = 0$ ist.

---

## 3.5 Parallelschaltung von Widerständen (Parallel Connection of Resistors)

- Bei der Parallelschaltung (parallel connection) rechnet man vorteilhaft mit dem **Leitwert** (conductance) $G$, wobei $G = 1/R$ ist.
- Der Leitwert $G$ hat die Einheit Siemens (S).
- Der Gesamtleitwert $G$ der Parallelschaltung ist gleich der **Summe der Leitwerte der Teilwiderstände** (sum of the conductances of the partial resistors): $$G = \sum_{i=1}^{n} G_i = G_1 + G_2 + \cdots + G_n$$
- Der Gesamtwiderstand $R$ ergibt sich somit: $$R = \frac{1}{G} = \frac{1}{\frac{1}{R_1} + \frac{1}{R_2} + \cdots + \frac{1}{R_n}}$$
- Für die Parallelschaltung zweier Widerstände $R_1$ und $R_2$ gilt: $$R = \frac{R_1 \cdot R_2}{R_1 + R_2}$$

---

## 3.6 Stromteiler (Current Divider)

- Eine Parallelschaltung wird auch als Stromteiler (current divider) bezeichnet, da der Gesamtstrom $I$ auf die Teilströme $I_1, I_2$ aufgeteilt wird.
- Die **Stromteilerformel** (current divider formula) für den Strom $I_2$ durch $R_2$ lautet: $$I_2 = \frac{G_2}{G_1 + G_2} \cdot I$$ $$I_2 = \frac{R_1}{R_1 + R_2} \cdot I$$
## 3.7 Spannungsmessung (Voltage Measurement)

- Ein Spannungsmessgerät (Voltmeter) wird zwischen den beiden Messpunkten angeschlossen (is connected between the two measuring points).
- Der innere Widerstand (internal resistance) des Voltmeters sollte **möglichst hoch** (as high as possible) sein, um die Schaltung kaum zu belasten und Messfehler zu minimieren.
- Zur Messbereichserweiterung (range extension) bei höheren Spannungen wird ein Spannungsteiler vorgeschaltet.

---

## 3.8 Strommessung (Current Measurement)

- Zur Strommessung (current measurement) wird das Messgerät in einen Zweig der Schaltung **eingefügt** (inserted into a branch).
- Ein Spannungsabfall (voltage drop) $\Delta U_{mess}$ über dem Messgerät verfälscht das Messresultat.
- Der innere Widerstand des Strommessgeräts (Ammeter) muss **möglichst klein** (as small as possible) sein.
- Zur Messbereichserweiterung wird ein Widerstand $R_p$ (Shunt) parallel zum Amperemeter geschaltet, wodurch ein Stromteiler realisiert wird.
- Der Widerstand $R_p$ wird so dimensioniert, dass nur ein Teil des Gesamtstroms durch das Amperemeter fliesst.