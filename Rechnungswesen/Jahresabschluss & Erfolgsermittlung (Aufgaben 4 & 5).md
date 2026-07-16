## 🧮 1. Der steuerliche Betriebsvermögensvergleich (§ 4 Abs. 1 EStG)

Der Betriebsvermögensvergleich ermittelt den steuerlichen Gewinn/Verlust einer Periode rein über die Bestandsgrößen (Eigenkapital) der Bilanz. Er neutralisiert alle nicht-betrieblichen (privaten) Vermögensverschiebungen.

### 📌 Die mathematische Definition

$$\text{Gewinn/Verlust} = EK_{t} - EK_{t-1} + \text{Privatentnahmen} - \text{Privateinlagen}$$

*Wobei:*
* **$EK_{t}$**: Eigenkapital am Ende des aktuellen Wirtschaftsjahres (31.12.)
* **$EK_{t-1}$**: Eigenkapital am Ende des vorherigen Wirtschaftsjahres (01.01.)
* **Privatentnahmen ($PE$):** Alle Wirtschaftsgüter (Geld, Waren, Dienstleistungen), die der Steuerpflichtige dem Betrieb für sich, seinen Haushalt oder für andere betriebsfremde Zwecke entnommen hat. Sie haben das $EK_{t}$ gemindert, ohne Aufwand zu sein $\rightarrow$ **Zurechnung (+)**.
* **Privateinlagen ($PI$):** Alle Wirtschaftsgüter, die der Steuerpflichtige dem Betrieb aus seinem Privatvermögen zugeführt hat. Sie haben das $EK_{t}$ erhöht, ohne Ertrag zu sein $\rightarrow$ **Abrechnung (-)**.

```mermaid
graph TD
    A[Eigenkapital 31.12. -Endbestand-] --> B( - )
    C[Eigenkapital 01.01. -Anfangsbestand-] --> B
    B --> D{Eigenkapital-Veränderung}
    D --> E( + Privatentnahmen )
    D --> F( - Privateinlagen )
    E --> G[Steuerlicher Gewinn / Verlust]
    F --> G
````

## ⏳ 2. Rechnungsabgrenzungsposten (RAP)

Die Rechnungsabgrenzung stellt die Einhaltung des **Prinzips der Periodenabgrenzung (§ 252 Abs. 1 Nr. 5 HGB)** sicher. Aufwendungen und Erträge müssen dem Jahr ihrer wirtschaftlichen Verursachung zugeordnet werden, unabhängig vom Zahlungszeitpunkt.

### 📌 Systematische Unterscheidung

```
                              🔍 ABGRENZUNGS-MATRIX
                              
                     Zahlung JETZT            Zahlung SPÄTER
                 (im alten Geschäftsjahr)  (im neuen Geschäftsjahr)
                ┌────────────────────────┬────────────────────────┐
   Aufwand/     │     TRANSITORISCH      │      ANTIZIPATIV       │
   Ertrag       │                        │                        │
   SPÄTER       │  Aktive/Passive RAP   │   (Keine Abgrenzung    │
                │     (ARA / PRA)        │      erforderlich)     │
                ├────────────────────────┼────────────────────────┤
   Aufwand/     │                        │      ANTIZIPATIV       │
   Ertrag       │   (Normale Buchung,    │                        │
   JETZT        │    keine Abgrenzung)   │  Sonst. Ford. / Verb.  │
                └────────────────────────┴────────────────────────┘
