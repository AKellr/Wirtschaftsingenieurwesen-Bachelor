### 1. Was ist der wesentliche Unterschied zwischen **Information** und **Repräsentation** ("Daten") im Kontext der Informatik?

**Antwort:** Die **Information** ist der abstrakte Gehalt, die "Bedeutung" oder die Semantik einer Nachricht. Die **Repräsentation** (die "Daten") ist die äußere, konkrete Form der Darstellung dieser Nachricht, beispielsweise als Text oder Bitfolge.

### 2. Auf welcher niedrigsten Ebene der Datenverarbeitung arbeitet ein Computer und wie wird diese Ebene technisch realisiert?

**Antwort:** Die niedrigste Ebene ist die **Null/Eins-Ebene** der Datenverarbeitung. Technisch wird dies durch **elektrische Signale** realisiert, die Transistoren und Widerstände beeinflussen. Konkrete Beispiele sind die Darstellung von '0' und '1' über Ladungszustände (ungeladen/geladen), Spannungen (z.B. 0 Volt/5 Volt) oder Magnetisierung.

### 3. Erklären Sie den Begriff **Bit** und geben Sie Beispiele für binäre Entscheidungen, die durch ein Bit dargestellt werden können.

**Antwort:** Das **Bit** ist die kleinstmögliche Informationseinheit. Es repräsentiert die Antwort auf eine Frage, die nur **zwei Möglichkeiten** zulässt, z.B. ja/nein, wahr/falsch, schwarz/weiß oder 0/1.

### 4. Was ist ein **Byte**, wie viele Bits enthält es, und welche typischen Informationen kann ein Byte in einem modernen Computersystem speichern?

**Antwort:** Ein **Byte** ist eine Bitfolge, die aus **8 Bit** besteht. Es ist die kleinste adressierbare Einheit im Speicher und kann zur Darstellung von **einem einzelnen Zeichen** (wie 'A' oder '5'), einem **Grau- oder Farbwert** oder einer **vorzeichenlosen, ganzen Zahl zwischen 0 und 255** (28−1) genutzt werden.

### 5. Erklären Sie den Prozess der **Interpretation** einer Repräsentation und in welchem Bereich der Informatik dieser Prozess formal schwierig zu erfassen ist.

**Antwort:** Die **Interpretation** ist der gedankliche Übergang von der Repräsentation (Daten) zur abstrakten Information (Bedeutungsinhalt). Der Prozess des Verstehens im Gehirn ist **formal schwierig erfassbar**, weshalb sich die mathematisch-logische Sichtweise in der Informatik damit begnügt, die Repräsentation auf ein mathematisches Modell abzubilden.

### 6. Wozu dienen **Hexziffern** und wie erleichtern sie die Darstellung von Bitfolgen für den Menschen?

**Antwort:** Hexziffern dienen dazu, lange Bitfolgen, die für den Menschen schwer erfassbar sind, zu vereinfachen. Dies geschieht, indem Bitfolgen zu **Vierergruppen** zusammengefasst werden, wobei jede Gruppe durch eine einzige Ziffer des Hexadezimalsystems (Basis 16) repräsentiert wird.

### 7. Was ist ein **Kontext** in einem Computersystem und warum ist er notwendig, um binäre Folgen als Text, Zahlen oder Video zu unterscheiden?

**Antwort:** Ein **Kontext** ist ein notwendiger Rahmen, der es erlaubt, eine gespeicherte binäre Folge (die selbst nur Nullen und Einsen enthält) richtig zu interpretieren. Da in einem Computersystem nur binäre Folgen abgespeichert werden können, ist der Kontext (z.B. Dateiformat oder Namenskonventionen) erforderlich, um dieselbe Bitfolge als Text, Zahl, Musik oder Video zu unterscheiden.

---

## 🔢 Fragen und Antworten zu Zahlensystemen und Arithmetik

### 8. Erläutern Sie die allgemeine Formel (N=∑ai​⋅Bi) zur Darstellung einer Zahl **N** in einem **Stellenwertsystem** zur Basis **B**.

