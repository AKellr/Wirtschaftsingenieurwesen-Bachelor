## Teil I: Bits, Bytes und Zahlensysteme
1. **Frage:** Definieren Sie den Begriff "**Information**" und grenzen Sie ihn von der "**Repräsentation (Daten)**" ab, wie es in der Informatik betrachtet wird.
    
    - **Antwort:** **Information** nennen wir den abstrakten Gehalt (die Bedeutung) eines Dokuments, einer Aussage, Beschreibung, Anweisung, Nachricht oder Mitteilung1. Die äußere Form der Darstellung nennen wir die **Repräsentation** (die konkrete Form der Nachricht, d.h., die Daten)2.
        
2. **Frage:** Was ist ein **Bit**, und wie erfolgt seine **technische Darstellung** in einem Computersystem? Nennen Sie dazu mindestens drei Beispiele für physikalische Repräsentationen.
    
    - **Antwort:** Ein **Bit** ist die kleinstmögliche Einheit der Information3. Die technische Darstellung erfolgt unter anderem mit Hilfe von:
        
        - **Ladung** ($0=$ ungeladen, $1=$ geladen)4.
            
        - **Spannung** ($0=0$ Volt, $1=5$ Volt)5.
            
        - **Magnetisierung** ($0=$ nicht magnetisiert, $1=$ magnetisiert)6.
            
        - **Licht** ($0=$ kein Licht, $1=$ Licht)7.
            
3. **Frage:** Wieviele **Bitfolgen** sind theoretisch mit **5 Bit** möglich? Wie groß ist der Zahlenbereich (von 0 bis $2^n-1$) der darstellbaren **nichtnegativen ganzen Zahlen** mit 8 Bit (einem Byte)?
    
    - **Antwort:** Mit $n$ Bit gibt es genau **$2^n$** mögliche Bitfolgen8.
        
        - Mit **5 Bit** sind $2^5 = **32**$ Bitfolgen möglich.
            
        - Mit **8 Bit** ist der Zahlenbereich $0$ bis $2^8 - 1 = **0$ bis $255**$9999.
            
4. **Frage:** Erläutern Sie das **Stellenwertsystem** zur Zahlendarstellung, indem Sie die allgemeine Formel für eine Zahl $N$ zur Basis $B$ angeben.
    
    - **Antwort:** Im **Stellenwertsystem** (Positionssystem) lässt sich jede Zahl $N$ als Sequenz von Zeichen $a_i$ zur Basis $B$ darstellen10. Die Anzahl der notwendigen unterscheidbaren Zeichen ist $B$11.
        
        - Die allgemeine Formel lautet: **$N=\sum{a_i} \cdot B^i$**12.
            
        - Für eine Ziffernfolge $a_m a_{m-1} \dots a_0$ zur Basis $N$ (im Text $N$) gilt: $a_m N^m + a_{m-1} N^{m-1} + \dots + a_0$13.
            
5. Frage: Konvertierungsaufgabe: Binär zu Dezimal
    
    Wandeln Sie die Hexadezimalzahl 4F61 in ihre Dezimaldarstellung um.
    
    - **Antwort:** $4\text{F}61_{16} = 4 \cdot 16^3 + 15 \cdot 16^2 + 6 \cdot 16^1 + 1 \cdot 16^0 = 4 \cdot 4096 + 15 \cdot 256 + 6 \cdot 16 + 1 = 16384 + 3840 + 96 + 1 = **20321**$.
        
    - (English: **20321**)
        
6. Frage: Konvertierungsaufgabe: Dezimal zu Binär
    
    Wandeln Sie die Dezimalzahl 19 und die Dezimalzahl mit Nachkomma 0,6875 mithilfe der Restwertmethode in ihre Binärdarstellung um.
    
    - **Antwort:** **$19_{10} = 10011_2$** und **$0,6875_{10} = 0,1011_2$**14141414.
        
    - (English: **$19_{10} = 10011_2$ and $0.6875_{10} = 0.1011_2$**)
        

---

## Teil II: Zeichen- und Zahlencodierung

