# 📊 Grundlagen der Kosten- und Leistungsrechnung (KLR)
## 1. Methoden der Materialverbrauchsermittlung

Die Erfassung des Werkstoffverbrauchs bildet die Basis der Materialkostenrechnung. Es werden primär drei Verfahren abgegrenzt:

### A. Skontrationsmethode (Fortschreibungsmethode)
* **Prinzip:** Fortlaufende und lückenlose Erfassung jedes Materialabgangs in Echtzeit.
* **Erfassungsinstrument:** Materialentnahmescheine, Barcode-Scanning oder RFID-Erfassung.
* **Formel:** $$\text{Endbestand}_{\text{Soll}} = \text{Anfangsbestand} + \text{Zugänge} - \text{Abgänge}$$
* **Vorteil:** Hohe Transparenz; Diebstahl oder Schwund fallen bei der Inventur durch Abweichungen zwischen Soll- und Ist-Bestand auf.

### B. Retrograde Methode (Rückrechnung)
* **Prinzip:** Der Verbrauch wird *nachträglich* und indirekt über die Menge der produzierten Ausbringungsgüter (Output) abgeleitet.
* **Erfassungsinstrument:** Stücklisten und Produktionsberichte.
* **Formel:** $$\text{Materialverbrauch} = \text{Produzierte Stückzahl} \times \text{Standardverbrauch laut Stückliste}$$
* **Nachteil:** Materialverluste, Ausschuss oder Diebstahl werden nicht separat erfasst, sondern erhöhen intransparent den kalkulatorischen Verbrauch.

----
### Fallstudie A: Kraftstoffverbrauch im Transportbetrieb
* **Klassifikation:** **Zweckaufwand** (= Grundkosten).
* **Begründung:** Der Verzehr mindert das Eigenkapital der Periode in der GuV (**Aufwand**) und dient gleichzeitig direkt dem primären Betriebszweck des Transportierens (**Kosten**).

### Fallstudie B: Anlagenverkauf auf Ziel über Buchwert
* **Stromgrößen-Abgrenzung:** **Einnahme** und **Ertrag** fallen zeitgleich an.
* **Analyse:**
  1. **Einnahme:** Der Verkauf „auf Ziel“ erhöht die Forderungen aus Lieferungen und Leistungen ($LuL$). Damit steigt das liquide Geldvermögen ($\text{Zahlungsmittelbestand} + \text{Forderungen} - \text{Verbindlichkeiten}$).
  2. **Ertrag:** Der Erlösanteil, der den bilanziellen Buchwert übersteigt, stellt einen außerordentlichen/periodenfremden Wertezuwachs dar, welcher das Eigenkapital in der Bilanz erhöht.

---

## 3. Kalkulatorische Kapitalverzinsung im Anlagevermögen

Kalkulatorische Zinsen erfassen die Opportunitätskosten des im Betrieb gebundenen Kapitals. Für abnutzbare Anlagegüter existieren zwei Rechenverfahren:

### A. Durchschnittsmethode (Standardverfahren)
Geht davon aus, dass das gebundene Kapital durch die lineare Abschreibung im Zeitverlauf gleichmäßig sinkt. Es wird über die gesamte Laufzeit hinweg ein konstanter, durchschnittlicher Zinsbetrag angesetzt.

* **Berechnung des durchschnittlich gebundenen Kapitals ($K_{\emptyset}$):**
  $$K_{\emptyset} = \frac{\text{Anschaffungswert} + \text{Restwert}}{2}$$
* **Kalkulatorische Zinsen pro Jahr ($Z_{\text{kalk}}$):**
  $$Z_{\text{kalk}} = K_{\emptyset} \cdot i$$

> **Anwendungsbeispiel (Restwert = 0 EUR, AW = 10.000 EUR, i = 5%):**
> $$K_{\emptyset} = \frac{10.000\ \text{EUR}}{2} = 5.000\ \text{EUR}$$
> $$Z_{\text{kalk}} = 5.000\ \text{EUR} \cdot 0,05 = \mathbf{250\ \text{EUR / Jahr}}$$

### B. Restwertmethode (Zinsstaffelmethode)
Berechnet die Zinsen in jeder Periode neu auf Basis des exakten, aktuellen Buchwerts (Restwerts) am Periodenanfang.
* **Effekt:** Die kalkulatorischen Zinskosten sinken degressiv von Jahr zu Jahr parallel zur fortschreitenden Abschreibung der Anlage.

# 📊 Systematisierung der Kosten- und Leistungsrechnung (Teil 2)

## 1. Institutionelle Abgrenzung des Rechnungswesens

Das betriebliche Rechnungswesen spaltet sich in zwei komplementäre Teilsysteme mit divergenten Adressaten und Zielsetzungen.

### Externes Rechnungswesen (Finanzbuchhaltung / FiBu)
* **Adressaten:** Externe Interessenten (Finanzamt, Banken, Gläubiger, Aktionäre, Öffentlichkeit).
* **Regelwerk:** Streng kodifiziert nach HGB / IFRS (Zweck: Gläubigerschutz, Fiskalbasis, Ausschüttungsbemessung).
* **Instrumente:** Bilanz, Gewinn- und Verlustrechnung (GuV), Anhang, Lagebericht.

