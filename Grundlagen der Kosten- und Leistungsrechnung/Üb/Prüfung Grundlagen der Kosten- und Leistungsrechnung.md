## 1. Abgrenzung der Stromgrößen im Rechnungswesen

Die exakte Trennung der Begriffspaare ist essenziell für die Abgrenzung zwischen externem Rechnungswesen (Finanzbuchhaltung) und internem Rechnungswesen (KLR).

| Begriff | Definition | Liquiditäts-/Vermögensänderung | Beispiel (Rohstoffe) |
| :--- | :--- | :--- | :--- |
| **Auszahlung** | Abfluss liquider Mittel (Bar + Bank) | Minderung des Zahlungsmittelbestands | Spätere Begleichung der Lieferantenrechnung per Banküberweisung. |
| **Ausgabe** | Wert aller zugegangenen Güter/Dienstleistungen | Minderung des Geldvermögens (inkl. Forderungen/Verbindlichkeiten) | Einkauf von Rohstoffen auf Ziel (Kredit). *Verbindlichkeiten steigen*. |
| **Aufwand** | Gesamter wertmäßiger Güterverzehr einer Periode | Minderung des Reinvermögens (Eigenkapital) | Physischer Verbrauch der Rohstoffe in der Produktion. |
| **Kosten** | Betriebsbedingter, ordentlicher Güterverzehr | Minderung des betriebsnotwendigen Vermögens | Einsatz der Rohstoffe zur Herstellung des betrieblichen Kernprodukts. |

---

## 2. Innerbetriebliche Leistungsverrechnung (ILV): Stufenleiterverfahren

Das **Stufenleiterverfahren** (auch Treppenverfahren) dient der schrittweisen Umlage von Gemeinkosten der Hilfskostenstellen (Vorkostenstellen) auf nachgelagerte Stellen im Betriebsabrechnungsbogen (BAB).

> [!CRITICAL] **Relevanz der Reihenfolge**
> Die Reihenfolge der Abrechnung der Vorkostenstellen ist **nicht** beliebig. 
> * Sobald eine Kostenstelle abgerechnet ist, gilt sie als **geschlossen**.
> * Leistungsbeziehungen von einer später abgerechneten Stelle zurück zu einer bereits geschlossenen Stelle werden **ignoriert**.
> * **Ziel der Anordnung:** Sukzessive Abrechnung nach dem Grad der Eigenversorgung (die Stelle mit den geringsten Empfängen von anderen Hilfsstellen beginnt), um Verrechnungsfehler zu minimieren.

---

## 3. Kalkulationsverfahren: Äquivalenzziffernkalkulation

Wird angewendet bei der **Sortenfertigung** (verwandte Produkte mit ähnlichen Rohstoffen/Herstellungsprozessen).

* **Basisprodukt:** Erhält die normierte Äquivalenzziffer ($\ddot{A}Z_1 = 1{,}0$).
* **Normierung:** Die Äquivalenzziffern der übrigen Sorten werden durch **Division** ihrer spezifischen Kostentreiber (z. B. Gewicht, Bearbeitungszeit) durch den Wert des Basisprodukts ermittelt:
$$\ddot{A}Z_i = \frac{\text{Eigenschaft Sorte } i}{\text{Eigenschaft Basisprodukt}}$$
* Die Kostenverteilung erfolgt anschließend über die Multiplikation von Produktionsmenge und Äquivalenzziffer zur Ermittlung der *Recheneinheiten*.

---

## 4. Deckungsbeitragsrechnung & Break-Even-Analyse

Die Teilkostenrechnung trennt streng in variable ($K_v$) und fixe Kosten ($K_f$), um die kurzfristige Erfolgsplanung zu unterstützen.

### Mathematische Kernformeln

* **Stückdeckungsbeitrag ($db$):**
$$db = p - k_v$$
*(mit $p =$ Stückpreis, $k_v =$ variable Stückkosten)*

* **Gesamtdeckungsbeitrag ($DB$):**
$$DB = E - K_v = x \cdot db$$
*(mit $E =$ Gesamterlöse, $K_v =$ variable Gesamtkosten, $x =$ Produktions-/Absatzmenge)*

* **Betriebsergebnis ($G$):**
$$G = DB - K_f$$

### Break-Even-Point (Gewinnschwelle)
Der Punkt, an dem die Gesamterlöse exakt den Gesamtkosten entsprechen ($E = K_g$). Das Unternehmen erwirtschaftet an dieser Schwelle weder Gewinn noch Verlust ($G = 0$).

$$\text{Break-Even-Menge } (x_{BEP}) = \frac{K_f}{db} = \frac{K_f}{p - k_v}$$

> [!INFO] **Wirtschaftliche Hebelwirkung (Ausschussreduktion)**
> Wird Ausschuss in einer bereits durchlaufenen Produktion auf $0$ reduziert, steigen die Herstellkosten nicht weiter an, da die Ressourcen bereits verbraucht wurden. Jedes zusätzlich verkaufte (fehlerfreie) Stück erhöht den Erlös um den vollen Verkaufspreis, wodurch der Gesamtgewinn linear um $\Delta G = \Delta x \cdot p$ ansteigt.

# 👥 Personalkostenrechnung & Kalkulatorische Periodenabgrenzung

Die Personalkostenrechnung ermittelt die gesamten primären Personalkosten einer Abrechnungsperiode. Für Zwecke des internen Controllings (Plan-Ist-Vergleiche, zeitliche Abgrenzung) werden unregelmäßige oder einmalige Zahlungen mittels kalkulatorischer Abgrenzung gleichmäßig auf die Monate verteilt.

---

## 1. Komponenten der Personalkosten in der KLR

Personalkosten unterteilen sich in direkt erfassbare Einzelkosten und betriebliche Gemeinkosten:

* **Fertigungslöhne (Einzelkosten):** Direkt auf den Kostenträger verrechenbare Arbeitszeiten (z. B. über Akkordsätze oder Zeiterfassungskarten).
* **Hilfslöhne & Gehälter (Gemeinkosten):** Nicht direkt zurechenbare Entgelte (z. B. Meistergehälter, Verwaltung, Geschäftsführung).
* **Personalnebenkosten (Gemeinkosten):** * *Gesetzlich:* Arbeitgeberanteile zur Sozialversicherung (Renten-, Kranken-, Arbeitslosen-, Pflegeversicherung, Berufsgenossenschaft).
	* *Tariflich / Betrieblich:* Einmalzahlungen wie Jahressonderzahlungen (Weihnachtsgeld) und Urlaubsentgelte.
	* *Kalkulatorisch:* Kosten für krankheitsbedingte Fehlzeiten und deren Substitution (z. B. durch externe Leiharbeitnehmer).

---

