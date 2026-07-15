## 📥 Projektparameter (Basisdaten)
Ermittlung der Wirtschaftlichkeit und Rentabilität einer Maschineninvestition auf Basis der **Durchschnittswertmethode** (statisches Verfahren).

* **Anschaffungskosten ($A_0$):** 500.000 €
* **Restwert ($RW$):** 0 €
* **Nutzungsdauer ($n$):** 5 Jahre (lineare Abschreibung)
* **Kalkulationszinssatz ($i$):** 8 % p.a.
* **Sonstige Kosten p.a.:** 230.000 €
* **Erlöse p.a. ($E$):** 400.000 €

---

## 📐 Mathematisches Instrumentarium & Berechnungen

### 1. Kapitalbindung und Werterhalt
* **Kalkulatorische Abschreibung:** Erfasst den linearen Wertverzehr pro Periode.
    $$\text{kalk. Abschreibung} = \frac{A_0 - RW}{n} = \frac{500.000\text{ €} - 0\text{ €}}{5} = \mathbf{100.000\text{ €/Jahr}}$$
* **Durchschnittlich gebundenes Kapital ($\emptyset\text{ GK}$):** Die Bemessungsgrundlage für kalkulatorische Zinsen und Renditen bei der Durchschnittswertmethode.
    $$\emptyset\text{ GK} = \frac{A_0 + RW}{2} = \frac{500.000\text{ €} + 0\text{ €}}{2} = \mathbf{250.000\text{ €}}$$
* **Kalkulatorische Zinsen:** Opportunitätskosten für das in der Maschine gebundene Kapital.
    $$\text{kalk. Zinsen} = \emptyset\text{ GK} \cdot i = 250.000\text{ €} \cdot 0{,}08 = \mathbf{20.000\text{ €/Jahr}}$$

### 2. Erfolgsrechnung (Kosten und Gewinn)
* **Gesamtkosten p.a. ($K$):**
    $$K = \text{Abschreibung} + \text{Zinsen} + \text{Sonstige Kosten}$$
    $$K = 100.000\text{ €} + 20.000\text{ €} + 230.000\text{ €} = \mathbf{350.000\text{ €/Jahr}}$$
* **Gewinn p.a. ($G$):**
    $$G = E - K = 400.000\text{ €} - 350.000\text{ €} = \mathbf{50.000\text{ €/Jahr}}$$

---

## 📈 Renditekennzahlen (Statische Rentabilität)

Die Rentabilitätsrechnung setzt den Periodenerfolg in Relation zum durchschnittlich eingesetzten Kapital ($\emptyset\text{ GK}$).

| Kennzahl | Definition / Fokus | Mathematische Formel | Berechnung | Ergebnis |
| :--- | :--- | :---: | :--- | :---: |
| **Nettorendite ($nr$)** | Reiner Mehrgewinn über die geforderte Mindestverzinsung hinaus. | $\frac{G}{\emptyset\text{ GK}}$ | $\frac{50.000\text{ €}}{250.000\text{ €}}$ | **20 %** |
| **Bruttorendite ($br$)** | Gesamte Verzinsung des Kapitals (Gewinn + kalkulatorischer Zinsansatz). | $\frac{G + \text{kalk. Zinsen}}{\emptyset\text{ GK}}$ | $\frac{50.000\text{ €} + 20.000\text{ €}}{250.000\text{ €}}$ | **28 %** |

---

## 🏛️ Ökonomische Interpretation

> [!info] **Zusammenhang zwischen Netto- und Bruttorendite**
> * Die **Bruttorendite ($28\%$)** zeigt die tatsächliche Gesamtverzinsung des gebundenen Kapitals auf. Sie setzt sich zusammen aus dem kalkulatorischen Zinssatz (Mindestverzinsung von **8 %**) und der **Nettorendite ($20\%$)**.
> * **Entscheidungskriterium:** Da die Nettorendite positiv ist ($> 0\%$) bzw. die Bruttorendite den Kalkulationszins übersteigt ($28\% > 8\%$), ist die Investition absolut vorteilhaft und ökonomisch sinnvoll.