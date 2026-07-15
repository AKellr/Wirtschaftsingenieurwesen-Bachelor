## 1. Mathematische Grundlagen & Verfahrensübersicht

### (1) Anbauverfahren (Blockverfahren)
* **Prinzip:** Ignoriert jegliche Leistungsbeziehungen zwischen Hilfskostenstellen komplett. Die Verrechnung erfolgt direkt auf die Hauptkostenstellen.
* **Formel Verrechnungssatz ($q_i$):**
  $$q_i = \frac{\text{Primärkosten}_i}{\text{Gesamtleistung}_i - \text{Leistung an andere Hilfs-KST}}$$

### (2) Stufenleiterverfahren (Treppenverfahren)
* **Prinzip:** Rechnet Hilfskostenstellen nacheinander in einer festgelegten Reihenfolge ab. Eine einmal abgerechnete Stelle darf keine Kosten mehr empfangen (einseitige Leistungsberücksichtigung).
* **Formel Verrechnungssatz ($q_i$ auf Stufe $i$):**
  $$q_i = \frac{\text{Primärkosten}_i + \text{bereits erhaltene Umlagen}}{\text{Gesamtleistung}_i - \text{Leistung an bereits geschlossene Hilfs-KST}}$$

### (3) Simultanverfahren (Gleichungsverfahren)
* **Prinzip:** Mathematisch exakte, simultane Berücksichtigung aller wechselseitigen Leistungsbeziehungen über ein lineares Gleichungssystem (LGS).
* **Gleichungsansatz pro Hilfs-KST:**
  $$\text{Gesamtkosten} = \text{Primärkosten} + \sum (\text{Empfangene Leistung} \cdot \text{Verrechnungssatz})$$

---

## 2. Klausurtypische Tabellenlösungen (BAB-Struktur)

Nachfolgend sind die exakten tabellarischen Darstellungen auf Basis des Referenzfalls aus **image_8d8fb9.png** abgebildet. Diese Struktur entspricht der geforderten Darstellung im universitären Prüfungskontext.

### Variante 1: Anbauverfahren (Tabellarischer BAB)

| Kostenstelle / Posten    | Hilfs-KST (R) | Hilfs-KST (E) | Haupt-KST (F)  | Haupt-KST (W)  | Haupt-KST (A)  |
| :----------------------- | :-----------: | :-----------: | :------------: | :------------: | :------------: |
| **Primärkosten (€)**     | **4.500.000** | **2.050.000** | **15.000.000** | **36.000.000** | **18.000.000** |
| Umlage Werkstatt (R) [1] |  -4.500.000   |      --       |    +900.000    |   +3.184.615   |    +415.385    |
| Umlage Lager (E) [2]     |      --       |  -2.050.000   |    +768.750    |    +922.500    |    +358.750    |
| **Sekundärkosten (€)**   |     **0**     |     **0**     | **1.668.750**  | **4.107.115**  |  **774.135**   |
| **Gesamtkosten (€)**     |     **0**     |     **0**     | **16.668.750** | **40.107.115** | **18.774.135** |

* **Berechnungsnachweise zur Tabelle:**
  * [1] $q_R = \frac{4.500.000\ \epsilon}{7.000 - 500} = 692,3077\ \epsilon/\text{Std.}$ 
  * [2] $q_E = \frac{2.050.000\ \epsilon}{480 - 80} = 5.125\ \epsilon/\text{Meter}$

---

### Variante 2: Stufenleiterverfahren (Reihenfolge: R $\rightarrow$ E)

| Kostenstelle / Posten | Hilfs-KST (R) | Hilfs-KST (E) | Haupt-KST (F) | Haupt-KST (W) | Haupt-KST (A) |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Primärkosten (€)** | **4.500.000** | **2.050.000** | **15.000.000** | **36.000.000** | **18.000.000** |
| Umlage Werkstatt (R) [1] | -4.500.000 | +321.429 | +835.714 | +2.957.143 | +385.714 |
| *Zwischensumme (€)* | *0* | *2.371.429* | *15.835.714* | *38.957.143* | *18.385.714* |
| Umlage Lager (E) [2] | -- | -2.371.429 | +889.286 | +1.067.143 | +414.999 |
| **Gesamtkosten (€)** | **0** | **0** | **16.725.000** | **40.024.286** | **18.800.713** |

* **Berechnungsnachweise zur Tabelle:**
  * [1] $q_R = \frac{4.500.000\ \epsilon}{7.000\ \text{Std.}} = 642,8571\ \epsilon/\text{Std.}$
  * [2] $q_E = \frac{2.371.429\ \epsilon}{480 - 80\ \text{Meter}} = 5.928,5725\ \epsilon/\text{Meter}$