### Internes Rechnungswesen (Kosten- und Leistungsrechnung / KLR)
* **Adressaten:** Interne Entscheidungsträger (Unternehmensleitung, Controlling, Abteilungsleiter).
* **Regelwerk:** Kaum gesetzliche Vorgaben; freie Ausgestaltung nach ökonomischen Zweckmäßigkeiten.
* **Instrumente:** Betriebsabrechnungsbogen (BAB), Kalkulationen, Abweichungsanalysen.
* **Zweck:** Betriebswirtschaftliche Dokumentation, Planung, Wirtschaftlichkeitskontrolle und fundierte Preispolitik.

---

## 2. Zurechenbarkeit von Kosten: Einzelkosten vs. Gemeinkosten

Die Kostenträgerrechnung differenziert Kosten danach, wie exakt sie einem finalen Endprodukt (**Kostenträger**) kausal zugeordnet werden können.

### A. Einzelkosten (Direkte Kosten)
Verursachungsgerechte Verrechnung direkt auf den Kostenträger ohne Zwischenschaltung von Kostenstellen.
* **Fertigungsmaterial (Rohstoffe):** Messbarer Materialverbrauch je Produkteinheit (z. B. Holzmenge für einen spezifischen Stuhl).
* **Fertigungslöhne:** Direkt am Produkt geleistete Arbeitszeit, erfasst über Stundenzettel, REFA-Zeitaufnahmen oder digitale BDE-Systeme (Betriebsdatenerfassung).

### B. Gemeinkosten (Indirekte Kosten / Overhead)
Kosten, die für mehrere Kostenträger gemeinsam anfallen. Eine direkte Zuordnung ist technisch unmöglich oder wirtschaftlich unzweckmäßig. Die Verteilung erfolgt indirekt über **Kostenstellen** mittels Verteilungsschlüsseln oder Zuschlagssätzen.
* **Verwaltungsgemeinkosten:** Gehälter der Buchhaltung, Personalabteilung oder Geschäftsführung. Diese Dienste unterstützen den Gesamtbetrieb, nicht das einzelne Produkt.

---

## 3. Stromgrößen-Matrix: Auszahlung vs. Einnahme

Zur präzisen Liquiditäts- und Erfolgsanalyse müssen Geld- und Werteflüsse trennscharf definiert werden.

### Auszahlung ($\Delta$ Zahlungsmittelbestand $< 0$)
* **Definition:** Abfluss von liquiden Mitteln (Bargeld + Sichtguthaben bei Banken).
* **Beispiel (Aktienkauf):** Der Barkauf von Aktien zur Beteiligung an einem Wettbewerber verringert sofort die Kasse/Bank. Es liegt eine **Auszahlung** vor. (Es ist *kein* Aufwand, sondern ein Aktivtausch: Flüssige Mittel sinken, Finanzanlagen steigen).

### Einnahme ($\Delta$ Geldvermögen $> 0$)
* **Definition:** Erhöhung des Geldvermögens ($\text{Zahlungsmittelbestand} + \text{Forderungen} - \text{Verbindlichkeiten}$).
* **Beispiel (Warenverkauf auf Kredit):** Ein Verkauf auf Ziel erhöht sofort die *Forderungen aus Lieferungen und Leistungen (LuL)*. Das Geldvermögen steigt im Moment des Verkaufs. Es liegt eine **Einnahme** vor, obwohl noch kein Bargeld fließt (keine Einzahlung).

---

## 📊 4. Synthese-Matrix der Klausurfragen (5–10)

| Aussage | Kernthese der Aufgabe | Status | Ökonomische Begründung |
| :--- | :--- | :--- | :--- |
| **5** | KLR dient primär externen Interessenten. | **FALSCH** | Die KLR ist das Instrument des *internen* Rechnungswesens zur Führung des Managements. |
| **6** | Materialkosten (Rohstoffe) sind Einzelkosten. | **RICHTIG** | Rohstoffe fließen direkt physisch in das Endprodukt ein und sind direkt mess- und zuordenbar. |
| **7** | Verwaltungsgehälter sind Kostenträgergemeinkosten. | **RICHTIG** | Verwaltungstätigkeiten erbringen Leistungen für die Gesamtorganisation, nicht für ein spezifisches Produkt. |
| **8** | Barkauf von Aktien ist eine Auszahlung. | **RICHTIG** | Der Bar- oder Bankabfluss reduziert unmittelbar den liquiden Zahlungsmittelbestand ($\text{Kasse}/\text{Bank}$). |
| **9** | Verkauf von Fertigware auf Kredit ist *keine* Einnahme. | **FALSCH** | Es entsteht eine Forderung, welche das Geldvermögen erhöht. Daher liegt explizit eine *Einnahme* vor. |
| **10** | Lohnkosten eines Fertigungsmitarbeiters sind Einzelkosten. | **RICHTIG** | Über Zeiterfassungssysteme (z. B. Stundenzettel) lässt sich die Arbeitszeit direkt dem Produkt zuschreiben (*Fertigungseinzellohn*). |

# 📊 Sekundärkostenverrechnung: Das Anbauverfahren (Blockverfahren)

Das **Anbauverfahren** (auch Blockverfahren genannt) ist das einfachste Verfahren der innerbetrieblichen Leistungsverrechnung (ILV). Es zeichnet sich durch eine radikale Vereinfachung des realen Leistungsflusses aus.

---

## 1. Theoretisches Kernkonzept

