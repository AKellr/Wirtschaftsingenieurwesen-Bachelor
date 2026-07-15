## 📥 Projektparameter (Basisdaten)
Umfassende Wirtschaftlichkeitsanalyse einer Unternehmensübernahme mit anfänglichen Verlustjahren und einem endfälligen Desinvestitionserlös (Asset- bzw. Share-Deal).

* **Kaufpreis ($A_0$):** 31.250.000 € (bei $t = 0$)
* **Kalkulationszinssatz ($i$):** 9 % p.a.
* **Zinsfaktor ($q$):** 1,09
* **Nutzungsdauer ($n$):** 7 Jahre
* **Verkaufserlös ($L_7$):** 55.000.000 € (am Ende von Jahr 7)

### Zahlungsstromübersicht ($Z_t$)
* **Jahr 1 ($Z_1$):** -1.600.000 € *(laufender Verlust)*
* **Jahr 2 ($Z_2$):** -1.250.000 € *(laufender Verlust)*
* **Jahr 3 ($Z_3$):** -600.000 € *(laufender Verlust)*
* **Jahr 4 ($Z_4$):** +1.200.000 € *(Einzahlungsüberschuss)*
* **Jahr 5 ($Z_5$):** +1.650.000 € *(Einzahlungsüberschuss)*
* **Jahr 6 ($Z_6$):** +1.900.000 € *(Einzahlungsüberschuss)*
* **Jahr 7 ($Z_7$):** +57.050.000 € *($2.050.000\text{ € } \text{Überschuss} + 55.000.000\text{ € } \text{Verkaufserlös}$)*

---

## 📐 Mathematische Auswertung

### 1. Einzelabzinsung & Barwert-Ermittlung
$$\text{Formel:} \quad C_t = Z_t \cdot q^{-t}$$

| Periode ($t$) | Cashflow ($Z_t$) | Abzinsungsfaktor ($q^{-t}$) | Barwert ($C_t$) |
| :--- | :--- | :--- | :--- |
| **Jahr 1** | -1.600.000 € | 0,9174 | **-1.467.889,91 €** |
| **Jahr 2** | -1.250.000 € | 0,8417 | **-1.052.099,99 €** |
| **Jahr 3** | -600.000 € | 0,7722 | **-463.310,09 €** |
| **Jahr 4** | 1.200.000 € | 0,7084 | **+850.110,25 €** |
| **Jahr 5** | 1.650.000 € | 0,6499 | **+1.072.386,79 €** |
| **Jahr 6** | 1.900.000 € | 0,5963 | **+1.132.907,92 €** |
| **Jahr 7** | 57.050.000 € | 0,5470 | **+31.208.303,67 €** |
| **Summe** | | | **+31.280.408,64 €** |

### 2. Berechnung des Kapitalwerts ($K_0$)
$$K_0 = -A_0 + \sum_{t=1}^{7} (Z_t \cdot q^{-t})$$
$$K_0 = -31.250.000,00\text{ €} + 31.280.408,64\text{ €} = \mathbf{30.408,64\text{ €}}$$

### 3. Berechnung der jährlichen Annuität ($A$)
Die Annuität transformiert den Kapitalwert in einen gleichbleibenden, jährlichen Zahlungsstrom über die gesamte Laufzeit.

* **Wiedergewinnungsfaktor ($WGF_{7; 9\%}$):**
$$WGF = \frac{0,09 \cdot 1,09^7}{1,09^7 - 1} \approx \mathbf{0,198691}$$

* **Annuität ($A$):**
$$A = K_0 \cdot WGF = 30.408,64\text{ €} \cdot 0,198691 = \mathbf{6.041,89\text{ €}}$$

---

## 🏛️ Ökonomische Beurteilung & Interpretation

> [!success] **Entscheidung zu Aufgabenteil a): Investition ist vorteilhaft ($K_0 > 0$)**
> Da der **Kapitalwert positiv** ist ($K_0 = 30.408,64\text{ €} > 0$), übersteigt das Akquisitionsobjekt den geforderten Renditeanspruch von 9 % p.a. Die Übernahme der Metallbau GmbH ist für die Schrecken AG ökonomisch absolut sinnvoll.

> [!info] **Bedeutung der Annuität zu Aufgabenteil b)**
> Ein jährlicher Entnahmeüberschuss von **6.041,89 €** über 7 Jahre hinweg zeigt den durchschnittlichen jährlichen Netto-Ertragwertzuwachs der Investition. Er signalisiert den konstanten Liquiditätsvorteil pro Periode nach vollständiger Abdeckung des kalkulatorischen Zinsfußes.