### 1. Mathematische Grundlagen & Steuereffekte (Folie 36)
* **Ausgangsszenario (Marktgleichgewicht):**
  * Nachfragefunktion: $p(q) = 120 - q$
  * Angebotsfunktion: $p(q) = 3q + 20$
  * **Gleichgewicht ohne Steuer ($q^*, p^*$):** $q^* = 25$, $p^* = 95$

* **Szenario: Mengensteuer $t = 20$ auf Produzenten**
  * Neue Angebotsfunktion: $p_S = 3q + 20 + 20 = 3q + 40$
  * Neues Marktgleichgewicht: $q = 20$
  * Konsumentenpreis (Brutto): $p_D = 100$
  * Produzentenpreis (Netto): $p_S = 80$
  * Staatseinnahmen ($G$): $t \cdot q = 20 \cdot 20 = 400$

---

### 2. Rentenberechnung (Marktphase vs. Steuerphase)

Die Wohlfahrtsmaße lassen sich sowohl geometrisch über die Dreiecksformel als auch über bestimmte Integrale bestimmen:

$$\text{CS} = \int_{0}^{q^*} (p_D(q) - p) \,dq \quad \text{und} \quad \text{PS} = \int_{0}^{q^*} (p - p_S(q)) \,dq$$

| Wohlfahrtskomponente | Ohne Steuer ($q^*=25$) | Mit Steuer ($q_{\text{Steuer}}=20$) |
| :--- | :---: | :---: |
| **Konsumentenrente (CS)** | $312,5$ | $200$ |
| **Produzentenrente (PS)** | $937,5$ | $600$ |
| **Staatseinnahmen (G)** | $0$ | $400$ |
| **Gesamtwohlfahrt (W)** | $1250$ | $1200$ |

---

### 3. Wohlfahrtsanalyse & Verlustbestimmung
Durch die Steuerallokation entsteht ein Wohlfahrtsverlust (Deadweight Loss), da die Marktmenge unter das gesellschaftliche Optimum sinkt.

* **Nettowohlfahrtsverlust (Deadweight Loss, DWL):**
  $$\Delta W = \text{W}_{\text{Ausgang}} - (\text{CS}_{\text{Steuer}} + \text{PS}_{\text{Steuer}} + G)$$
  $$\Delta W = \frac{1}{2} \cdot t \cdot (q^* - q_{\text{Steuer}})$$
  $$\Delta W = \frac{1}{2} \cdot 20 \cdot (25 - 20) = 50$$