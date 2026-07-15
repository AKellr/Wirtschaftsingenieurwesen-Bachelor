## 1. Mathematische Grundlagen & Definitionen
Die Tilgungsrechnung modelliert die planmäßige Rückzahlung von langfristigen Schulden. Jede periodische Gesamtzahlung (**Kapitaldienst**) spaltet sich finanzmathematisch in einen Zins- und einen Tilgungsanteil auf.

- $K_0$: Nominalwert des Kredits (Ausgangsschuld bei $t=0$)
- $K_{t-1}$: Restschuld zu Beginn der Periode $t$
- $i$: Nominalzinssatz p.a. (als Dezimalzahl)
- $n$: Laufzeit in Jahren
- $T_t$: Tilgungsrate in der Periode $t$ (reine Schuldenreduktion)
- $Z_t$: Zinsbetrag in der Periode $t$ (Preis für das überlassene Kapital)
- $A_t$: Kapitaldienst der Periode $t$ (Gesamtzahlung; bei Annuität konstant: $A_t = A$)

### Das fundamentale Postulat der Tilgung:
$$A_t = T_t + Z_t$$
$$Z_t = K_{t-1} \cdot i$$
$$K_t = K_{t-1} - T_t$$

---

## ⚙️ 2. Die Tilgungsmodelle im strukturellen Vergleich

### A. Ratentilgung (Lineare / Konstante Tilgung)
- **Charakteristik:** Die reine Tilgungsquote bleibt über die gesamte Laufzeit absolut konstant.
- **Formel für die Tilgung:** $$T_t = T = \frac{K_0}{n}$$
- **Dynamik:** Da die Restschuld $K_{t-1}$ linear sinkt, nehmen die Zinsen $Z_t$ degressiv ab. Dies führt zu einem kontinuierlich fallenden jährlichen Kapitaldienst ($A_t \downarrow$).
- **Belastungsprofil:** Maximale Liquiditätsbelastung in Periode $t=1$, minimale Belastung in Periode $t=n$.

### B. Annuitätentilgung (Konstante Gesamtzahlung)
- **Charakteristik:** Der jährliche Kapitaldienst (die Annuität $A$) bleibt über die gesamte Laufzeit konstant.
- **Formel über den Annuitätenfaktor (Wiedergewinnungsfaktor $a_n$):**
  $$A = K_0 \cdot a_n = K_0 \cdot \frac{i \cdot (1+i)^n}{(1+i)^n - 1}$$
- **Dynamik:** Durch die fallende Restschuld sinkt der Zinsanteil $Z_t$ im Zeitverlauf. Da $A$ konstant ist, steigt der Tilgungsanteil $T_t$ komplementär an (**progressive Tilgungsdynamik**).
- **Belastungsprofil:** Lineare, perfekt kalkulierbare Liquiditätsbelastung über alle Perioden.

---

## 🧮 3. Vergleichendes Berechnungsbeispiel ($K_0 = 100.000\ €, i = 5\%, n = 4$)

### Variante 1: Ratentilgung ($T = 25.000\ €$)

| Jahr ($t$) | Restschuld Beginn ($K_{t-1}$) | Zinsen ($Z_t = K_{t-1} \cdot 0,05$) | Tilgung ($T_t$) | Kapitaldienst ($A_t$) |
| :--- | :--- | :--- | :--- | :--- |
| **1** | 100.000 € | 5.000 € | 25.000 € | **30.000 €** |
| **2** | 75.000 € | 3.750 € | 25.000 € | **28.750 €** |
| **3** | 50.000 € | 2.500 € | 25.000 € | **27.500 €** |
| **4** | 25.000 € | 1.250 € | 25.000 € | **26.250 €** |
| **$\sum$** | | **12.500 €** | **100.000 €** | **112.500 €** |

### Variante 2: Annuitätentilgung ($A = 28.201,18\ €$)
*Berechnung Faktor:* $a_4 = \frac{0,05 \cdot 1,05^4}{1,05^4 - 1} \approx 0,28201183$

| Jahr ($t$) | Restschuld Beginn ($K_{t-1}$) | Zinsen ($Z_t = K_{t-1} \cdot 0,05$) | Tilgung ($T_t = A - Z_t$) | Annuität ($A$) |
| :--- | :--- | :--- | :--- | :--- |
| **1** | 100.000 € | 5.000 € | 23.201 € | **28.201 €** |
| **2** | 76.799 € | 3.840 € | 24.361 € | **28.201 €** |
| **3** | 52.438 € | 2.622 € | 25.579 € | **28.201 €** |
| **4** | 26.858 € | 1.343 € \* | 26.858 € | **28.201 €** |
| **$\sum$** | | **12.805 €** | **100.000 €** | **112.805 €** |

*\*gerundet inklusive minimaler Rundungsdifferenz in der Finalperiode.*

---

## ⚖️ 4. Strategische Entscheidung & Zielkonflikt (Klausur-Matrix)

| Kriterium | Ratentilgung | Annuitätentilgung |
| :--- | :--- | :--- |
| **Gesamtkosten (Zinslast)** | **Günstiger (12.500 €)** <br>↳ *Weil die Restschuld schneller/linearer abgebaut wird.* | **Teurer (12.805 €)** <br>↳ *Weil in den frühen Jahren weniger getilgt wird.* |
| **Anfangsbelastung** | **Sehr hoch (30.000 €)** <br>↳ *Belastet die Liquidität direkt nach Investition.* | **Niedriger (28.201 €)** <br>↳ *Schont die Liquidität in der kritischen Anlaufphase.* |
| **Planungssicherheit** | Variabel (sinkend) | **Konstant** <br>↳ *Perfekt für langfristiges Budgeting.* |

### 🎯 Handlungsempfehlung für die Praxis:
1. **Wahl der Annuitätentilgung**, wenn das Investitionsobjekt in den ersten Jahren noch keine maximalen Erträge abwirft und die Liquidität geschont werden muss (niedrigere Einstiegsbarriere).
2. **Wahl der Ratentilgung**, wenn von Beginn an eine hohe Liquidität vorliegt, um die Gesamtzinslast des Unternehmens effektiv zu minimieren.