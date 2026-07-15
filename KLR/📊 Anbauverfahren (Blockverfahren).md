Das Anbauverfahren ist das einfachste einstufige Verfahren der **innerbetrieblichen Leistungsverrechnung (IBLV)** im Rahmen der Kostenstellenrechnung. Es dient dazu, die primären Gemeinkosten von Hilfskostenstellen (Vorkostenstellen) auf die Hauptkostenstellen (Endkostenstellen) umzulegen, bevor Kalkulationssätze (z. B. Zuschlagsätze) ermittelt werden.

---

## 1. Verrechnungsprinzip und Prämisse

* **Gegenseitige Leistungsbeziehungen:** Das fundamentale Merkmal des Anbauverfahrens ist die vollständige **Ignorierung des innerbetrieblichen Leistungsaustauschs** zwischen den Hilfskostenstellen.
* **Direkter Anbau:** Es wird fingiert, dass Hilfskostenstellen ausschließlich Leistungen für die Hauptkostenstellen erbringen. Verbrauchsmengen anderer Hilfskostenstellen werden aus der mathematischen Basis eliminiert.
* **Anwendungsbereich:** Zulässig und ökonomisch sinnvoll nur dann, wenn die gegenseitige Verflechtung der Hilfskostenstellen vernachlässigbar gering ist oder die Verrechnungskomplexität minimiert werden soll.

---

## 2. Mathematische Formeln und Kennzahlen

### Modifizierte Ermittlung des Verrechnungssatzes ($q_i$)
Da die an andere Hilfskostenstellen abgegebenen Einheiten gestrichen werden, reduziert sich die Basis im Nenner um diese Mengen. Der Verrechnungssatz $q_i$ der Hilfskostenstelle $i$ berechnet sich wie folgt:

$$q_i = \frac{K_{\text{prim}, i}}{\sum_{j \in \text{Haupt}} x_{ij}}$$

Alternative Formulierung über die Gesamtleistung:
$$q_i = \frac{K_{\text{prim}, i}}{X_{\text{Gesamt}, i} - \sum_{k \in \text{Hilf}} x_{ik}}$$

*Bedeutung der Variablen:*
* $K_{\text{prim}, i}$: Primäre Gemeinkosten der Hilfskostenstelle $i$
* $x_{ij}$: Abgegebene Leistungseinheiten der Hilfskostenstelle $i$ an die Hauptkostenstelle $j$
* $X_{\text{Gesamt}, i}$: Gesamte abgegebene Leistung der Hilfskostenstelle $i$
* $x_{ik}$: Abgegebene Leistungseinheiten der Hilfskostenstelle $i$ an andere Hilfskostenstellen $k$

### Sekundäre Gemeinkosten der Hauptkostenstelle ($K_{\text{sek}, j}$)
Die Belastung einer Hauptkostenstelle $j$ ergibt sich aus dem tatsächlichen Verbrauch multipliziert mit dem berechneten Verrechnungssatz:

$$K_{\text{sek}, j} = \sum_{i \in \text{Hilf}} (x_{ij} \cdot q_i)$$

---

## 3. Exemplarisches Kalkulationsbeispiel (BAB-Umlage)

*Ausgangsdaten:*
* **HKST Strom:** $K_{\text{prim}} = 12.000\ \text{€}$ | Gesamtleistung = $4.000\ \text{kWh}$
  *(Abgabe: Reparatur: $1.000\ \text{kWh}$ | Material: $1.000\ \text{kWh}$ | Fertigung: $2.000\ \text{kWh}$)*
* **HKST Reparatur:** $K_{\text{prim}} = 6.000\ \text{€}$ | Gesamtleistung = $500\ \text{Std.}$
  *(Abgabe: Strom: $100\ \text{Std.}$ | Material: $100\ \text{Std.}$ | Fertigung: $300\ \text{Std.}$)*

### Schritt 1: Berechnung der Verrechnungssätze ($q$)
* **Strom ($q_{\text{Strom}}$):**
  $$q_{\text{Strom}} = \frac{12.000\ \text{€}}{1.000\ \text{kWh (Material)} + 2.000\ \text{kWh (Fertigung)}} = \frac{12.000\ \text{€}}{3.000\ \text{kWh}} = \mathbf{4\ \text{€/kWh}}$$
* **Reparatur ($q_{\text{Rep}}$):**
  $$q_{\text{Rep}} = \frac{6.000\ \text{€}}{100\ \text{Std. (Material)} + 300\ \text{Std. (Fertigung)}} = \frac{6.000\ \text{€}}{400\ \text{Std.}} = \mathbf{15\ \text{€/Std.}}$$

### Schritt 2: Verteilung im Betriebsabrechnungsbogen (BAB)

| Kostenstelle | Primäre Gemeinkosten | Umlage Strom ($4\ \text{€/kWh}$) | Umlage Reparatur ($15\ \text{€/Std.}$) | Sekundäre Gemeinkosten |
| :--- | :---: | :---: | :---: | :---: |
| **HKST Strom** | 12.000 € | -12.000 € | — | **0 €** |
| **HKST Reparatur** | 6.000 € | — | -6.000 € | **0 €** |
| **MKST Material** | *gegeben* | +4.000 € | +1.500 € | **+5.500 €** |
| **FKST Fertigung** | *gegeben* | +8.000 € | +4.500 € | **+12.500 €** |

---

## 🔍 4. Controlling- & Klausurrelevanz

> [!Concept] **Vor- und Nachteile (Kritische Würdigung)**
> * **Vorteile:** Extrem geringer Rechenaufwand; keine mathematischen Vorkenntnisse über simultane Gleichungssysteme erforderlich; hohe Übersichtlichkeit im BAB.
> * **Nachteile:** Verstoß gegen das Verursachungsprinzip. Da Verflechtungen zwischen Hilfskostenstellen vollständig ausgeblendet werden, kommt es zu ungenauen Verrechnungssätzen und somit zu Fehlallokationen (Kostenverschiebung) bei den Endprodukten.

> [!Alert] **Typische Klausurfalle im Nenner**
> Der häufigste Fehler in Prüfungen besteht darin, bei der Division der primären Gemeinkosten die *Gesamtleistung* (z. B. $4.000\ \text{kWh}$) statt der bereinigten Leistung an die Hauptkostenstellen ($3.000\ \text{kWh}$) heranzuziehen. Wird dieser Fehler begangen, verbleiben rechnerisch Kosten auf den Hilfskostenstellen zurück, und der BAB geht am Ende mathematisch nicht auf (Summe der Entlastungen $\neq$ Summe der primären Kosten).