[[Math]]

## 2.1 Folgen ($\text{Sequences}$)

### Definition: Reelle Zahlenfolge

Eine reelle Zahlenfolge ist eine geordnete Menge reeller Zahlen:

$$\langle a_n \rangle = a_1, a_2, a_3, \dots, a_n, \dots \quad \text{mit } n \in \mathbb{N}. $$

- Die Zahlen $a_1, a_2, a_3, \dots$ heißen **Folgenglieder** ($\text{terms of the sequence}$).
    
- $a_n$ ist das $\mathbf{n}$-**te Glied** ($\text{the } n\text{-th term}$).
    
- Eine Zahlenfolge kann als spezielle Funktion $\mathbf{n \in \mathbb{N} \to a_n \in \mathbb{R}}$ aufgefasst werden.
    

### Darstellung von Folgen

Folgen können auf verschiedene Arten dargestellt werden:

- Explizite Darstellung ($\text{Explicit Representation}$):
    
    $$a_n = f(n). $$
    
- Rekursive Darstellung ($\text{Recursive Representation}$):
    
    $$a_{n+1} = f(a_1; a_2; \dots; a_n). $$
    
    - Häufig: $a_{n+1} = f(a_n). $
        
- **Graphische Darstellung**: Durch einen Graphen oder auf der Zahlengeraden.
    

### Spezielle Folgen

|**Typ (Type)**|**Definition (Definition)**|**Rekursives Bildungsgesetz (Recursive Rule)**|**Explizites Bildungsgesetz (Explicit Rule)**|**Wachstum (Growth Behavior)**|
|---|---|---|---|---|
|**Arithmetische Folge** ($\text{Arithmetic Sequence}$)|Die Differenz $d$ zweier aufeinander folgender Glieder ist gleich groß: $a_{n+1} - a_n = d$.|$$a_{n+1} = a_n + d. $$|$$a_n = a_1 + (n-1) \cdot d.$$|Lineares Wachstum ($\text{Linear growth}$)|
|**Geometrische Folge** ($\text{Geometric Sequence}$)|Der Quotient $q$ zweier aufeinander folgender Glieder ist gleich groß: $\frac{a_{n+1}}{a_n} = q$.|$$a_{n+1} = a_n \cdot q. $$|$$a_n = a_1 \cdot q^{n-1}.$$|Im Trend exponentielles Wachstum ($\text{Exponential growth in trend}$)|

**Zusätzliche Regeln für Geometrische Folgen**:

- Wenn $|q| < 1$, nähern sich die Folgenglieder für große $n$ **Null** an ($\text{terms approach zero}$).
    
- Wenn $q > 1$, **wachsen** die Folgenglieder über alle Grenzen ($\text{terms grow beyond all limits}$).
    

---

## Grenzwert einer Folge ($\text{Limit of a Sequence}$)

### Definition: Grenzwert

Eine reelle Zahl $g$ heißt Grenzwert (oder Limes) einer Folge $\langle a_n \rangle$, wenn es zu jedem $\mathbf{\epsilon > 0}$ ($\text{epsilon greater than zero}$) einen Folgenindex $n_0$ gibt, sodass

$$|a_n - g| < \epsilon \quad \text{für } n \geq n_0. $$

- Alle Folgenglieder ab $a_{n_0}$ liegen näher am Grenzwert $g$ als $\epsilon$.
    
- Eine Folge kann höchstens einen Grenzwert $g$ haben.
    

### Konvergenz und Divergenz

- Eine Folge $\langle a_n \rangle$ heißt **konvergent** ($\text{convergent}$), wenn sie einen Grenzwert $g$ besitzt.
    
    - Schreibweise:
        
        $$\lim_{n \to \infty} a_n = g. $$
        
- Folgen, die keinen Grenzwert besitzen, heißen **divergent** ($\text{divergent}$).
    
    - Wenn die Glieder über alle Grenzen wachsen, heißt die Folge bestimmt divergent gegen Unendlich:
        
        $$\lim_{n \to \infty} a_n = \infty. $$
        
    - Analog, wenn die Glieder unter alle Grenzen fallen: bestimmt divergent gegen minus Unendlich:
        
        $$\lim_{n \to \infty} a_n = -\infty. $$
        