## 2. Mathematische Modellierung & Formelschema

### Jährliche Gesamtkosten ($PK_{\text{Jahr}}$)
$$PK_{\text{Jahr}} = L_{\text{Stamm}} + K_{\text{Leih}} + NK_{\text{Sozial}} + SZ_{\text{Sonder}}$$

* **Lohnkosten Stammbelegschaft ($L_{\text{Stamm}}$):**
$$L_{\text{Stamm}} = n \cdot h_{\text{Monat}} \cdot 12 \cdot w_{\text{Stamm}}$$
*(mit $n = \text{Anzahl Arbeiter}$, $h_{\text{Monat}} = \text{Arbeitsstunden/Monat}$, $w_{\text{Stamm}} = \text{Stundenlohn}$)*

* **Kosten Leiharbeitskräfte als Krankheitsersatz ($K_{\text{Leih}}$):**
$$K_{\text{Leih}} = h_{\text{Krank}} \cdot w_{\text{Leih}}$$
*(mit $h_{\text{Krank}} = \text{Gesamte Ausfallstunden}$, $w_{\text{Leih}} = \text{Stundensatz Leiharbeit}$)*

* **Sonderzahlungen ($SZ_{\text{Sonder}}$):**
$$SZ_{\text{Sonder}} = n \cdot (SZ_{\text{Urlaub}} + SZ_{\text{Weihnacht}})$$

### Kalkulatorische Monatsabgrenzung ($PK_{\text{Monat}}$)
Um saisonale Verzerrungen im monatlichen Erfolgsbericht zu eliminieren, wird das mathematische Durchschnittsprinzip angewendet:
$$PK_{\text{Monat}} = \left\lceil \frac{PK_{\text{Jahr}}}{12} \right\rceil \quad \text{(kaufmännisch gerundet)}$$

---

## 3. Fallbeispiel (Controlling-Analyse)

*Parameter: 20 Arbeiter, 160 Std./Monat, 20 €/Std. Grundlohn. Krankheitsausfall: 640 Std./Jahr kompensiert durch Leiharbeit zu 25 €/Std. Gesetzliche Sozialkosten: 180.000 €/Jahr. Sonderzahlungen: je 400 € Urlaubs- und Weihnachtsgeld pro Person.*

### Berechnung der Jahreskomponenten:
1. **Bruttolohn Stamm:** $20 \text{ Pers.} \cdot 160 \text{ Std.} \cdot 12 \text{ Monate} \cdot 20\ \text{€/Std.} = 768.000\ \text{€}$
2. **Kosten Leiharbeit:** $640 \text{ Std.} \cdot 25\ \text{€/Std.} = 16.000\ \text{€}$
3. **Gesetzliche Sozialkosten:** Vorgegeben $= 180.000\ \text{€}$
4. **Sonderzahlungen:** $20 \text{ Pers.} \cdot (400\ \text{€} + 400\ \text{€}) = 16.000\ \text{€}$

$$\mathbf{PK_{\text{Jahr}}} = 768.000\ \text{€} + 16.000\ \text{€} + 180.000\ \text{€} + 16.000\ \text{€} = \mathbf{980.000\ \text{€}}$$

### Monatliche Abgrenzung (Beispiel: Monat Januar)
Obwohl das Weihnachtsgeld real im Dezember abfließt und Krankheitswellen saisonal schwanken, belastet das Controlling jeden Monat mit dem exakt gleichen Abgrenzungsbetrag:
$$PK_{\text{Januar}} = \frac{980.000\ \text{€}}{12} = 81.666,\overline{66}\ \text{€} \approx \mathbf{81.667\ \text{€}}$$

---

## 🔍 4. Analytische Klausurkomponenten

> [!INFO] **Das Prinzip der kalkulatorischen Abgrenzung**
> Würde man in der KLR auf die monatliche Glättung verzichten und Kosten nach dem Realisations- oder Auszahlungszeitpunkt erfassen (wie in der Finanzbuchhaltung), würde der Monat Dezember durch die Ballung von Weihnachtsgeldern unzulässig unrentabel wirken. Die kalkulatorische Verteilung stellt die **Vergleichbarkeit** der Periodenergebnisse sicher.

> [!WARNING] **Fehlzeiten-Kalkulation**
> Der reguläre Lohn der Stammbelegschaft läuft auch während des Urlaubsmonats und der Krankheitstage weiter (Lohnfortzahlung). Die Kosten für die Leiharbeiter stellen daher **Zusatzaufwendungen** dar, die additiv zu den normalen Bruttolöhnen hinzuzurechnen sind, um den realen wertmäßigen Verzehr der Periode abzubilden.

# 📊 Lohnzuschlagskalkulation mit Ausschussberücksichtigung

Die Lohnzuschlagskalkulation ist ein Verfahren der Nutzeffekt- und Kostenträgerrechnung. Sie dient dazu, die Fertigungsgemeinkosten (FGK) über einen prozentualen Zuschlagsatz proportional auf die Fertigungseinzelkosten (FEK / Fertigungslöhne) zu verrechnen. Tritt in der Fertigung Ausschuss auf, erhöht dies die Stückkosten der verbleibenden, verkaufsfähigen Einheiten (Äquivalenzprinzip der Kostenverteilung auf Gutmengen).

---

## 1. Kostenstruktur und Verrechnungsprinzipien

* **Fertigungseinzelkosten (FEK):** Direkte Produktlöhne. Stehen keine expliziten Verrechnungssätze je Produkt fest, erfolgt die Allokation von Gesamtlohnsummen proportional über die beanspruchte Fertigungszeit (Maschinen- oder Mitarbeiterstunden).
* **Fertigungsgemeinkosten (FGK):** Indirekte Kosten der Fertigung (z. B. Abschreibungen auf Maschinen, Hallenmiete, Gehälter der Fertigungsleitung). Sie werden über den FGK-Zuschlagsatz auf die FEK aufgeschlagen.
* **Ausschuss (Scrap Rate):** Fehlerhafte Produktionseinheiten, die nicht veräußert werden können. Die für den Ausschuss angefallenen Herstellkosten müssen von der verbleibenden Gutmenge getragen werden, wodurch sich die kalkulatorischen Stückkosten ex post erhöhen.

---

## 2. Mathematische Formeln und Kennzahlen

### Proportionale FEK-Zuteilung über Zeitbasis
Zunächst wird die Gesamtfertigungszeit ($H_{\text{Gesamt}}$) ermittelt:
$$H_{\text{Gesamt}} = \sum_{i} (x_{\text{Prod}, i} \cdot t_{i})$$
*(mit $x_{\text{Prod}, i} = \text{Produktionsmenge von Produkt } i$, $t_{i} = \text{Vorgabezeit je Stück von Produkt } i$)*

