### 1. Theoretischer Hintergrund & Kernbegriffe
Die **Break-Even-Analyse** (Gewinnschwelle) ermittelt die Absatzmenge, bei der die Umsatzerlöse exakt den Gesamtkosten entsprechen. An diesem Punkt ist der kalkulatorische Erfolg genau Null.

*   **Fixkosten ($K_f$):** Beschäftigungsunabhängige Kosten (z. B. Miete, zeitabhängige Abschreibungen), die als Block gedeckt werden müssen.
*   **Variable Stückkosten ($k_v$):** Beschäftigungsabhängige Kosten, die direkt pro Leistungseinheit anfallen (z. B. Rohstoffe).
*   **Stückdeckungsbeitrag ($db$):** Der Beitrag einer einzelnen Leistungseinheit zur Deckung der Fixkosten.
    $$db = p - k_v$$

---

### 2. Mathematische Modelle & Formelwerk

#### Einprodukt-Unternehmen
*   **Mengenmäßige Gewinnschwelle ($x_{BE}$):**
    $$x_{BE} = \frac{K_f}{p - k_v} = \frac{K_f}{db}$$
*   **Wertmäßige Gewinnschwelle ($U_{BE}$):**
    $$U_{BE} = x_{BE} \cdot p$$
*   **Zielgewinnplanung ($x_G$):** Erforderliche Absatzmenge für einen definierten Wunschgewinn ($G$).
    $$x_G = \frac{K_f + G}{db}$$

#### Mehrprodukt-Unternehmen (Sortimentsanalyse)
Bei heterogenen Produktstrukturen erfolgt die Berechnung über einen fiktiven, gewichteten **Produktkorb** basierend auf der konstanten Absatzstruktur (Mengenverhältnis).
*   **Gewichteter Deckungsbeitrag des Korbs ($db_{Korb}$):**
    $$db_{Korb} = \sum_{i=1}^{n} (v_i \cdot db_i)$$
    *wobei $v_i$ das Verhältnisgewicht des Produkts $i$ im Korb darstellt.*
*   **Break-Even-Körbe ($x_{Korb}$):**
    $$x_{Korb} = \frac{K_f}{db_{Korb}}$$
*   **Spezifische Produktmengen ($x_i$):**
    $$x_i = x_{Korb} \cdot v_i$$

---

### 3. Grafische Systematik & Kurvenverschiebungen
Das zweidimensionale Koordinatensystem stellt Geldbeträge (€) auf der Y-Achse der Ausbringungsmenge ($x$) auf der X-Achse gegenüber.

*   **Erlöskurve ($E = p \cdot x$):** Startet im Koordinatenursprung $(0,0)$ mit der Steigung $p$.
*   **Gesamtkostenkurve ($K = K_f + k_v \cdot x$):** Startet auf der Y-Achse auf Höhe des Fixkostenblocks $K_f$ mit der Steigung $k_v$.
*   **Schnittpunkt (Break-Even-Point):** Trennt die linksseitige *Verlustzone* von der rechtsseitigen *Gewinnzone*.

| Parameteränderung                   | Verschiebung Break-Even-Point       | Klausurrelevante Logik                                                 |
| :---------------------------------- | :---------------------------------- | :--------------------------------------------------------------------- |
| **Fixkosten $\uparrow$**            | Nach **rechts** (Menge $\uparrow$)  | Höhere Fixkosten erfordern mehr Absatz zur Deckung.                    |
| **Fixkosten $\downarrow$**          | Nach **links** (Menge $\downarrow$) | Die Risikoschwelle sinkt, Gewinne entstehen früher.                    |
| **Verkaufspreis $p \uparrow$**      | Nach **links** (Menge $\downarrow$) | Der $db$ steigt $\rightarrow$ Fixkosten werden schneller abgetragen.   |
| **Var. Stückkosten $k_v \uparrow$** | Nach **rechts** (Menge $\uparrow$)  | Der $db$ sinkt $\rightarrow$ es müssen mehr Einheiten verkauft werden. |