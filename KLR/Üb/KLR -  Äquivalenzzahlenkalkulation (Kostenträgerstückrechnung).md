### 1. Theoretischer Hintergrund & Relevanz
Die **Äquivalenzzahlenkalkulation** ist eine erweiterte Form der Divisionskalkulation. Sie wird bei der **Sortenfertigung** angewendet. 

* **Voraussetzung:** Das Unternehmen stellt mehrere Produktvarianten (Sorten) her, die auf denselben Produktionsanlagen mit ähnlichen Rohstoffen erzeugt werden (z. B. verschiedene Biersorten, Schokoladentafeln, Papierstärken oder Walzstahlprodukte).
* **Das Prinzip:** Da sich die Produkte in ihren Kosten stark ähneln, werden ihre Kostenstrukturen über Verhältniswerte – die sogenannten **Äquivalenzzahlen (ÄZ)** – ausgedrückt. Ein Standardprodukt (Basissorte) erhält die Äquivalenzzahl $1,0$. Alle anderen Sorten werden relativ dazu bewertet (z. B. $1,5$ für $50\,\%$ höhere Kosten).

---

### 2. Das Kalkulationsschema im Klausur-Ablauf

Die Berechnung erfolgt immer in vier systematischen Schritten:

| Schritt | Rechenschritt | Formel / Erklärung |
| :--- | :--- | :--- |
| **1. Recheneinheiten** | $\text{Menge} \cdot \text{Äquivalenzzahl}$ | Ermittlung der Recheneinheiten (RE) pro Sorte. |
| **2. Summe RE** | $\sum \text{Recheneinheiten}$ | Addition aller RE der Periode zur Gesamtsumme. |
| **3. Basiswert** | $\frac{\text{Gesamtkosten}}{\text{Summe RE}}$ | Berechnung der Kosten für eine einzige Recheneinheit (RE-Satz). |
| **4. Stückkosten** | $\text{Basiswert} \cdot \text{Äquivalenzzahl}$ | Ermittlung der finalen Selbstkosten pro Stück/Einheit der jeweiligen Sorte. |

---

### 3. Konkretes Berechnungsbeispiel

#### Ausgangsdaten
Gesamtkosten einer Brauerei: $7.000\ \text{€}$

* **Sorte A (Standard):** Produktionsmenge = $2.000\ \text{Liter}$ | $\text{ÄZ} = 1,0$
* **Sorte B (Premium):** Produktionsmenge = $1.000\ \text{Liter}$ | $\text{ÄZ} = 1,5$

#### Mathematische Umsetzung
1.  **Berechnung der Recheneinheiten (RE):**
    * Sorte A: $2.000\ \text{l} \cdot 1,0 = 2.000\ \text{RE}$
    * Sorte B: $1.000\ \text{l} \cdot 1,5 = 1.500\ \text{RE}$
    * **Gesamte RE** $= 2.000 + 1.500 = \mathbf{3.500\ \text{RE}}$

2.  **Berechnung des Basiswerts (Kosten je RE):**
    $$\text{Kosten je RE} = \frac{7.000\ \text{€}}{3.500\ \text{RE}} = \mathbf{2\ \text{€ / RE}}$$

3.  **Ermittlung der Stückkosten (Selbstkosten je Liter):**
    * **Sorte A:** $2\ \text{€/RE} \cdot 1,0 = \mathbf{2,00\ \text{€ / Liter}}$
    * **Sorte B:** $2\ \text{€/RE} \cdot 1,5 = \mathbf{3,00\ \text{€ / Liter}}$

---

### 4. Bewertung des Verfahrens

| Vorteile | Nachteile / Klausurhinweis |
| :--- | :--- |
| **Effizienz:** Deutlich weniger Aufwand als eine differenzierende Zuschlagskalkulation mit separaten Kostenstellen. | **Gefahr von Starrheit:** Die Äquivalenzzahlen basieren oft auf historischen Daten oder Schätzungen. Ändern sich Produktionsbedingungen, stimmen die Relationen nicht mehr. |
| **Verursachungsgerecht:** Bildet geringe Kostenunterschiede bei verwandten Produkten mathematisch einfach ab. | **Klausurfalle:** Achte darauf, im letzten Schritt die Stückkosten zu berechnen ($\text{Basiswert} \cdot \text{ÄZ}$) und nicht fälschlicherweise die Gesamt-RE einer Sorte zu verwenden. |