Der kalkulatorische Stundensatz ($R_{\text{Std}}$) berechnet sich aus den gesamten Fertigungslöhnen ($L_{\text{Gesamt}}$):
$$R_{\text{Std}} = \frac{L_{\text{Gesamt}}}{H_{\text{Gesamt}}}$$

Die Fertigungseinzelkosten eines Produkts ($FEK_{i}$) lauten:
$$FEK_{i} = (x_{\text{Prod}, i} \cdot t_{i}) \cdot R_{\text{Std}}$$

### Gemeinkostenzuschlagsatz ($Z_{\text{FGK}}$)
Der Zuschlagsatz setzt die gesamten Fertigungsgemeinkosten ($FGK_{\text{Gesamt}}$) in Relation zu den gesamten Einzelkosten ($FEK_{\text{Gesamt}} = L_{\text{Gesamt}}$):
$$Z_{\text{FGK}} = \frac{FGK_{\text{Gesamt}}}{FEK_{\text{Gesamt}}} \cdot 100\%$$

Die gesamten Fertigungskosten eines Produkts ($FK_{i}$) betragen:
$$FK_{i} = FEK_{i} \cdot (1 + Z_{\text{FGK}})$$

### Gutmenge ($x_{\text{Gut}, i}$) und Stückkosten ($k_{\text{Stück}, i}$)
Die tatsächlich verkäufliche Menge reduziert sich um den Ausschussanteil ($a_{i}$):
$$x_{\text{Gut}, i} = x_{\text{Prod}, i} \cdot (1 - a_{i})$$

Die kalkulatorischen Fertigungskosten pro Stück ($k_{\text{Stück}, i}$) unter Berücksichtigung des Ausschusses steigen entsprechend:
$$k_{\text{Stück}, i} = \frac{FK_{i}}{x_{\text{Gut}, i}}$$

---

## 3. Exemplarisches Kalkulationsbeispiel

*Parameter: Gesamtlöhne = 500.000 €, Gesamt-FGK = 350.000 €.*

| Produkt | $x_{\text{Prod}}$ (Stck.) | Arbeitszeit $t$ (Std./Stck.) | Gesamtstunden $H$ | Ausschuss $a$ | Preis (€/Stck.) |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **A** | 1.000 | 0,10 | 100 | 15% | 400 |
| **B** | 10.000 | 0,05 | 500 | 15% | 100 |
| **C** | 4.000 | 0,10 | 400 | 20% | 500 |
| **Gesamt**| **15.000** | — | **1.000** | — | — |

### Schritt 1: FEK-Allokation via Stundensatz
* Kalkulatorischer Stundensatz: $R_{\text{Std}} = \frac{500.000\ \text{€}}{1.000\ \text{Std.}} = 500\ \text{€/Std.}$
* $FEK_{A} = 100 \cdot 500 = \mathbf{50.000\ \text{€}}$
* $FEK_{B} = 500 \cdot 500 = \mathbf{250.000\ \text{€}}$
* $FEK_{C} = 400 \cdot 500 = \mathbf{200.000\ \text{€}}$

### Schritt 2: FGK-Zuschlag
* Zuschlagsatz: $Z_{\text{FGK}} = \frac{350.000\ \text{€}}{500.000\ \text{€}} = \mathbf{70\%}$
* $FK_{A} = 50.000\ \text{€} \cdot 1,70 = \mathbf{85.000\ \text{€}}$
* $FK_{B} = 250.000\ \text{€} \cdot 1,70 = \mathbf{425.000\ \text{€}}$
* $FK_{C} = 200.000\ \text{€} \cdot 1,70 = \mathbf{340.000\ \text{€}}$

### Schritt 3: Ausschuss- und Stückkostenrechnung
* **Produkt A:** $x_{\text{Gut}} = 1.000 \cdot 0,85 = 850\ \text{Stck.} \implies k_{\text{Stück}} = \frac{85.000\ \text{€}}{850\ \text{Stck.}} = \mathbf{100\ \text{€/Stck.}}$
* **Produkt B:** $x_{\text{Gut}} = 10.000 \cdot 0,85 = 8.500\ \text{Stck.} \implies k_{\text{Stück}} = \frac{425.000\ \text{€}}{8.500\ \text{Stck.}} = \mathbf{50\ \text{€/Stck.}}$
* **Produkt C:** $x_{\text{Gut}} = 4.000 \cdot 0,80 = 3.200\ \text{Stck.} \implies k_{\text{Stück}} = \frac{340.000\ \text{€}}{3.200\ \text{Stck.}} = \mathbf{106,25\ \text{€/Stck.}}$

### Schritt 4: Erlösrechnung (Umsatz)
Der Umsatz basiert ausschließlich auf den verkauften Gutmengen ($\sum x_{\text{Gut}} \cdot \text{Preis}$):
* $U_{A} = 850 \cdot 400\ \text{€} = 340.000\ \text{€}$
* $U_{B} = 8.500 \cdot 100\ \text{€} = 850.000\ \text{€}$
* $U_{C} = 3.200 \cdot 500\ \text{€} = 1.600.000\ \text{€}$
* $\mathbf{U_{\text{Gesamt}}} = 340.000\ \text{€} + 850.000\ \text{€} + 1.600.000\ \text{€} = \mathbf{2.790.000\ \text{€}}$

---

## 🔍 4. Controlling- & Klausurrelevanz

> [!Concept] **Kalkulatorische Kostenüberwälzung**
> Mathematisch führt ein Ausschuss von $15\%$ dazu, dass die Stückkosten nicht etwa um $15\%$ steigen, sondern durch den verringerten Divisor (Division durch $0,85$) um den Faktor $\frac{1}{1-0,15} \approx 1,1765$ (also um ca. $+17,65\%$). In Preiskalkulationen muss dieser progressive Effekt zwingend vorab einkalkuliert werden, um Margenverluste zu vermeiden.

> [!Alert] **Fehlerquelle Basiswerte**
> Bei der Ermittlung des Umsatzes darf niemals die *Produktionsmenge* herangezogen werden, wenn Ausschuss verzeichnet wurde. Der Umsatz entsteht am Markt ausschließlich durch die Veräußerung fehlerfreier Einheiten (*Gutmenge*). Die Kosten für den produzierten Ausschuss schlagen sich direkt in verminderten Periodenerfolgen nieder, sofern sie nicht über höhere Marktpreise kompensiert werden können.

# 📉 Abschreibungsmethoden: Degressive- & Leistungsabschreibung

Die Abschreibung (Absetzung für Abnutzung, AfA) erfasst den wertmäßigen Verzehr von Anlagegütern über deren betriebsgewöhnliche Nutzungsdauer. Je nach Ursache des Wertverlusts (zeitlich-wirtschaftlich vs. gebrauchsbedingt) kommen unterschiedliche kalkulatorische und bilanzielle Verfahren zur Anwendung.

