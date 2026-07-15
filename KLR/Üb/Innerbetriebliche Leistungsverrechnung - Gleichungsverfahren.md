### 1. Theoretischer Kontext
Das **Gleichungsverfahren** (auch mathematisches Verfahren) ist das exakteste Verfahren der innerbetrieblichen Leistungsverrechnung im Betriebsabrechnungsbogen (BAB). Im Gegensatz zum Treppen- oder Anbauverfahren berücksichtigt es **gegenseitige Leistungsbeziehungen** (Verflechtungen) zwischen den Vorkostenstellen (Hilfskostenstellen) mathematisch exakt über ein lineares Gleichungssystem.

### 2. Mathematischer Ansatz (Beispiel aus image_25f0c3.jpg)
Jede Vorkostenstelle wird durch eine eigene Gleichung repräsentiert. Die Grundstruktur lautet:
$$\text{Gesamtkosten} = \text{Primärkosten} + \text{Sekundärkosten (Leistungsbezug)}$$

Bei vorhandenem **Eigenverbrauch** (Kostenstelle leistet an sich selbst) wird dieser direkt von der Gesamtleistung auf der linken Gleichungsseite subtrahiert (Netto-Ansatz), um den externen Verrechnungspreis zu bestimmen.

#### Gleichungssystem aufstellen (Aufgabe 5.1)
* **Variablen:** 
  * $x =$ Verrechnungspreis für $V_1$ [€/LE]
  * $y =$ Verrechnungspreis für $V_2$ [€/LE]
* **Gleichung für $V_1$:** Total $600\ \text{LE} - 20\ \text{LE}$ (Eigenverbrauch) $= 580\ \text{LE}$ abgetretene Leistung.
  $$580x = 8.560 + 600y$$
* **Gleichung für $V_2$:** Total $6.000\ \text{LE} - 200\ \text{LE}$ (Eigenverbrauch) $= 5.800\ \text{LE}$ abgetretene Leistung.
  $$5.800y = 6.480 + 30x$$

---

### 3. Berechnung der Verrechnungspreise (Aufgabe 5.2)
Durch Auflösung des linearen Gleichungssystems (z. B. Einsetzungsverfahren) ergeben sich die exakten Verrechnungssätze pro Leistungseinheit (LE):

* **Verrechnungspreis $V_1$ ($x$):** $\mathbf{16,00\ \text{€ / LE}}$
* **Verrechnungspreis $V_2$ ($y$):** $\mathbf{1,20\ \text{€ / LE}}$

---

### 4. Belastung der Endkostenstellen (Aufgabe 5.3)
Die sekundäre Kostenverrechnung erfasst ausschließlich die Leistungsströme, die an die Haupt- bzw. Endkostenstellen ($E_1, E_2, E_3$) fließen. 

| Vorkostenstelle | Leistungsabgabe an Endkostenstellen ($E_1 + E_2 + E_3$) | Verrechnungssatz | Sekundärkosten gesamt |
| :--- | :--- | :--- | :--- |
| **$V_1$** | $280 + 170 + 100 = 550\ \text{LE}$ | $16,00\ \text{€/LE}$ | $8.800\ \text{€}$ |
| **$V_2$** | $2.000 + 1.900 + 1.300 = 5.200\ \text{LE}$ | $1,20\ \text{€/LE}$ | $6.240\ \text{€}$ |
| **Summe** | | | **$\mathbf{15.040\ \text{€}}$** |

> [!NOTE] Key Takeaway für Klausuren
> Der Eigenverbrauch einer Kostenstelle erhöht nicht die Belastung der Hauptkostenstellen, sondern wird mathematisch über die Bereinigung der Basis-Leistungsmenge (Netto-Methode) neutralisiert. Die Summe der primären Gemeinkosten der Vorkostenstellen ($8.560\ \text{€} + 6.480\ \text{€} = 15.040\ \text{€}$) entspricht nach dem Gleichungsverfahren exakt der Summe der weiterverrechneten Sekundärkosten auf die Endkostenstellen.