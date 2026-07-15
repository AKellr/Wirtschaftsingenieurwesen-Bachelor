## 📥 Projektparameter (Basisdaten)
Vollständige Wirtschaftlichkeitsanalyse für den Erwerb einer Produktionsanlage mittels Einzeldiskontierung unregelmäßiger Zahlungsüberschüsse.

* **Anschaffungsauszahlung ($A_0$):** 3.500.000 € (bei $t = 0$)
* **Kalkulationszinssatz ($i$):** 10 % p.a.
* **Abzinsungsfaktor ($q^{-n}$):** $(1 + i)^{-n} = 1,10^{-n}$
* **Nutzungsdauer ($n$):** 4 Jahre
* **Liquidationserlös ($L_4$):** 0 €

### Erwartete Einzahlungsüberschüsse ($Z_n$)
* **Jahr 1 ($Z_1$):** 700.000 €
* **Jahr 2 ($Z_2$):** 1.200.000 €
* **Jahr 3 ($Z_3$):** 1.400.000 €
* **Jahr 4 ($Z_4$):** 1.400.000 €

---

## 📐 Mathematisches Instrumentarium & Berechnungen

### 1. Barwertfaktoren ($BWF_n$) und abgezinste Cashflows ($C_n$)
$$\text{Formel:} \quad C_n = Z_n \cdot \frac{1}{(1+i)^n}$$

* **Jahr 1:** $700.000\text{ €} \cdot 1,10^{-1} = 700.000\text{ €} \cdot 0,909091 = \mathbf{636.363,64\text{ €}}$
* **Jahr 2:** $1.200.000\text{ €} \cdot 1,10^{-2} = 1.200.000\text{ €} \cdot 0,826446 = \mathbf{991.735,54\text{ €}}$
* **Jahr 3:** $1.400.000\text{ €} \cdot 1,10^{-3} = 1.400.000\text{ €} \cdot 0,751315 = \mathbf{1.051.840,72\text{ €}}$
* **Jahr 4:** $1.400.000\text{ €} \cdot 1,10^{-4} = 1.400.000\text{ €} \cdot 0,683013 = \mathbf{956.218,80\text{ €}}$

### 2. Berechnung des Kapitalwerts ($K_0$ / NPV)
Der Kapitalwert ist die Summe aller abgezinsten Einzahlungsüberschüsse abzüglich der Anfangsinvestition.

$$K_0 = -A_0 + \sum_{t=1}^{n} \frac{Z_t}{(1+i)^t}$$

$$K_0 = -3.500.000\text{ €} + (636.363,64\text{ €} + 991.735,54\text{ €} + 1.051.840,72\text{ €} + 956.218,80\text{ €})$$

$$K_0 = -3.500.000\text{ €} + 3.636.158,70\text{ €} = \mathbf{136.158,70\text{ €}}$$

---

## 🏛️ Ökonomische Interpretation & Entscheidungsvorbereitung

> [!success] **Handlungsempfehlung: Investition durchführen ($K_0 > 0$)**
> Da der **Kapitalwert positiv ist ($K_0 > 0$)**, ist die Investition für die Automobil AG absolut vorteilhaft. 
> 
> **Die drei ökonomischen Dimensionen des Ergebnisses:**
> 1. **Amortisation:** Die anfänglichen Anschaffungskosten von 3.500.000 € werden durch die Rückflüsse vollständig wiedergewonnen.
> 2. **Mindestverzinsung:** Das gebundene Kapital erwirtschaftet exakt die geforderten 10 % p.a. (Opportunitätskosten abgedeckt).
> 3. **Mehrwert:** Die Investition generiert über die Mindestverzinsung hinaus einen zusätzlichen, auf den heutigen Tag bezogenen Vermögenszuwachs von **136.158,70 €**.