---

## 1. Geometrisch-degressive Abschreibung

Die geometrisch-degressive Abschreibung ist ein zeitorientiertes Verfahren, bei dem die jährlichen Abschreibungsbeträge progressiv sinken. Ein konstanter Prozentsatz wird dabei stets auf den verbleibenden Restbuchwert des Vorjahres angewendet.

### Mathematische Grundlagen & Formeln

* **Kalkulatorischer Abschreibungssatz ($p$):** Um bei einer festgelegten Nutzungsdauer ($n$) exakt von einem Anfangswert ($AW$) auf einen definierten Restwert ($RW_n$) abzuschreiben, wird der Prozentsatz über die Berechnungsformel der Zinseszinsrechnung (Wurzelmethode) bestimmt:
  $$p = 1 - \sqrt[n]{\frac{RW_n}{AW}}$$

* **Abschreibungsbetrag der Periode $t$ ($A_t$):**
  $$A_t = RBW_{t-1} \cdot p$$
  *(mit $RBW_{t-1} = \text{Restbuchwert am Ende der Vorperiode}$)*

* **Restbuchwert am Ende der Periode $t$ ($RBW_t$):**
  $$RBW_t = AW \cdot (1 - p)^t$$

### Kennzeichen & Verlauf Charakteristika
1. **Unterproportional fallende Beträge:** Der absolute Abschreibungsbetrag sinkt von Jahr zu Jahr, da die Bemessungsgrundlage ($RBW$) schrumpft.
2. **Kein mathematischer Nullwert:** Da immer nur ein Prozentsatz des Restwertes abgezogen wird, kann der Buchwert rein rechnerisch nie $0\ \text{€}$ erreichen. Es muss ein Erinnerungswert (z. B. $1\ \text{€}$) oder ein fixer Endwert vorgegeben werden.

---

## 2. Leistungsabschreibung (nach Nutzung)

Die Leistungsabschreibung ist ein verbrauchsorientiertes Verfahren. Der Wertverzehr wird nicht an die Zeit, sondern an die tatsächliche physische Inanspruchnahme (z. B. Betriebsstunden, Kilometerleistung, Produktionsvolumen) gekoppelt.

### Mathematische Grundlagen & Formeln

* **Abschreibungssatz je Leistungseinheit ($a_v$):**
  $$a_v = \frac{AW - RW_n}{L_{\text{Gesamt}}}$$
  *(mit $L_{\text{Gesamt}} = \text{voraussichtliche Gesamtleistung über die gesamte Nutzungsdauer}$)*

* **Abschreibungsbetrag der Periode $t$ ($A_t$):**
  $$A_t = L_t \cdot a_v$$
  *(mit $L_t = \text{tatsächliche Leistung in der Periode } t$)*

### Kennzeichen & Verlauf Charakteristika
1. **Variable Kostenstruktur:** Die Abschreibung verhält sich vollkommen variabel zur Beschäftigung. In Hochproduktionsphasen steigen die Periodenkosten; bei Stillstand sinken sie auf Null.
2. **Verursachungsgerechte Zuordnung:** Verhindert eine künstliche Fixkostenbelastung in strukturschwachen Perioden.

---

## 3. Vergleichende Synopse (Beispiel: Gabelstapler)

*Anfangswert ($AW$) = 10.000 € | Nutzungsdauer ($n$) = 3 Jahre (Berechnungen auf 4 Nachkommastellen exakt)*

### Szenario A: Degressiv (Endwert = 1 €)
*Berechneter Prozentsatz:* $p = 1 - \sqrt[3]{\frac{1}{10.000}} \approx \mathbf{95,36\% \ (0,9536)}$

| Jahr ($t$) | Restbuchwert (Anfang) | Abschreibungsbetrag ($A_t$) | Restbuchwert (Ende) |
| :--- | :--- | :--- | :--- |
| **1** | 10.000,0000 € | 9.536,0000 € | 464,0000 € |
| **2** | 464,0000 € | 442,4704 € | 21,5296 € |
| **3** | 21,5296 € | 20,5306 € | **0,9990 €** ($\approx 1\ \text{€}$) |

### Szenario B: Leistungsbasiert ($L_{\text{Gesamt}}$ = 13.500 Std., $RW$ = 0 €)
*Kosten pro Betriebsstunde:* $a_v = \frac{10.000\ \text{€}}{13.500\ \text{Std.}} \approx \mathbf{0,7407\ \text{€/Std.}}$

| Jahr ($t$) | Leistung ($L_t$) | Berechnungskette | Abschreibungsbetrag ($A_t$) |
| :--- | :--- | :--- | :--- |
| **1** | 5.000 Std. | $5.000 \cdot 0,7407\ \text{€}$ | 3.703,7037 € |
| **2** | 4.000 Std. | $4.000 \cdot 0,7407\ \text{€}$ | 2.962,8000 € |
| **3** | 4.500 Std. | $4.500 \cdot 0,7407\ \text{€}$ | 3.333,1500 € |
| **Gesamt** | **13.500 Std.** | — | **10.000,0000 €** |

---

## 🔍 4. Controlling- & Klausurrelevanz

> [!Concept] **Wirtschaftliche Begründung der Degression**
> Die degressive Abschreibung spiegelt den tatsächlichen ökonomischen Wertverlauf vieler Wirtschaftsgüter (insb. Kraftfahrzeuge, IT-Hardware) realistischer wider, da der Wertverlust direkt nach der Anschaffung am höchsten ist. Zudem harmonisiert sie den Gesamtperiodenaufwand: In den ersten Jahren stehen hohen Abschreibungen geringe Instandhaltungskosten gegenüber; in den späten Jahren verhält es sich umgekehrt.

> [!Alert] **Rundungsdifferenzen bei Leistungsabschreibung**
> Wird der Abschreibungssatz je Leistungseinheit als gerundeter Dezimalbruch ($0,7407\ \text{€}$) statt als exakter Bruch ($\frac{20}{27}\ \text{€}$) fortgeführt, entstehen am Ende der Laufzeit mathematische Rundungsdifferenzen (hier: $3.703,7037 + 2.962,8000 + 3.333,1500 = 9.999,6537\ \text{€}$). In Klausuren ist strikt auf die Vorgabe der Nachkommastellen im Aufgabentext zu achten, um Folgefehler bei der Bestimmung von Restbuchwerten zu vermeiden.

# 🧮 Mathematisches Gleichungsverfahren (Simultanverfahren)

