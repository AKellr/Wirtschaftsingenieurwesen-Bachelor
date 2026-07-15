## 📥 Projektparameter im Szenarienvergleich
Analyse einer Investition in eine Windkraftanlage mittels der **Durchschnittswertmethode** bei gesetzlich garantierter Einspeisevergütung (Fixpreis) über die gesamte Laufzeit.

| Parameter | Real-Case-Szenario | Change ($\Delta$) | Worst-Case-Szenario |
| :--- | :---: | :---: | :---: |
| **Anschaffungskosten ($A_0$)** | 6.000.000 € | $+20\%$ | 7.200.000 € |
| **Liquidationserlös ($L_n$)** | 800.000 € | $\to 0$ | 0 € |
| **Nutzungsdauer ($n$)** | 20 Jahre | $-2\text{ Jahre}$ | 18 Jahre |
| **Kalk. Zinssatz ($i$)** | 8 % p.a. | $+2\%$ | 10 % p.a. |
| **Ausbeute ($x$)** | 7.200.000 kWh/Jahr | $-20\%$ | 5.760.000 kWh/Jahr |
| **Einspeisepreis ($p$)** | 0,20 €/kWh | *unverändert* | 0,20 €/kWh |
| **Betriebskosten p.a.** | 50.000 € | $+50\%$ | 75.000 € |
| **Pachtkosten p.a.** | 20.000 € | *unverändert* | 20.000 € |
| **Overheadkosten p.a.** | 15.000 € | *unverändert* | 15.000 € |

---

## 📐 Mathematisches Instrumentarium
* Die Anschaffungskosten ($A_0$) werden als einmalige Auszahlung über die **kalkulatorische Abschreibung** (Wertverzehr) und die **kalkulatorischen Zinsen** (Kapitalbindungskosten) periodengerecht auf die Jahre verteilt.

$$\text{kalk. Abschreibung} = \frac{A_0 - L_n}{n} \qquad \text{kalk. Zinsen} = \frac{A_0 + L_n}{2} \cdot i$$

---

## 📊 Kosten- und Ergebnisrechnung

| Position | Berechnung Real-Case | Real-Case | Berechnung Worst-Case | Worst-Case |
| :--- | :--- | :---: | :--- | :---: |
| **kalk. Abschreibung** | $\frac{6.000.000 - 800.000}{20}$ | 260.000 € | $\frac{7.200.000 - 0}{18}$ | 400.000 € |
| **kalk. Zinsen** | $\frac{6.000.000 + 800.000}{2} \cdot 0{,}08$ | 272.000 € | $\frac{7.200.000 + 0}{2} \cdot 0{,}10$ | 360.000 € |
| Betriebskosten p.a. | *gegeben* | 50.000 € | $50.000 \cdot 1{,}5$ | 75.000 € |
| Pachtkosten p.a. | *gegeben* | 20.000 € | *gegeben* | 20.000 € |
| Overheadkosten p.a. | *gegeben* | 15.000 € | *gegeben* | 15.000 € |
| **Gesamtkosten ($K$)** | **Summe p.a.** | **617.000 €** | **Summe p.a.** | **870.000 €** |

---

## 📐 Wirtschaftliche Kennzahlen im Vergleich

### 1. Stückkosten ($k = \frac{K}{x}$)
* **Real-Case:** $\frac{617.000\text{ €}}{7.200.000\text{ kWh}} = \mathbf{0{,}0857\text{ €/kWh}}$
* **Worst-Case:** $\frac{870.000\text{ €}}{5.760.000\text{ kWh}} = \mathbf{0{,}1510\text{ €/kWh}}$

### 2. Stückgewinn ($g = p - k$)
* **Real-Case:** $0{,}20\text{ €} - 0{,}0857\text{ €} = \mathbf{0{,}1143\text{ €/kWh}}$
* **Worst-Case:** $0{,}20\text{ €} - 0{,}1510\text{ €} = \mathbf{0{,}0490\text{ €/kWh}}$

### 3. Jährlicher Gesamtgewinn ($G = g \cdot x$)
* **Real-Case:** $0{,}1143\text{ €} \cdot 7.200.000\text{ kWh} = \mathbf{822.960\text{ €/Jahr}}$
* **Worst-Case:** $0{,}0490\text{ €} \cdot 5.760.000\text{ kWh} = \mathbf{282.240\text{ €/Jahr}}$

---

## 🏛️ Sensitivitätsurteil

> [!success] **Ergebnis der Risikoanalyse**
> Die Sensitivitätsanalyse (Worst-Case) simuliert eine kumulierte Verschlechterung aller wesentlichen Risikotreiber (Investitions- und Betriebskostensteigerung, Zinsanstieg, Ertragsminderung und Laufzeitverkürzung). 
> 
> **Ergebnis:** Das Projekt reagiert sensitiv auf die Parameteränderungen (Gewinnrückgang um ca. $65{,}7\%$), verbleibt jedoch mit einem jährlichen Gesamtgewinn von **282.240 €** auch unter Extrembedingungen in der **Gewinnzone**. Die Investition erweist sich damit als robust.