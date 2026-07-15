Vergleich zwischen dem Real-case-Szenario und einem extremen Worst-case-Szenario (Sensitivitätsanalyse) auf Basis der **Durchschnittswertmethode**.

---

## 🟢 1. Real-case-Szenario

### Basisdaten & Kostenblöcke (jährlich)
* **Anschaffungskosten ($A$):** 6.000.000 €
* **Liquidationswert ($L_n$):** 800.000 €
* **Nutzungsdauer ($n$):** 20 Jahre
* **Kalkulatorischer Zinssatz ($i$):** 8 % (0,08)

* **Kalkulatorische Abschreibung:** 
  $$\text{AfA} = \frac{6.000.000 - 800.000}{20} = 260.000 \text{ €/Jahr}$$
* **Kalkulatorische Zinsen:** 
  $$\text{Zinsen} = \frac{6.000.000 + 800.000}{2} \cdot 0,08 = 272.000 \text{ €/Jahr}$$
* **Laufende Betriebskosten:** 50.000 € (Betrieb) + 20.000 € (Pacht) + 15.000 € (Overhead) = 85.000 €/Jahr

### Kennzahlen & Ergebnisse (Real-case)
* **Gesamtkosten ($K$):** **617.000 €/Jahr** ($260.000 + 272.000 + 85.000$)
* **Ausbeute ($x$):** **7.200.000 kWh/Jahr**
* **Stückkosten ($k$):** **0,08569 €/kWh** ($\frac{617.000}{7.200.000}$)
* **Stückgewinn ($g$):** **0,1143 €/kWh** ($0,20 - 0,08569$) bei $p = 0,20\text{ €}$
* **Gesamtgewinn ($G$):** **823.032 €/Jahr** (exakt: 823.000 €)

---

## 🔴 2. Worst-case-Szenario (Sensitivitätsanalyse)

### Modifizierte Parameter
* **Anschaffungskosten ($A_{neu}$):** 7.200.000 € (+20 %)
* **Liquidationswert ($L_{n,neu}$):** 0 € (kein Erlös)
* **Nutzungsdauer ($n_{neu}$):** 18 Jahre
* **Kalkulatorischer Zinssatz ($i_{neu}$):** 10 % (0,10)
* **Ausbeute ($x_{neu}$):** 5.760.000 kWh (-20 %)
* **Betriebskosten (Betrieb):** 75.000 € (+50 %) | *Pacht & Overhead konstant*

### Kostenblöcke (jährlich im Worst-case)
* **Kalkulatorische Abschreibung:** 
  $$\text{AfA} = \frac{7.200.000 - 0}{18} = 400.000 \text{ €/Jahr}$$
* **Kalkulatorische Zinsen:** 
  $$\text{Zinsen} = \frac{7.200.000 + 0}{2} \cdot 0,10 = 360.000 \text{ €/Jahr}$$
* **Laufende Betriebskosten:** 75.000 € (Betrieb) + 20.000 € (Pacht) + 15.000 € (Overhead) = 110.000 €/Jahr

### Kennzahlen & Ergebnisse (Worst-case)
* **Gesamtkosten ($K$):** **870.000 €/Jahr** ($400.000 + 360.000 + 110.000$)
* **Ausbeute ($x$):** **5.760.000 kWh/Jahr**
* **Stückkosten ($k$):** **0,1510 €/kWh** ($\frac{870.000}{5.760.000}$)
* **Stückgewinn ($g$):** **0,0490 €/kWh** ($0,20 - 0,1510$)
* **Gesamtgewinn ($G$):** **282.000 €/Jahr** ($0,04896 \cdot 5.760.000$)

---

## 🏛️ Ökonomischer Quervergleich

| Kennzahl | Real-case-Szenario | Worst-case-Szenario | Differenz |
| :--- | :---: | :---: | :---: |
| **Gesamtkosten ($K$)** | 617.000 € | 870.000 € | +253.000 € (+41 %) |
| **Ausbeute ($x$)** | 7.200.000 kWh | 5.760.000 kWh | -1.440.000 kWh (-20 %) |
| **Stückkosten ($k$)** | 0,08569 € | 0,1510 € | +0,06531 € (+76 %) |
| **Gesamtgewinn ($G$)** | **823.032 €** | **282.000 €** | **-541.032 € (-66 %)** |

> [!info] **Fazit der Risikoanalyse**
> Trotz massiver, kumulierter Verschlechterungen aller Variablen (Kostensteigerungen bei gleichzeitigem Einbruch der Ausbeute um 20 %) verbleibt das Projekt auch im Worst Case in der **Gewinnzone** ($G = 282.000\text{ €}$). Das Projekt weist somit eine hohe Robustheit auf.