Das mathematische Gleichungsverfahren ist das exakteste Verfahren der **innerbetrieblichen Leistungsverrechnung (IBLV)** in der Kostenstellenrechnung. Im Gegensatz zu einstufigen Verfahren (Anbauverfahren) oder einfachen sequenziellen Verfahren (Stufenleiterverfahren) erfasst es alle gegenseitigen und zweiseitigen Leistungsverflechtungen zwischen den Hilfskostenstellen (Vorkostenstellen) mathematisch exakt über ein lineares Gleichungssystem (LGS).

---

## 1. Verrechnungsprinzip und Prämisse

* **Vollständige mathematische Exaktheit:** Das Verfahren berücksichtigt, dass Vorkostenstellen sich gegenseitig (bzw. auch sich selbst) Leistungen erbringen (sogenannte mathematische Verflechtungen oder Eigenverbrauch).
* **Gleichgewichtsprämisse:** Für jede Vorkostenstelle gilt der Grundsatz, dass die Summe ihrer Gesamtkosten (primäre Gemeinkosten + Wert der von anderen Kostenstellen empfangenen Leistungen) exakt dem kalkulatorischen Wert ihrer gesamten Leistungsabgabe entsprechen muss.
* **Zielgröße:** Bestimmung von mathematisch exakten, internen Verrechnungspreisen ($q_i$) pro Leistungseinheit (LE).

---

## 2. Mathematischer Ansatz & Systemaufstellung

Für jede Vorkostenstelle $i$ wird eine Zeilengleichung nach folgendem Muster aufgestellt:

$$\text{Gesamtleistung}_i \cdot q_i = K_{\text{prim}, i} + \sum_{k} (\text{Empfangene Leistung}_{i \leftarrow k} \cdot q_k)$$

### Allgemeine Systemmatrix (für $m$ Vorkostenstellen)
Überführt man alle Variablen auf die linke Seite, entsteht ein lineares Gleichungssystem in Standardform:

$$(X_{\text{Gesamt}, i} - x_{ii}) \cdot q_i - \sum_{k \neq i} x_{ik} \cdot q_k = K_{\text{prim}, i}$$

*Bedeutung der Variablen:*
* $q_i, q_k$: Gesuchte Verrechnungspreise der Vorkostenstellen $i$ und $k$ [€/LE]
* $K_{\text{prim}, i}$: Primäre Gemeinkosten der Vorkostenstelle $i$ [€]
* $X_{\text{Gesamt}, i}$: Gesamte abgegebene Leistung der Vorkostenstelle $i$ [LE]
* $x_{ii}$: Eigenverbrauch der Vorkostenstelle $i$ [LE]
* $x_{ik}$: Leistungsübertragung von Stelle $k$ an Stelle $i$ [LE]

---

## 3. Konkretes Berechnungsbeispiel (BAB-Analyse)

### 1. Ausgangsdaten & Primärkostenbelastung
* **Vorkostenstelle V1:** $K_{\text{prim}} = 8.560\ \text{€}$ | Gesamtleistung = $600\ \text{LE}$
  *(Verbraucher: V1 = 20 LE | V2 = 30 LE | E1 = 280 LE | E2 = 170 LE | E3 = 100 LE)*
* **Vorkostenstelle V2:** $K_{\text{prim}} = 6.480\ \text{€}$ | Gesamtleistung = $6.000\ \text{LE}$
  *(Verbraucher: V1 = 600 LE | V2 = 200 LE | E1 = 2.000 LE | E2 = 1.900 LE | E3 = 1.300 LE)*

### 2. Aufstellen des Gleichungssystems
1. **Gleichung V1:** $600 \cdot q_1 = 8.560 + 20 \cdot q_1 + 600 \cdot q_2$
2. **Gleichung V2:** $6.000 \cdot q_2 = 6.480 + 30 \cdot q_1 + 200 \cdot q_2$

### 3. Überführung in die Standardform
1. $$580 \cdot q_1 - 600 \cdot q_2 = 8.560$$
2. $$-30 \cdot q_1 + 5.800 \cdot q_2 = 6.480$$

### 4. Mathematische Auflösung (Einsetzungsverfahren)
Auflösung von Gleichung (2) nach $q_1$:
$$30 \cdot q_1 = 5.800 \cdot q_2 - 6.480 \implies q_1 = \frac{580}{3} \cdot q_2 - 216$$

Einsetzen in Gleichung (1):
$$580 \cdot \left(\frac{580}{3} \cdot q_2 - 216\right) - 600 \cdot q_2 = 8.560$$
$$\frac{334.600}{3} \cdot q_2 = 133.840 \implies \mathbf{q_2 = 1,20\ \text{€/LE}}$$

Rückrechnung für $q_1$:
$$q_1 = \frac{580}{3} \cdot 1,20 - 216 \implies \mathbf{q_1 = 16,00\ \text{€/LE}}$$

### 5. Sekundärkostenumlage auf Hauptkostenstellen (Endkostenstellen)
Die Belastung der Endkostenstellen ($E_j$) erfolgt exakt nach der beanspruchten Nettoleistung:

* **Endkostenstelle E1:** $(280 \cdot 16\ \text{€}) + (2.000 \cdot 1,20\ \text{€}) = 4.480\ \text{€} + 2.400\ \text{€} = \mathbf{6.880\ \text{€}}$
* **Endkostenstelle E2:** $(170 \cdot 16\ \text{€}) + (1.900 \cdot 1,20\ \text{€}) = 2.720\ \text{€} + 2.280\ \text{€} = \mathbf{5.000\ \text{€}}$
* **Endkostenstelle E3:** $(100 \cdot 16\ \text{€}) + (1.300 \cdot 1,20\ \text{€}) = 1.600\ \text{€} + 1.560\ \text{€} = \mathbf{3.160\ \text{€}}$

$$\text{Gesamtsumme der Sekundärkosten} = 6.880\ \text{€} + 5.000\ \text{€} + 3.160\ \text{€} = \mathbf{15.040\ \text{€}}$$

---

## 🔍 4. Controlling- & Klausurrelevanz

> [!Concept] **Vorteile gegenüber Approximationsverfahren**
> Das Gleichungsverfahren liefert als einziges IBLV-Verfahren ökonomisch fehlerfreie Verrechnungssätze, da es unabhängig von der Anordnung der Kostenstellen im BAB arbeitet. Es verhindert zirkuläre Rechenschleifen und liefert die exakte informationelle Grundlage für die Kostenträgerstückrechnung (Kalkulation) sowie für Make-or-Buy-Entscheidungen im operativen Controlling.

