## 📥 Projektparameter (Basisdaten)
Effiziente Ermittlung des heutigen Gesamtwertes (Barwert) einer Reihe von zeitlich gleichbleibenden, **konstanten** zukünftigen Zahlungsströmen (Rente) ohne Einzelabzinsung.

* **Konstante Nettoeinzahlung ($R$):** 100.000 € p.a.
* **Laufzeit ($n$):** 3 Jahre
* **Kalkulationszinssatz ($i$):** 5 % p.a.
* **Zinsfaktor ($q$):** $1 + i = 1,05$

---

## 📐 Mathematisches Instrumentarium & Berechnungen

### 1. Diskontierungssummenfaktor ($DSF$ / Rentenbarwertfaktor)
Der DSF summiert die einzelnen Barwertfaktoren über die Gesamtlaufzeit geometrisch auf. Er gibt an, wie viel eine konstante Rentenzahlung von 1 € über $n$ Jahre heute wert ist.

$$DSF = \frac{q^n - 1}{q^n \cdot (q - 1)}$$

$$DSF = \frac{1,05^3 - 1}{1,05^3 \cdot (1,05 - 1)} = \frac{1,157625 - 1}{1,157625 \cdot 0,05} \approx \mathbf{2,723248}$$

### 2. Rentenbarwert ($K_0$)
Die Bestimmung des Gesamtwertes zum Zeitpunkt $t = 0$ erfolgt durch die Multiplikation der jährlichen konstanten Zahlung mit dem Diskontierungssummenfaktor.

$$K_0 = R \cdot DSF$$

$$K_0 = 100.000\text{ €} \cdot 2,723248 \approx \mathbf{272.324,80\text{ €}}$$

---

## 🏛️ Ökonomische Interpretation & Abgrenzung

> [!tip] **Verfahrensvorteil in der Investitionsrechnung**
> * **Effizienzgewinn:** Bei unregelmäßigen Zahlungsströmen muss jede Periode einzeln mit dem Barwertfaktor ($q^{-n}$) diskontiert werden (vgl. klassische Kapitalwertmethode). Bei konstanten Überschüssen verkürzt der **DSF** das Rechenverfahren auf eine einzige Multiplikation.
> * **Wertkompression:** Obwohl nominal $3 \cdot 100.000\text{ €} = 300.000\text{ €}$ erwirtschaftet werden, beträgt der heutige ökonomische Wert unter Berücksichtigung von Opportunitätskosten (5 % Zins) lediglich **272.324,80 €**.