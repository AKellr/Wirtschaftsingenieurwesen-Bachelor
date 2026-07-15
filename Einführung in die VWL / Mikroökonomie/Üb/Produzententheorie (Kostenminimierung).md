## 4. Kostenminimierung bei vorgegebenem Outputniveau

### 4.1. Analyse der Skalenerträge (Returns to Scale)

* **Produktionsfunktion ($f$):** $$f(L,K) = 3LK$$
* **Skalenerträge:** Es liegen **steigende Skalenerträge** (*Increasing Returns to Scale* – irs) vor, da die Summe der Exponenten der Produktionsfaktoren größer als 1 ist: 
  $$1 + 1 = 2 > 1$$

> [!NOTE] Ökonomische Implikation
> Ein proportionaler Zuwachs aller Inputfaktoren führt zu einem **überproportionalen Zuwachs** des Outputs. 
> * Eine Steigerung des Faktoreinsatzes um 1% induziert eine Erhöhung der Produktionsmenge um 2%.
> * Eine Verdoppelung der Inputs führt zu einer Vervierfachung des Outputs.

---

### 4.2. Analytische Bestimmung des Kostenoptimums via Lagrange

#### Gegebene Parameter
* **Faktorpreise:** Lohnsatz $w = 10$, Kapitalzins $r = 20$
* **Ziel-Outputmenge ($q$):** $q = 180$

#### Schritt 1: Formulierung der Output-Nebenbedingung (NB)
$$3LK = 180 \implies 180 - 3LK = 0$$

#### Schritt 2: Aufstellen der Lagrange-Funktion ($\mathcal{L}$)
Bei der Kostenminimierung bildet die Kostenfunktion die Basis, ergänzt um die Nullform der Produktionsbeschränkung:
$$\mathcal{L}(L, K, \lambda) = 10L + 20K + \lambda(180 - 3LK)$$

#### Schritt 3: Bedingungen erster Ordnung (FOC)
$$\text{(I)} \quad \frac{\partial \mathcal{L}}{\partial L} = 10 - 3\lambda K \stackrel{!}{=} 0 \implies 10 = 3\lambda K$$
$$\text{(II)} \quad \frac{\partial \mathcal{L}}{\partial K} = 20 - 3\lambda L \stackrel{!}{=} 0 \implies 20 = 3\lambda L$$
$$\text{(III)} \quad \frac{\partial \mathcal{L}}{\partial \lambda} = 180 - 3LK \stackrel{!}{=} 0$$

#### Schritt 4: Bestimmung der Optimalitätsbedingung (Faktorsubstitutionsverhältnis)
Division von $\text{(I)}$ durch $\text{(II)}$ eliminiert den Lagrange-Multiplikator $\lambda$ und setzt das Faktorpreisverhältnis gleich der **Grenzrate der technischen Substitution (GRTS)**:
$$\frac{10}{20} = \frac{3\lambda K}{3\lambda L} \implies \frac{1}{2} = \frac{K}{L} \implies L = 2K$$

#### Schritt 5: Substitution in die Produktionsfunktion $\text{(III)}$
$$3 \cdot (2K) \cdot K = 180 \implies 6K^2 = 180$$
$$K^2 = 30 \implies K^* = \sqrt{30} \approx \mathbf{5,48}$$

#### Schritt 6: Berechnung der optimalen Menge des Faktors Arbeit ($L^*$)
$$L^* = 2 \cdot 5,4772 \approx \mathbf{10,96}$$

#### Schritt 7: Berechnung des optimalen Lagrange-Multiplikators $\lambda^*$
Nutze die umgestellte Gleichung $\text{(I)}$:
$$\lambda^* = \frac{10}{3K^*} = \frac{10}{3 \cdot 5,48} \approx \mathbf{0,61}$$

---

### 4.3. Ökonomische Gesamtkosten im Optimum

Die minimalen Gesamtkosten ($C^*$) zur Realisierung des vorgegebenen Outputniveaus von 180 Einheiten ergeben sich durch Einsetzen der optimalen Faktorkombinationen in die Isokostengerade:

$$C^* = wL^* + rK^*$$
$$C^* = 10 \cdot 10,96 + 20 \cdot 5,48 = 109,60 + 109,60 = \mathbf{219,20\text{ €}}$$

> [!TIP] Zusammenfassung der optimalen Werte
> 
> | Variable | Optimaler Wert | Bedeutung |
> | :--- | :--- | :--- |
> | **$K^*$** | 5,48 | Optimaler Kapitaleinsatz |
> | **$L^*$** | 10,96 | Optimaler Arbeitseinsatz |
> | **$\lambda^*$** | 0,61 | Grenzkosten einer zusätzlichen Outputeinheit |
> | **$C^*$** | 219,20 € | Minimierte Gesamtkosten |