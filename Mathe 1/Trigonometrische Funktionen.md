[[Math]]

## 1.5 Trigonometrische Funktionen (Trigonometric Functions)
### 1.5.1 Eigenschaften (Properties)
#### Erinnerung: Trigonometrie (Recap: Trigonometry)
Im rechtwinkligen Dreieck (In the right-angled triangle):
- **Sinus** (Sine): $$\sin \alpha = \frac{\text{Gegenkathete}}{\text{Hypothenuse}} = \frac{a}{c}$$
- **Kosinus** (Cosine): $$\cos \alpha = \frac{\text{Ankathete}}{\text{Hypothenuse}} = \frac{b}{c}$$
- **Tangens** (Tangent): $$\tan \alpha = \frac{a}{b} = \frac{\sin \alpha}{\cos \alpha}$$
- **Kotangens** (Cotangent): $$\cot \alpha = \frac{b}{a} = \frac{\cos \alpha}{\sin \alpha} = \frac{1}{\tan \alpha}$$
- Diese Definitionen gelten für $0^\circ < \alpha < 90^\circ$ (These definitions apply for $0^\circ < \alpha < 90^\circ$).
#### Erweiterung auf andere Winkel (Extension to other angles)
- Für $\alpha \ge 90^\circ$ werden Sinus und Kosinus als **Koordinaten eines Punkts $P(x; y)$ auf dem Einheitskreis** definiert (For $\alpha \ge 90^\circ$, sine and cosine are defined as the coordinates of a point $P(x; y)$ on the unit circle).
- Es gilt $x = \cos(\alpha)$ und $y = \sin(\alpha)$.
- Negative Winkel $\alpha$ entsprechen einer **Drehung im Uhrzeigersinn** (Negative angles $\alpha$ correspond to a rotation clockwise).
    - $$\cos(-\alpha) = \cos(\alpha)$$
    - $$\sin(-\alpha) = - \sin(\alpha)$$
- Sinus- und Kosinuswerte wiederholen sich alle $360^\circ$ (Sine and cosine values repeat every $360^\circ$):
    - $$\sin(\alpha + k \cdot 360^\circ) = \sin(\alpha) \quad \text{für } k \in \mathbb{Z}$$

#### Bogenmaß (Radian Measure)
- Die Größe $x$ im Bogenmaß ist die **Länge des Kreisbogens** ($\Delta s$), den der Winkel $\alpha$ aus dem Einheitskreis ($r=1$) schneidet.
- $$x = \frac{\Delta s}{r} = \Delta s$$
- Die Größe $x$ ist dimensionslos (The quantity $x$ is dimensionless), häufig wird die formale Einheit "Radiant (rad)" verwendet (The formal unit "Radian (rad)" is often used).
- **Umrechnung** (Conversion):
    - $$\alpha = \frac{180^\circ}{\pi} \cdot x \quad \text{bzw.} \quad x = \frac{\pi}{180^\circ} \cdot \alpha$$
#### Sinusfunktion (Sine Function)
- **Definition:** Die Sinusfunktion $x \mapsto \sin x$ ordnet einem $x \in \mathbb{R}$ den Sinus des entsprechenden Winkels im Bogenmaß zu (The sine function assigns to $x \in \mathbb{R}$ the sine of the corresponding angle in radian measure).
- **Periode:** Die Funktion ist periodisch mit der Periode $p = 2\pi$ bzw. $360^\circ$.
- **Eigenschaften**:
    - Definitionsbereich (Domain): $-\infty < x < \infty$
    - Bildbereich (Range): $-1 \le y \le 1$
    - Symmetrie (Symmetry): **ungerade** (odd)
    - Nullstellen (Zeros): $$x_k = k\pi \quad \text{bzw.} \quad x_k = k \cdot 180^\circ \quad (k \in \mathbb{Z})$$