---

### Variante 3: Stufenleiterverfahren (Reihenfolge: E $\rightarrow$ R)

| Kostenstelle / Posten | Hilfs-KST (R) | Hilfs-KST (E) | Haupt-KST (F) | Haupt-KST (W) | Haupt-KST (A) |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Primärkosten (€)** | **4.500.000** | **2.050.000** | **15.000.000** | **36.000.000** | **18.000.000** |
| Umlage Lager (E) [1] | +341.667 | -2.050.000 | +640.625 | +768.750 | +298.958 |
| *Zwischensumme (€)* | *4.841.667* | *0* | *15.640.625* | *36.768.750* | *18.298.958* |
| Umlage Werkstatt (R) [2] | -4.841.667 | -- | +968.333 | +3.426.411 | +446.923 |
| **Gesamtkosten (€)** | **0** | **0** | **16.608.958** | **40.195.161** | **18.745.881** |

* **Berechnungsnachweise zur Tabelle:**
  * [1] $q_E = \frac{2.050.000\ \epsilon}{480\ \text{Meter}} = 4.270,8333\ \epsilon/\text{Meter}$
  * [2] $q_R = \frac{4.841.667\ \epsilon}{7.000 - 500\ \text{Std.}} = 744,8718\ \epsilon/\text{Std.}$

---

### Variante 4: Simultanverfahren (Mathematisch exakt)

* **LGS-Aufstellung & Lösung:**
  1) $7.000 \cdot q_R = 4.500.000 + 80 \cdot q_E \implies 7.000 \cdot q_R - 80 \cdot q_E = 4.500.000$
  2) $480 \cdot q_E = 2.050.000 + 500 \cdot q_R \implies -500 \cdot q_R + 480 \cdot q_E = 2.050.000$
  * **Ergebnis:** $q_R = 700\ \epsilon/\text{Std.}$, $q_E = 5.000\ \epsilon/\text{Meter}$

| Kostenstelle / Posten | Hilfs-KST (R) | Hilfs-KST (E) | Haupt-KST (F) | Haupt-KST (W) | Haupt-KST (A) |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Primärkosten (€)** | **4.500.000** | **2.050.000** | **15.000.000** | **36.000.000** | **18.000.000** |
| Umlage Werkstatt (R) | -4.900.000 | +350.000 | +910.000 | +3.220.000 | +420.000 |
| Umlage Lager (E) | +400.000 | -2.400.000 | +750.000 | +900.000 | +350.000 |
| **Sekundärkosten (€)** | **-500.000** | **-2.050.000** | **1.660.000** | **4.120.000** | **770.000** |
| **Gesamtkosten (€)** | **0** | **0** | **16.660.000** | **40.120.000** | **18.770.000** |

> [!Note] **Klausur-Verrechnungslogik im Simultan-BAB**
> Im Simultanverfahren wird die Hilfskostenstelle mit ihren mathematischen Gesamtkosten ($q \cdot \text{Gesamtleistung}$) im Schnittpunkt entlastet (z. B. R mit $700 \cdot 7.000 = 4.900.000\ \epsilon$). Die Zeile "Sekundärkosten" saldiert Umlagen und Entlastungen und muss für alle Hilfskostenstellen exakt dem negativen Wert der ursprünglichen Primärkosten entsprechen, damit das mathematische Saldo Null aufgeht.

---

## 🔍 3. Klausur-Fallstricke & Korrekturhinweise

> [!Alert] **Fehlerquelle: Reihenfolgenkriterium beim Stufenleiterverfahren**
> In Klausuren wird oft verlangt, die optimale Abrechnungsreihenfolge selbstständig zu ermitteln. Das Standardkriterium hierfür ist der **einseitige Leistungsempfang** oder die **Summe der abgegebenen Leistungen**. Die Stelle, die am wenigsten von anderen empfängt, aber am meisten an andere Hilfskostenstellen abgibt, muss zwingend **zuerst** abgerechnet werden, um den Fehler der Vernachlässigung zu minimieren.

> [!Alert] **Fehlerquelle: Verrechnungs-Nenner im Stufenleiterverfahren**
> Sobald eine Hilfskostenstelle abgerechnet ist (z.B. R in Variante 2), ist sie für nachfolgende Stufen "tot". Bei der Berechnung des Folgesatzes ($q_E$) darf die Leistung, die zurück an R floss (80 m), keinesfalls im Nenner stehen. Der Nenner verkürzt sich sukzessive um die Anteile bereits geschlossener Kostenstellen.