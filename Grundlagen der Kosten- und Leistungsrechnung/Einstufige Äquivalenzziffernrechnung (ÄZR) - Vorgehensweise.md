## 📌 1. Mathematisches Fundament & Definitionen
Die einstufige Äquivalenzziffernrechnung (ÄZR) homogenisiert mehrteilige, aber artverwandte Produktionsmengen (**Sortenfertigung**) ohne Berücksichtigung von Lagerbestandsveränderungen.

- $x_i$: Reale Produktionsmenge der Sorte $i$
- $\text{ÄZ}_i$: Äquivalenzziffer der Sorte $i$ (Gewichtungsfaktor relativ zum Basisprodukt mit $\text{ÄZ} = 1,00$)
- $\text{RE}_i$: Recheneinheiten der Sorte $i$ (homogenisierte Rechenbasis)
- $K_{\text{ges}}$: Zu verteilende Gesamtkosten der Periode
- $k_{\text{RE}}$: Kostensatz pro Recheneinheit [€/RE]
- $K_i$: Periodenkosten der Sorte $i$
- $k_{s,i}$: Stückkosten (Selbstkosten pro Einheit) der Sorte $i$

---

## ⚙️ 2. Das 5-Schritte-Kalkulationsschema (Algorithmus)

### Schritt 1: Homogenisierung der Mengen (Ermittlung der RE)
Die realen Mengen werden über die Äquivalenzziffer in fiktive Standardeinheiten umgerechnet:
$$\text{RE}_i = x_i \cdot \text{ÄZ}_i$$

### Schritt 2: Aggregation der Recheneinheiten
Bildung der Summe aller Recheneinheiten über alle $n$ Sorten:
$$\sum_{i=1}^{n} \text{RE}_i = \text{RE}_1 + \text{RE}_2 + \dots + \text{RE}_n$$

### Schritt 3: Ermittlung des Kostensatzes pro RE ($k_{\text{RE}}$)
Division der Periodengesamtkosten durch die aggregierten Recheneinheiten:
$$k_{\text{RE}} = \frac{K_{\text{ges}}}{\sum_{i=1}^{n} \text{RE}_i}$$

### Schritt 4: Berechnung der Sortengesamtkosten ($K_i$)
Rückführung der Kosten auf die jeweiligen Produktsorten:
$$K_i = \text{RE}_i \cdot k_{\text{RE}}$$
*Kontrollrechnung:* $\sum_{i=1}^{n} K_i = K_{\text{ges}}$

### Schritt 5: Ermittlung der Stückkosten ($k_{s,i}$)
Division der Sortenkosten durch die reale Produktionsmenge:
$$k_{s,i} = \frac{K_i}{x_i}$$

---

## 🧮 3. Strukturiertes Berechnungsbeispiel ($K_{\text{ges}} = 5.000\ €$)

| Sorte | Menge ($x_i$) | $\text{ÄZ}_i$ | $\text{RE}_i$ ($x \cdot \text{ÄZ}$) | $k_{\text{RE}}$ | $K_i$ ($\text{RE} \cdot k_{\text{RE}}$) | $k_{s,i}$ ($K_i / x_i$) |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **A** | 1.000 | 1,20 | 1.200 | 2,7027 € | 3.243,24 € | **3,24 €** |
| **B (Basis)**| 200 | 1,00 | 200 | 2,7027 € | 540,54 € | **2,70 €** |
| **C** | 500 | 0,90 | 450 | 2,7027 € | 1.216,22 € | **2,43 €** |
| **$\sum$** | | | **1.850** | | **5.000,00 €** | |

$$\text{Kostensatz: } k_{\text{RE}} = \frac{5.000}{1.850\ \text{RE}} \approx 2,7027027\ \text{RE}$$

---

## ⚡ 4. Klausur-Shortcuts & Effizienz-Hacks
- **Direktweg zu den Stückkosten ($k_{s,i}$):** Schritt 4 und Schritt 5 können mathematisch komprimiert werden. Die Stückkosten einer Sorte lassen sich direkt durch Multiplikation des RE-Kostensatzes mit der spezifischen Äquivalenzziffer berechnen:
  $$k_{s,i} = k_{\text{RE}} \cdot \text{ÄZ}_i$$
  *Beweis Sorte A:* $2,7027027 \cdot 1,20 = 3,2432 \approx 3,24$.
- **Rundungsdifferenzen:** In Klausuren immer mit dem ungerundeten Speicherwert von $k_{\text{RE}}$ weiterrechnen, um Abweichungen bei den Sortengesamtkosten ($K_i$) durch kaufmännische Rundung zu vermeiden.