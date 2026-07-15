
> [!INFO] Eckdaten & Kernmetriken
> * **Prüfungsdauer:** 90 Minuten
> * **Gesamtpunktzahl:** 104 Punkte
> * **Fokus:** Formale Marktmechanismen, mathematische Optimierung (Lagrange), Wohlfahrtsanalyse
> * **Grundregel:** Es werden ausschließlich die in der Vorlesung behandelten Lösungsmethoden und Inhalte bewertet.

---

## 1. Themenschwerpunkte & Gewichtung

### A. Marktgleichgewicht, Eingriffe & Wohlfahrt (38% / 40 Punkte)

* **Unreguliertes Gleichgewicht:** Gleichsetzen von Nachfrage und Angebot ($q_D = q_S$ oder $p_D = p_S$), um den gleichgewichtigen Preis $p^*$ und die Menge $q^*$ zu bestimmen.
* **Wohlfahrtsberechnung:**
  * **Konsumentenrente ($CS$):** $\frac{(\text{Prohibitivpreis} - p^*) \cdot q^*}{2}$ oder über das Integral $\int_{0}^{q^*} [D(q) - p^*] dq$
  * **Produzentenrente ($PS$):** $\frac{(p^* - \text{Mindestangebotspreis}) \cdot q^*}{2}$ oder über das Integral $\int_{0}^{q^*} [p^* - S(q)] dq$
* **Mengensteuer ($t$):** Verschiebt die Angebotskurve nach oben auf $p = S(q) + t$.
  * **Bruttopreis ($p_D$):** Der vom Konsumenten gezahlte Preis.
  * **Nettopreis ($p_S$):** Der dem Produzenten verbleibende Preis ($p_D - t$).
  * **Steuereinnahmen ($G$):** $t \cdot q_t$
  * **Wohlfahrtsverlust ($DWL$):** Der Nettoverlust der aggregierten Gesamurente.
* **Höchstpreise ($p_{\max}$):** Nur bindend, wenn $p_{\max} < p^*$. Führt zu einem **Nachfrageüberhang** ($q_D - q_S > 0$). Die gehandelte Menge wird durch die kurze Marktseite ($q_S$) bestimmt.
  * *Wohlfahrtseffekte:* Produzenten verlieren $-a - c$; Konsumenten verändern sich um $+a - b$.

### B. Optimierung unter Nebenbedingungen & Mikroökonomische Theorie (31% / 32 Punkte)

* **Konsumententheorie (Aufgabe 2):** Nutzenmaximierung unter Einhaltung der Budgetrestriktion ($I = p_1 q_1 + p_2 q_2$).
  $$\mathcal{L}(q_1, q_2, \lambda) = U(q_1, q_2) + \lambda(I - p_1 q_1 - p_2 q_2)$$
  * *Kernbedingung:* $\text{GRS} = \frac{MU_1}{MU_2} = \frac{p_1}{p_2}$ (Grenzrate der Substitution entspricht dem Preisverhältnis).
* **Produktionstheorie (Aufgabe 4):** Kostenminimierung unter der Nebenbedingung eines vorgegebenen Produktionsniveaus ($f(L, K) = \bar{q}$) bei gegebenen Lohnsätzen ($w$) und Kapitalkosten ($r$).
  $$\mathcal{L}(L, K, \lambda) = wL + rK + \lambda(\bar{q} - f(L, K))$$
  * *Kernbedingung:* $\text{GRTS} = \frac{MP_L}{MP_K} = \frac{w}{r}$ (Grenzrate der technischen Substitution entspricht dem Faktorpreisverhältnis).
* **Skalenerträge (Returns to Scale):** Bestimmung über die Summe der Cobb-Douglas-Exponenten ($\alpha + \beta$).
  * $\alpha + \beta > 1$: Steigende Skalenerträge ($\text{irs}$)
  * $\alpha + \beta = 1$: Konstante Skalenerträge ($\text{crs}$)
  * $\alpha + \beta < 1$: Sinkende Skalenerträge ($\text{drs}$)

### C. Internationaler Handel (14% / 15 Punkte)

* **Freihandels-Szenario:** Vergleich zwischen Autarkie und offener Volkswirtschaft. Liegt der Weltmarktpreis ($p_W$) unter dem inländischen Gleichgewichtspreis ($p^*$), importiert das Land die Menge $q_D - q_S$.
* **Zölle vs. Quoten:** Ein Importzoll ($t$) erhöht den Inlandspreis auf $p_0 = p_W + t$, verringert die Importe und generiert staatliche Zolleinnahmen (Fläche $d$).
* **Wirtschaftspolitische Empfehlung:** Eine Quote ist einem Zoll ökonomisch strikt unterlegen. Die Fläche $d$ fließt hierbei als Knappheitsrente an ausländische Produzenten ab, anstatt vom inländischen Staat abgeschöpft zu werden. Dies verschlechtert die nationale Gesamtwohlfahrt zusätzlich.

### D. Grundlagenkonzepte & Elastizitäten (16% / 17 Punkte)

* **Preiselastizität der Nachfrage ($\epsilon$):** Misst die Stärke der Mengenreaktion auf Preisänderungen.
  $$\epsilon = \frac{\partial q}{\partial p} \cdot \frac{p}{q}$$
  * $|\epsilon| > 1$: Elastisch; $|\epsilon| < 1$: Unelastisch.
* **Erfolgsbegriffe:**
  * **Buchhalterischer Gewinn** = $\text{Erlös} - \text{Explizite Kosten}$
  * **Ökonomischer Gewinn** = $\text{Erlös} - (\text{Explizite Kosten} + \text{Implizite Opportunitätskosten})$
  * Langfristig führt vollständiger Wettbewerb zu einem ökonomischen Gewinn von null (**Nullgewinn**).

---

## 2. Formelsammlung & Mathematische Bedingungen

| Mathematisches Ziel | Kernbedingung / Berechnungsformel | Schlüsselvariablen |
| :--- | :--- | :--- |
| **Markträumung** | $q_D(p) = q_S(p)$ | Marktpreis $p^*$, Menge $q^*$ |
| **Preiselastizität** | $\epsilon = q'(p) \cdot \frac{p}{q}$ | Punktelastizität |
| **Konsumoptimum** | $\frac{\partial U / \partial q_1}{\partial U / \partial q_2} = \frac{p_1}{p_2}$ | Grenznutzen ($MU$), Güterpreise |
| **Produktionsoptimum** | $\frac{\partial f / \partial L}{\partial f / \partial K} = \frac{w}{r}$ | Grenzprodukt ($MP$), Faktorpreise |
| **Wohlfahrtsverlust (Steuer)** | $DWL = \frac{t \cdot (q^* - q_t)}{2}$ | Steuersatz $t$, Mengendifferenz |