#### Kosinusfunktion (Cosine Function)
- **Definition:** Die Kosinusfunktion $x \mapsto \cos x$ ordnet einem $x \in \mathbb{R}$ den Kosinus des entsprechenden Winkels im Bogenmaß zu (The cosine function assigns to $x \in \mathbb{R}$ the cosine of the corresponding angle in radian measure).
- **Periode:** Die Funktion ist periodisch mit der Periode $p = 2\pi$ bzw. $360^\circ$.
- **Eigenschaften**:
    - Definitionsbereich (Domain): $-\infty < x < \infty$
    - Bildbereich (Range): $-1 \le y \le 1$
    - Symmetrie (Symmetry): **gerade** (even)
    - Nullstellen (Zeros): $$x_k = \frac{\pi}{2} + k\pi \quad \text{bzw.} \quad x_k = 90^\circ + k \cdot 180^\circ \quad (k \in \mathbb{Z})$$
- **Verschiebung:** Es gilt $\sin(x) = \cos(x - \frac{\pi}{2})$ bzw. $\cos(x) = \sin(x + \frac{\pi}{2})$.

#### Tangens- und Kotangensfunktion (Tangent and Cotangent Functions)
- **Definitionen**:
    
    - $$\tan x = \frac{\sin x}{\cos x}$$
    - $$\cot x = \frac{\cos x}{\sin x} = \frac{1}{\tan x}$$
- **Eigenschaften Tangensfunktion**:
    - Periode (Period): $\pi$ bzw. $180^\circ$
    - Bildbereich (Range): $-\infty < y < \infty$
    - Symmetrie (Symmetry): ungerade (odd)
    - Nullstellen (Zeros): $x_k = k\pi$ ($k \in \mathbb{Z}$)
    - Polstellen (Poles): $x_k = \frac{\pi}{2} + k\pi$ ($k \in \mathbb{Z}$)
- **Eigenschaften Kotangensfunktion**:
    - Periode (Period): $\pi$ bzw. $180^\circ$
    - Bildbereich (Range): $-\infty < y < \infty$
    - Symmetrie (Symmetry): ungerade (odd)
    - Nullstellen (Zeros): $x_k = \frac{\pi}{2} + k\pi$ ($k \in \mathbb{Z}$)
    - Polstellen (Poles): $x_k = k\pi$ ($k \in \mathbb{Z}$)

#### Additionstheoreme (Addition Theorems)
Wichtige Zusammenhänge zwischen trigonometrischen Funktionen:
1. **Trigonometrischer Pythagoras** (Trigonometric identity): $$\sin^2(x) + \cos^2(x) = 1$$
2. **Addition und Subtraktion von Winkeln** (Addition and subtraction of angles): $$\sin(x_1 \pm x_2) = \sin(x_1) \cdot \cos(x_2) \pm \sin(x_2) \cdot \cos(x_1)$$ $$\cos(x_1 \pm x_2) = \cos(x_1) \cdot \cos(x_2) \mp \sin(x_1) \cdot \sin(x_2)$$
3. **Phasenverschiebung** (Phase shift): $$\cos(x) = \sin \left(x + \frac{\pi}{2}\right) \quad \text{bzw.} \quad \sin(x) = \cos \left(x - \frac{\pi}{2}\right)$$
### 1.5.2 Anwendungen (Applications)
#### Trigonometrische Funktionen in der Anwendung (Trigonometric Functions in Application)
- Dienen zur **Beschreibung periodischer Vorgänge** (Used for describing periodic processes).
- Beispiele sind mechanische Schwingungen, Wellenausbreitung, Wechselspannungen und -ströme (Examples are mechanical oscillations, wave propagation, alternating voltages and currents).
#### Allgemeine Sinusfunktion (General Sine Function)
- Die allgemeine Form ist $f(x) = A \cdot \sin(k \cdot x + \phi)$.
- $k = \frac{2\pi}{p}$, wobei $p$ die Periode ist.
- $A$: Amplitude.
- $\phi$: Phase.
- Bei Zeitfunktionen $f(t) = A \cdot \sin(\omega \cdot t + \phi)$ wird $\omega$ als **Kreisfrequenz** bezeichnet (In time functions, $\omega$ is called the angular frequency).
#### Darstellung im Zeigerdiagramm (Representation in Phasor Diagram)
- Die Funktion kann durch einen **Zeiger** (Phasor) mit der **Länge $A$** dargestellt werden, der mit der **Winkelgeschwindigkeit $\omega$** rotiert (The function can be represented by a phasor of length $A$ rotating with angular velocity $\omega$).
- Oft wird nur der Zeiger zum Startzeitpunkt $t = 0$ dargestellt (Often only the phasor at start time $t = 0$ is shown).
- Die Koordinaten des rotierenden Zeigers sind (The coordinates of the rotating phasor are):
    - $$x = A \cdot \cos(\phi + \omega t)$$
    - $$y = A \cdot \sin(\phi + \omega t)$$

