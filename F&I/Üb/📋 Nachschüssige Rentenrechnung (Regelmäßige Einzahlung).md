## 📥 Projektparameter (Basisdaten)
Berechnung des Endwerts einer regelmäßigen, zeitlich gleichbleibenden Zahlungsreihe (Rente) bei **nachschüssiger** Zahlungsweise (Einzahlung am Periodenende).

* **Regelmäßige Sparrate ($R$):** 2.000 € p.a.
* **Laufzeit ($n$):** 5 Jahre
* **Zinssatz ($i$):** 2,5 % p.a.
* **Zinsfaktor ($q$):** $1 + i = 1,025$

---

## 📐 Mathematisches Instrumentarium & Berechnungen

### 1. Nachschüssiger Endwertfaktor ($EWF$)
Der Endwertfaktor verdichtet die Zinseszins-Effekte aller Einzelrenten über die Gesamtlaufzeit in einer einzigen Kennzahl.

$$EWF = \frac{q^n - 1}{q - 1}$$

$$EWF = \frac{1,025^5 - 1}{1,025 - 1} = \frac{1,131408 - 1}{0,025} \approx \mathbf{5,25633}$$

### 2. Rentenendwert ($K_5$)
Der Endwert der Rentenreihe ergibt sich aus der Multiplikation der jährlichen Rate mit dem berechneten Endwertfaktor.

$$K_n = R \cdot \frac{q^n - 1}{q - 1}$$

$$K_5 = 2.000\text{ €} \cdot 5,25633 = \mathbf{10.512,66\text{ €}}$$

---

## 🏛️ Ökonomische Struktur der Wertschöpfung

* **Eingezahltes Eigenkapital:** $5 \cdot 2.000\text{ €} = 10.000\text{ €}$
* **Zinsertrag (Zins & Zinseszins):** $10.512,66\text{ €} - 10.000\text{ €} = 512,66\text{ €}$

> [!info] **Nachschüssige vs. Vorschüssige Rente**
> Da die Einzahlung jeweils **am Ende** des Jahres erfolgt, wird die allerletzte Rate im Jahr 5 direkt am Stichtag eingezahlt und somit überhaupt nicht mehr verzinst. Sie geht mit dem reinen Nennwert (2.000 €) in den Endwert ein.