> [!Alert] **Der absolute Klausur-Kontrollschritt**
> Da nach der vollständigen Umlage der mathematischen Verrechnungssätze die Vorkostenstellen exakt auf Saldo Null aufgehen müssen, gilt für das Gesamtsystem eine strikte Erhaltungskette:
> $$\sum K_{\text{sek, Endkostenstellen}} \equiv \sum K_{\text{prim, Vorkostenstellen}}$$
> In Klausuren lässt sich die Korrektheit der ermittelten Preise sofort validieren, indem die Summe der primären Kosten der Vorkostenstellen ($8.560\ \text{€} + 6.480\ \text{€} = 15.040\ \text{€}$) mit der summierten Sekundärkostenbelastung der Endkostenstellen verglichen wird. Weichen diese Werte ab, liegt ein Rechen- oder Rundungsfehler beim Auflösen des LGS vor.

# 📦 Äquivalenzzahlenkalkulation (Sortenkalkulation)

Die Äquivalenzzahlenkalkulation ist eine Verfeinerung der Divisionskalkulation. Sie wird in Unternehmen mit **Sortenfertigung** angewendet, bei denen verwandte Produkte (Sorten) aus ähnlichen Rohstoffen und mittels gleichartiger Fertigungsverfahren hergestellt werden. Die Sorten weisen feste Kostenproportionen zueinander auf (z. B. bedingt durch unterschiedliche Gewichte, Maße, Dicken oder Bearbeitungszeiten).

---

## 1. Kalkulationsprinzip und Prämisse

* **Homogenisierung über Kennzahlen:** Da die Produkte nicht völlig identisch sind, können die Gesamtkosten nicht einfach durch die absolute Stückzahl dividiert werden. Stattdessen werden die Mengen mithilfe von Verhältniszahlen (Äquivalenzziffern) auf eine fiktive Standard-Sorte (die Basissorte mit der Äquivalenzziffer 1,00) normiert.
* **Proportionalitätsprämisse:** Das Verfahren setzt voraus, dass sich die Kosten der verschiedenen Sorten proportional zu den gewählten technischen Merkmalen (z. B. Abmessung, Gewicht, Produktionsdauer) verhalten.

---

## 2. Ablaufstufen und mathematische Logik

### Schritt 1: Festlegung der Basiswerte und Normierung
Ein technisches Merkmal (oder ein Produkt aus mehreren Merkmalen) dient als Basis. Die Sorte mit dem kleinsten Basiswert erhält üblicherweise die Äquivalenzziffer ä = 1.
* Formel Äquivalenzziffer (ä_i) für Sorte i: 
  ä_i = Basiswert_i / Basiswert_Standard

### Schritt 2: Ermittlung der fiktiven Recheneinheiten (Basiseinheiten)
Die realen Produktionsmengen (Stückzahlen m_i) werden mit den jeweiligen Äquivalenzziffern gewichtet:
* Basiseinheiten_i = m_i * ä_i
* Gesamte Basiseinheiten (Summe RE) = Summe über alle i (m_i * ä_i)

### Schritt 3: Berechnung der Kosten pro Basiseinheit (k_base)
Die Gesamtkosten der Periode (K_gesamt) werden durch die Summe aller Basiseinheiten geteilt:
* k_base = K_gesamt / (Summe RE)

### Schritt 4: Rückrechnung auf die realen Stückkosten (k_i)
Die Stückkosten einer spezifischen Sorte ergeben sich durch Multiplikation des Basissatzes mit der jeweiligen Äquivalenzziffer:
* k_i = k_base * ä_i

---

## 3. Exemplarisches Kalkulationsbeispiel (Abrechnung)

*Ausgangsdaten:*
* **Gesamtkosten der Periode:** 421.504 €
* **Sorte 1:** 100g, 50cm  | Menge = 10.000 Stck
* **Sorte 2:** 120g, 100cm | Menge = 2.000 Stck
* **Sorte 3:** 120g, 120cm | Menge = 200 Stck
* **Sorte 4:** 150g, 100cm | Menge = 30.000 Stck

### Schritt 1 & 2: Bestimmung der Äquivalenzziffern (ä) und Basiseinheiten (RE)
Die Verrechnungsbasis basiert auf dem Produkt aus Gewicht * Höhe. Der kleinste Wert (Sorte 1: 5.000) wird auf 1,00 normiert.

| Sorte | Merkmal (Gew. * Höhe) | Äquivalenzziffer (ä) | Reale Menge (Stck) | Basiseinheiten (RE) |
| :---: | :------------------: | :------------------: | :----------------: | :-----------------: |
| **1** | 5.000 (Minimum)      | 5.000 / 5.000 = 1,00 | 10.000             | 10.000              |
| **2** | 12.000               | 12.000 / 5.000 = 2,40| 2.000              | 4.800               |
| **3** | 14.400               | 14.400 / 5.000 = 2,88| 200                | 576                 |
| **4** | 15.000               | 15.000 / 5.000 = 3,00| 30.000             | 90.000              |
| **Summe**| —                 | —                    | **42.200** | **105.376** |

### Schritt 3: Kosten pro Basiseinheit
* k_base = 421.504 € / 105.376 RE = **4,00 € pro Basiseinheit**

### Schritt 4: Stückkostenkalkulation & Ergebnisrechnung
* **Stückkosten Sorte 1:** 1,00 * 4,00 € = **4,00 €/Stck**
* **Stückkosten Sorte 2:** 2,40 * 4,00 € = **9,60 €/Stck**
* **Stückkosten Sorte 3:** 2,88 * 4,00 € = **11,52 €/Stck**
* **Stückkosten Sorte 4:** 3,00 * 4,00 € = **12,00 €/Stck**

---

## 🔍 4. Controlling- & Klausurrelevanz

> [!Concept] **Vor- und Nachteile (Kritische Würdigung)**
> * **Vorteile:** Deutlich geringerer Erfassungs- und Verrechnungsaufwand als bei einer differenzierten Zuschlagskalkulation; ideal für standardisierte Variantenfertigung; sehr einfache Handhabung im operativen Controlling nach einmaliger Festlegung der Ziffern.
> * **Nachteile:** Starrheit des Systems. Ändern sich die technologischen Produktionsbedingungen einer einzelnen Sorte (z. B. durch eine neue Maschine, die nur Sorte 4 schneller fertigt), verschieben sich die realen Kostenproportionen. Die Äquivalenzziffern bilden die Realität dann nicht mehr exakt ab und müssen aufwendig neu bestimmt werden (Gefahr von Fehlkalkulationen).

> [!Alert] **Typische Klausurfalle bei mehrdimensionalen Merkmalen**
> Werden in der Aufgabenstellung zwei Dimensionen (z. B. Gewicht und Höhe) genannt, darf die Äquivalenzziffer nicht separat für nur eine Dimension berechnet werden. Das mathematische Produkt beider Eigenschaften bildet das korrekte, kombinierte Gewichtungsverhältnis. Ein weiterer beliebter Fehler ist das Verwechseln der realen Stückzahlen mit den umgerechneten Basiseinheiten beim Ermitteln des Kostensatzes im Nenner.

