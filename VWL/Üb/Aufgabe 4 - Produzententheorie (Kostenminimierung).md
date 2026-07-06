# VWL I: Mikroökonomik - Klausurvorbereitung

## 4. Kostenminimierung bei vorgegebenem Outputniveau

### 4.1. Analyse der Skalenerträge (Returns to Scale)
* **Produktionsfunktion ($f$):** $f(L,K) = 3LK$[cite: 1]
* **Skalenerträge:** Es liegen **steigende Skalenerträge** (*Increasing Returns to Scale - irs*) vor, da die Summe der Exponenten der Produktionsfaktoren größer als 1 ist ($1 + 1 = 2 > 1$)[cite: 1].
* **Ökonomische Implikation:** Ein proportionaler Zuwachs aller Inputfaktoren führt zu einem überproportionalen Zuwachs des Outputs[cite: 1]. Konkret induziert eine Steigerung des Factoreinsatzes um $1\,\%$ eine Erhöhung der Produktionsmenge um $2\,\%$[cite: 1]. Eine Verdoppelung der Inputs führt zu einer Vervierfachung des Outputs.

---

### 4.2. Analytische Bestimmung des Kostenoptimums via Lagrange

#### Gegebene Parameter
* **Faktorpreise:** Lohnsatz $w = 10$, Kapitalzins $r = 20$[cite: 1]
* **Ziel-Outputmenge ($q$):** $q = 180$[cite: 1]

#### Schritt 1: Formulierung der Output-Nebenbedingung (NB)
$$3LK = 180 \implies 180 - 3LK = 0[cite: 1]$$

#### Schritt 2: Aufstellen der Lagrange-Funktion ($\mathcal{L}$)
Bei der Kostenminimierung bildet die Kostenfunktion die Basis, ergänzt um die Nullform der Produktionsbeschränkung[cite: 1]:
$$\mathcal{L}(L, K, \lambda) = 10L + 20K + \lambda(180 - 3LK)[cite: 1]$$

#### Schritt 3: Bedingungen erster Ordnung (FOC)
$$\text{(I)} \quad \frac{\partial \mathcal{L}}{\partial L} = 10 - 3\lambda K \stackrel{!}{=} 0 \implies 10 = 3\lambda K[cite: 1]$$
$$\text{(II)} \quad \frac{\partial \mathcal{L}}{\partial K} = 20 - 3\lambda L \stackrel{!}{=} 0 \implies 20 = 3\lambda L[cite: 1]$$
$$\text{(III)} \quad \frac{\partial \mathcal{L}}{\partial \lambda} = 180 - 3LK \stackrel{!}{=} 0[cite: 1]$$

#### Schritt 4: Bestimmung der Optimalitätsbedingung (Faktorsubstitutionsverhältnis)
Division von $\text{(I)}$ durch $\text{(II)}$ eliminiert den Lagrange-Multiplikator $\lambda$ und setzt das Faktorpreisverhältnis gleich der Grenzrate der technischen Substitution (GRTS)[cite: 1]:
$$\frac{10}{20} = \frac{3\lambda K}{3\lambda L} \implies \frac{1}{2} = \frac{K}{L} \implies L = 2K[cite: 1]$$

#### Schritt 5: Substitution in die Produktionsfunktion $\text{(III)}$
$$3 \cdot (2K) \cdot K = 180 \implies 6K^2 = 180[cite: 1]$$
$$K^2 = 30 \implies K^* = \sqrt{30} \approx \mathbf{5,48}[cite: 1]$$

#### Schritt 6: Berechnung der optimalen Menge des Faktors Arbeit ($L^*$)
$$L^* = 2 \cdot 5,4772 \approx \mathbf{10,96}[cite: 1]$$

#### Schritt 7: Berechnung des optimalen Lagrange-Multiplikators $\lambda^*$
Nutze umgestellte Gleichung $\text{(I)}$:
$$\lambda^* = \frac{10}{3K^*} = \frac{10}{3 \cdot 5,48} \approx \mathbf{0,61}[cite: 1]$$

---

### 4.3. Ökonomische Gesamtkosten im Optimum

Die minimalen Gesamtkosten ($C^*$) zur Realisierung des vorgegebenen Outputniveaus von 180 Einheiten ergeben sich durch Einsetzen der optimalen Factorkombinationen in die Isokostengerade[cite: 1]:

$$C^* = wL^* + rK^*[cite: 1]$$
$$C^* = 10 \cdot 10,96 + 20 \cdot 5,48 = 109,60 + 109,60 = \mathbf{219,20\text{ €}}[cite: 1]$$