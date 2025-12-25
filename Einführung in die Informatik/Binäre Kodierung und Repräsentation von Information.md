[[INF]]
## Bits und Bytes (Bits and Bytes)
### 1. Grundlagen der Repräsentation (Fundamentals of Representation)
• Die niedrigste Ebene der Datenverarbeitung ist **Null/Eins**. (The lowest level of data processing is **Zero/One**).

• **Information** ist der abstrakte Gehalt ("Bedeutungsinhalt", "Semantik") einer Nachricht. (Information is the abstract content ("meaning content", "semantics") of a message).
• **Repräsentation** ist die äußere, konkrete Form der Nachricht (z.B. Zeichenfolgen, gesprochenes Wort). (Representation is the outer, concrete form of the message (e.g., character strings, spoken word)).

![[Pasted image 20251014131403.png]]

• **Interpretation** ist der gedankliche Übergang von der Repräsentation zur abstrakten Information. (Interpretation is the conceptual transition from representation to abstract information).
• Die Wurzeln der Informatik liegen in der **Mathematik**, weshalb die Darstellung von Zahlen (binär) und algebraischen (bool'schen) Objekten besonders relevant ist. (The roots of computer science lie in **Mathematics**, which is why the representation of numbers (binary) and algebraic (Boolean) objects is particularly relevant).

• In einem Computersystem können nur **Binärfolgen** abgespeichert werden. Der **Kontext** ist notwendig, um diese Binärfolgen als Text, Zahlen, Musik oder Video zu interpretieren. (Only **binary sequences** can be stored in a computer system. **Context** is necessary to interpret these binary sequences as text, numbers, music, or video).

### 2. Bits und ihre Darstellung (Bits and their Representation)
• Das **Bit** ist die kleinstmögliche Informationseinheit. (The **Bit** is the smallest possible unit of information).

• Es erlaubt die Antwort auf Fragen mit zwei Möglichkeiten (z.B. ja/nein, wahr/falsch, 0/1). (It allows the answer to questions with two possibilities (e.g., yes/no, true/false, 0/1)).
• Die Darstellung von Bits erfolgt im **Binärcode** (oft 0 und 1). (Bits are represented in **Binary code** (often 0 and 1)).

• Technische Darstellungsformen umfassen: **Ladung** (0=ungeladen, 1=geladen), **Spannung** (0=0 Volt, 1=5 Volt), **Magnetisierung** oder **Licht**. (Technical forms of representation include: **Charge**, **Voltage**, **Magnetization**, or **Light**).

• Die Zahl der möglichen Antworten verdoppelt sich mit jedem zusätzlichen Bit. (The number of possible answers doubles with every additional bit).

• Bei $n$ Bit gibt es genau $2^n$ mögliche Bitfolgen. (For $n$ bits, there are exactly $2^n$ possible bit sequences).

### 3. Byte und Wort (Byte and Word)
• Ein **Byte** ist eine Bitfolge, die aus **8 Bit** besteht. (A **Byte** is a bit sequence consisting of **8 bits**).
• Bytes sind die kleinsten Bitfolgen, mit denen moderne Computer arbeiten können. (Bytes are the smallest bit sequences that modern computers can work with).

• Im Speicher ist ein Byte die kleinste **adressierbare Einheit**. (In memory, a byte is the smallest **addressable unit**).

• Ein Byte kann ein Zeichen (z.B. 'A'), einen Grau-/Farbwert oder eine vorzeichenlose, ganze Zahl zwischen 0 und 255 ($2^8 - 1$) darstellen. (A Byte can represent a character, a grayscale/color value, or an unsigned integer between 0 and 255).

• Zur Klarstellung wird für 8 Bit auch der Begriff **Oktett** verwendet. (For clarification, the term **Octet** is also used for 8 bits).

• **Worte** ("Words") sind die "natürliche" Gruppierung von Bits im Rechner, wobei die Definition stark uneinheitlich ist (heute oft 4 Byte auf einem 32-Bit-Rechner). (Words are the "natural" grouping of bits in the computer, although the definition is highly inconsistent (often 4 bytes on a 32-bit computer today)).

• Lange Bitfolgen werden oft in **Hexziffern** (Hexadezimalsystem, Basis 16) zusammengefasst, um sie für Menschen leichter handhabbar zu machen (Bitfolgen werden zu Vierergruppen zusammengefasst). (Long bit sequences are often summarized in **Hexadecimal digits** (base 16) to make them easier for humans to handle (bit sequences are grouped into fours)).
### Zahlensysteme (Number Systems)
• **Stellenwertsysteme:** Jede Zahl $N$ lässt sich als Sequenz von Zeichen $a_i$ darstellen ($N = \sum a_i \cdot B^i$), wobei $B$ die Basis ist. (Positional systems: Every number $N$ can be represented as a sequence of characters $a_i$, where $N = \sum a_i \cdot B^i$, and $B$ is the base).

• In einem Zahlensystem zur Basis $N$ gibt es $N$ Ziffern mit Werten von $0$ bis $N-1$. (In a number system with base $N$, there are $N$ digits with values from $0$ to $N-1$).

• **Übliche Positionssysteme** sind: (Common positional systems are):
    ◦ **Dezimalsystem:** Basis 10, Ziffern 0-9.
    ◦ **Binärsystem:** Basis 2, Ziffern 0, 1.
    ◦ **Oktalsystem:** Basis 8, Ziffern 0-7.
    ◦ **Hexadezimalsystem:** Basis 16, Ziffern 0-9 und A-F.

• Die Darstellung von Zahlen mit verschiedener Basis wird oft durch Präfixe oder tiefgestellte Indizes angezeigt (z.B. $97_{10} = 61_{16} = 01100001_2$). (The representation of numbers with different bases is often indicated by prefixes or subscripts).

### Kodierung Ganzer Zahlen (Encoding of Integers)
• Mit $N$ Bits können $2^N$ Zahlen repräsentiert werden. (With $N$ bits, $2^N$ numbers can be represented).

• **Nichtnegative Zahlen (unsigned):** Werden von $0$ bis $2^N-1$ dargestellt. (Non-negative numbers (unsigned): Are represented from $0$ to $2^N-1$).

• **Ganze Zahlen (signed):** Werden von $-2^{N-1}$ bis $2^{N-1}-1$ dargestellt. (Integers (signed): Are represented from $-2^{N-1}$ to $2^{N-1}-1$).

• Heutige Rechner verwenden die **Zweierkomplementdarstellung**. (Current computers use the **Two's Complement representation**).

• **Zweierkomplement:** Eine negative Zahl wird durch bitweise Komplementierung (Einer-Komplement) und anschließende Addition von 1 erzeugt ($x^* = \bar{x} + 1$). (Two's Complement: A negative number is generated by bitwise complementation (one's complement) and subsequent addition of 1).

• Vorteile des Zweierkomplements: Eindeutige Darstellung der Zahl 0 und das Vorzeichen ist im ersten Bit enthalten. Subtraktion kann durch Addition des Zweierkomplements ausgeführt werden (Überlauf wird weggelassen). (Advantages: Unique representation of the number 0, and the sign is included in the first bit. Subtraction can be performed by adding the two's complement).

• Ein **Überlauf** (Overflow) tritt auf, wenn das Ergebnis einer Addition größer oder gleich $2^N$ ist. (An **Overflow** occurs when the result of an addition is greater than or equal to $2^N$).

### Kodierung von Text (Encoding of Text)
• **Plain Text** (Klartext) ist eine Folge von Symbolen, die auf Informationen wie Schriftart, Größe oder Farbe verzichtet. (Plain Text is a sequence of symbols that dispenses with information such as font, size, or color).

• **Historische und gängige Codes:** EBCDIC, **ASCII**, ISO 8859, **Unicode**. (Historical and common codes).

• **ASCII** (American Standard Code for Information Interchange): Ist ein 7-Bit-Zeichensatz (128 Zeichen) für das englische Alphabet, inklusive Steuerzeichen. Ziffern, Groß- und Kleinbuchstaben sind systematisch durchgehend nummeriert.
![[Pasted image 20251014131520.png]]

• **ISO 8859:** Nutzt die Werte über 127 zur Erweiterung von ASCII, um nationale Sonderzeichen (z.B. deutsche Umlaute) darzustellen. Es gibt viele Varianten (z.B. Latin-1, Latin-9).

• **Unicode:** Die Lösungsidee für unterschiedliche Alphabete ist eine eindeutige Codierung für jedes Zeichen, unabhängig von Plattform oder Sprache ("Über"-Alphabet).
    ◦ Ursprünglich war Unicode ein 16-Bit-Zeichensatz, heute ist er ein 31-Bit-Zeichensatz ($17 \cdot 2^{16}$ Zeichen).
    ◦ **Unicode ist keine Binärcodierung**. (Unicode is not a binary encoding).
![[Pasted image 20251014131558.png]]

• **UTF-8** (Unicode Transformation Format): Kodiert Unicode in Bytes, wobei es eine **variable Zahl von 1 bis 4 Bytes pro Zeichen** verwendet.
    ◦ Zeichen $<128$ benötigen 1 Byte und sind äquivalent zu ASCII.
![[Pasted image 20251014131617.png]]

• **Stringende:** In C/C++ wird das Ende einer Zeichenkette durch ein **Null-Byte (Wert 0)** markiert. In anderen Systemen (Pascal, Java, Python) wird die Länge zusammen mit dem String gespeichert.

• Der ASCII-Wert 10 ist für **"Newline" (NL)** reserviert, um Zeilenumbrüche in Dateien anzuzeigen.

### Kodierung Gebrochener Zahlen (Encoding of Fractional Numbers)
• Zur Darstellung extrem großer und extrem kleiner Zahlen wird die **Exponentialdarstellung** verwendet. (To represent extremely large and extremely small numbers, **exponential notation** is used).

• Die Idee ist, die **signifikanten Stellen** und die **Größenordnung** getrennt zu speichern. (The idea is to store the **significant digits** and the **magnitude** separately).

• **Gleitkommazahlen (Floating Point Numbers):** Darstellung durch drei Komponenten: **Vorzeichen (S), Mantisse (M) und Exponent (E)**: $(-1)^S \times M \times 2^E$.

• **Normalform (IEEE 754):** Eine Zahl ist normalisiert, wenn $1.0 \le M < 2.0$ gilt.

• Das führende Bit 1 links der Dezimalstelle wird nicht gespeichert (**„hidden bit“**). (The leading bit 1 to the left of the decimal point is not stored (**"hidden bit"**)).
![[Pasted image 20251014131716.png]]

• Der Exponent wird mit einem **Bias** versehen, um negative Exponenten zu vermeiden. (The exponent is provided with a **Bias** to avoid negative exponents).

• Spezielle Exponenten werden zur Darstellung von Null, Unendlich ($\infty$) und NaN (not a number) verwendet.

• Da nicht jede gebrochene Dezimalzahl endlich binär darstellbar ist, entstehen bei der Konvertierung **Rundungsfehler**. (Since not every fractional decimal number can be finitely represented in binary, **rounding errors** occur during conversion).

### Farben und Bilder (Colors and Images)
• Das menschliche Auge unterscheidet Farben durch **drei Arten von Zäpfchen**, die für Rot, Grün und Blau empfindlich sind. (The human eye distinguishes colors using **three types of cones** sensitive to red, green, and blue).

• **RGB-Schema (Additive Farbmischung):** Eine Farbe wird durch ein Zahlentripel $(r, g, b)$ definiert (oft im Bereich [0...255]).
    ◦ Wenn Lichtquellen verschiedener Farben zusammenkommen, addieren sich deren Farbanteile. Rot + Grün + Blau ergibt **Weiß**.
    ◦ RGB ist der Standard für Bildschirme.

• **Subtraktive Farbmischung:** Wird beim Mischen von Farben (Malen) oder in Farbdruckern verwendet.
    ◦ Hier werden die verschluckten (subtrahierten) Farbanteile addiert. Rot + Grün + Blau ergibt **Schwarz**.

• **CMYK-Farbmodell:** Ein subtraktives Modell, das im Druck eingesetzt wird: Cyan, Magenta, Yellow, ergänzt durch BlacK (K).

• **Bilder** sind Matrizen/Tabellen aus Farbwerten.

• Jeder Farbwert bezeichnet ein **Pixel** (Picture Element).

• Da der Computerspeicher eindimensional ist, werden die Farbwerte der Pixel sequenziell hintereinander gespeichert. **Metadaten** (im Header der Datei) geben an, wie das Bild wiederhergestellt werden kann (z.B. die Zeilenlänge).

• **Pixel-Grafiken** (Bitmaps) eignen sich gut für Fotos, lassen sich aber schlecht vergrößern.

• **Vektorgrafiken** zerlegen Bilder in geometrische Basiselemente (Punkte, Linien, Polygone) und lassen sich dadurch leichter an neue Größen anpassen. (Vector graphics decompose images into geometric base elements and can therefore be more easily adjusted to new sizes).

