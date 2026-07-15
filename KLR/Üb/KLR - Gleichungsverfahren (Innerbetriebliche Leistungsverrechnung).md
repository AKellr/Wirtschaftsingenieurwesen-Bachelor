### 1. Theoretischer Hintergrund & Relevanz
Das **Gleichungsverfahren** (auch *mathematisches Verfahren* oder *Simultanverfahren*) ist das exakteste Verfahren der **Innerbetrieblichen Leistungsverrechnung (ILV)** im Rahmen der Kostenstellenrechnung. 

*   **Problemstellung:** Hilfskostenstellen (Vorkostenstellen wie z. B. Fuhrpark, Kantine, IT, Werkstatt) tauschen häufig gegenseitig Leistungen aus (Kostenstelle A liefert an B, und B liefert gleichzeitig an A).
*   **Die mathematische Lösung:** Während heuristische Verfahren (Anbauverfahren, Stufenleiterverfahren) diesen gegenseitigen Austausch vernachlässigen oder nur einseitig abbilden, erfasst das Gleichungsverfahren die Verflechtungen über ein **lineares Gleichungssystem (LGS)** simultan und mathematisch exakt.

---

### 2. Mathematischer Ansatz
Für jede am Leistungsaustausch beteiligte Hilfskostenstelle wird eine eigene Zeile im Gleichungssystem aufgestellt. Die logische Grundstruktur lautet stets:

$$\text{Gesamtkosten einer Stelle} = \text{Primärkosten} + \text{Sekundärkosten (erhaltene Leistungen)}$$

Formuliert als mathematischer Ansatz für $n$ Hilfskostenstellen:
$$x_i \cdot q_i = K_i + \sum_{j=1}^{n} (x_j \cdot m_{ji})$$

*   $x_i$: Gesuchter Verrechnungssatz (Kostenstellensatz) der Kostenstelle $i$
*   $q_i$: Gesamtleistung (Menge) der Kostenstelle $i$
*   $K_i$: Primäre Gemeinkosten der Kostenstelle $i$ (direkt aus dem BAB)
*   $m_{ji}$: Leistungsmenge, die von Kostenstelle $j$ an Kostenstelle $i$ geliefert wurde

---

### 3. Klausur-Schema am konkreten Berechnungsbeispiel

#### Ausgangsdaten (2 Hilfskostenstellen)
1.  **Werkstatt ($x_1$):** Primärkosten $K_1 = 10.000\ \text{€}$, Gesamtleistung $q_1 = 500\ \text{Std.}$
2.  **Stromanlage ($x_2$):** Primärkosten $K_2 = 20.000\ \text{€}$, Gesamtleistung $q_2 = 1.000\ \text{kWh}$

**Verflechtung:** 
*   Stromanlage verbraucht $50\ \text{Std.}$ aus der Werkstatt ($m_{12} = 50$)
*   Werkstatt verbraucht $100\ \text{kWh}$ vom Strom ($m_{21} = 100$)

#### Schritt 1: Gleichungssystem aufstellen
*   Gleichung I (Werkstatt): $500 \cdot x_1 = 10.000 + 100 \cdot x_2$
*   Gleichung II (Strom): $1.000 \cdot x_2 = 20.000 + 50 \cdot x_1$

#### Schritt 2: Gleichung II nach $x_2$ auflösen (durch 1.000 teilen)
$$x_2 = 20 + 0,05 \cdot x_1$$

#### Schritt 3: $x_2$ in Gleichung I einsetzen und nach $x_1$ auflösen
$$500 \cdot x_1 = 10.000 + 100 \cdot (20 + 0,05 \cdot x_1)$$
$$500 \cdot x_1 = 10.000 + 2.000 + 5 \cdot x_1 \quad \mid - 5 \cdot x_1$$
$$495 \cdot x_1 = 12.000 \quad \mid : 495$$
$$\mathbf{x_1 \approx 24,24\ \text{€ / Std.}}$$

#### Schritt 4: $x_1$ in die umgeformte Gleichung II einsetzen
$$x_2 = 20 + 0,05 \cdot 24,2424$$
$$\mathbf{x_2 \approx 21,21\ \text{€ / kWh}}$$

---

### 4. Bewertung des Verfahrens

| Vorteile | Nachteile / Klausurhinweis |
| :--- | :--- |
| **Exaktheit:** Keine mathematischen Rundungsfehler oder systematischen Ungenauigkeiten bei gegenseitigen Leistungsbeziehungen. | **Rechenaufwand:** Bei mehr als drei Kostenstellen ohne Hilfsmittel (Excel/Matrizenrechnung) manuell kaum noch in der Klausurzeit lösbar. |
| **Vollständigkeit:** Entspricht theoretisch perfekt dem informationellen Anspruch der Kostenstellenrechnung. | **Klausurfalle:** Achte darauf, im Ansatz auf der rechten Seite nur die *erhaltenen* Mengen einzutragen, nicht die abgegebenen Mengen an Endkostenstellen. |