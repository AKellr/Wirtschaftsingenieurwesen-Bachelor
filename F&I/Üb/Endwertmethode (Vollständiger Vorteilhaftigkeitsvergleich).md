### 1. Theoretischer Hintergrund
Die **Endwertmethode** (auch Vermögensendwertmethode) zählt zu den dynamischen Verfahren der Investitionsrechnung. Sie ermittelt den Vermögenszuwachs am Ende eines festgelegten Planungshorizonts ($t_n$), der über eine geforderte Mindestverzinsung (Kalkulationszinssatz $i$) hinausgeht.

*   **Zahlungszeitpunkte:** Einzahlungen, die am Ende einer Periode $t$ anfallen, werden über die verbleibende Restlaufzeit bis zum Planungshorizont aufgezinst: $(1+i)^{n-t}$.
*   **Zahlungen im Zieljahr ($t_n$):** Zahlungen, die exakt am Ende des Planungshorizonts anfallen, werden nicht mehr aufgezinst ($t=n$), da sie bereits im Zielzeitpunkt liegen.
*   **Differenzinvestition:** Bei unterschiedlichen Nutzungsdauern der Investitionsobjekte wird durch die implizite Aufzinsung des Endwerts der kürzeren Investition bis zum gemeinsamen Planungshorizont (meist das kleinste gemeinsame Vielfache) ein vollständiger Vergleich ermöglicht.

---

### 2. Falldaten & Parameter
Basierend auf den Angaben aus `image_fa8ad7.png`:
*   **Kalkulationszinssatz ($i$):** 12% p.a.
*   **Planungshorizont ($n$):** 4 Jahre ($t_4$)

| Parameter | Objekt A | Objekt B |
| :--- | :--- | :--- |
| **Nutzungsdauer** | 4 Jahre | 2 Jahre |
| **Anschaffungskosten ($t_0$)** | -300.000 EUR | -150.000 EUR |
| **Jährliche Überschüsse** | +120.000 EUR ($t_1$ bis $t_4$) | +115.000 EUR ($t_1$ bis $t_2$) |
| **Liquidationserlös** | 0 EUR | 0 EUR |

---

### 3. Berechnung der Endwerte ($EW$ in $t_4$)

#### Objekt A (Nutzungsdauer = Planungshorizont)
*   **Aufgezinste Anschaffungskosten ($t_0 \rightarrow t_4$):**
    $$-300.000 \text{ EUR} \cdot 1,12^4 = -472.055,81 \text{ EUR}$$
*   **Rentenendwert der Einzahlungen ($t_1$ bis $t_4 \rightarrow t_4$):**
    $$120.000 \text{ EUR} \cdot \frac{1,12^4 - 1}{0,12} = +573.519,36 \text{ EUR}$$
*   **Gesamtendwert Objekt A:**
    $$EW_A = -472.055,81 \text{ EUR} + 573.519,36 \text{ EUR} = \mathbf{101.463,55 \text{ EUR}}$$

#### Objekt B (Aufzinsung über den Endwert in $t_2$)
*   **Schritt 1: Endwert in $t_2$ ermitteln:**
    *   Anschaffungskosten ($t_0 \rightarrow t_2$): $-150.000 \text{ EUR} \cdot 1,12^2 = -188.160,00 \text{ EUR}$
    *   Einzahlung $t_1$ ($t_1 \rightarrow t_2$): $+115.000 \text{ EUR} \cdot 1,12^1 = +128.800,00 \text{ EUR}$
    *   Einzahlung $t_2$ (keine Aufzinsung): $+115.000,00 \text{ EUR}$
    *   $EW_{B, t2} = -188.160,00 \text{ EUR} + 128.800,00 \text{ EUR} + 115.000,00 \text{ EUR} = 55.640,00 \text{ EUR}$
*   **Schritt 2: Aufzinsung zum Planungshorizont ($t_2 \rightarrow t_4$):**
    $$EW_B = 55.640,00 \text{ EUR} \cdot 1,12^2 = \mathbf{69.794,82 \text{ EUR}}$$

---

### 4. Entscheidung / Vorteilhaftigkeitsvergleich
Der vollständige Vergleich im gemeinsamen Zieljahr $t_4$ zeigt:

$$EW_A \ (101.463,55 \text{ EUR}) > EW_B \ (69.794,82 \text{ EUR})$$

**Fazit:** Beide Investitionsobjekte sind absolut vorteilhaft, da ihre Endwerte größer als Null sind. Im relativen Vergleich ist **Objekt A vorzuziehen**, da es den höheren Vermögensendwert am Ende des Planungshorizonts generiert.