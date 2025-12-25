[[Math]]

4.1 Area Calculation (_Flächenberechnung_)
### The Area Problem (_Flächeninhaltsproblem_)

- **Goal:** Calculate the area of arbitrary shapes, specifically the area between the graph of a function $f(x)$ and the x-axis over an interval $[a, b]$. 
    
- **Oriented Area (_Orientierter Flächeninhalt_):**
    
    - Areas lying **above** the x-axis are positive ($A > 0$). 
        
    - Areas lying **below** the x-axis are negative ($A < 0$). 
        
    - **Total Geometric Area:** Calculated by summing the absolute values: $A = |A_1| + [cite_start]|A_2|$. 
        

### Approximation by Rectangles (_Annäherung durch Rechtecke_)

The area is approximated by dividing the interval $[a, b]$ into $n$ sub-intervals of width $\Delta x_i$. 

- **Lower Sum (_Untersumme_, $U_n$):** Calculated using the minimum function value in each sub-interval. 
    
    $$U_n = \sum_{i=1}^n \Delta x_i \cdot f(x_{i-1})$$

- **Upper Sum (_Obersumme_, $O_n$):** Calculated using the maximum function value in each sub-interval. 
    
    $$O_n = \sum_{i=1}^n \Delta x_i \cdot f(x_i)$$

- The true area $A$ lies between these sums: $U_n \le A \le O_n$. 
    

### The Definite Integral (_Bestimmtes Integral_)

- **Integrable (_integrierbar_):** A function is integrable if the limits of the Upper Sum and Lower Sum are equal as the number of intervals approaches infinity ($n \to \infty$).
    
- Definition: This common limit is the definite integral.
    
    $$\lim_{n \to \infty} O_n = \lim_{n \to \infty} U_n = \int_a^b f(x) \, dx$$

- **Terminology:**
    
    - $a$: **Lower integration limit (_untere Integrationsgrenze_)** 
        
    - $b$: **Upper integration limit (_obere Integrationsgrenze_)** 
        
    - $x$: **Integration variable (_Integrationsvariable_)** 
        
    - $f(x)$: **Integrand (_Integrand_)** 
        

---

4.2 The Indefinite Integral (_Das unbestimmte Integral_) 

### Area Function (_Flächeninhaltsfunktion_)

- The function $F_a(x) = \int_a^x f(t) \, dt$ represents the area under the curve from a fixed point $a$ to a variable point $x$. 

### Fundamental Theorem of Calculus (_Hauptsatz der Differential- und Integralrechnung_)

- The area function is an **Antiderivative (_Stammfunktion_)** of the original function $f$. 
    
    $$F'_a(x) = f(x)$$

### Indefinite Integral Definition

- The indefinite integral represents the set of all antiderivatives of $f$. 
    
- Since antiderivatives differ only by a constant, it is written as:
    
    $$\int f(x) \, dx = F(x) + C$$

- $F(x)$: Any antiderivative.
    
- $C$: **Integration Constant (_Integrationskonstante_)** ($C \in \mathbb{R}$). 
    

### Basic Integrals (_Grundintegrale_)

Key antiderivatives to memorize: 

|**Function f(x)**|**Integral ∫f(x)dx**|**Note**|
|---|---|---|
|**Power Function (_Potenzfunktion_)** $x^n$|$\frac{1}{n+1}x^{n+1} + C$|$n \neq -1$|
|$x^{-1} = \frac{1}{x}$|$\ln|x|
|**Exponential (_Exponentialfunktion_)** $e^x$|$e^x + C$||
|**Sine (_Sinus_)** $\sin x$|$-\cos x + C$||
|**Cosine (_Kosinus_)** $\cos x$|$\sin x + C$||
|**Hyperbolic Sine (_Sinus hyperbolicus_)** $\sinh x$|$\cosh x + C$||
|**Hyperbolic Cosine (_Kosinus hyperbolicus_)** $\cosh x$|$\sinh x + C$||
|$\frac{1}{\sqrt{1-x^2}}$|$\arcsin x + C$||

### Calculating Definite Integrals

Using the antiderivative $F(x)$, the definite integral is calculated as:

$$\int_a^b f(x) \, dx = [F(x)]_a^b = F(b) - F(a)$$

- **Properties:**
    
    - $\int_b^a f(x) \, dx = - \int_a^b f(x) \, dx$ 
        
    - $\int_a^a f(x) \, dx = 0$ 
        

---

4.3 Integration Methods (_Integrationsmethoden_) 

### 4.3.1 Calculation Rules (_Rechenregeln_)

1. **Factor Rule (_Faktorregel_):** Constant factors can be pulled out of the integral. 
    
    $$\int K \cdot f(x) \, dx = K \cdot \int f(x) \, dx$$
    
2. **Sum Rule (_Summenregel_):** A sum of functions can be integrated term by term. 
    
    $$\int (f_1(x) + \dots + f_n(x)) \, dx = \int f_1(x) \, dx + \dots + \int f_n(x) \, dx$$
    

4.3.2 Integration by Substitution (_Integration durch Substitution_) 

This method is the reverse of the chain rule. 

**Procedure for Indefinite Integrals:**

1. **Substitute:** Choose $u = g(x)$ (usually the inner function). 
    
2. **Differential:** Calculate $dx = \frac{1}{g'(x)} du$. 
    
3. **Rewrite:** Transform $\int f(g(x)) \cdot g'(x) \, dx$ into $\int \phi(u) \, du$. 
    
4. **Integrate:** Find the antiderivative $\Phi(u) + C$. 
    
5. **Back-substitution (_Rücksubstitution_):** Replace $u$ with $g(x)$. 
    

**Procedure for Definite Integrals:**

- **Option A:** Calculate indefinite integral, back-substitute, then insert original limits $a$ and $b$. 
    
- **Option B:** Transform the limits. Substitute $a \to g(a)$ and $b \to g(b)$ and calculate directly with $u$. 
    
    $$\int_a^b f(x) \, dx = \int_{g(a)}^{g(b)} \phi(u) \, du$$
    

4.3.3 Integration by Parts (_Partielle Integration_) 

This method is the reverse of the product rule. 

Formula:

$$\int u(x) \cdot v'(x) \, dx = u(x) \cdot v(x) - \int u'(x) \cdot v(x) \, dx$$


**Strategy for choosing $u$ and $v'$:**

- Choose $v'(x)$ such that integrating it to find $v(x)$ does not make it more complex (e.g., $e^x$, $\sin x$).
    
- Choose $u(x)$ such that differentiating it to find $u'(x)$ simplifies it (e.g., polynomials $x^n$ reduce in degree).