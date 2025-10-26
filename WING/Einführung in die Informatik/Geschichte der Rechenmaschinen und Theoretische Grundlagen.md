Pioniere der Informatik
• **Kurt Gödel** (1906-1978): Liefert theoretische Aussagen zum Algorithmenbegriff.
• **Alan M. Turing** (1911-1954): Definiert den Algorithmenbegriff über eine hypothetische Maschine (Turing-Maschine).
• **John von Neumann** (1903-1957): Seine grundlegenden Arbeiten betreffen die Computerarchitektur, insbesondere die Speicherung der Daten und Programme auf dem **gleichen Medium** sowie die Definition von Registern (Indexregister). Er schlug vor, das Programm im Speicher des Rechners abzulegen.

**Historischer Überblick**
• **Rechenbretter** werden seit dem Altertum in China, Japan und Russland verwendet. Addition und Subtraktion sind ähnlich schnell wie mit einem Taschenrechner.
• **Gottfried Wilhelm von Leibniz** (1646-1716) entwickelte die Arithmetik des Dualsystems.
• **Jacquard-Webstuhl (1805):** Die Steuerung (Programmierung) erfolgte durch gelochte Holzplättchen (perforated wooden tilesw).
• **Charles Babbage** (1792-1871): Entwickelte eine mechanische Rechenmaschine und hatte die Idee, Programme nach dem Jacquard-Prinzip zu speichern (was an technischem Mangel scheiterte).

**Die ersten Rechner**
• **Konrad Zuse** (1910-1995) hatte 1934 die Idee, das **duale Zahlensystem** zum Rechnen zu nutzen.
    ◦ Die **Z1** war eine Rechenmaschine mit mechanischen Schaltern.
    ◦ Anfang der 1940er Jahre entwickelte er die **Z3** und **Z4**, elektromechanische Relaisrechner im Dualsystem mit Lochkartensteuerung.
    ◦ Die **Z3 (1941)** gilt als **erster voll funktionsfähiger programmgesteuerter Computer**. Sie arbeitete elektromechanisch und lief mit $10 \text{ Hz}$.
    ◦ Die Schaltzeiten elektromechanischer Relaisrechner lagen bei **$100 \text{ ms}$**.
    ◦ Zuses Programmiersprache war der **„Plankalkul“** (1945/46).

• **Aiken (USA, 1944):** Röhrenrechner **Mark I** im Dezimalsystem. Schaltzeiten: **$0,1 \text{ ms}$**.
• **Eckert/Mauchly (1946):** Elektronenrechner **ENIAC** ("Electronic Numerical Integrator And Computer").
    ◦ Er hatte $18.000$ Röhren und $1.500$ Relais.
    ◦ Der ENIAC (1947) wog $27$ Tonnen, hatte eine Größe von $10 \times 17 \times 3 \text{ Metern}$ und kostete $468.000$ Dollar.
    ◦ Programmänderungen beim ENIAC dauerten einige Tage.
    ◦ Der ENIAC hatte nur $1 \text{ Kbit}$ Arbeitsspeicher.

• **EDSAC (1949, Cambridge University):** Gilt als der erste „von-Neumann-Rechner“.

Stand der Technik 1950
• Zweiwertige Zustände ersetzten zehnwertige Daten.
• Elektronik ersetzte Mechanik.
• Das Programm lag im Speicher des Rechners.

Rechnergenerationen

|                      |            |                                                                        |                                                                                |                                            |
| -------------------- | ---------- | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------ | ------------------------------------------ |
| Generation           | Zeitraum   | Technologie                                                            | Wichtige Merkmale                                                              | Geschwindigkeit (Addition/Instruktionen)   |
| **1. (Pionierzeit)** | Bis 1960   | Relais und Elektronenröhren                                            | Speicher: $< 1000$ Zahlen; praktisch keine Software.                           | Addition: $100\text{-}1000$ Mikrosekunden. |
| **2.**               | Bis 1970   | Transistoren, Ferritkern-, Band-, Trommel-, Plattenspeicher            | FORTRAN, Cobol; maschinenunabhängige Betriebssysteme, Stapelbetrieb.           | $10.000$ Instruktionen/sec.                |
| **3.**               | Bis 1980   | Teilweise integrierte Schaltkreise (LSI)                               | Time sharing, Terminals, grafische Datenverarbeitung; 8-bit Architektur (Z80). | $500.000$ Instruktionen/sec.               |
| **4.**               | Heutige    | Hochintegrierte Schaltungen (VLSI)                                     | $16/32/64$-bit Architekturen, MultiCore/ManyCore, Netzwerke, TB Speicher.      | $> 1.000.000$ Instruktionen/sec.           |
| **5.**               | Zukünftige | Optische, biologische Systeme, Quantencomputer, hochparallele Systeme. |                                                                                |                                            |

Moore’s Law

