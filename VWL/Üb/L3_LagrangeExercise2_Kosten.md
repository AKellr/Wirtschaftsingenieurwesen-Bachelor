### 1. Theoretischer Rahmen (Kostenminimierung)
* **Zielsetzung:** Ein Unternehmen möchte eine vorgegebene Outputmenge ($\bar{q}$) zu den geringstmöglichen Gesamtkosten produzieren (duales Problem zur Nutzen-/Gewinnmaximierung).
* **Ökonomische Variablen:**
  * $L$: Menge des Produktionsfaktors Arbeit (Labor).
  * $K$: Menge des Produktionsfaktors Kapital (Capital).
  * $w$: Faktorpreis für Arbeit (Lohnsatz).
  * $r$: Faktorpreis für Kapital (Zinssatz/Mietpreis).
* **Der Lagrange-Multiplikator ($\lambda$):** Repräsentiert ökonomisch den **Schattenpreis** der Restriktion. Im Optimum entspricht $\lambda$ exakt den **Grenzkosten** ($MC$) der Produktion. Er gibt an, um wie viele Geldeinheiten die Gesamtkosten näherungsweise steigen, wenn der Output um eine marginale Einheit erhöht wird.

---

### 2. Mathematischer Ansatz (Lagrange-Verfahren)
Die Struktur der Lagrange-Funktion $\mathcal{L}$ bei der Kostenminimierung lautet:

$$\mathcal{L}(L, K, \lambda) = \text{Zielfunktion (Kosten)} + \lambda \cdot \left[\text{Nebenbedingung (Nullform)}\right]$$

$$\mathcal{L}(L, K, \lambda) = w \cdot L + r \cdot K + \lambda \cdot \left[\bar{q} - f(L, K)\right]$$

#### Bedingungen erster Ordnung (First-Order Conditions, FOC):
Zur Bestimmung des Extremums werden die partiellen Ableitungen nach allen drei Variablen gebildet und gleich null gesetzt:
1. $\frac{\partial \mathcal{L}}{\partial L} = w - \lambda \cdot \frac{\partial f}{\partial L} = 0 \implies w = \lambda \cdot MP_L$
2. $\frac{\partial \mathcal{L}}{\partial K} = r - \lambda \cdot \frac{\partial f}{\partial K} = 0 \implies r = \lambda \cdot MP_K$
3. $\frac{\partial \mathcal{L}}{\partial \lambda} = \bar{q} - f(L, K) = 0$

#### Minimierungskriterium (Marginale Rate der technischen Substitution):
Durch das Teilen von Gleichung (1) durch Gleichung (2) eliminiert sich $\lambda$, und es entsteht die Optimalitätsbedingung (Tangentialpunkt von Isokoste und Isoquante):

$$\frac{w}{r} = \frac{MP_L}{MP_K} = MRTS$$

---

### 3. Konkretes Berechnungsbeispiel

#### Gegebene Parameter:
* Produktionsfunktion: $q = 5\sqrt{LK} = 5 L^{0,5} K^{0,5}$
* Faktorpreise: $w = 2$, $r = 8$
* Restriktion (Outputziel): $\bar{q} = 40$

#### Schritt-für-Schritt-Lösung:

1. **Lagrange-Funktion aufstellen:**
   $$\mathcal{L}(L, K, \lambda) = 2L + 8K + \lambda(40 - 5L^{0,5}K^{0,5})$$

2. **Partielle Ableitungen (FOC):**
   * $\frac{\partial \mathcal{L}}{\partial L} = 2 - 2,5\lambda L^{-0,5}K^{0,5} = 0 \implies 2 = 2,5\lambda L^{-0,5}K^{0,5}$
   * $\frac{\partial \mathcal{L}}{\partial K} = 8 - 2,5\lambda L^{0,5}K^{-0,5} = 0 \implies 8 = 2,5\lambda L^{0,5}K^{-0,5}$
   * $\frac{\partial \mathcal{L}}{\partial \lambda} = 40 - 5L^{0,5}K^{0,5} = 0$

3. **Faktoreinsatzverhältnis bestimmen (Gleichung 1 / Gleichung 2):**
   $$\frac{2}{8} = \frac{2,5\lambda L^{-0,5}K^{0,5}}{2,5\lambda L^{0,5}K^{-0,5}} \implies 0,25 = \frac{K}{L} \implies K = 0,25L$$

4. **Einsetzen in die Nebenbedingung:**
   $$40 = 5 \cdot \sqrt{L \cdot (0,25L)} \implies 40 = 5 \cdot \sqrt{0,25L^2}$$
   $$40 = 5 \cdot 0,5L \implies 40 = 2,5L \implies \mathbf{L = 16}$$

5. **Optimales Kapital berechnen:**
   $$K = 0,25 \cdot 16 \implies \mathbf{K = 4}$$

6. **Lagrange-Multiplikator ($\lambda$) berechnen:**
   $$2 = 2,5 \cdot \lambda \cdot (16)^{-0,5} \cdot (4)^{0,5} \implies 2 = 2,5 \cdot \lambda \cdot \frac{1}{4} \cdot 2$$
   $$2 = 1,25 \cdot \lambda \implies \lambda = \frac{2}{1,25} \implies \mathbf{\lambda = 1,6}$$

#### Ergebnismatrix:
| Variable | Optimaler Wert | Ökonomische Bedeutung |
| :--- | :--- | :--- |
| **Arbeit ($L^*$)** | $16$ Einheiten | Kostenminimierender Einsatz des Faktors Arbeit. |
| **Kapital ($K^*$)** | $4$ Einheiten | Kostenminimierender Einsatz des Faktors Kapital. |
| **Schattenpreis ($\lambda^*$)** | $1,6$ Geldeinheiten | Grenzkosten für eine zusätzliche Outputeinheit ($MC = 1,6$). |
| **Gesamtkosten ($C_{min}$)** | $64$ Geldeinheiten | Minimale Kosten zur Produktion von $40$ Einheiten ($2 \cdot 16 + 8 \cdot 4$). |