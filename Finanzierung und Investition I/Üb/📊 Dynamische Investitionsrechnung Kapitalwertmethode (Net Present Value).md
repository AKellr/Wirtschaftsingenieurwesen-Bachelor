## 📥 Projektparameter (Basisdaten)
Ermittlung des heutigen Gesamtwertes unregelmäßiger, zukünftiger Rückflüsse (Nettoeinzahlungen) einer Maschine durch Einzeldiskontierung auf den Bezugszeitpunkt $t = 0$.

* **Kalkulationszinssatz ($i$):** 5 % p.a.
* **Abzinsungsfaktor ($q^{-n}$):** $(1 + i)^{-n} = 1,05^{-n}$
* **Betrachtungszeitraum ($n$):** 3 Jahre

### Zeitlicher Zahlungsstrom
| Periode ($n$) | Nettoeinzahlung ($Z_n$) |
| :--- | :---: |
| **Jahr 1** | 100 € |
| **Jahr 2** | 250 € |
| **Jahr 3** | 280 € |

---

## 📐 Mathematisches Instrumentarium & Berechnungen

### 1. Spezifische Barwertfaktoren ($BWF_n$)
$$\text{Formel:} \quad BWF_n = \frac{1}{1,05^n}$$

* **$BWF_1$:** $\frac{1}{1,05^1} \approx \mathbf{0,9524}$
* **$BWF_2$:** $\frac{1}{1,05^2} \approx \mathbf{0,9070}$
* **$BWF_3$:** $\frac{1}{1,05^3} \approx \mathbf{0,8638}$

### 2. Ermittlung der Barwerte ($C_n$) und des Kapitalwerts ($C_0$)
$$\text{Formel:} \quad C_n = Z_n \cdot BWF_n \quad \Longrightarrow \quad C_0 = \sum_{t=1}^{n} (Z_t \cdot q^{-t})$$

| Periode ($n$) | Nettoeinzahlung ($Z_n$) | Abzinsungsfaktor ($BWF_n$) | Barwert ($C_n$) |
| :--- | :---: | :---: | :---: |
| **Jahr 1** | 100 € | 0,9524 | 95,24 € |
| **Jahr 2** | 250 € | 0,9070 | 226,76 € |
| **Jahr 3** | 280 € | 0,8638 | 241,87 € |
| **Summe ($C_0$)** | | | **563,87 €** |

*(Gerundete Addition ergibt $563,87\text{ €}$; exakt mathematisch aufsummiert beträgt der Wert $563,83\text{ €}$)*

---

## 🏛️ Ökonomische Beurteilung

> [!success] **Maximal zulässige Anschaffungsauszahlung**
> * **Kapitalwert der Einzahlungen:** Die zukünftigen Cashflows besitzen heute einen ökonomischen Wert von **563,87 €**.
> * **Investitionsentscheidung:** Das Investitionsobjekt ist absolut vorteilhaft, sofern die tatsächlichen Anschaffungskosten ($A_0$) am heutigen Tag **geringer** als 563,87 € sind. In diesem Fall übersteigt die effektive Verzinsung den geforderten Kalkulationszins von 5 %.