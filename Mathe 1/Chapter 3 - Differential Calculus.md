[[Math]]

## 3.1 Differentiability (Differenzierbarkeit)

### 🔹 Concept of Rate of Change (Änderungsrate)
We ask: *How strongly does a quantity change?*  
Examples:

- Physics (Physik): displacement → velocity  
  $$v = \frac{Δs}{Δt}$$
- Electrical engineering (Elektrotechnik): charge → current  
  $$I = \frac{Δq}{Δt}$$
- Economics (Wirtschaft): price index → inflation rate  

Mathematically, this is the **slope (Steigung)** of the function $f(x)$ at point $(x_0, y_0)$.

---

### 🔹 Definition: Derivative (Ableitung)

A function $f$ is **differentiable (differenzierbar)** at $x_0$ if the following limit exists:

$$
f'(x_0) = \lim_{Δx→0} \frac{f(x_0 + Δx) - f(x_0)}{Δx}
$$

- $f'(x_0)$: derivative (Ableitung) of $f$ at $x_0$  
- Also written as:
  $$f'(x_0) = \frac{dy}{dx}\Big|_{x_0}$$
- Represents the **instantaneous slope (Momentansteigung)** of the tangent (Tangente).

---

### 🔹 Basic Derivatives (Ableitungen elementarer Funktionen)

| Function $f(x)$ | Derivative $f'(x)$ | Notes |
|-----------------|--------------------|--------|
| $x^n$ | $n \cdot x^{n-1}$ | Power rule (Potenzregel) |
| $\sin x$ | $\cos x$ |  |
| $\cos x$ | $-\sin x$ |  |
| $\tan x$ | $\frac{1}{\cos^2 x}$ |  |
| $e^x$ | $e^x$ | Exponential function (Exponentialfunktion) |
| $a^x$ | $(\ln a) \cdot a^x$ |  |
| $\sinh x$ | $\cosh x$ | Hyperbolic sine (Sinus hyperbolicus) |
| $\cosh x$ | $\sinh x$ | Hyperbolic cosine (Kosinus hyperbolicus) |
| $\tanh x$ | $\frac{1}{\cosh^2 x}$ | Hyperbolic tangent (Tangens hyperbolicus) |

---

## 3.2 Differentiation Rules (Ableitungsregeln)

### 🔹 Constant Factor Rule (Faktorregel)
$$(C \cdot u(x))' = C \cdot u'(x)$$

### 🔹 Sum Rule (Summenregel)
$$(f_1(x) + f_2(x) + \dots + f_n(x))' = f'_1(x) + f'_2(x) + \dots + f'_n(x)$$

### 🔹 Product Rule (Produktregel)
$$(u(x) \cdot v(x))' = u'(x) \cdot v(x) + u(x) \cdot v'(x)$$

### 🔹 Quotient Rule (Quotientenregel)
$$
\left( \frac{u(x)}{v(x)} \right)' = \frac{u'(x) \cdot v(x) - u(x) \cdot v'(x)}{[v(x)]^2}
$$

### 🔹 Chain Rule (Kettenregel)
If $f(x) = u(v(x))$, then:
$$
f'(x) = v'(x) \cdot u'(v(x))
$$
Mnemonic: *inner derivative times outer derivative*  
(innere Ableitung mal äußere Ableitung)

### 🔹 Derivative of Inverse Function (Ableitung der Umkehrfunktion)
$$
(f^{-1})'(x) = \frac{1}{f'(f^{-1}(x))}
$$

---

## 3.3 Curve Discussion & Extremum Problems (Kurvendiskussion und Extremwertaufgaben)

### 🔹 Monotonicity (Monotonieverhalten)
- $f'(x) > 0$ → increasing (monoton steigend)  
- $f'(x) < 0$ → decreasing (monoton fallend)

---

### 🔹 Curvature (Krümmung)
- $f''(x_0) > 0$ → concave up (linkskrümmung)  
- $f''(x_0) < 0$ → concave down (rechtskrümmung)

---

### 🔹 Relative Extrema (relative Extrema)
- **Necessary condition (notwendige Bedingung):** $f'(x_0) = 0$
- **Sufficient condition (hinreichende Bedingung):**
  - $f''(x_0) > 0$ → local minimum (relatives Minimum)
  - $f''(x_0) < 0$ → local maximum (relatives Maximum)
- $f'(x_0) = 0$, $f''(x_0) = 0$ → possible saddle point (Sattelstelle)

---

### 🔹 Inflection Points (Wendepunkte)
- $f''(x_0) = 0$ and $f'''(x_0) \neq 0$
- If also $f'(x_0) = 0$ → saddle point (Sattelstelle)

---

### 🔹 Complete Curve Discussion (vollständige Kurvendiskussion)

1. Domain (Definitionsbereich)  
2. Range (Wertebereich)  
3. Zeros (Nullstellen)  
4. Poles (Polstellen)  
5. Limits as $x → ±∞$  
6. Asymptotes (Asymptoten)  
7. Extrema (Extrema)  
8. Inflection/Saddle points (Wendepunkte / Sattelpunkte)  
9. Graph sketch (Funktionsgraph)

---

## 3.4 L’Hospital’s Rule (L’Hospitalsche Regel)

Used for indeterminate forms (unbestimmte Ausdrücke).

If  
$$\lim_{x→a} f(x) = \lim_{x→a} g(x) = 0 \quad \text{(type 0/0)}$$  
or  
$$\lim_{x→a} f(x) = \lim_{x→a} g(x) = ±∞ \quad \text{(type ∞/∞)}$$  

then  
$$
\lim_{x→a} \frac{f(x)}{g(x)} = \lim_{x→a} \frac{f'(x)}{g'(x)}
$$

Also applicable to $0 \cdot ∞$, $∞ − ∞$, $0^0$, $∞^0$, $1^∞$ after suitable algebraic manipulation.

---

## 3.5 Newton’s Method (Newton-Verfahren)

Used to find zeros (Nullstellen) of $f(x)$ approximately.

### Formula:
$$
x_{n+1} = x_n - \frac{f(x_n)}{f'(x_n)}
$$

- Start with an initial guess $x_0$
- Converges **quadratically (quadratische Konvergenz)** if convergence occurs

### Stopping Criteria (Abbruchkriterien)
1. $|f(x_n)| < ε$
2. $\frac{|x_{n+1} - x_n|}{|x_n|} < δ$
3. $n = N_{max}$

---

## ✅ Summary Table (Überblick)

| Concept | German Term | Formula / Note |
|----------|--------------|----------------|
| Derivative | Ableitung | $f'(x) = \lim_{Δx→0} \frac{Δy}{Δx}$ |
| Differentiable | differenzierbar | Limit must exist |
| Product Rule | Produktregel | $u'v + uv'$ |
| Quotient Rule | Quotientenregel | $\frac{u'v - uv'}{v^2}$ |
| Chain Rule | Kettenregel | inner × outer derivative |
| Extremum | Extremum | $f'(x)=0, f''(x)\neq0$ |
| Inflection Point | Wendepunkt | $f''(x)=0, f'''(x)\neq0$ |
| L’Hospital’s Rule | Regel von L’Hospital | $\frac{f'(x)}{g'(x)}$ |
| Newton’s Method | Newton-Verfahren | $x_{n+1}=x_n - \frac{f(x_n)}{f'(x_n)}$ |

---