Das primäre Charakteristikum des Anbauverfahrens lautet: **Der gegenseitige Leistungsaustausch zwischen den Vorkostenstellen wird vollständig ignoriert.**

* **Fiktion:** Es wird unterstellt, dass Vorkostenstellen ihre Leistungen *ausschließlich* an Hauptkostenstellen abgeben.
* **Konsequenz:** Mathematisch müssen keine Gleichungssysteme gelöst werden. Die primären Gemeinkosten einer Vorkostenstelle werden direkt auf die empfangenden Hauptkostenstellen umgelegt.

## 2. Mathematischer Algorithmus (Schritt-für-Schritt)

### Schritt 1: Ermittlung der modifizierten Verrechnungsbasis
Um den Leistungsaustausch zwischen den Hilfskostenstellen zu eliminieren, wird die an andere Vorkostenstellen abgegebene Leistungsmenge von der Gesamtleistung subtrahiert:

$$\text{Relevante Leistungsbasis} = \text{Gesamte Leistungsabgabe} - \text{Leistungsabgabe an andere Vorkostenstellen}$$

### Schritt 2: Berechnung des Verrechnungspreises ($q$)
Die primären Gemeinkosten der Vorkostenstelle werden durch diese reduzierte Leistungsbasis dividiert:

$$q = \frac{\text{Primäre Gemeinkosten der Vorkostenstelle}}{\text{Relevante Leistungsbasis}}$$

### Schritt 3: Allokation auf die Hauptkostenstellen
Die sekundären Gemeinkosten einer Hauptkostenstelle ergeben sich durch Multiplikation der von ihr real bezogenen Leistungsmenge mit dem ermittelten Verrechnungspreis $q$.

---

## 3. Konkrete Fallstudie (Klausuraufgabe)

### Vorgabedaten & Verrechnungssätze

1. **Stromstelle:**
   * Primäre Gemeinkosten: $4.000\ \text{EUR}$
   * Gesamtleistung: $50.000\ \text{kWh}$ (davon $5.000\ \text{kWh}$ an Vorkostenstelle Reparatur)
   * Relevante Basis: $50.000 - 5.000 = 45.000\ \text{kWh}$
   * Verrechnungssatz: $$q_{\text{Strom}} = \frac{4.000\ \text{EUR}}{45.000\ \text{kWh}} = \mathbf{0,0889\ \text{EUR/kWh}}$$

2. **Reparaturstelle:**
   * Primäre Gemeinkosten: $19.500\ \text{EUR}$
   * Gesamtleistung: $2.000\ \text{h}$ (davon $100\ \text{h}$ an Vorkostenstelle Strom)
   * Relevante Basis: $2.000 - 100 = 1.900\ \text{h}$
   * Verrechnungssatz: $$q_{\text{Reparatur}} = \frac{19.500\ \text{EUR}}{1.900\ \text{h}} = \mathbf{10,2632\ \text{EUR/h}}$$

### Vollständiger Betriebsabrechnungsbogen (BAB)
*Gemäß Rundungsvorgabe: Verrechnungspreise auf 4 Nachkommastellen, EUR-Werte auf glatte Zahlen gerundet.*

| Kostenstelle / Posten | Material | Fertigung | Verwaltung | Vertrieb | Gesamt-Umlage |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Primäre Gemeinkosten** | **26.500 EUR** | **80.000 EUR** | **10.000 EUR** | **20.000 EUR** | *136.500 EUR* |
| Umlage Stromstelle | 889 EUR | 2.667 EUR | 178 EUR | 267 EUR | *4.000 EUR* |
| *Rechenweg Strom* | *(10.000 × 0,0889)* | *(30.000 × 0,0889)* | *(2.000 × 0,0889)* | *(3.000 × 0,0889)* | |
| Umlage Reparaturstelle | 3.079 EUR | 15.395 EUR | 205 EUR | 821 EUR | *19.500 EUR* |
| *Rechenweg Reparatur* | *(300 × 10,2632)* | *(1.500 × 10,2632)* | *(20 × 10,2632)* | *(80 × 10,2632)* | |
| **Sekundäre Gemeinkosten** | **3.968 EUR** | **18.062 EUR** | **383 EUR** | **1.088 EUR** | *23.500 EUR* |
| **Gesamte Gemeinkosten** | **30.468 EUR** | **98.062 EUR** | **10.383 EUR** | **21.088 EUR** | **160.000 EUR** |

---

## 4. Kritische Würdigung des Verfahrens

* **Vorteile:** Mit minimalem Rechenaufwand extrem schnell durchführbar. Keine mathematischen Vorkenntnisse (Matrixinversion) erforderlich.
* **Nachteile:** Ungenau bei starken Leistungsverflechtungen der Vorkostenstellen untereinander. Führt zu verfälschten Verrechnungspreisen und kann Fehlentscheidungen in der Produktkalkulation nach sich ziehen (Verstoß gegen das Verursachungsprinzip).
# 🧮 Sekundärkostenverrechnung: Das Gleichungsverfahren (Mathematisches Verfahren)

Das **Gleichungsverfahren** (auch mathematisches oder Simultanverfahren genannt) ist das exakteste Instrument der innerbetrieblichen Leistungsverrechnung (ILV). Es löst das Problem zyklischer Leistungsverflechtungen mathematisch simultan auf.

---