### Rechenregeln für Grenzwerte

$$\text{Sei } \lim_{n \to \infty} a_n = g \text{ und } \lim_{n \to \infty} b_n = h: $$

- $$\lim_{n \to \infty} \frac{1}{n} = 0 \quad \text{und} \quad \lim_{n \to \infty} n = \infty. $$
    
- Wenn $\lim_{n \to \infty} a_n = \pm\infty$, so ist $\lim_{n \to \infty} \frac{1}{a_n} = 0.$
    
- Wenn $\lim_{n \to \infty} a_n = 0$, so ist $\lim_{n \to \infty} \frac{1}{a_n} = \pm\infty.$
    
- Summe/Differenz:
    
    $$\lim_{n \to \infty} (a_n \pm b_n) = g \pm h. $$
    
- Produkt:
    
    $$\lim_{n \to \infty} (a_n \cdot b_n) = g \cdot h. $$
    
- Quotient:
    
    $$\lim_{n \to \infty} \left(\frac{a_n}{b_n}\right) = \frac{g}{h} \quad \text{wenn } h \neq 0. $$
    
- Konstantes Vielfaches:
    
    $$\lim_{n \to \infty} (c \cdot a_n) = c \cdot g. $$
    
- Potenz:
    
    $$\lim_{n \to \infty} (a_n)^m = g^m. $$
    

---

## 2.2 Grenzwert von Funktionen ($\text{Limit of Functions}$)

### Definition: Grenzwert von Funktionen

Ist eine Funktion $f$ in der Nähe von $x_0$ definiert, so heißt die reelle Zahl $g$ Grenzwert von $f$ für $x$ gegen $x_0$ ($\text{limit of } f \text{ for } x \text{ towards } x_0$), wenn für jede Zahlenfolge $\langle x_n \rangle$ mit $\lim_{n \to \infty} x_n = x_0$ gilt:

$$\lim_{n \to \infty} f(x_n) = g. $$

- Schreibweise:
    
    $$\lim_{x \to x_0} f(x) = g. $$
    
- $f$ muss bei $x_0$ **nicht** definiert sein.
    
- $x_0 = \pm\infty$ ist möglich.
    

### Rechenregeln für Grenzwerte von Funktionen

Die Regeln sind **analog** zu denen für Folgen und gelten, wenn $f$ und $g$ konvergent sind:

- $$\lim_{x \to \infty} \frac{1}{x} = 0 \quad \text{und} \quad \lim_{x \to \infty} x = \infty. $$
    
- Ist $\lim_{x \to x_0} f(x) = 0$, so gilt $\lim_{x \to x_0} \frac{1}{f(x)} = \pm\infty$, und umgekehrt.
    
- Regeln für **Summe, Produkt, Quotient, Vielfaches** und **Potenz** sind analog zu den Folgengrenzwerten.
    

### Polstellen und Definitionslücken

$$\text{Für eine gebrochen rationale Funktion } f(x) = \frac{g(x)}{h(x)}: \text{ Ist } x_0 \text{ eine Nullstelle von } h, \text{ so hat } f \text{ bei } x_0: $$

1. Eine **behebbare Definitionslücke** ($\text{removable discontinuity}$), wenn $\lim_{x \to x_0} f(x)$ existiert.
    
2. Eine **Polstelle** ($\text{pole}$), wenn $f$ bei $x_0$ bestimmt divergent ist ($\lim_{x \to x_0} f(x) = \pm\infty$).
    

### Wichtige Grenzwerte

- Echt gebrochen rationale Funktionen ($\text{Proper rational functions}$) ($\text{Zählergrad } < \text{ Nennergrad}$):
    
    $$\lim_{x \to \pm\infty} f(x) = 0. $$
    
- Unecht gebrochen rationale Funktionen ($\text{Improper rational functions}$) mit Zählergrad = Nennergrad:
    
    $$\lim_{x \to \pm\infty} f(x) = \frac{a_n}{b_n}. $$
    
    ($a_n$ und $b_n$ sind die Koeffizienten der höchsten Potenzen).
    