7. **Frage:** Wozu dient das **Unicode**-System, und **was ist UTF-8**? Beschreiben Sie den wesentlichen Vorteil von UTF-8 in Bezug auf die Rückwärtskompatibilität zu ASCII.
    
    - **Antwort:** **Unicode** ist als "**Über-Alphabet**" konzipiert, um eine eindeutige Codierung für jedes Zeichen zu schaffen, unabhängig von Plattform, Programm oder Sprache15.
        
    - **UTF-8** ist ein **Unicode Transformation Format** zur Codierung von Unicode in Bytes, das eine **variable Zahl von 1 bis 4 Bytes pro Zeichen** verwendet16161616.
        
    - **Vorteil (Rückwärtskompatibilität):** Zeichen unter $128$ benötigen nur **1 Byte** und sind somit **äquivalent zu ASCII**17.
        
8. **Frage:** Erklären Sie kurz den Unterschied zwischen **Byte-Folgen** und **Zeichen-Folgen** in Bezug auf die interne Speicherung von Strings in Programmiersprachen wie C/C++ im Vergleich zu Java/C#.
    
    - **Antwort:**
        
        - In Sprachen wie **C** und **C++** sind Strings **Folgen von Bytes**; die Interpretation der Bytes (z.B. als Zeichen eines bestimmten Zeichensatzes) obliegt der Anwendung18.
            
        - In Sprachen wie **Java** und **C#** sind Strings **Folgen von Unicode-Zeichen**; jedes Unicodezeichen wird intern durch mehrere Bytes repräsentiert19.
            
9. **Frage:** Beschreiben Sie kurz die **BCD-Codierung (Binary Coded Decimal)**. Nennen Sie einen Vorteil und einen Nachteil dieser Darstellung im Vergleich zur reinen Binärdarstellung.
    
    - **Antwort:** Die **BCD-Codierung** verwendet **4 Bit pro Dezimalziffer** zur Kodierung von $0$ bis $9$20202020.
        
    - **Vorteil:** Die Codierung ist **effizienter als Textdarstellung** (0,5 B pro Ziffer) und **leicht in Dezimaldarstellung umrechenbar**21.
        
    - **Nachteil:** Arithmetische Operationen sind in Hardware **aufwändiger realisierbar** (z.B. Addition erfordert eine Justierung um 6, wenn das Ergebnis $>9$ ist)22222222.
        
10. **Frage:** Welche Darstellungsform für **vorzeichenbehaftete (negative) ganze Zahlen** wird heute in modernen Computern **ausschließlich verwendet**? Erklären Sie kurz, wie die Negativität einer Zahl in dieser Darstellung erkannt wird.
    
    - **Antwort:** Alle modernen Rechner verwenden heute die **Zweierkomplementdarstellung**23.
        
    - Die Negativität wird durch das **erste Bit** (Vorzeichenbit) erkannt: $0$ für nicht-negativ, $1$ für negativ24. Ein großer Vorteil ist, dass diese Darstellung eine **eindeutige Darstellung der Zahl Null** ($00\dots0$) ermöglicht und die Subtraktion durch einfache Addition realisiert werden kann25252525.
        

---

## Teil III: Reelle Zahlen, Farben und Bilder

11. **Frage:** Erläutern Sie, warum für die Darstellung von **sehr großen und sehr kleinen Zahlen** die **Festkommadarstellung** ungeeignet ist und welche **Grundidee** zur Lösung dieses Problems in der **Exponentialdarstellung** verfolgt wird.
    
    - **Antwort:** **Festkommadarstellung** ist ungeeignet, da zur Darstellung extrem großer und extrem kleiner Zahlen (z.B. physikalischer Konstanten) **sehr viele Bits** benötigt würden (z.B. 194 Bit), was eine **große Verschwendung** wäre26. Die **relative Genauigkeit** ist wichtiger als die absolute27.
        
    - Die **Grundidee der Exponentialdarstellung** (Gleitkommazahl) ist die **Trennung** der **signifikanten Stellen (Mantisse)** und der **Größenordnung (Exponent)**28. Dies ermöglicht es, mit einer gegebenen Anzahl von Ziffern einen **größeren Zahlenbereich** abzudecken29.
        
    - (English: **MARKED AS UNANSWERED**)
        