# 📊 Deckungsbeitragsrechnung & Break-Even-Analyse

Die Deckungsbeitragsrechnung ist ein zentrales Instrument der **Teilkostenrechnung** (Direct Costing). Im Gegensatz zur Vollkostenrechnung verzichtet sie auf die willkürliche Schlüsselung von Fixkosten auf die Kostenträger. Sie trennt die Kosten strikt in variable (beschäftigungsabhängige) und fixe (beschäftigungsunabhängige) Bestandteile, um die kurzfristige operative Entscheidungsfindung im Controlling zu unterstützen.

---

## 1. Kalkulationsprinzip und mathematische Grundlagen

* **Stückdeckungsbeitrag ($db$):** Gibt an, wie viel der Erlös eines einzelnen verkauften Produkts zur Deckung der Fixkosten beiträgt. Ist das $db$ positiv, erhöht jedes verkaufte Stück das Betriebsergebnis.
  $$db = p - k_v$$
  * $p$: Preis pro Stück (Nettoerlös)
  * $k_v$: Variable Stückkosten ($K_v / x$)

* **Gesamtdeckungsbeitrag ($DB$):** Die Summe aller generierten Deckungsbeiträge einer Periode.
  $$DB = x \cdot db = E - K_v$$
  * $x$: Absatzmenge (Stückzahl)
  * $E$: Gesamterlös (Umsatz)
  * $K_v$: Gesamte variable Kosten

* **Betriebsergebnis / Gewinn ($G$):** Der verbleibende Erfolg nach Abzug der Fixkosten vom Gesamtdeckungsbeitrag.
  $$G = DB - K_f = (x \cdot db) - K_f$$
  * $K_f$: Gesamte Fixkosten der Periode

---

## 2. Die Gewinnschwelle (Break-Even-Analyse)

Der **Break-Even-Punkt (BEP)** kennzeichnet die Absatzmenge, bei der die Gesamterlöse exakt den Gesamtkosten entsprechen. Das Betriebsergebnis ist an dieser Stelle genau Null ($G = 0$).

$$\text{Bedingung:} \quad x_{\text{BEP}} \cdot db = K_f \implies x_{\text{BEP}} = \frac{K_f}{db}$$

### Erweiterung: Zielgewinn-Formel
Soll ein vordefinierter Zielgewinn ($G_{\text{Ziel}}$) erwirtschaftet werden, erweitert sich die Formel um den Gewinnanspruch im Zähler:

$$x_{\text{Ziel}} = \frac{K_f + G_{\text{Ziel}}}{db}$$

---

## 3. Konkretes Fallbeispiel (Preiselastizität & Mengeneffekt)

### Szenario-Vergleich: Plan A (Standard) vs. Plan B (Preisaggressiv)
* **Konstante Systemgrößen:** $K_f = 4.000\ \text{€}$ | Variable Stückkosten $k_v = \frac{8.000\ \text{€}}{1.000\ \text{Stck}} = 8,00\ \text{€/Stck}$

| Kennzahl | Plan A (Ausgangsszenario) | Plan B (Preisstrategie) |
| :--- | :--- | :--- |
| **Verkaufspreis ($p$)** | $16,00\ \text{€/Stck}$ | $10,00\ \text{€/Stck}$ |
| **Variable Stückkosten ($k_v$)** | $8,00\ \text{€/Stck}$ | $8,00\ \text{€/Stck}$ |
| **Stückdeckungsbeitrag ($db$)** | $16 - 8 = \mathbf{8,00\ \text{€/Stck}}$ | $10 - 8 = \mathbf{2,00\ \text{€/Stck}}$ |
| **Break-Even-Menge ($x_{\text{BEP}}$)**| $\frac{4.000\ \text{€}}{8\ \text{€}} = \mathbf{500\ \text{Stck}}$ | $\frac{4.000\ \text{€}}{2\ \text{€}} = \mathbf{2.000\ \text{Stck}}$ |
| **Geplante Absatzmenge ($x$)** | $1.000\ \text{Stck}$ | **$4.000\ \text{Stck}$** *(Errechnet für $G_{\text{Ziel}}$)* |
| **Gesamtdeckungsbeitrag ($DB$)** | $1.000 \cdot 8\ \text{€} = 8.000\ \text{€}$ | $4.000 \cdot 2\ \text{€} = 8.000\ \text{€}$ |
| **Fixkosten ($K_f$)** | $4.000\ \text{€}$ | $4.000\ \text{€}$ |
| **Betriebsergebnis ($G$)** | $8.000 - 4.000 = \mathbf{4.000\ \text{€}}$ | $8.000 - 4.000 = \mathbf{4.000\ \text{€}}$ |

---

## 🔍 4. Controlling- & Klausurrelevanz

> [!Concept] **Der Hebeleffekt von Preisänderungen (Operating Leverage)**
> Das Fallbeispiel demonstriert den asymmetrischen Zusammenhang zwischen Preis und erforderlicher Absatzmenge. Eine Preissenkung um **37,5 %** (von 16 € auf 10 €) führt zu einer Reduktion des Stückdeckungsbeitrags um **75 %** (von 8 € auf 2 €). Um denselben Absolutgewinn zu halten, muss die Absatzmenge folglich um **300 %** (Vervierfachung von 1.000 auf 4.000 Stück) gesteigert werden.

> [!Alert] **Typische Klausurfehler**
> * **Fixkosten-Proportionalisierung:** Ein häufiger Fehler ist das Herunterrechnen der Fixkosten auf die Stückeebene ($\frac{4.000\ \text{€}}{1.000\ \text{Stck}} = 4\ \text{€}$) und das Beibehalten dieses Satzes bei Mengenänderungen. Fixkosten bleiben per Definition innerhalb der relevanten Kapazitätsgrenze absolut konstant.
> * **Umsatzerlös vs. Deckungsbeitrag:** Bei der Ermittlung der Zielabsatzmenge für einen bestimmten Gewinn wird im Nenner oft fälschlicherweise der Preis ($p$) statt des Stückdeckungsbeitrags ($db$) angesetzt. Das vernachlässigt die variablen Kostenverzehre pro zusätzlichem Stück.

# 📊 Elektive Zuschlagskalkulation & Preisuntergrenzen

Die differenzierende Zuschlagskalkulation ist ein Verfahren der **Vollkostenrechnung**. Sie trennt die Kosten in Einzelkosten (direkt zurechenbar) und Gemeinkosten (indirekt über Schlüsselungen im Betriebsabrechnungsbogen [BAB] verteilbar). Der Übergang zur Teilkostenrechnung isoliert die variablen Komponenten zur Ermittlung von kurzfristigen Preisuntergrenzen.