#### Überlagerung im Zeigerdiagramm (Superposition in Phasor Diagram)
- Die einfache Überlagerung von Sinus- und Kosinusfunktionen erfolgt graphisch durch **Vektoraddition** (Parallelogrammregel) (Simple superposition is done graphically via vector addition (parallelogram rule)).
- Die rechnerische Überlagerung von $A_1 \cos(\omega t + \phi_1) + A_2 \cos(\omega t + \phi_2) = A \cos(\omega t + \phi)$ führt zu komplexeren Formeln.
### 1.5.3 Umkehrfunktionen (Inverse Functions)
- Da trigonometrische Funktionen **periodisch** sind, sind sie **nicht umkehrbar** (Since trigonometric functions are periodic, they are not invertible).
- Um Umkehrfunktionen definieren zu können, muss der **Definitionsbereich eingeschränkt** werden (To define inverse functions, the domain must be restricted).

#### Arkussinusfunktion ($\text{arcsin}$) (Arcsine Function)
- **Definition:** Die Umkehrfunktion der auf $\left[ -\frac{\pi}{2}, \frac{\pi}{2} \right]$ (bzw. $\left[ -90^\circ, 90^\circ \right]$) eingeschränkten Sinusfunktion.
- **Eigenschaften**:
    - Definitionsbereich (Domain): $-1 \le x \le 1$
    - Bildbereich (Range): $-\frac{\pi}{2} \le y \le \frac{\pi}{2}$
    - Symmetrie (Symmetry): ungerade (odd)

#### Arkuskosinusfunktion ($\text{arccos}$) (Arccosine Function)
- **Definition:** Die Umkehrfunktion der auf $\left[ 0, \pi \right]$ (bzw. $\left[ 0^\circ, 180^\circ \right]$) eingeschränkten Kosinusfunktion.
- **Eigenschaften**:
    - Definitionsbereich (Domain): $-1 \le x \le 1$
    - Bildbereich (Range): $0 \le y \le \pi$

#### Arkustangensfunktion ($\text{arctan}$) (Arctangent Function)
- **Definition:** Die Umkehrfunktion der auf $\left( -\frac{\pi}{2}, \frac{\pi}{2} \right)$ (bzw. $\left( -90^\circ, 90^\circ \right)$) eingeschränkten Tangensfunktion.
- Es werden offene Intervalle verwendet, da die Tangensfunktion bei $\pm \frac{\pi}{2}$ nicht definiert ist (Open intervals are used because the tangent function is not defined at $\pm \frac{\pi}{2}$).
- **Eigenschaften**:
    - Definitionsbereich (Domain): $-\infty < x < \infty$
    - Bildbereich (Range): $-\frac{\pi}{2} < y < \frac{\pi}{2}$
    - Symmetrie (Symmetry): ungerade (odd)

#### Arkuskotangensfunktion ($\text{arccot}$) (Arccotangent Function)
- **Definition:** Die Umkehrfunktion der auf $\left( 0, \pi \right)$ (bzw. $\left( 0^\circ, 180^\circ \right)$) eingeschränkten Kotangensfunktion.
- **Eigenschaften**:
    - Definitionsbereich (Domain): $-\infty < x < \infty$
    - Bildbereich (Range): $0 < y < \pi$