## 1. Theoretisches Kernkonzept

Im Gegensatz zu Heuristiken (wie dem Anbauverfahren) bildet das Gleichungsverfahren den **gegenseitigen Leistungsaustausch** zwischen Hilfskostenstellen realitätsgetreu ab.

* **Prinzip:** Eine Vorkostenstelle verbraucht oft Eigenleistungen einer anderen Vorkostenstelle (z. B. die Stromstelle benötigt Reparaturstunden, die Reparaturstelle benötigt Strom).
* **Mathematischer Ansatz:** Jede Vorkostenstelle wird als lineare Gleichung abgebildet. Die Verrechnungspreise werden durch das Lösen eines linearen Gleichungssystems (LGS) simultan bestimmt.
   [ Vorkostenstelle A ] <=========> [ Vorkostenstelle B ]
             |        (Wechselseitige)       |
             |          Leistung             |
             |                               |
  +----------+----------+        +----------+----------+
  |          |          |        |          |          |
  v          v          v        v          v          v

[ Haupt-KS ] [ Haupt-KS ] [ Haupt-KS ] [ Haupt-KS ] [ Haupt-KS ]

Material Fertigung Verwaltung Vertrieb ...

## 2. Mathematisches Gleichungssystem

Die allgemeine Struktur für die Gesamtkosten $K_i$ einer Vorkostenstelle lautet:

$$\text{Gesamtkosten} = \text{Primäre Gemeinkosten} + \text{Sekundäre Gemeinkosten (Zulieferungen)}$$

Für das konkrete Fallbeispiel mit der Stromstelle ($P_S$) und der Reparaturstelle ($P_R$):

### I. Gleichungsaufstellung
1. **Stromstelle:** $$4.000 + 100 \cdot P_R = 50.000 \cdot P_S$$
2. **Reparaturstelle:** $$19.500 + 5.000 \cdot P_S = 2.000 \cdot P_R$$

### II. Exakte Berechnung der Verrechnungssätze
Durch Substitution von $P_S$ in Gleichung II:

$$19.500 + 5.000 \cdot \left(\frac{4.000 + 100 \cdot P_R}{50.000}\right) = 2.000 \cdot P_R$$
$$19.500 + 400 + 10 \cdot P_R = 2.000 \cdot P_R$$
$$19.900 = 1.990 \cdot P_R \implies \mathbf{P_R = 10\ \text{EUR/h}}$$

Einsetzen von $P_R$ in Gleichung I liefert:

$$4.000 + 100 \cdot 10 = 50.000 \cdot P_S \implies \mathbf{P_S = 0,10\ \text{EUR/kWh}}$$

---

## 📊 3. Endgültiger Betriebsabrechnungsbogen (BAB)
*Gemäß Klausurvorgabe: Verrechnungspreise exakt, EUR-Werte auf glatte Zahlen gerundet.*

| Kostenstelle / Posten | Material | Fertigung | Verwaltung | Vertrieb | Gesamt-Umlage |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Primäre Gemeinkosten** | **26.500 EUR** | **80.000 EUR** | **10.000 EUR** | **20.000 EUR** | *136.500 EUR* |
| Umlage Stromstelle | 1.000 EUR | 3.000 EUR | 200 EUR | 300 EUR | *4.500 EUR\** |
| *Rechenweg Strom* | *(10.000 × 0,10)* | *(30.000 × 0,10)* | *(2.000 × 0,10)* | *(3.000 × 0,10)* | |
| Umlage Reparaturstelle | 3.000 EUR | 15.000 EUR | 200 EUR | 800 EUR | *19.000 EUR\** |
| *Rechenweg Reparatur* | *(300 × 10)* | *(1.500 × 10)* | *(20 × 10)* | *(80 × 10)* | |
| **Sekundäre Gemeinkosten** | **4.000 EUR** | **18.000 EUR** | **400 EUR** | **1.100 EUR** | *23.500 EUR* |
| **Gesamte Gemeinkosten** | **30.500 EUR** | **98.000 EUR** | **10.400 EUR** | **21.100 EUR** | **160.000 EUR** |

*\*Hinweis zur Kontrollsumme:* Die umgelegten Gesamtkosten der Vorkostenstellen ($4.500\ \text{EUR} + 19.000\ \text{EUR} = 23.500\ \text{EUR}$) entsprechen exakt der Summe ihrer primären Gemeinkosten ($4.000\ \text{EUR} + 19.500\ \text{EUR}$). Die innerbetriebliche Verflechtung hebt sich mathematisch auf Null auf.

---

## 🔍 4. Methodischer Vergleich: Anbau vs. Gleichung

Warum weichen die Ergebnisse der beiden Verfahren voneinander ab?

| Dimension | Anbauverfahren (1) | Gleichungsverfahren (2) |
| :--- | :--- | :--- |
| **Innerbetrieblicher Fokus** | Ignoriert Leistungsaustausch zwischen Vorkostenstellen komplett. | Bildet gegenseitige Leistungsbeziehungen exakt und simultan ab. |
| **Mathematische Basis** | Reduktion des Nenners (Leistungsbasis wird gekürzt). | Lineares Gleichungssystem ($n$ Gleichungen mit $n$ Variablen). |
| **Genauigkeit** | Ungenau (Näherungsverfahren). Verstoß gegen das Verursachungsprinzip. | Absolut exakt. Mathematisch fehlerfreie Allokation. |
| **Konkretes Ergebnisdelta** | **Material:** $30.468\ \text{EUR}$<br>**Fertigung:** $98.062\ \text{EUR}$ | **Material:** $30.500\ \text{EUR}$ ($\mathbf{+32\ \text{EUR}}$)<br>**Fertigung:** $98.000\ \text{EUR}$ ($\mathbf{-62\ \text{EUR}}$) |

