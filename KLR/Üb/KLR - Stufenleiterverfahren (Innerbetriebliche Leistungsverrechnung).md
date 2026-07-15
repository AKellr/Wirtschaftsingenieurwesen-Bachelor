### 1. Theoretischer Hintergrund & Logik
Das **Stufenleiterverfahren** (auch *Treppenverfahren* oder *sukzessives Anbauverfahren*) ist ein heuristisches (näherungsweises) Verfahren der **Innerbetrieblichen Leistungsverrechnung (ILV)**. 

*   **Problemstellung:** Wenn Hilfskostenstellen sich gegenseitig Leistungen erbringen, erfordert die exakte Berechnung ein Gleichungssystem. Das Stufenleiterverfahren umgeht diesen Rechenaufwand durch eine bewusste Vereinfachung.
*   **Die Kernregel:** Die Hilfskostenstellen werden in einer sequentiellen Reihenfolge (wie Stufen einer Treppe) nacheinander abgerechnet. Eine Kostenstelle, die bereits abgerechnet wurde, ist "geschlossen". Sie kann von nachfolgenden Kostenstellen **keine Kosten mehr empfangen**. Leistungsströme zurück nach oben werden ignoriert.

---

### 2. Festlegung der Abrechnungsreihenfolge
Um die Ungenauigkeit des Verfahrens so gering wie möglich zu halten, muss die Reihenfolge der Kostenstellen strategisch gewählt werden. In der Klausur ist die Reihenfolge entweder gegeben oder wird nach folgenden Kriterien bestimmt:

1.  **Einseitigkeitskriterium:** Die Stelle, die nur abgibt, aber nichts empfängt, kommt ganz nach oben.
2.  **Abgabekriterium (häufigste Praxis):** Die Kostenstellen werden nach der Anzahl der belieferten Kostenstellen sortiert. Die Stelle, die die meisten *anderen* Hilfskostenstellen beliefert, wird zuerst abgerechnet.
3.  **Primärkostenkriterium:** Sortierung nach der Höhe der primären Gemeinkosten.

---

### 3. Klausur-Schema am konkreten Berechnungsbeispiel

#### Ausgangsdaten (Reihenfolge: Kantine $\rightarrow$ IT-Service)
1.  **Kantine ($H_1$):** Primärkosten = $5.000\ \text{€}$, Gesamtleistung = $100\ \text{Essen}$
2.  **IT-Service ($H_2$):** Primärkosten = $10.000\ \text{€}$, Gesamtleistung = $550\ \text{Std.}$

**Leistungsverflechtung:**
*   Kantine liefert $20\ \text{Essen}$ an den IT-Service und $80\ \text{Essen}$ an Hauptkostenstellen.
*   IT-Service liefert $50\ \text{Std.}$ an die Kantine und $500\ \text{Std.}$ an Hauptkostenstellen.