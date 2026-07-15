### 1. Theoretischer Kontext
Die **Abschreibung** erfasst den wertmäßigen Verzehr von Anlagegütern im Zeitverlauf. Neben der standardmäßigen linearen Abschreibung gibt es Verfahren, die den tatsächlichen Werteverzehr oder den wirtschaftlichen Nutzenverlauf präziser abbilden sollen:
* **Geometrisch-degressive Abschreibung:** Trägt dem Umstand Rechnung, dass der Wertverlust zu Beginn der Nutzungsdauer oft am höchsten ist (z. B. bei Fahrzeugen oder IT).
* **Leistungsabschreibung (nach Nutzung):** Koppelt den periodischen Werteverzehr direkt an die tatsächliche Inanspruchnahme (z. B. Maschinenstunden, Kilometerleistung).

---

### 2. Geometrisch-degressive Abschreibung (Aufgabe 4.2)
Das zentrale Kennzeichen ist ein **konstanter Abschreibungsprozentsatz**, der jährlich auf den jeweiligen **Restbuchwert (RBW)** des Vorjahres angewendet wird. Dadurch sinken die Abschreibungsbeträge im Zeitverlauf degressiv.

#### Berechnung des Abschreibungssatzes ($p$)
Die Ermittlung auf einen definierten Endwert ($R$) bei gegebenem Anfangswert ($A$) erfolgt über die Formel:
$$p = 1 - \sqrt[n]{\frac{R}{A}}$$

Für die Werte aus image_26c6f2.jpg ($A = 10.000\ \text{€}$, $R = 1\ \text{€}$, $n = 3\ \text{Jahre}$):
$$p = 1 - \sqrt[3]{\frac{1}{10.000}} \approx 0,9536\ \text{bzw.}\ \mathbf{95,3600\%}$$

#### Abschreibungsverlauf (Präzise vs. Gerundet)

| Jahr | Basis (RBW Vorjahr) | Abschreibungsbetrag (exakt) | Abschreibungsbetrag (mit $p=0,9536$) | Restbuchwert (RBW) |
| :--- | :--- | :--- | :--- | :--- |
| **0** | - | - | - | $10.000,0000\ \text{€}$ |
| **1** | $10.000,0000\ \text{€}$ | $9.535,8411\ \text{€}$ | $\mathbf{9.536,0000\ \text{€}}$ | $464,0000\ \text{€}$ |
| **2** | $464,0000\ \text{€}$ | $442,6145\ \text{€}$ | $\mathbf{442,4704\ \text{€}}$ | $21,5296\ \text{€}$ |
| **3** | $21,5296\ \text{€}$ | $20,5443\ \text{€}$ | $\mathbf{20,5306\ \text{€}}$ | $\approx 1,0000\ \text{€}$ |

---

### 3. Leistungsabschreibung / Nach Nutzung (Aufgabe 4.3)
Hierbei richtet sich die Abschreibung nach den tatsächlich geleisteten Betriebsstunden.

* **Gesamtleistung:** $5.000 + 4.000 + 4.500 = \mathbf{13.500\ \text{Stunden}}$
* **Abschreibungssatz pro Stunde:** 
  $$\frac{10.000\ \text{€}}{13.500\ \text{Stunden}} \approx \mathbf{0,7407\ \text{€ / Stunde}}$$

#### Jährliche Abschreibungsbeträge

* **Jahr 1 ($5.000\ \text{Std.}$):** $5.000 \cdot 0,7407\ \text{€} = \mathbf{3.703,5000\ \text{€}}$ *(Exakt: $3.703,7037\ \text{€}$)*
* **Jahr 2 ($4.000\ \text{Std.}$):** $4.000 \cdot 0,7407\ \text{€} = \mathbf{2.962,8000\ \text{€}}$ *(Exakt: $2.962,9630\ \text{€}$)*
* **Jahr 3 ($4.500\ \text{Std.}$):** $4.500 \cdot 0,7407\ \text{€} = \mathbf{3.333,1500\ \text{€}}$ *(Exakt: $3.333,3333\ \text{€}$)*

> [!TIP] Klausur-Hinweis zu Rundungsdifferenzen
> Bei fortgeführten Rundungen ($0,7407\ \text{€}$) summiert sich der Gesamtabschreibungsbetrag auf $9.999,45\ \text{€}$. Um exakt auf einen Restwert von $0\ \text{€}$ zu kommen, wird in der Praxis im letzten Jahr der verbleibende Restbuchwert als Abschreibung angesetzt oder konsequent mit dem ungerundeten Bruch im Taschenrechner gerechnet ($3.333,33\ \text{€}$).