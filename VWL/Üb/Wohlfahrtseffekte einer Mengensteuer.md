### 5.1. Das unregulierte Marktgleichgewicht
* **Nachfragefunktion:** $p = 200 - q_D$
* **Angebotsfunktion:** $p = 80 + 2q_S$

#### Schritt 1: Berechnung der Gleichgewichtsmenge ($q^*$)
Im Marktgleichgewicht gilt $q_D = q_S = q^*$:
$$200 - q^* = 80 + 2q^* \implies 120 = 3q^* \implies q^* = \mathbf{40}$$

#### Schritt 2: Berechnung des Gleichgewichtspreises ($p^*$)
Einsetzen von $q^* = 40$ in die Nachfragefunktion:
$$p^* = 200 - 40 = \mathbf{160\text{ €}}$$

#### Schritt 3: Bestimmung der Renten im unregulierten Markt
Da die Funktionen linear sind, werden Konsumenten- und Produzentenrente als Dreiecksflächen ($\frac{\text{Basis} \cdot \text{Höhe}}{2}$) berechnet:
* **Konsumentenrente ($CS$):** Maximaler Preis ($p(0) = 200$) minus Gleichgewichtspreis ($160$).
  $$CS = \frac{40 \cdot (200 - 160)}{2} = \frac{40 \cdot 40}{2} = \mathbf{800}$$
* **Produzentenrente ($PS$):** Gleichgewichtspreis ($160$) minus Mindestangebotspreis ($p(0) = 80$).
  $$PS = \frac{40 \cdot (160 - 80)}{2} = \frac{40 \cdot 80}{2} = \mathbf{1.600}$$
* **Gesamtwohlfahrt ($W_{\text{gesamt}}$):** $CS + PS = 800 + 1.600 = \mathbf{2.400}$

---

### 5.2. Marktgleichgewicht unter Einführung einer Mengensteuer ($t = 30$)
Die Steuer erhöht die Grenzkosten der Produzenten um den Betrag $t$, wodurch sich die Angebotskurve vertikal nach oben verschiebt.

#### Schritt 1: Aufstellen der modifizierten Angebotsfunktion
$$p_t = 80 + 2q_S + 30 \implies p_t = 110 + 2q_S$$

#### Schritt 2: Berechnung der neuen Gleichgewichtsmenge ($q_t$)
$$200 - q_t = 110 + 2q_t \implies 90 = 3q_t \implies q_t = \mathbf{30}$$

#### Schritt 3: Berechnung des Bruttopreises für Konsumenten ($p_t$)
Einsetzen von $q_t = 30$ in die Nachfragefunktion:
$$p_t = 200 - 30 = \mathbf{170\text{ €}}$$

#### Schritt 4: Berechnung des Nettopreises für Produzenten ($p_nt$)
Der vom Produzenten effektiv einbehaltene Preis nach Abzug der Steuer:
$$p_nt = p_t - t = 170 - 30 = \mathbf{140\text{ €}}$$

---

### 5.3. Wohlfahrtsanalyse des Steuereingriffs

Durch die Mengensteuer kommt es zu einer Umverteilung der Renten sowie einer Vernichtung von ökonomischer Wohlfahrt:

* **Neue Konsumentenrente ($CS_t$):**
  $$CS_t = \frac{30 \cdot (200 - 170)}{2} = \frac{30 \cdot 30}{2} = \mathbf{450}$$
  *Verlust an $CS$: $-350$*

* **Neue Produzentenrente ($PS_t$):**
  $$PS_t = \frac{30 \cdot (140 - 80)}{2} = \frac{30 \cdot 60}{2} = \mathbf{900}$$
  *Verlust an $PS$: $-700$*

* **Staatseinnahmen ($G$):** Steuer pro Einheit multipliziert mit der gehandelten Menge.
  $$G = t \cdot q_t = 30 \cdot 30 = \mathbf{900\text{ €}}$$

* **Wohlfahrtsverlust (Deadweight Loss - $DWL$):** Das Harberger-Dreieck misst die verloren gegangene Wohlfahrt der nicht mehr realisierten Markttransaktionen.
  $$DWL = \frac{(q^* - q_t) \cdot t}{2} = \frac{(40 - 30) \cdot 30}{2} = \frac{10 \cdot 30}{2} = \mathbf{150}$$

> **Kontrollrechnung über die Gesamtwohlfahrt:**
> $W_{\text{neu}} = CS_t + PS_t + G = 450 + 900 + 900 = 2.250$
> $DWL = W_{\text{alt}} - W_{\text{neu}} = 2.400 - 2.250 = \mathbf{150}$ (Konsistent)