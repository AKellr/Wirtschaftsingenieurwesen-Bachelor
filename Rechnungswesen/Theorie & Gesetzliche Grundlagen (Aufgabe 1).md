### 1. Kaskade der Buchführungspflicht
Die Buchführungspflicht wird durch das Zusammenspiel von Handelsrecht (HGB) und Steuerrecht (AO) geregelt.

```text
              [ START: Prüfe HGB ]
                       │
         ┌─────────────┴─────────────┐
         ▼                           ▼
  Formkaufmann (§ 6)          Istkaufmann (§ 1)
 (GmbH, AG, OHG, KG)        (Kaufmännische Struktur)
         │                           │
         └─────────────┬─────────────┘
                       ▼
          Ja ──> § 238 HGB Pflicht
                       │
                       ▼
             § 140 AO (Derivativ)
         (Buchführungspflicht im Steuerrecht)
                       │
         Nein ─────────┘
         ▼
   [ Prüfe AO ]
         │
         ▼
§ 141 AO (Originär)
(Grenzwerte überschritten?)
┌───────────┴───────────┐
▼                       ▼
Umsatz > 800.000 €      Gewinn > 80.000 €
(Wachstumschancengesetz ab 2024/2026)
│                       │
└───────────┬───────────┘
            ▼
  Ja ──> Steuerlich pflichtig
```

> [!INFO] **HGB-Vorschriften**
> * **Istkaufmann (§ 1 HGB):** Kaufmann kraft Gewerbebetriebs, sofern dieser nach Art und Umfang einen in kaufmännischer Weise eingerichteten Geschäftsbetrieb erfordert. Die Eintragung ins Handelsregister ist **deklaratorisch** (rechtsbezeugend).
> * **Formkaufmann (§ 6 HGB):** Kaufmann kraft Rechtsform (z. B. GmbH, AG). Unabhängig von Größe oder Umsatz immer buchführungspflichtig nach § 238 HGB. Die Eintragung ins Handelsregister ist **konstitutiv** (rechtserzeugend).

> [!INFO] **AO-Vorschriften (Steuerrecht)**
> * **Derivative Pflicht (§ 140 AO):** Wer nach Handelsrecht Bücher führen muss, ist automatisch auch steuerlich dazu verpflichtet (Ableitung HGB ➔ AO).
> * **Originäre Pflicht (§ 141 AO):** Für Gewerbetreibende und Landwirte, die *nicht* bereits nach § 140 AO verpflichtet sind.
>   * **Grenzwerte (Wachstumschancengesetz ab 2024/2026):**
>     * Umsatz **> 800.000 €** im Kalenderjahr **oder**
>     * Gewinn **> 80.000 €** im Wirtschaftsjahr.

> [!WARNING] **Wichtige Ausnahmen**
> * **Freiberufler (§ 18 EStG):** Unabhängig von Umsatz- oder Gewinnhöhe **nie** buchführungspflichtig nach § 141 AO! Sie dürfen stets die Einnahmenüberschussrechnung (EÜR) nach § 4 Abs. 3 EStG anwenden.
> * **Land- und Forstwirte:** Unterliegen der originären Pflicht nach § 141 AO nur bei Überschreiten der Grenzwerte (oder bei einem Wirtschaftswert der selbstbewirtschafteten Flächen **> 25.000 €**).

---

### 2. Definition des Gewerbebetriebs (§ 15 Abs. 2 EStG)
Eine Tätigkeit gilt als Gewerbebetrieb, wenn alle **4 positiven Merkmale** kumulativ vorliegen und die **3 negativen Merkmale** ausgeschlossen werden können.

| Positive Merkmale (MÜSSEN vorliegen) | Beschreibung |
| :--- | :--- |
| **1. Selbstständigkeit** | Handeln auf eigene Rechnung und eigene Verantwortung (keine Weisungsgebundenheit). |
| **2. Nachhaltigkeit** | Auf Wiederholung und Dauer angelegte Tätigkeit (keine Einmalaktion). |
| **3. Gewinnerzielungsabsicht** | Streben nach einem Totalüberschuss über die gesamte Lebensdauer des Betriebs. |
| **4. Beteiligung am Markt** | Offenes, nach außen gerichtetes Anbieten von Gütern/Dienstleistungen gegen Entgelt. |

| Negative Merkmale (DÜRFEN NICHT vorliegen) | Rechtsfolge bei Vorliegen |
| :--- | :--- |
| **1. Keine Land- und Forstwirtschaft** | Einkünfte nach § 13 EStG |
| **2. Keine selbstständige Arbeit** | Freie Berufe/Künstler nach § 18 EStG (keine Gewerbesteuer!) |
| **3. Keine private Vermögensverwaltung** | Reine Nutzung des Vermögens (z. B. private Wertpapieranlagen). |

---

## 🪵 Teil 2: Klausurrelevante Buchungssätze (Fälle 6.1 – 6.8)

### 📌 Fall 6.1: Anschaffung Anlagevermögen auf Ziel & spätere Zahlung
Kauf einer Maschine für **10.000 €** netto auf Ziel. Spätere Begleichung per Banküberweisung.

* **1. Einbuchung des Kaufs (Anschaffung):**
```text
0400 Maschinen                     10.000,00 €
2600 Vorsteuer                      1.900,00 €
  an 4400 Verbindlichkeiten a.L.u.L.           11.900,00 €
```