### Ökonomische Begründung der Differenz
Da das Anbauverfahren die Verflechtungsströme ($5.000\ \text{kWh}$ an Reparatur und $100\ \text{h}$ an Strom) ausblendet, verschieben sich die resultierenden Verrechnungspreise künstlich ($q_{\text{Strom}} \approx 0,0889$ vs. $P_S = 0,10$). Dies führt zu einer Fehlallokation auf den Hauptkostenstellen. Erst das Gleichungsverfahren ordnet die Kosten exakt dort zu, wo die Leistungen final verbraucht werden.

# 📈 Kostenstellenauswertung: Zuschlagskalkulation & Herstellkosten

Nach Abschluss der Sekundärkostenverrechnung (im BAB) bildet die Ermittlung der **Gemeinkostenzuschlagssätze** das Bindeglied zwischen der Kostenstellenrechnung und der Kostenträgerrechnung (Kalkulation der Produkte).

---

## 1. Mathematisches Grundschema (Zuschlagsbasen)

Gemeinkostenzuschlagssätze setzen die Gemeinkosten einer Hauptkostenstelle ins Verhältnis zu einer sachlich passenden Bezugsgröße (in der Regel den jeweiligen Einzelkosten).

$$\text{Zuschlagssatz (\%)} = \frac{\text{Gemeinkosten der Kostenstelle}}{\text{Einzelkosten (Bezugsgröße)}} \cdot 100$$

### Die Verrechnungsstrukturen im klassischen BAB:
* **Materialbereich:** Gemeinkosten bezogen auf die Materialeinzelkosten (MEK).
* **Fertigungsbereich:** Gemeinkosten bezogen auf die Fertigungseinzelkosten (FEK).
* **Verwaltungs- & Vertriebsbereich:** Gemeinkosten bezogen auf die gesamten **Herstellkosten**.

---

## 2. Kalkulationsschema (Schritt-für-Schritt)

### Schritt 1: Berechnung der Herstellkosten (HSK)
Die Herstellkosten des Zeitraums fassen alle direkt und indirekt in der Produktion angefallenen Kosten zusammen:

$$\begin{aligned}
& \phantom{+} \text{Materialeinzelkosten (MEK)} \\
& + \text{Materialgemeinkosten (MGK)} \\
& + \text{Fertigungseinzelkosten (FEK)} \\
& + \text{Fertigungsgemeinkosten (FGK)} \\
\hline
& = \mathbf{\text{Herstellkosten (HSK)}}
\end{aligned}$$

### Schritt 2: Berechnung der Verwaltungs- und Vertriebszuschläge
Da Verwaltungs- und Vertriebsaktivitäten der Unterstützung des gesamten betrieblichen Leistungsprozesses dienen, bilden die Herstellkosten ihre gemeinsame Basis.

---

## 3. Konkrete Fallstudie (Klausuraufgabe)

### Ausgangsdaten (Basis: Anbauverfahren)
* $\text{MEK} = 100.000\ \text{EUR}$ | $\text{FEK} = 50.000\ \text{EUR}$
* $\text{MGK} = 30.468\ \text{EUR}$ | $\text{FGK} = 98.061\ \text{EUR}$
* $\text{VwGK} = 10.383\ \text{EUR}$ | $\text{VtGK} = 21.088\ \text{EUR}$

### I. Exakte Ermittlung der Herstellkosten
$$100.000\ \text{EUR} + 30.468\ \text{EUR} + 50.000\ \text{EUR} + 98.061\ \text{EUR} = \mathbf{278.529\ \text{EUR}}$$

### II. Berechnung & kaufmännische Rundung der Zuschlagssätze
*Gemäß Klausurvorgabe: Exakt gerundet auf genau 2 Nachkommastellen.*

| Hauptkostenstelle | Mathematischer Ansatz | Ungekürzter Wert | Gerundeter Klausurwert |
| :--- | :--- | :--- | :--- |
| **Materialzuschlag ($Z_M$)** | $\frac{30.468\ \text{EUR}}{100.000\ \text{EUR}} \cdot 100$ | $30,468\%$ | **30,47 %** (aufgerundet) |
| **Fertigungszuschlag ($Z_F$)** | $\frac{98.061\ \text{EUR}}{50.000\ \text{EUR}} \cdot 100$ | $196,122\%$ | **196,12 %** (abgerundet) |
| **Verwaltungszuschlag ($Z_{Vw}$)** | $\frac{10.383\ \text{EUR}}{278.529\ \text{EUR}} \cdot 100$ | $3,72779\%$ | **3,73 %** (aufgerundet) |
| **Vertriebszuschlag ($Z_{Vt}$)** | $\frac{21.088\ \text{EUR}}{278.529\ \text{EUR}} \cdot 100$ | $7,57120\%$ | **7,57 %** (abgerundet) |

---

## 🔍 4. Typische Fehlerquellen in Klausuren

