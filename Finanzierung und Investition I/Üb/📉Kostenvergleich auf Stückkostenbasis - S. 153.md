## 1. Rechenweg & Ermittlung der Werte

### Alte Investition
* **Kalkulatorische Abschreibung = 0 €**
* **Kalkulatorische Zinsen = 0 €**
  * *Begründung:* Da kein Liquidationswert vorhanden ist ($L_n = 0$) und die historischen Anschaffungskosten der alten Maschine versunkene Kosten ("Sunk Costs") darstellen, ist kein Kapital mehr gebunden. Die alten Kapitalkosten sind für die Entscheidung irrelevant.
* **Summe relevanter Kosten:** * Fixe Betriebskosten (7.000 €) + Variable Betriebskosten (176.000 €) = **183.000 €**

### Neue Investition
* **Kalkulatorische Abschreibung:** * Anschaffungskosten / Nutzungsdauer = 140.000 € / 10 Jahre = **14.000 €**
* **Kalkulatorische Zinsen (i = 10 %):** * (Anschaffungskosten / 2) * Zinssatz = (140.000 € / 2) * 0,10 = **7.000 €**
* **Summe relevanter Kosten:** * Abschreibung (14.000 €) + Zinsen (7.000 €) + Fixe Betriebskosten (20.000 €) + Variable Betriebskosten (164.200 €) = **205.200 €**

---

## 2. Ergänzte Ergebnismatrix

| Kosten in Euro | Alte Investition | Neue Investition |
| :--- | :--- | :--- |
| Anschaffungskosten | 100.000 | 140.000 |
| Nutzungsdauer in Jahren | 8 | 10 |
| Auslastung in Leistungseinheiten je Jahr | 20.000 | 20.000 |
| **Kalkulatorische Abschreibung** | **0** | **14.000** |
| **Kalkulatorische Zinsen, i = 10 %** | **0** | **7.000** |
| Fixe Betriebskosten | 7.000 | 20.000 |
| Variable Betriebskosten | 176.000 | 164.200 |
| **Summe relevanter Kosten** | **183.000** | **205.200** |

## 3. Entscheidung
* **Entscheidung:** Die **Alte Investition beibehalten** (die Ersatzinvestition wird abgelehnt).
* **Begründung:** Ein Ersatz ist laut der Bedingung auf der Folie nur wirtschaftlich, wenn die reinen Betriebskosten der alten Investition (183.000 €) *höher* sind als die Gesamtkosten (Betriebs- + Kapitalkosten) der Neuinvestition (205.200 €). Da die Beibehaltung der alten Anlage pro Periode um **22.200 € günstiger** ist, lohnt sich der Austausch nicht.
---

## 📥 Gegebene Basisdaten (Ausgangssituation)
* **Investition A:** Auslastung $x_A = 20.000$ Leistungseinheiten p.a.
* **Investition B (neu):** Auslastung $x_B = 24.000$ Leistungseinheiten p.a. (vorher 20.000)

### 📊 Kostenstruktur-Tableau
| Kostenkategorie | Investition A ($x = 20.000$) | Investition B ($x = 24.000$) |
| :--- | :---: | :---: |
| **Kalkulatorische Abschreibung** | 12.500 € | 14.000 € |
| **Kalkulatorische Zinsen ($i = 10\%$)** | 5.000 € | 7.000 € |
| **Sonstige fixe Kosten** | 7.000 € | 20.000 € |
| ➖ **Summe fixer Kosten ($K_f$)** | **24.500 €** | **41.000 €** |
| | | |
| **Löhne** | 95.000 € | 108.000 € |
| **Fertigungsmaterial** | 70.000 € | 78.000 € |
| **Energiekosten** | 10.000 € | 9.600 € |
| **Sonstige variable Kosten** | 1.000 € | 1.440 € |
| ➖ **Summe variabler Kosten ($K_v$)** | **176.000 €** | **197.040 €** |
| ============================== | ============ | ============ |
| 📐 **Gesamtkosten je Jahr ($K$)** | **200.500 €** | **238.040 €** |
| 📈 **Stückkosten ($k$)** | **10,03 €** | **9,92 €** |

---

## 🧮 Mathematische Methodik & Anpassungsschritte

### 1. Proportionale Anpassung der variablen Kosten ($K_v$) für B
Da Investition B eine höhere Kapazität auslastet ($24.000$ statt $20.000$ Einheiten), müssen die variablen Kosten linear hochgerechnet werden.
$$\text{Anpassungsfaktor} = \frac{\text{Neue Auslastung}}{\text{Alte Auslastung}} = \frac{24.000}{20.000} = \mathbf{1{,}2} \implies (+20\%)$$

*Beispielhafte Hochrechnung einzelner Positionen für Spalte B:*
* Löhne: $90.000\text{ €} \cdot 1{,}2 = 108.000\text{ €}$
* Fertigungsmaterial: $65.000\text{ €} \cdot 1{,}2 = 78.000\text{ €}$
* Neue Summe $K_v$: $164.200\text{ €} \cdot 1{,}2 = \mathbf{197.040\text{ €}}$

### 2. Konstanz der fixen Kosten ($K_f$)
Die fixen Kosten reagieren *nicht* auf Beschäftigungsänderungen. Die Summe der Fixkosten von Objekt B bleibt starr bei **41.000 €** (Abschreibung + Zinsen + Sonstige Fixkosten).

### 3. Berechnung der Stückkosten ($k$)
$$\text{Stückkosten } (k) = \frac{\text{Gesamtkosten } (K)}{\text{Auslastung } (x)}$$

* **Objekt A:** $k_A = \frac{200.500\text{ €}}{20.000\text{ Stück}} = \mathbf{10{,}025\text{ €/Stück}} \approx \mathbf{10{,}03\text{ €}}$
* **Objekt B:** $k_B = \frac{238.040\text{ €}}{24.000\text{ Stück}} = \mathbf{9{,}918\text{ €/Stück}} \approx \mathbf{9{,}92\text{ €}}$

---

## 💡 Controlling-Effekt: Die Fixkostendegression

> [!success] **Klausur-Entscheidung**
> Auf Basis des Stückkostenvergleichs ist **Investition B vorzuziehen**. Die Kosten pro hergestellter Leistungseinheit liegen mit **9,92 €** unter denen von Investition A (**10,03 €**).

> [!info] **Der "Fixkostendegressionseffekt" (Economies of Scale)**
> Warum schlägt Investition B das Objekt A, obwohl die absoluten Gesamtkosten deutlich höher sind (238.040 € vs. 200.500 €)? 
> Grund ist der mathematische Effekt der Fixkostendegression: Da die hohen Fixkosten von B (41.000 €) auf eine größere Produktionsmenge ($24.000$ Stück) verteilt werden, sinkt der fixe Kostenanteil pro Stück (*Nutzeffekt steigt, Leerkosten sinken*). Bei unterschiedlichen Auslastungen ist der Stückkostenvergleich das einzig valide statische Instrument.