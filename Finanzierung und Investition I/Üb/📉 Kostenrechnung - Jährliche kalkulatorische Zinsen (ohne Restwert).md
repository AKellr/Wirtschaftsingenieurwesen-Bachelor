## 📥 Gegebene Basisdaten
* **Anschaffungskosten ($A_0$):** 40.000 €
* **Nutzungsdauer ($n$):** 4 Jahre (linear abgeschrieben)
* **Kalkulationszinssatz ($i$):** 8 % ($0{,}08$)
* **Liquidationserlös (Restwert $R_n$):** 0 €

---

## 🧮 Mathematische Kernformel (Durchschnittsmethode)
Wenn am Ende der Nutzungsdauer kein Liquidationserlös (Restwert) erzielt wird, halbiert sich das gebundene Kapital im linearen Zeitverlauf exakt:

$$z = \frac{A_0}{2} \cdot i$$

Wobei:
- $z$: Jährliche kalkulatorische Zinsen
- $A_0$: Anschaffungskosten der Investition
- $\frac{A_0}{2}$: Durchschnittlich gebundenes Kapital über die Gesamtlaufzeit
- $i$: Kalkulatorischer Zinssatz (Opportunitätskostensatz)

---

## 🔢 Schritt-für-Schritt-Berechnung

### Schritt 1: Berechnung des durchschnittlich gebundenen Kapitals
Da der Buchwert der Maschine durch die lineare Abschreibung jährlich um exakt 10.000 € sinkt (von 40.000 € im Jahr 0 auf 0 € im Jahr 4), beträgt das mathematische Mittel des gebundenen Kapitals:
$$\text{Gebundenes Kapital} = \frac{40.000\text{ €}}{2} = \mathbf{20.000\text{ €}}$$

### Schritt 2: Berechnung der jährlichen Zinskosten ($z$)
Multiplikation des durchschnittlich gebundenen Kapitals mit dem geforderten Zinssatz:
$$z = 20.000\text{ €} \cdot 0{,}08 = \mathbf{1.600\text{ € } p.a.}$$

---

## 💡 Controlling-Interpretation & Klausur-Fazit

> [!info] **Warum wird durch 2 geteilt?**
> Im Gegensatz zu echten Kreditzinsen, die auf Basis der tatsächlichen Restschuld berechnet werden, ermittelt das Controlling in der statischen Investitionsrechnung einen **konstanten Durchschnittswert** pro Jahr. Im ersten Jahr sind zwar volle 40.000 € gebunden, im letzten Jahr jedoch fast 0 €. Die Division durch 2 glättet diesen Verlauf über die gesamte Nutzungsdauer.

> [!warning] **Kalkulatorische Zinsen als Anderskosten**
> Kalkulatorische Zinsen sind **Opportunitätskosten** und keine echten Auszahlungen an eine Bank. Sie erfassen den entgangenen Ertrag, den das Unternehmen hätte erzielen können, wenn das Kapital nicht in der Maschine gebunden, sondern stattdessen am Kapitalmarkt zu 8 % angelegt worden wäre. Sie fließen in die Kosten- und Leistungsrechnung ($KLR$) ein, um die tatsächliche wirtschaftliche Belastung des Projekts abzubilden.

------------
# 📉 Kostenrechnung: Jährliche kalkulatorische Zinsen (mit Restwert)

## 📥 Gegebene Basisdaten
* **Anschaffungskosten ($A_0$):** 40.000 €
* **Liquidationserlös / Restwert ($L_n$):** 6.000 €
* **Nutzungsdauer ($n$):** 4 Jahre
* **Kalkulationszinssatz ($i$):** 8 % ($0{,}08$)

---

## 🧮 Mathematische Kernformel (Erweiterte Durchschnittsmethode)
Wird ein Anlagegut am Ende der Nutzungsdauer nicht verschrottet, sondern weiterverkauft, bleibt der Liquidationserlös ($L_n$) über die gesamte Laufzeit als Mindestwert im Unternehmen gebunden. Das gebundene Kapital sinkt im Zeitverlauf nicht auf 0 €, sondern nur auf $L_n$:

$$z = \frac{A_0 + L_n}{2} \cdot i$$

Wobei:
- $z$: Jährliche kalkulatorische Zinsen
- $A_0$: Anschaffungskosten
- $L_n$: Liquidationserlös (Restwert am Ende der Periode $n$)
- $\frac{A_0 + L_n}{2}$: Durchschnittlich gebundenes Kapital inklusive Restwertbindung
- $i$: Kalkulatorischer Zinssatz

---

## 🔢 Schritt-für-Schritt-Berechnung

### Schritt 1: Berechnung des durchschnittlich gebundenen Kapitals
Da das Kapital am Ende der Laufzeit nicht komplett abgebaut ist, sondern 6.000 € Werthaltigkeit verbleiben, lautet das mathematische Mittel des gebundenen Kapitals:
$$\text{Gebundenes Kapital} = \frac{40.000\text{ €} + 6.000\text{ €}}{2} = \frac{46.000\text{ €}}{2} = \mathbf{23.000\text{ €}}$$

### Schritt 2: Berechnung der jährlichen Zinskosten ($z$)
Multiplikation des korrigierten durchschnittlich gebundenen Kapitals mit dem Zinssatz:
$$z = 23.000\text{ €} \cdot 0{,}08 = \mathbf{1.840\text{ € } p.a.}$$

---

## 💡 Controlling-Interpretation & Klausur-Vergleich

| Merkmal | Ohne Liquidationserlös ($L_n = 0$) | Mit Liquidationserlös ($L_n > 0$) |
| :--- | :---: | :---: |
| **Formel für Kapital** | $\frac{A_0}{2}$ | $\frac{A_0 + L_n}{2}$ |
| **Durchschnittliches Kapital** | 20.000 € | 23.000 € |
| **Kalkulatorische Zinsen p.a.** | **1.600 €** | **1.840 €** |

> [!info] **Der Bindungseffekt des Restwerts**
> Warum steigen die kalkulatorischen Zinsen, wenn man am Ende Geld zurückerhält? Ganz einfach: Der Betrag von 6.000 € wird über die gesamten 4 Jahre niemals durch Abschreibungen freigesetzt. Er bleibt „festgef