> [!CAUTION] **Flüchtigkeitsfehler-Warnung**
> 1. **Rundungsvorgaben missachten:** Das Beibehalten von 3 Nachkommastellen (wie $30,468\%$) führt trotz richtigem Rechenweg zu formalem Punktabzug.
> 2. **Falsche Zuschlagsbasis bei Vw/Vt:** Ein beliebter Fehler ist es, die Verwaltungs- und Vertriebsgemeinkosten fälschlicherweise auf die Einzelkosten zu beziehen, statt auf die summierten **Herstellkosten** ($278.529\ \text{EUR}$).
> 3. **Additionsfehler bei HSK:** Ein einfacher Rechenfehler bei der Summe der Herstellkosten pflanzt sich als Folgefehler linear in die Sätze für Verwaltung und Vertrieb fort.

# 📉 Break-Even-Analyse (Gewinnschwellenanalyse)

Die **Break-Even-Analyse** ist ein zentrales Instrument der operativen Unternehmensplanung und des Controllings. Sie bestimmt die Absatzmenge (oder den Umsatz), bei der die Erlöse eines Unternehmens exakt dessen Gesamtkosten decken. An diesem Punkt ist der Erfolg (Gewinn) genau Null.

---

## 1. Kostentheoretische Grundlagen

Die Analyse basiert auf der **Teilkostenrechnung** und setzt die Verhaltenssteuerung von Kosten bei Beschäftigungsänderungen voraus:

* **Fixkosten ($K_f$):** Beschäftigungsunabhängige Kosten (z. B. zeitabhängige Abschreibungen, Gehälter, Mieten), die kurzfristig konstant bleiben, degressiv sinken jedoch die fixen Stückkosten ($k_f$) bei steigender Menge.
* **Variable Kosten ($K_v$):** Beschäftigungsabhängige Kosten (z. B. produktionsabhängige Akkordlöhne, Rohstoffe), die sich proportional zur Produktionsmenge ($x$) verhalten. Die variablen Stückkosten ($k_v$) bleiben konstant.
* **Gesamtkosten ($K$):** Die Summe aus fixen und variablen Kosten:
    $$K = K_f + K_v = K_f + k_v \cdot x$$

---

## 2. Der Deckungsbeitrag (Contribution Margin)

Der Deckungsbeitrag gibt an, wie viel ein verkauftes Produkt zur Deckung der Fixkosten beiträgt, nachdem die variablen Kosten gedeckt sind.

* **Stückdeckungsbeitrag ($db$):**
    $$db = p - k_v$$
    *(wobei $p$ = Stückpreis)*
* **Gesamtdeckungsbeitrag ($DB$):**
    $$DB = E - K_v = db \cdot x$$
    *(wobei $E$ = Gesamterlös/Umsatz)*

---

## 3. Mathematische Herleitung der Break-Even-Menge

Die Gewinnschwelle ist definiert durch das Kriterium: $\text{Gewinn } (G) = 0$, was äquivalent zu $\text{Erlös } (E) = \text{Gesamtkosten } (K)$ ist.

$$\begin{aligned}
E &= K \\
p \cdot x &= K_f + k_v \cdot x \quad \lvert \, - (k_v \cdot x) \\
p \cdot x - k_v \cdot x &= K_f \\
x \cdot (p - k_v) &= K_f \quad \lvert \, : (p - k_v) \\
\mathbf{x_{BEP}} &= \mathbf{\frac{K_f}{p - k_v} = \frac{K_f}{db}}
\end{aligned}$$

> [!NOTE] **Interpretation**
> Die Break-Even-Menge ($x_{BEP}$) dividiert die gesamten Fixkosten durch den Stückdeckungsbeitrag. Sie zeigt an, wie viele Einheiten verkauft werden müssen, um die Fixkosten-Barriere vollständig abzutragen.

---

## 📊 4. Empirische Anwendung (Fallstudie)

### I. Datenbasis (Auszug aus operativem Jahr)
* **Absatz/Produktion ($x$):** $100.000\ \text{Stück}$
* **Stückpreis ($p$):** $32{,}00\ \text{EUR}$
* **Kostenstruktur:**
    * *Variable Kosten:* Akkordlöhne ($50.000\ \text{EUR}$) + Rohstoffe ($70.000\ \text{EUR}$) = **$120.000\ \text{EUR}$**
    * *Fixe Kosten:* Abschreibungen ($15.000\ \text{EUR}$) + Gehälter ($100.000\ \text{EUR}$) + Miete ($15.000\ \text{EUR}$) = **$130.000\ \text{EUR}$**

### II. Kennzahlenermittlung
* **Variable Stückkosten ($k_v$):** $\frac{120.000\ \text{EUR}}{100.000\ \text{Stck}} = \mathbf{1{,}20\ \text{EUR/Stck}}$
* **Fixe Stückkosten ($k_f$):** $\frac{130.000\ \text{EUR}}{100.000\ \text{Stck}} = \mathbf{1{,}30\ \text{EUR/Stck}}$
* **Stückdeckungsbeitrag ($db$):** $32{,}00\ \text{EUR} - 1{,}20\ \text{EUR} = \mathbf{30{,}80\ \text{EUR/Stck}}$

### III. Berechnung der Gewinnschwelle
$$x_{BEP} = \frac{130.000\ \text{EUR}}{30{,}80\ \text{EUR/Stck}} \approx 4220{,}779$$

