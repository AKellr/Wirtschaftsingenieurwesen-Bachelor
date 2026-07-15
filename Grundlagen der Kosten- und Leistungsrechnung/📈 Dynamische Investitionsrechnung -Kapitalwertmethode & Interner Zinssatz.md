## 1. Theoretisches Fundament & Definitionen
Die dynamische Investitionsrechnung berücksichtigt den zeitlichen Anfall von Zahlungsströmen durch das Konzept des Zeitwerts des Geldes. Zukünftige Zahlungsströme werden mittels Abzinsung (Diskontierung) vergleichbar gemacht.

- **t**: Zeitpunkt der Periode (t = 0: Anschaffung, t = 1 bis n: Nutzungsdauer)
- **E(t)**: Einzahlungen im Zeitpunkt t
- **A(t)**: Auszahlungen im Zeitpunkt t
- **Z(t)**: Netto-Zahlungsstrom im Zeitpunkt t -> Z(t) = E(t) - A(t)
- **i**: Kalkulationszinssatz (geforderte Mindestrentabilität)
- **C_0 (NPV)**: Kapitalwert (Net Present Value) zum Zeitpunkt t = 0
- **IKS (IRR)**: Interner Zinssatz (tatsächliche Rendite der Investition, bei der C_0 = 0 wird)

---

## 2. Mathematische Algorithmen (Standard-Notation)

### Barwert-Ermittlung (Diskontierung)
Barwert = Z(t) / (1 + i)^t

### Kapitalwert (C_0)
C_0 = -Anschaffungsauszahlung + Summe von t=1 bis n [ Z(t) / (1 + i)^t ]
*Hinweis:* Der Liquidationserlös (Verkaufserlös am Ende) wird dem Einzahlungsstrom E(n) im letzten Jahr t = n hinzugerechnet.

### Lineare Interpolation (Näherung für Internen Zinssatz)
IKS = i_1 - C_1 * [ (i_2 - i_1) / (C_2 - C_1) ]
- **i_1**: Niedrigerer Zinssatz (liefert positiven Kapitalwert C_1)
- **i_2**: Höherer Zinssatz (liefert negativen Kapitalwert C_2)

---

## 3. Strukturiertes Berechnungsbeispiel (Aufgabe 2)

### Zahlungsreihe & Barwert-Vergleichstabelle

| Zeitpunkt (t) | Einzahlung E(t) | Auszahlung A(t) | Cashflow Z(t) | Barwert bei i = 5% | Barwert bei i = 7% |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **t = 0** | 0 | 1.200.000 | -1.200.000 | -1.200.000,00 EUR | -1.200.000,00 EUR |
| **t = 1** | 480.000 | 500.000 | -20.000 | -19.047,62 EUR | -18.691,59 EUR |
| **t = 2** | 890.000 | 620.000 | +270.000 | +244.897,96 EUR | +235.828,46 EUR |
| **t = 3** | 1.040.000 | 740.000 | +300.000 | +259.151,36 EUR | +244.889,35 EUR |
| **t = 4** | 1.340.000 | 860.000 | +480.000 | +394.897,19 EUR | +366.188,27 EUR |
| **t = 5** | 1.310.000 * | 830.000 | +480.000 | +376.092,56 EUR | +342.232,81 EUR |
| **KAPITALWERT**| | | | **C_1 = +55.991,45 EUR**| **C_2 = -29.550,70 EUR**|

*\*Inklusive Liquidationserlös von 50.000 EUR (1.260.000 + 50.000 = 1.310.000 EUR)*

### Wirtschaftliche Beurteilung (Kapitalwertmethode)
- **Kriterium:** C_0 > 0
- **Befund:** Da C_1 (+55.991,45 EUR) positiv ist, deckt die Investition die Anschaffungskosten, erzielt die Mindestverzinsung von 5% und generiert zusätzlichen Vermögenszuwachs. 
- **Entscheidung:** Die Investition ist absolut vorteilhaft.

---

## 4. Berechnung des Internen Zinssatzes (IKS)

### Mathematischer Durchlauf (Lineare Interpolation)
Einsetzen der ermittelten Stützpunkte in das Näherungsverfahren:

1. Differenzen bestimmen:
   - Zinsdifferenz (Zähler): 0,07 - 0,05 = 0,02
   - Kapitalwertdifferenz (Nenner): -29.550,70 - 55.991,45 = -85.542,15

2. Bruch auflösen:
   - 0,02 / -85.542,15 = -0,000000233791

3. Finaler Zinssatz:
   - IKS = 0,05 - [ 55.991,45 * (-0,000000233791) ]
   - IKS = 0,05 - (-0,013091)
   - IKS = 0,05 + 0,013091 = 0,063091 -> **6,31%**

### Wirtschaftliche Beurteilung (IKS-Methode)
- **Kriterium:** IKS >= i
- **Vergleich:** 6,31% > 5,00%
- **Fazit:** Die tatsächliche Eigenrendite der Maschine liegt bei ca. 6,31%. Da die interne Rendite die geforderten Kapitalkosten (5%) überschreitet, bestätigt auch diese Methode die Vorteilhaftigkeit der Investition.