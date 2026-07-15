### 1. Temporal Horizon in Cost Theory
* **Kurze Frist (Short-Run):** Defined by the existence of at least one fixed factor of production, which generates output-independent fixed costs ($FC$). 
* **Lange Frist (Long-Run):** Defined by complete operational asset flexibility, meaning all inputs can be adjusted. All costs are entirely variable ($VC$), meaning the constant term of the total cost function equals zero.

---

### 2. Analytical Cost Decomposition
The total cost function ($TC$) extracted from `image_c490f6.png` is structurally composed of two distinct components:
$$TC(q) = 7q^2 + 5q + 1500$$

* **Variable Cost Component ($VC$):** The quantity-dependent terms that scale with production output $q$.
  $$VC(q) = 7q^2 + 5q$$
* **Fixed Cost Component ($FC$):** The invariant, static parameter that remains constant even at zero production volume ($q = 0$).
  $$FC = 1500$$
* **Structural Conclusion:** Because $FC = 1500 \neq 0$, the production environment is bound by short-run constraints.

---

### 3. Derivation of Marginal Costs (MC)
* **Economic Definition:** Marginal costs ($MC$) measure the rate of change of total costs relative to an incremental change in the quantity produced. It reflects the cost of the last unit generated.
* **Mathematical Derivation:** $MC$ is operationalized by taking the first first-order partial derivative of the total cost function ($TC$) with respect to the output quantity ($q$):
  $$MC(q) = \frac{\partial TC}{\partial q} = \frac{\partial (7q^2 + 5q + 1500)}{\partial q}$$
* **Calculus Execution:** 
  $$\frac{\partial (7q^2)}{\partial q} = 14q$$
  $$\frac{\partial (5q)}{\partial q} = 5$$
  $$\frac{\partial (1500)}{\partial q} = 0$$
* **Final Marginal Cost Function:**
  $$MC(q) = 14q + 5$$