Da unvollständige Stücke am Markt nicht abgesetzt werden können, muss zur Erreichung der Verlustfreiheit stets auf die nächste ganze Zahl **aufgerundet** werden:
$$\mathbf{x_{BEP} = 4.221\ \text{Stück}}$$

---

## 🔍 5. Kritische Würdigung & Prämissen

Die klassische Break-Even-Analyse unterliegt restriktiven Modellannahmen (Linearantwortmodell):
1. **Linearität:** Konstante Verkaufspreise und konstante variable Stückkosten über die gesamte Beschäftigungsbreite (keine Mengenrabatte, keine Skaleneffekte).
2. **Eingütermodell:** Es wird entweder nur ein Produkt betrachtet oder ein konstanter Produktmix vorausgesetzt.
3. **Lagerhaltungsfreiheit:** Die Produktionsmenge entspricht exakt der Absatzmenge ($\Delta \text{Lager} = 0$).

# 📊 Differenzierende (Mehrstufige) Zuschlagskalkulation

Die differenzierende Zuschlagskalkulation spaltet die Gemeinkosten in mehrere Material- und Fertigungsbereiche auf. Dies erhöht die Verursachungsgerechtigkeit im Vergleich zur einstufigen Zuschlagskalkulation erheblich, da Produkte die Kostenstellen nur nach ihrer tatsächlichen Inanspruchnahme belasten.

---

## 1. Kalkulationsschema (Mehrstufiger Aufbau)

Bei mehreren Hauptkostenstellen werden die Gemeinkosten stufenweise auf die Einzelkosten der jeweiligen Stellen aufgeschlagen, um die Herstellkosten zu ermitteln. Verwaltung und Vertrieb werden anschließend auf Basis der gesamten Herstellkosten zugeschlagen.

```text
   Materialeinzelkosten I (MEK I)
+  Materialgemeinkosten I (MGK I)       -> (Basis: MEK I)
+  Materialeinzelkosten II (MEK II)
+  Materialgemeinkosten II (MGK II)     -> (Basis: MEK II)
+  Fertigungseinzelkosten I (FEK I)
+  Fertigungsgemeinkosten I (FGK I)     -> (Basis: FEK I)
+  Fertigungseinzelkosten II (FEK II)
+  Fertigungsgemeinkosten II (FGK II)   -> (Basis: FEK II)
-----------------------------------------------------------------
=  Herstellkosten der Periode (HK)
+  Verwaltungsgemeinkosten (VwGK)       -> (Basis: HK)
+  Vertriebsgemeinkosten (VtGK)         -> (Basis: HK)
-----------------------------------------------------------------
=  Selbstkosten (SK)
````

## 2. Ermittlung der Zuschlagssätze (Periodenbetrachtung)

**Grundformel:** Zuschlagssatz = (Gemeinkosten der Stelle / Einzelkosten der Stelle) * 100

### Datenbasis & Ergebnisse der Kostenstellenrechnung:

- **Herstellkosten-Basis der Periode:** 691.080,00 EUR (Summe aller Kosten der Material- und Fertigungsstellen)
    

|**Kostenstelle**|**Einzelkosten (Basis)**|**Gemeinkosten (Stelle)**|**Zuschlagssatz (%)**|
|---|---|---|---|
|**Materialstelle I**|68.300,00 EUR|40.980,00 EUR|**60,00 %**|
|**Materialstelle II**|55.000,00 EUR|41.800,00 EUR|**76,00 %**|
|**Fertigungsstelle I**|160.000,00 EUR|40.000,00 EUR|**25,00 %**|
|**Fertigungsstelle II**|250.000,00 EUR|35.000,00 EUR|**14,00 %**|
|**Verwaltung**|691.080,00 EUR (HK)|86.385,00 EUR|**12,50 %**|
|**Vertrieb**|691.080,00 EUR (HK)|120.939,00 EUR|**17,50 %**|

## 3. Kostenträgerstückrechnung (Kalkulation Produkt X)

_Hinweis: Konsequente kaufmännische Rundung auf genau zwei Nachkommastellen pro Zeile._

- **Materialeinzelkosten I:** 49,00 EUR
    
- **+ Materialgemeinkosten I (60,00 %):** 29,40 EUR
    
- **+ Materialeinzelkosten II:** 110,00 EUR
    
- **+ Materialgemeinkosten II (76,00 %):** 83,60 EUR
    
- **+ Fertigungseinzelkosten I:** 205,00 EUR
    
- **+ Fertigungsgemeinkosten I (25,00 %):** 51,25 EUR
    
- **+ Fertigungseinzelkosten II:** 190,00 EUR
    
- **+ Fertigungsgemeinkosten II (14,00 %):** 26,60 EUR
    

- **= Herstellkosten (HK) pro Stück:** **744,85 EUR**
    
- **+ Verwaltungsgemeinkosten (12,50 % von HK):** 93,11 EUR _(gerundet von 93,106)_
    
- **+ Vertriebsgemeinkosten (17,50 % von HK):** 130,35 EUR _(gerundet von 130,349)_
    

- **= Selbstkosten (SK) pro Stück:** **968,31 EUR**
    

## 🔍 4. Typische Klausur-Fallstricke

> [!CAUTION] **Kostenabgrenzung & Basisfehler**
> 
> 1. **Hilfslöhne vs. Fertigungslöhne:** Fertigungslöhne sind immer Einzelkosten (Zuschlagsbasis). Hilfslöhne zählen laut Definition und Klausurvorgabe zu den Gemeinkosten (Zähler im Zuschlagssatz).
>     
> 2. **Gehälter & Abschreibungen:** Gehälter und zeitabhängige Abschreibungen lassen sich keinem Produkt direkt zuordnen und fließen vollständig in die Gemeinkosten der jeweiligen Stelle ein.
>     
> 3. **Gemeinsame Basis für Vw/Vt:** VwGK und VtGK dürfen niemals auf die Material- oder Fertigungs-EK bezogen werden. Ihre gemeinsame Basis sind immer die gesamten, zuvor ermittelten Herstellkosten (HK).
# 💶 Verkaufskalkulation & Ergänzende Kostenträgerrechnung

Die Verkaufskalkulation (Kostenträgererfolgsrechnung) ermittelt auf Basis der Selbstkosten den endgültigen Brutto- bzw. Nettolistenverkaufspreis für den Kunden. Dabei müssen Erlösminderungen (Skonto, Rabatt) und der geplante Gewinn einkalkuliert werden.

---

## 1. Kalkulationsschema (Vorwärtskalkulation)

Da Kunden angebotene Rabatte und Skonti vom Rechnungsbetrag *abziehen*, müssen diese Beträge in der Kalkulation vom Zielwert aus rückwärts ("im Hundert") aufgeschlagen werden.

```text
   Selbstkosten (SK)