- **Grenzwertsätze für Exponential- und Logarithmusfunktion**:
    
    - $$\lim_{x \to \infty} \frac{x^n}{a^x} = 0 \quad \text{für } a > 1. $$
        
    - $$\lim_{x \to \infty} \frac{\log_a(x)}{x^n} = 0 \quad \text{für } a > 1, n > 0. $$
        

### Stetigkeit ($\text{Continuity}$)

**Definition: Stetige Funktion**

Eine bei $x_0$ und in der Nähe von $x_0$ definierte Funktion $f$ heißt stetig bei $x_0$ ($\text{continuous at } x_0$), wenn gilt:

$$\lim_{x \to x_0} f(x) = f(x_0). $$

- Der Grenzwert bei $x_0$ existiert und stimmt mit dem Funktionswert $f(x_0)$ überein.
    
- **Überall stetige Funktionen** sind z.B. ganzrationale Funktionen, Exponentialfunktionen sowie die Sinus- und Kosinusfunktion.
    

---

## 2.3 Reihen ($\text{Series}$)

### Definition: Unendliche Reihe

- Die Partialsumme ($\text{Partial Sum}$) $s_n$ ist die Summation der ersten $n$ Glieder einer Folge $\langle a_n \rangle$:
    
    $$s_n = a_1 + a_2 + a_3 + \dots + a_n = \sum_{k=1}^{n} a_k. $$
    
- Die Folge der Partialsummen $\langle s_n \rangle$ einer Zahlenfolge $\langle a_n \rangle$ heißt **unendliche Reihe** ($\text{infinite series}$).
    
- Ist $\langle s_n \rangle$ konvergent, so heißt der Grenzwert Summenwert $s$:
    
    $$s = \lim_{n \to \infty} s_n = \sum_{n=1}^{\infty} a_n. $$
    

### Geometrische Reihe

Eine geometrische Reihe ist vom Typ:

$$\sum_{n=1}^{\infty} q^{n-1} = 1 + q + q^2 + \dots. $$

- Partialsumme:
    
    $$s_n = 1 + q + q^2 + \dots + q^{n-1} = \frac{1 - q^n}{1 - q}. $$
    
- Konvergenz: Für $|q| < 1$ ist die geometrische Reihe konvergent mit dem Summenwert:
    
    $$s = \sum_{n=1}^{\infty} q^{n-1} = \frac{1}{1 - q}. $$
    
- **Divergenz**: Für $|q| \geq 1$ ist die geometrische Reihe divergent.
    

### Konvergenzkriterien

#### Notwendiges Kriterium für Konvergenz

Eine unendliche Reihe $\sum_{n=1}^{\infty} a_n$ kann nur dann konvergent sein, wenn:

$$\lim_{n \to \infty} a_n = 0. $$

$$\text{Die Umkehrung gilt nicht } (\text{The reverse is not true}). $$

#### Quotientenkriterium ($\text{Ratio Test}$)

Eine unendliche Reihe $\sum_{n=1}^{\infty} a_n$ ist:

- konvergent, wenn
    
    $$\lim_{n \to \infty} \left| \frac{a_{n+1}}{a_n} \right| < 1. $$
    
- divergent, wenn
    
    $$\lim_{n \to \infty} \left| \frac{a_{n+1}}{a_n} \right| > 1. $$
    
- $$\text{Für } \lim_{n \to \infty} \left| \frac{a_{n+1}}{a_n} \right| = 1 \text{ ist **keine Aussage** möglich}. $$
    

#### Leibniz-Kriterium für alternierende Reihen

$$\text{Ist } \langle b_n \rangle \text{ eine Folge mit } b_n \geq 0, \text{ so ist eine **alternierende Reihe** vom Typ } b_1 - b_2 + b_3 - b_4 + \dots = \sum_{n=1}^{\infty} (-1)^{n-1} \cdot b_n \text{ konvergent, wenn gilt:} $$

1. $$b_1 > b_2 > b_3 > \dots \quad (\text{monoton fallend}). $$
    
2. $$\lim_{n \to \infty} b_n = 0. $$