12. **Frage:** Beschreiben Sie die **drei Komponenten** einer **Gleitkommazahl** im Binärsystem nach dem IEEE 754 Standard. Was ist das "**hidden bit**" bei normalisierten Gleitkommazahlen?
    
    - **Antwort:** Die drei Komponenten sind: **Vorzeichen** ($S$), **Mantisse** ($M$), und **Exponent** ($E$)30.
        
        - **Formel:** $(-1)^S \times \text{Mantisse} \times 2^{\text{Exponent}}$31.
            
        - Das **"hidden bit"** (verstecktes Bit) ist die Ziffer **1** links der Dezimalstelle bei **normalisierten Gleitkommazahlen** ($1.0 \le M < 2.0$)32. Da diese führende 1 redundant (immer vorhanden) ist, wird sie **nicht gespeichert**, um Platz für eine weitere Mantissenziffer zu schaffen33333333.
            
    - (English: **MARKED AS UNANSWERED**)
        
13. **Frage:** Wie wird eine **Farbe** im **RGB-Farbmodell** definiert? Erklären Sie das **physikalische Prinzip** der **additiven Farbmischung** und nennen Sie ein typisches Beispiel für deren Anwendung.
    
    - **Antwort:** Eine Farbe wird durch ein **Zahlentripel** $(r, g, b)$ definiert, wobei jede Zahl den Anteil der Grundfarben **Rot, Grün und Blau** angibt (oft im Bereich [0...255])34.
        
    - Das **Prinzip der additiven Farbmischung** tritt auf, wenn das **Licht von mehreren Lichtquellen** verschiedener Farbe **zusammenkommt** und deren Farbanteile **addiert** werden (z.B. **Rot + Grün + Blau = Weiß**)35353535.
        
    - **Beispiel:** Die Farbwahrnehmung bei einem **Farbfernseher oder Monitor**, zusammengesetzt aus den rot, grün und blau leuchtenden Pixeln36.
        
    - (English: **MARKED AS UNANSWERED**)
        
14. **Frage:** Erklären Sie die **Codierung von Bildern** in einem Computerspeicher. Welche Rolle spielen "**Pixel**" und "**Metadaten**" (im Header der Datei) in diesem Prozess?
    
    - **Antwort:** Bilder sind im Prinzip **Matrizen/Tabellen aus Farbwerten**37. Jeder Farbwert bezeichnet einen **Pixel** (Picture Element)38. Da Computerspeicher eindimensional sind, werden die Farbwerte der Pixel **hintereinander** im Speicher abgelegt39393939.
        
    - **Metadaten** (im Header der Datei) enthalten **zusätzliche Informationen** wie die **Anzahl der Pixel pro Zeile** (Breite des Bildes) 40404040, das Dateiformat (z.B. JPEG, GIF) und weitere Angaben zur Entstehung41. Diese Metadaten sind **essenziell**, um das Bild korrekt aus der sequentiellen Folge von Farbwerten **wiederherzustellen**42.
        
    - (English: **MARKED AS UNANSWERED**)
        
15. **Frage:** Grenzen Sie die Begriffe "**Pixel-Grafiken**" und "**Vektorgrafiken**" voneinander ab. Für welche Art von Bildmaterial ist jeweils die Pixel-Grafik **besonders geeignet**?
    
    - **Antwort:** **Pixel-Grafiken** (Rastergrafiken) basieren auf einer Matrix von Farbwerten/Punkten (Pixeln)43. Sie eignen sich **sehr gut für Fotos**44.
        
    - **Vektorgrafiken** basieren auf der Beschreibung des Bildes durch **geometrische Basiselemente** (Punkte, Linien, Polygone, Kurven)45. Der Hauptvorteil ist, dass Vektorgrafiken **leichter an neue Größen angepasst** werden können46.
        
    - (English: **MARKED AS UNANSWERED**)Teil I: Bits, Bytes und Zahlensysteme