+  Gewinnaufschlag (%)                  -> Basis: SK (vom Hundert)
---------------------------------------------------------------------
=  Barverkaufspreis (BVP)               -> Basis für Skonto (= 100% - Skonto%)
+  Kundenskonto (%)                     -> Berechnung "im Hundert"
---------------------------------------------------------------------
=  Zielverkaufspreis (ZVP)              -> Basis für Rabatt (= 100% - Rabatt%)
+  Kundenrabatt (%)                     -> Berechnung "im Hundert"
---------------------------------------------------------------------
=  Listenverkaufspreis (LVP, netto)     -> Angebotspreis exkl. USt.
````

## 2. Mathematische Formeln ("Im Hundert")

Standardprozentrechnung ("vom Hundert") scheitert bei Skonto und Rabatt, da der Prozentwert auf eine Summe bezogen ist, die im Kalkulationsschritt noch gar nicht bekannt ist.

### Kundenskonto (Ermittlung des ZVP):

$$\text{ZVP} = \frac{\text{BVP}}{100 - \text{Skonto}\%} \cdot 100$$

$$\text{Skontobetrag} = \text{ZVP} - \text{BVP}$$

### Kundenrabatt (Ermittlung des LVP):

$$\text{LVP} = \frac{\text{ZVP}}{100 - \text{Rabatt}\%} \cdot 100$$

$$\text{Rabattbetrag} = \text{LVP} - \text{ZVP}$$

## 3. Fallbeispiel: Produkt X

_Vorgaben: SK = 968,00 €, Gewinn = 232,00 €, Skonto = 2 %, Rabatt = 10 %. Konsequente kaufmännische Rundung auf zwei Nachkommastellen._

- **Selbstkosten (SK):** 968,00 EUR
    
- **+ Gewinnaufschlag (fix):** 232,00 EUR
    

- **= Barverkaufspreis (BVP):** **1.200,00 EUR** `(entspricht 98% des ZVP)`
    
- **+ Kundenskonto (2 % im Hundert):** 24,49 EUR `(1.200 / 98 * 2)`
    

- **= Zielverkaufspreis (ZVP):** **1.224,49 EUR** `(entspricht 90% des LVP)`
    
- **+ Kundenrabatt (10 % im Hundert):** 136,05 EUR `(1.224,49 / 90 * 10)`
    

- **= Listenverkaufspreis (LVP):** **1.360,54 EUR**
    

## 🔍 4. Analytische Klausurkomponenten

> [!INFO] **Plausibilitätsprüfung des Produktionsprogramms**
> 
> Ob ein Unternehmen exklusiv die kalkulierten Produkte herstellt, lässt sich über die Ganzzahligkeit der Periodenmengen prüfen:
> 
> $$\text{Theoretische Menge} = \frac{\text{Gesamte Einzelkosten der Stelle in der Periode}}{\text{Einzelkosten des Produkts pro Stück}}$$
> 
> Ergibt diese Division keine reelle Ganzzahl ($\in \mathbb{N}$), ist bewiesen, dass die Kostenstelle in der Periode noch durch andere, nicht explizit aufgeführte Kostenträger beansprucht wurde.

> [!💡] **Kostenstellen-Zuordnung von Abschreibungen**
> 
> Abschreibungen erfassen den wertmäßigen Verschleiß des Anlagevermögens und müssen verursachungsgerecht den Hauptkostenstellen zugeordnet werden:
> 
> - **Fertigungsstelle:** Abschreibung auf produktionsrelevante Sachanlagen (z. B. CNC-Fräsmaschinen, Schweißroboter, Fabrikhallen).
>     
> - **Materialstelle:** Abschreibung auf Logistik- und Lagerinfrastruktur (z. B. Förderzeuge/Gabelstapler, Hochregalsysteme, Lagergebäude).
>