* **2. Bezahlung der Rechnung per Bank:**
```text
4400 Verbindlichkeiten a.L.u.L.    11.900,00 €
  an 2800 Bank                                 11.900,00 €
```

---

### 📌 Fall 6.2: Sofortabschreibung GWG bei Barzahlung
Kauf eines Smartphones für **450 €** netto (**535,50 €** brutto) gegen Barzahlung. Direkte Sofortabschreibung unter Berücksichtigung der GWG-Grenzwerte.

* **Sofortabschreibung im Anschaffungsjahr:**
```text
6820 Sofortabschreibung GWG         450,00 €
2600 Vorsteuer                       85,50 €
  an 2880 Kasse                                  535,50 €
```

---

### 📌 Fall 6.3: Bildung von Steuerrückstellungen am Jahresende
Zum Jahresabschluss werden Steuerrückstellungen gebildet (Körperschaftsteuer **15.000 €** und Gewerbesteuer **12.000 €**).

* **Bildung der Rückstellungen (Aufwand an Rückstellung):**
```text
7610 Körperschaftsteueraufwand     15.000,00 €
7600 Gewerbesteueraufwand          12.000,00 €
  an 3000 Steuerrückstellungen                 27.000,00 €
```

---

### 📌 Fall 6.4: Endgültiger Forderungsausfall wegen Insolvenz
Eine Forderung von **23.800 €** brutto (inkl. 19 % USt) fällt wegen Insolvenz des Kunden vollständig aus.

* **Berechnung:**
  * Bruttoforderung: **23.800,00 €**
  * Netto-Ausfall: **20.000,00 €** (Berechnung: 23.800,00 € / 1,19)
  * Umsatzsteuer-Korrektur: **3.800,00 €** (Berechnung: 23.800,00 € - 20.000,00 €)

* **Buchungssatz:**
```text
6950 Abschreibungen auf Forderungen 20.000,00 €
4800 Umsatzsteuer                    3.800,00 €
  an 2400 Forderungen a.L.u.L.                 23.800,00 €
```

---

### 📌 Fall 6.5: Erlösminderung / Gutschrift an Kunden
Einem Kunden wird nachträglich eine Netto-Gutschrift von **20.000 €** (**23.800 €** brutto) erteilt (z. B. wegen Mängeln).

* **Buchungssatz (Erlösberichtigung & USt-Korrektur):**
```text
5001 Erlösberichtigungen            20.000,00 €
4800 Umsatzsteuer                    3.800,00 €
  an 2400 Forderungen a.L.u.L.                 23.800,00 €
```

---

### 📌 Fall 6.6 & 6.7: Rohstoffeinkauf mit fehlerhafter Rechnung & spätere Korrektur

* **Ausgangslage (Fall 6.6):** Rohstoffeinkauf für **41.650,00 €** brutto auf Ziel. Die Rechnung enthält keine Rechnungsnummer. Die Vorsteuer darf wegen fehlender Pflichtangaben vorerst nicht abgezogen werden. Der Einkauf wird erfolgsneutral verbucht (Bruttomethode).
```text
2000 Rohstoffe                      41.650,00 €
  an 4400 Verbindlichkeiten a.L.u.L.           41.650,00 €
```

* **Korrektur (Fall 6.7):** Zwei Monate später liefert der Lieferant eine korrigierte Rechnung. Die Vorsteuer darf nachträglich gezogen werden.
  * *Berechnung Steueranteil:* 41.650,00 € / 1,19 = **35.000,00 €** netto. Vorsteuer = **6.650,00 €**.
```text
2600 Vorsteuer                       6.650,00 €
  an 2000 Rohstoffe                             6.650,00 €
```

---

### 📌 Fall 6.8: Verkauf auf Ziel & Bestandsveränderung (Doppelbuchung)

* **Teil 1: Verkauf von Erzeugnissen auf Ziel**
  Eigene Erzeugnisse im Wert von **238.000 €** brutto (inkl. 19 % USt) werden auf Ziel verkauft.
  * *Berechnung:* Netto-Erlös = **200.000,00 €**; Umsatzsteuer = **38.000,00 €**.
```text
2400 Forderungen a.L.u.L.          238.000,00 €
  an 5000 Umsatzerlöse                         200.000,00 €
  an 4800 Umsatzsteuer                          38.000,00 €
```

* **Teil 2: Bestandsminderung fertige Erzeugnisse**e
  Durch den Verkauf reduziert sich der Bestand fertiger Erzeugnisse im Lager um **85.000 €** (Herstellungskosten).
  * *Merkhilfe:* Eine Minderung des Lagers (Aktivkonto 2200 nimmt ab ➔ Haben) stellt eine Bestandsminderung dar. Dies mindert den Periodenerfolg und wird über das Ertragskonto "Bestandsveränderungen" im Soll erfasst.
```text
5200 Bestandsveränderungen          85.000,00 €
  an 2200 Fertige Erzeugnisse                  85.000,00 €
```

> [!TIP] **Erfolgsrelevanz bei Bestandsveränderungen**
> * **Lageraufbau (Bestandsmehrung):** `2200 Fertige Erzeugnisse` an `5200 Bestandsveränderungen` ➔ Ertrag erhöht sich ➔ Gewinn steigt 📈.
> * **Lagerabbau (Bestandsminderung):** `5200 Bestandsveränderungen` an `2200 Fertige Erzeugnisse` ➔ Ertrag verringert sich ➔ Gewinn sinkt 📉.