```

### 🅰️ Transitorische Abgrenzung (Ausgabe/Einnahme jetzt, Aufwand/Ertrag später)

- **Aktiver Rechnungsabgrenzungsposten (ARA) - § 250 Abs. 1 HGB / § 5 Abs. 5 EStG:**
    
    - _Definition:_ Ausgaben vor dem Abschlussstichtag, soweit sie Aufwand für eine bestimmte Zeit nach diesem Tag darstellen.
        
    - _Eselsbrücke:_ **Ausgabe jetzt, Aufwand später** (Guthaben-Charakter).
        
    - _Buchungssatz am 31.12.:_ `2900 ARA an Aufwandskonto`
        
    - _Rückbuchung im neuen Jahr:_ `Aufwandskonto an 2900 ARA`
        
- **Passiver Rechnungsabgrenzungsposten (PRA) - § 250 Abs. 2 HGB / § 5 Abs. 5 EStG:**
    
    - _Definition:_ Einnahmen vor dem Abschlussstichtag, soweit sie Ertrag für eine bestimmte Zeit nach diesem Tag darstellen.
        
    - _Eselsbrücke:_ **Einnahme jetzt, Ertrag später** (Verpflichtungs-Charakter).
        
    - _Buchungssatz am 31.12.:_ `Ertragskonto an 2990 PRA`
        
    - _Rückbuchung im neuen Jahr:_ `2990 PRA an Ertragskonto`
        

### 🅱️ Antizipative Abgrenzung (Aufwand/Ertrag jetzt, Zahlung später)

- **Sonstige Forderungen (Sonst. Ford.):**
    
    - _Definition:_ Ertrag gehört wirtschaftlich ins alte Jahr, die Zahlung geht aber erst im neuen Jahr ein.
        
    - _Buchungssatz am 31.12.:_ `2690 Sonstige Forderungen an Ertragskonto` (erfolgsrelevante Einbuchung).
        
- **Sonstige Verbindlichkeiten (Sonst. Verb.):**
    
    - _Definition:_ Aufwand gehört wirtschaftlich ins alte Jahr, die Zahlung erfolgt aber erst im neuen Jahr.
        
    - _Buchungssatz am 31.12.:_ `Aufwandskonto an 4890 Sonstige Verbindlichkeiten` (erfolgsrelevante Einbuchung).
        

## 👤 3. Privatvorgänge & Korrekturen bei Einzelunternehmen

Einzahlungen und Entnahmen des Unternehmers dürfen den steuerlichen Gewinn nicht verändern. Sie werden über das **Eigenkapital-Unterkonto "Privat" (3000)** abgewickelt.

### 📌 Entnahme von Dienstleistungen / Nutzung von Arbeitskraft

Nimmt der Unternehmer betriebliche Ressourcen (wie die Arbeitskraft von Angestellten) für private Zwecke in Anspruch, liegt eine **Nutzungsentnahme** vor.

- **Problem:** Die Gehälter der Mitarbeiter wurden als betrieblicher Aufwand verbucht (`6200 Lohnaufwand` / `6300 Gehaltsaufwand`), wodurch der Gewinn fälschlicherweise sinkt.
    
- **Korrektur:** Der privat veranlasste Aufwandsteil muss neutralisiert (im Haben ausgebucht) und dem Privatkonto (im Soll) belastet werden.
    
- **Buchungssatz:**
    
    ```
    3001 Privatentnahmen 
      an 6200 Lohnaufwand (bzw. Gehaltsaufwand)
    ```

### 📌 Umsatzsteuerliche Relevanz bei Sachentnahmen / Unentgeltlichen Wertabgaben

Entnimmt der Unternehmer Gegenstände (Waren, Erzeugnisse) oder Dienstleistungen aus dem Unternehmen für private Zwecke, unterliegt dies der Umsatzsteuer als **unentgeltliche Wertabgabe (§ 3 Abs. 1b bzw. Abs. 9a UStG)**.

- _Sachentnahme (z. B. Entnahme von Lebensmitteln im Supermarkt):_
    
    ```
    3001 Privatentnahmen (Bruttobetrag)
      an 8910 Entnahme durch den Unternehmer für private Zwecke (Nettowert)
      und 4800 Umsatzsteuer (19% / 7%)
    ```
    
- _Privatnutzung eines Firmenwagens (1%-Regelung):_
    
    ```
    3001 Privatentnahmen (Bruttobetrag)
      an 8921 Verwendung von Gegenständen für Zwecke außerhalb des Unternehmens (Nettowert)
      und 4800 Umsatzsteuer (19%)
    ```