**Antwort:** Die Formel N=∑ai​⋅Bi besagt, dass eine Zahl N im Stellenwertsystem als Summe dargestellt wird, bei der jede Ziffer ai​ (das "Zeichen") mit der entsprechenden Potenz der Basis B (dem "Stellenwert") multipliziert wird. Die Basis B definiert dabei die Anzahl der unterscheidbaren Ziffern, die im System verwendet werden.

### 9. Nennen Sie die vier üblichen **Positionssysteme** in der Informatik und die jeweilige Basis, sowie die Menge der verwendeten Ziffern.

**Antwort:** Die üblichen Positionssysteme sind:

- **Dezimalsystem**: Basis 10, Ziffern 0,…,9.
    
- **Binärsystem**: Basis 2, Ziffern 0,1.
    
- **Oktalsystem**: Basis 8, Ziffern 0,…,7.
    
- **Hexadezimalsystem**: Basis 16, Ziffern 0,…,9,A,B,C,D,E,F.
    

### 10. Beschreiben Sie die "Intuitivmethode" zur **Konvertierung** einer Dezimalzahl in eine Binärzahl.

**Antwort:** Bei der **Intuitivmethode** (Addition von geeigneten Zweierpotenzen) sucht man die größte Zweierpotenz, die noch in die umzuwandelnde Zahl passt. Man subtrahiert diese Potenz von der Zahl und wiederholt den Vorgang mit dem Ergebnis, bis der Rest Null ist. Wird eine Potenz verwendet, steht an der entsprechenden Binärstelle eine 1, andernfalls eine 0.

### 11. Wie funktioniert die **Addition** im Binärsystem im Falle von 1+1?

**Antwort:** Die Addition von 1+1 im Binärsystem ergibt 0 mit einem **Übertrag** (_Carry_) von 1 zur nächsthöheren Stelle.

### 12. Ein Überlauf tritt auf, wenn das Ergebnis einer Addition größer oder gleich 2N ist. Welche Konsequenz hat das Verwerfen des Carry-Bits?

**Antwort:** Ein **Überlauf** (_Overflow_) tritt bei N-Bit-Zahlen auf, wenn das Ergebnis gleich oder größer als 2N ist. Das **Verwerfen des Carry-Bits** (oder Übertrags) führt dazu, dass die Operation **modulo 2N** ausgeführt wird. Die Konsequenz ist, dass das Ergebnis **falsch** ist, da es in den darstellbaren Zahlenbereich "zurückspringt" (z.B. 11+8→3 bei 4 Bit).

### 13. Was ist der Hauptgrund, warum die **Zweierkomplementdarstellung** heutzutage für die Speicherung **vorzeichenbehafteter ganzer Zahlen** verwendet wird, im Vergleich zur Vorzeichen-und-Wert- oder Einer-Komplement-Darstellung?

**Antwort:** Die Zweierkomplementdarstellung bietet mehrere Vorteile, die sie zur Standardmethode machen: Sie ermöglicht eine **eindeutige Darstellung der Zahl 0** , das Vorzeichen ist im ersten Bit enthalten , und sie **vermeidet Probleme beim formalen Addieren**. Vor allem kann die Subtraktion elegant durch die **Addition des Zweierkomplements** des Subtrahenden realisiert werden (wobei ein Überlauf ignoriert wird).

---

## 📝 Fragen und Antworten zu Zeichen, Text, und Gleitkommazahlen

### 14. Was ist **Plain Text** und welche Informationen über die Textformatierung werden bei dieser Darstellung weggelassen?

**Antwort:** **Plain Text** (Klartext) ist eine Folge von Symbolen wie Buchstaben, Zahlen und Interpunktion. Er **verzichtet** auf jegliche typografische oder semantische Informationen wie Schriftart, Schriftgröße, Schriftfarbe oder Seitenstruktur. Er unterstützt nur rudimentär Zeilen- und Absatzstrukturen.