• Das „Gesetz“ (Gesetzmäßigkeit) besagt, dass sich die **Komplexität integrierter Schaltkreise** bei vergleichbaren Komponentenkosten **regelmäßig verdoppelt**.
• Als Verdopplungszeitraum werden $12$, $18$ oder $24$ Monate genannt.
• Ein heutiges Smartphone hat **deutlich mehr als $10^{12}$ Transistoren**.
• Würde man diese Komplexität mit Vakuumröhren umsetzen, wären die Konsequenzen extrem, z.B. das Gewicht von ca. $2500$ Flugzeugträgern oder Kosten in Höhe der gesamten Weltwirtschaftsleistung von 1951.

Programmierung und Sprachen
Definition
• Ein Computer ist ein Gerät, das **mittels programmierbarer Rechenvorschriften Daten verarbeitet**.
Maschinensprache
• Dient zur direkten Steuerung des Prozessors.
• Hängt von der Prozessorarchitektur ab; jeder Rechner hat seine eigene Maschinensprache.
• Befehle und Argumente sind als **Binärstrings** (Folgen von 0 und 1) kodiert und werden vom Rechner direkt ausgeführt.
• Grundlegende Maschinen-Befehle gliedern sich in:
    ◦ Arithmetische Operationen (Berechnungen).
    ◦ Speicheroperationen (Datenübertragung zwischen Registern und Speicher).
    ◦ Vergleichsoperationen.
    ◦ Steueroperationen (Verzweigungen).

Assembler Code
• Ersetzt die Binärstrings der Maschinen-Befehle durch **mnemonische Codes**.
• Erleichtert die Programmierung (ein wenig) durch die Übersetzung mittels einfacher Tabelle.
• Beispiel: Der Maschinen-Befehl `10110000 01100001` (x86) entspricht dem Assemblerbefehl `mov al, 61h`.
• Dennoch bleibt maschinennahe Programmierung mühselig, da eine große konzeptuelle Distanz zwischen Algorithmus und Implementierung besteht.

Höhere Programmiersprachen
• Sie fungieren als Mittler zwischen Mensch und Maschine.
• **Compiler:** Übersetzt das Programm vor der Ausführung.
• **Interpreter:** „Dolmetscht“ das Programm während der Ausführung.
• **Syntax:** Definiert die zulässigen Worte/Sätze in einem Programm (z.B. `int`, `while`).
• **Semantik:** Definiert die Bedeutung der Syntax.
• **Programmbibliotheken (Libraries):** Sammlungen vordefinierter Routinen, die die Programmierung durch Wiederverwendung vereinfachen und verbessern.

Software- und Hardwarekomplexität & Qualität
Komplexität
• Ein Smartphone verfügt heute über die Rechenleistung aller weltweit verfügbarer Computer im Jahr 1980.
• Ein Smartphone besitzt mehrere Prozessoren (Hauptprozessor, Graphikprozessor, WLAN Prozessor, etc.).
• Ein normales Auto enthält heute mehr als **$100 \text{ Millionen}$ Zeilen Programmcode**.

**Historische Fehler und Ursachen**
• Bekannte historische Softwarefehler umfassen den Mars Climate Orbiter, Ariane 5, 737MAX und Mariner 1 Trägerrakete.
• Diese Fehler traten in den neunziger Jahren verstärkt auf, nachdem die Software zuvor Jahrzehnte lang zuverlässig funktioniert hatte.
• **Ursachen:**
    ◦ **Wachsende Komplexität** der Software.
    ◦ Sparzwänge und übertriebenes Selbstvertrauen.
    ◦ Managementfehler, Verteilung der Verantwortung und fehlende Kommunikation.
    ◦ Schlechte Spezifikation der Anforderungen.
    
    
**Fehlende Systemtests** mit der vollständigen Hardware (Simulationen wurden genutzt, aber die Bugs steckten im Detail des Zusammenspiels von Komponenten).
    ◦ Wiederverwendung von ungeeigneter Software (z.B. bei Ariane 5, wo Software ausgeführt wurde, die eigentlich nicht benötigt wurde).

**Qualität der Softwareentwicklung**
• Es besteht ein **Trade-off** zwischen der Effizienz in der Entwicklung und der Effizienz in der Ausführung der Software.
• **Mangel an erfahrenen Entwicklern:** Die Anzahl der Software-Entwickler verdoppelt sich ca. alle $5$ Jahre, was bedeutet, dass die Hälfte aller Entwickler weniger als $5$ Jahre Erfahrung hat.
• Ein großer Teil der Software wurde von 25-jährigen Entwicklern programmiert.
• Die Gesellschaft ist vollständig auf Softwaresysteme angewiesen.
• Schlechte Software führt dazu, dass Menschen sterben.
• Die Softwareentwicklung ist eine der letzten wichtigen Domänen für die Gesellschaft, die **keiner „Ethik“, „Regeln“ oder vergleichbarem folgen MUSS**. Es gibt (noch) keine Reglementierung durch den Gesetzgeber.