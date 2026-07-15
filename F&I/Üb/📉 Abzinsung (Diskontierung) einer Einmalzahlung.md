## 📥 Projektparameter (Basisdaten)
Ermittlung des heutigen Gegenwertes (Barwert) eines zukünftigen, feststehenden Kapitalziels unter Berücksichtigung von Zinseszins-Effekten.

* **Zukünftiger Zielwert ($ZW_n$ bzw. $K_{10}$):** 100.000 €
* **Laufzeit ($n$):** 10 Jahre
* **Kalkulationszinssatz ($i$):** 7 % p.a.
* **Aufzinsungsfaktor ($q$):** $1 + i = 1,07$

---

## 📐 Mathematisches Instrumentarium & Berechnungen

### 1. Barwertfaktor ($BWF$ / Diskontierungsfaktor)
Der Barwertfaktor gibt an, wie viel ein Euro, den man in $n$ Jahren erhält, heute wert ist. Er ist der Kehrwert des Aufzinsungsfaktors.

$$BWF = \frac{1}{(1 + i)^n} = (1 + i)^{-n}$$

$$BWF = \frac{1}{1,07^{10}} = \frac{1}{1,967151} \approx \mathbf{0,508349}$$

### 2. Barwert ($K_0$)
Die Ermittlung des notwendigen heutigen Anlagekapitals erfolgt durch Multiplikation des zukünftigen Zielwerts mit dem Barwertfaktor (Diskontierung).

$$K_0 = ZW_n \cdot BWF$$

$$K_0 = 100.000\text{ €} \cdot 0,508349 = \mathbf{50.834,93\text{ €}}$$

---

## 🏛️ Ökonomische Interpretation

> [!info] **Der Barwert als Barwertäquivalent**
> * **Zeitwert des Geldes:** Ein Betrag von **50.834,93 €** heute ist unter einem Zinssatz von 7 % p.a. ökonomisch exakt gleichwertig zu einem Betrag von **100.000,00 €** in 10 Jahren.
> * **Zinseszinseffekt:** Die Differenz von $100.000\text{ €} - 50.834,93\text{ €} = \mathbf{49.165,07\text{ €}}$ entspricht dem absoluten Zinszuwachs, den das Startkapital über die 10-jährige Laufzeit generiert.