### 15. Erklären Sie die historische Entwicklung vom **ASCII**-Code zum **Unicode** in Bezug auf die Anzahl der darstellbaren Zeichen.

**Antwort:** Der **ASCII**-Code war ein **7-Bit-Code** und konnte somit nur 128 Zeichen darstellen (hauptsächlich das englische Alphabet und Steuerzeichen). Die Erweiterungen wie ISO 8859 nutzten ein achtes Bit für nationale Sonderzeichen. **Unicode** wurde als Lösung für das Problem unterschiedlicher Alphabete konzipiert, indem es ursprünglich ein **Zwei-Byte-Code** war (heute ein 31-Bit-Zeichensatz) und damit eine **eindeutige Codierung für jedes Zeichen** aller Schriftsysteme ermöglicht, unabhängig von der Sprache oder Plattform.

### 16. Wie wird das **Ende** eines Textes (eines _Strings_) im Speicher eines Rechners in der Programmiersprache C/C++ im Vergleich zu Pascal/Java/Python signalisiert?

**Antwort:** In Sprachen wie **C und C++** wird das Ende der Zeichenkette (String) durch ein reserviertes **Null-Byte** (ASCII-Wert 0) signalisiert. In Sprachen wie **Pascal, Java und Python** wird die **Länge** des Strings zusammen mit dem String gespeichert, um das Ende festzulegen.

### 17. Was ist der Hauptgrund für die Verwendung der **Exponentialdarstellung** (**Gleitkommazahlen**) im Binärsystem im Vergleich zur Festkommadarstellung?

**Antwort:** Der Hauptgrund ist die Notwendigkeit, einen **sehr großen Zahlenbereich** (von extrem kleinen bis extrem großen Zahlen) abbilden zu können. Im Gegensatz zur Festkommadarstellung, die eine große Verschwendung von Bits wäre , ermöglicht die Exponentialdarstellung eine effiziente Speicherung, indem die **Signifikanten Stellen (Mantisse)** und die **Größenordnung (Exponent)** getrennt gespeichert werden.

### 18. Welche drei Hauptkomponenten bestimmen eine **Gleitkommazahl** im Binärsystem nach dem IEEE 754 Standard?

**Antwort:** Eine Gleitkommazahl wird durch die folgenden drei Komponenten bestimmt:

- Das **Vorzeichen** (S).
    
- Die **Mantisse** (M).
    
- Der **Exponent** (E).
    

---

## 🖼️ Fragen und Antworten zu Bildern und Farben

### 19. Wie wird eine **Farbe** im **RGB-Farbschema** definiert und welche Wertebereiche haben die Farbanteile in der Praxis?

**Antwort:** Eine Farbe im **RGB-Schema** (Rot, Grün, Blau) wird durch ein **Zahlentripel** (r,g,b) definiert. Jede Zahl repräsentiert die Intensität des jeweiligen Farbanteils. In der Praxis hat jeder dieser Farbwerte oft einen Bereich von **0 bis 255** (was 28 Werte ergibt).

### 20. Beschreiben Sie den Unterschied zwischen **additiver** und **subtraktiver Farbmischung** und nennen Sie ein typisches Anwendungsbeispiel für jeden Typ.

**Antwort:**

- **Additive Farbmischung:** Hierbei **überlagert** sich das Licht von mehreren Lichtquellen, und deren Farbanteile werden addiert. Die Mischung von Rot, Grün und Blau ergibt **Weiß**. Ein typisches Beispiel ist die Farbwahrnehmung auf einem **Monitor oder Farbfernseher**.
    
- **Subtraktive Farbmischung:** Hierbei wird Farbe gemischt (z.B. Pigmente), wobei die Oberfläche die entgegengesetzten Farbanteile **verschluckt** (subtrahiert). Die Mischung der drei Grundfarben (Cyan, Magenta, Yellow) ergibt theoretisch **Schwarz**. Ein typisches Beispiel ist der **Farbdrucker** oder das Mischen von Farben beim Malen.