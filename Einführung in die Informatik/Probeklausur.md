[[GDM]]
## Block 1

**1. Was ist Informatik?** 
- Informatik ist die Wissenschaft von der systematischen Verarbeitung von Informationen, besonders der automatischen Verarbeitung mit Hilfe von Computern

**2. Was ist der Unterschied zwischen einem Anwender und einem Entwickler?**
 - Der **Entwickler** befasst sich mit der Lösung von Probleme durch Analyse, Entwurf von Algorithmen und deren Codierung in Programme.
 - Der **Anwender** nutzt die fertigen Systeme zur Lösung seiner Aufgaben, ohne zwingend die inneren Abläufe zu kennen.

**3. Was ist ein Algorithmus?**
- Ein Algorithmus ist ein Verfahren zur schrittweisen Lösung einer Klasse von Probleme. Es ist eine intuitive Rechenvorschrift und bildet die Grundlage jeglicher maschineller Informationsvorbereitung.

**4. Nennen und erläutern Sie typische Eigenschaften eines Algorithmus.**
1. Deterministisch: die Abfolge der Schritte ist für das gleiche Problem immer gleich
2. Terminiert: es kommt in endlicher Zeit zu einem Ende
3. Resultat: er produziert immer das gewünschte Resultat
4. Präzise Darstellung: die Daten und die Verarbeitungsvorschrift müssen unmissverständlich aufgeschrieben sein
5. Effektivität: jeder Schritt muss ausführbar sein

**5. Nennen und beschreiben Sie zwei grundsätzliche Bestandteile / Komponenten eines Algorithmus.**
1. Daten: die Objekte, die verarbeitet werden
2. Anweisungen: die präzise Beschreibung, was mit den Daten geschehen soll.

**6. Was ist der Unterschied zwischen Programm und Prozess?**
- Ein Programm ist die Implementierung eines Algorithmus (der ruhende Code im speicher)
- Ein Prozess ist ein ausgeführtes Programm

**7. Was ist der Unterschied zwischen Information und Daten? Nutzen Sie ein Beispiel.**
- Information ist der abstrakte Gehalt oder die Bedeutung einer Nachricht
- Daten sind die äußere Form der Darstellung, die nötig ist, um Information zu speichern oder zu verarbeiten
- Beispiel: Die Information "Es regnet" kann durch verschiedene Daten repräsentiert werden: das deutsche Wort "Es regnet" oder das russische "Дождь идёт". Die Information (Bedeutung) bleibt gleich.

**8. Was ist der Unterschied zwischen Algorithmus und Programm?**
- Der Algorithmus ist die abstrakte Definition einer Vorgehensweise zur Problemlösung
- Das Programm ist die konkrete Umsetzung dieses Algorithmus in einer bestimmten Sprache, die von einem Computer ausgeführt werden.

**9. Wie nennt man den Übergang von Algorithmus zu einem Programm?**
- Dieser Schritt nennt sich Codierung

**10. Nennen Sie vier Teilgebiete der Informatik.**
1. Technische Informatik
2. Praktische Informatik
3. Theoretische Informatik
4. Angewandte Informatik

## Block 2

**11. In welchem Jahrzehnt wurde der erste elektrische Computer gebaut?**
- In den 1940er Jahren

**12. Wie haben sich Computer im Laufe der Geschichte verändert (1 bis 2 Sätze)?**
- Computer haben sich von riesigen, tonnenschweren Anlagen zu winzigen, leistungsstarken Geräten entwickelt. Dabei stieg die Rechenleistung und Speicherkapazität exponentiell an, während Größe, Kosten und Energieverbrauch massiv sanken.

**13. Was ist der Unterschied zwischen Prozessor und Speicher? Sind beide für einen Computer wichtig? Was sind deren wichtigste Aufgaben?**
- Beide sind essenziell
	- Prozessor: führt Programme aus, verarbeitet Eingaben und generiert Ausgaben 
	- Speicher: speichert Daten und Programme dauerhaft oder temporär

**14. Was versteht man unter Moore's Law?**
- Moore's Law besagt als empirische Regelmäßigkeit, dass sich die Anzahl der Transistoren auf integrierten Schaltkreisen (und damit die Komplexität bei gleichen Kosten) etwa alle zwei Jahre verdoppelt.

**15. Man unterscheidet drei Ebenen von Programmiersprachen. Welche sind das?**
1. Maschinensprache: Binärstrings, die der Prozessor direkt versteht
2. Assembler: mnemonische Codes, die Maschinenbefehle lesbarer machen
3. Höhere Programmiersprache: abstrakte Sprachen (Python, C), die für Menschen verständlich sind und von Compilern übersetzt werden

**16. Nennen Sie Ursachen für Fehler in der Softwareentwicklung.**
- Managmentfehler und fehlende Kommunikation
- Schlechte Spezifikation der Anforderungen
- Unzureichende Tests
- Wiederverwendung ungeeigneter Software
- Wachsende Komplexität der Software

**17. Erläutern Sie den Unterschied zwischen Information und Repräsentation. Welche Ebenen? Welche Übergänge?**
- Information: der abstrakte Gehalt oder die Bedeutung einer Nachricht (semantische Ebene)
- Repräsentation: die äußere, konkrete Form der Darstellung, z.B. als Zeichenfolge (syntaktische Ebene)
- Übergänge: 
	- Repräsentation $\rightarrow$ Information: **Interpretation**
	- Information $\rightarrow$ Repräsentation: **Kodierung**

**18. Wenn man Information in Daten umwandelt, nennt man das ...**
- Kodierung

**19. Was ist ein Bit? Wie kann die Information gespeichert werden?**
- Ein Bit ist die kleinstmögliche Informationseinheit und kann zwei Zustände annehmen (0 oder 1, Ja oder Nein)
	- Speicherung: physikalisch durch Ladung (geladen/ungeladen), Spannung, Magnetisierung oder Licht

**20. Was ist ein Byte?**
- Eine Zussamenhang von 8 Bit. Es ist die kleinste adressierbare Einheit im Speicher und kann Werte zwischen 0 und 255 darstellen

**21. Was sind die wichtigsten Komponenten eines Computers? Was sind deren Aufgaben?**
1. CPU (Prozessor): Verarbeitung von Daten und Befehlen
2. Speicher (RAM): Speicherung von Daten/Programmen
3. I/O (Eingabe/Ausgabe): Kommunikation mit der Außenwelt (Monitor, Tastatur)
4. Bus-System: Verbindung der Komponenten zum Datentransport

**22. Was unterscheidet die Harvard-Architektur von der Zuse Architektur?**
- Zuse Architektur: das Programm liegt extern auf einem Lochstreifen, während die Daten in einem internen Speicher liegen.
- Harvard Architektur: besitzt zwei getrennte interne Speicherbereiche mit eigenen Bussen: einen für Befehle (Programmspeicher) und einen für Daten (Datenspeicher)
- Gemeinsamkeit: beide trennen Daten und Befehle (im Gegensatz zu Von Neumann), aber Harvard intergriert beides in adressierbare Speicherbausteine

**23. Beschreiben Sie die Von-Neumann-Architektur.**
- Bei der Von Neumann Architektur liegen Programme (Befehle) und Daten im selben gemeinsamen Speicher. Es gibt ein gemeinsames Bus-System für beides. Dies ermöglicht flexible Speicheraufteilung, führt aber zum "Von Neumann Flaschenhals", da Befehle und Daten nicht gleichzeitig geladen werden können.