---

## 1. Kalkulationsschema (Vollkostenbasis)

Das klassische mehrstufige Kalkulationsschema baut progressiv aufeinander auf:

$$\begin{aligned}
&\quad \text{Fertigungsmaterial (Materialeinzelkosten = MEK)} \\
+\,&\quad \text{Materialgemeinkosten (MGK)} \\
\hline
=\,&\quad \text{Materialkosten} \\
\\
&\quad \text{Fertigungslöhne (Fertigungseinzelkosten = FEK)} \\
+\,&\quad \text{Fertigungsgemeinkosten (FGK)} \\
\hline
=\,&\quad \text{Fertigungskosten} \\
\\
\hline
=\,&\quad \mathbf{\text{Herstellkosten (HK)}} \quad [= \text{Materialkosten} + \text{Fertigungskosten}] \\
+\,&\quad \text{Verwaltungs- und Vertriebsgemeinkosten (VwVtGK)} \\
\hline
=\,&\quad \mathbf{\text{Selbstkosten (SK)}}
\end{aligned}$$

---

## 2. Mathematische Ermittlung der Zuschlagssätze

Die Gemeinkostenzuschlagssätze ($ZS$) beziehen sich jeweils auf ihre spezifische Einzelkostenbasis bzw. Bezugsgröße der Abrechnungsperiode:

* **Materialzuschlagssatz ($MGK\_ZS$):**
  $$MGK\_ZS = \frac{\text{Gesamt-MGK}}{\text{Gesamt-MEK}} \cdot 100\%$$

* **Fertigungszuschlagssatz ($FGK\_ZS$):**
  $$FGK\_ZS = \frac{\text{Gesamt-FGK}}{\text{Gesamt-FEK}} \cdot 100\%$$

* **Verwaltungs- und Vertriebszuschlagssatz ($VwVtGK\_ZS$):**
  Bezieht sich als einzige Stufe **nicht** auf Einzelkosten, sondern auf die kumulierten Herstellkosten der Periode.
  $$VwVtGK\_ZS = \frac{\text{Gesamt-VwVtGK}}{\text{Gesamt-HK}} \cdot 100\%$$

---

## 3. Exemplarisches Kalkulationsbeispiel (Produkt Alpha)

### Stufe 1: Ermittlung der Perioden-Zuschlagssätze
* *Basisdaten Periode:* MEK = 100k €, FEK = 300k €, MGK = 30k €, FGK = 420k €, VwVtGK = 170k €
* $MGK\_ZS = \frac{30.000}{100.000} \cdot 100\% = \mathbf{30\%}$
* $FGK\_ZS = \frac{420.000}{300.000} \cdot 100\% = \mathbf{140\%}$
* $HK_{\text{Periode}} = 100.000 + 30.000 + 300.000 + 420.000 = 850.000\ \text{€}$
* $VwVtGK\_ZS = \frac{170.000}{850.000} \cdot 100\% = \mathbf{20\%}$

### Stufe 2: Kostenträgerrechnung (Objektkalkulation Alpha)
* *Objektdaten Alpha:* MEK = 1.500 €, FEK = 1.800 €

| Kalkulationsstufe | Berechnungsgrundlage | Wert in € |
| :--- | :--- | :--- |
| Fertigungsmaterial (MEK) | *Gegeben* | 1.500,00 |
| + Materialgemeinkosten (MGK) | $1.500 \cdot 30\%$ | 450,00 |
| **= Materialkosten** | | **1.950,00** |
| Fertigungslöhne (FEK) | *Gegeben* | 1.800,00 |
| + Fertigungsgemeinkosten (FGK) | $1.800 \cdot 140\%$ | 2.520,00 |
| **= Fertigungskosten** | | **4.320,00** |
| **= Herstellkosten (HK)** | $1.950 + 4.320$ | **6.270,00** |
| + Verw.-/Vertriebsgemeinkosten | $6.270 \cdot 20\%$ | 1.254,00 |
| **= Selbstkosten (SK)** | $6.270 + 1.254$ | **7.524,00** |

---

## 4. Teilsystem: Preisuntergrenzen (PUG)

Unter der Prämisse, dass **sämtliche Gemeinkosten fixer Natur** und die **Einzelkosten variabel** sind ($k_v = \text{MEK} + \text{FEK}$), gelten für ein geplantes Marktpreis-Szenario von $p = 8.000\ \text{€}$ folgende pricing-relevante Metriken:

* **Variable Stückkosten ($k_v$):**
  $$k_v = 1.500\ \text{€} + 1.800\ \text{€} = 3.300\ \text{€}$$
* **Stückdeckungsbeitrag ($db$):**
  $$db = p - k_v = 8.000\ \text{€} - 3.300\ \text{€} = 4.700\ \text{€}$$
* **Stückerfolg (langfristiges Betriebsergebnis pro Stück):**
  $$\text{Erfolg} = p - \text{SK} = 8.000\ \text{€} - 7.524\ \text{€} = \mathbf{476\ \text{€}}$$

---

## 🔍 5. Controlling- & Klausurrelevanz

> [!Concept] **Dichotomie der Preisuntergrenzen**
> * **Absolute (kurzfristige) Preisuntergrenzen ($PUG_{\text{abs}}$):** Entspricht exakt den variablen Stückkosten ($PUG_{\text{abs}} = k_v = 3.300\ \text{€}$). Ein Preis unterhalb dieser Grenze führt zu einem unmittelbaren Liquiditätsabfluss pro verkaufter Einheit, da nicht einmal die direkt verursachten Einzelkosten (Material/Lohn) gedeckt werden. Kurzfristig tolerierbar nur bei extremen Marktbarrieren oder strategischem Markteintritt.
> * **Langfristige Preisuntergrenze ($PUG_{\text{lang}}$):** Entspricht den vollen Selbstkosten ($PUG_{\text{lang}} = \text{SK} = 7.524\ \text{€}$). Langfristig müssen alle fixen Gemeinkostenkomponenten amortisiert werden, um die Unternehmenssubstanz zu erhalten.

> [!Alert] **Klausurfalle: Die Verrechnungsbasis im Nenner**
> Der mathematische Fehler mit der höchsten Frequenz in Prüfungen liegt in der Ermittlung des $VwVtGK\_ZS$. Studenten setzen im Nenner häufig fälschlicherweise die Summe aus MEK + FEK an (die primären Einzelkosten) statt der korrekten **Herstellkosten** (welche bereits die Material- und Fertigungsgemeinkosten beinhalten). Dies führt zu einer massiven Überhöhung des berechneten Zuschlagssatzes.