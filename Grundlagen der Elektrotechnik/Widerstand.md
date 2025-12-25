[[GDE]]
## 2.5 Widerstand (Resistance)
### Definition und das Ohmsche Gesetz (Definition and Ohm's Law)
- Bei einem Bauelement mit zwei Anschlüssen (Zweipol) besteht ein **Zusammenhang zwischen der Spannung ($U_{AB}$) über dem Bauelement und dem Strom ($I$) durch das Bauelement**. (For a component with two terminals (two-port), there is a **relationship between the voltage ($U_{AB}$) across the component and the current ($I$) through the component**).
- Bei einer wichtigen Klasse von Bauelementen ist dieser Zusammenhang **proportional** (linear). (For an important class of components, this relationship is **proportional** (linear)).
- Diese Bauelemente werden als **ohmsche Zweipole** bezeichnet. (These components are referred to as **ohmic two-ports**).
- Die Beziehung wird **ohmsches Gesetz** genannt: $$U_{AB} = R \cdot I.$$(The relationship is called **Ohm's Law**).
- Der Proportionalitätsfaktor **$R$** heißt **ohmscher Widerstand**. (The proportionality factor **$R$** is called **ohmic resistance**).
- Oft wird das Bauelement selbst als ohmscher Widerstand bezeichnet. (The component itself is often referred to as an ohmic resistor).
- Das Ohmsche Gesetz kann auch umgeformt werden zu $I = \frac{U}{R}$ und $R = \frac{U}{I}$. (Ohm's Law can also be rearranged to $I = \frac{U}{R}$ and $R = \frac{U}{I}$).

### Einheit und Kennlinie (Unit and Characteristic Curve)
- Die Einheit des ohmschen Widerstands ist das **Ohm ($\Omega$)**. (The unit of ohmic resistance is the **Ohm ($\Omega$)**). $$[R] = \left[\frac{U}{I}\right] = \frac{V}{A} = \text{Ohm} = \Omega.	$$
	- Die **Strom-Spannungskennlinie** eines ohmschen Zweipols ist eine **Gerade durch den Nullpunkt**. (The **current-voltage characteristic** of an ohmic two-port is a **straight line through the origin**).
- Die **Steigung der Geraden** ist gleich dem ohmschen Widerstand $R$. (The **slope of the line** equals the ohmic resistance $R$).

### Leitwert (Conductance)
- Der **Kehrwert des Widerstands $R$** wird **Leitwert $G$** genannt. (The **reciprocal of the resistance $R$** is called **conductance $G$**). $$G = \frac{1}{R}.$$
- Die Einheit des Leitwerts ist $1/\text{Ohm}$ oder **Siemens ($S$)**. (The unit of conductance is $1/\text{Ohm}$ or **Siemens ($S$)**).
- In den USA ist auch die eigentlich veraltete Einheit **mho** für den Leitwert gebräuchlich. (In the USA, the actually obsolete unit **mho** is also common for conductance).

## 2.6 Widerstand eines Leiters (Resistance of a Conductor)
### Abhängigkeit von Material und Geometrie (Dependence on Material and Geometry)
- Der Widerstand eines Leiters hängt von **dessen Abmessungen und dem verwendeten Material** ab. (The resistance of a conductor depends on **its dimensions and the material used**).
- Der Widerstand nimmt mit der **Länge $\ell$ des Leiters zu**. (The resistance **increases with the length $\ell$ of the conductor**).
- Der elektrische Widerstand ist umso **kleiner, je größer der Querschnitt $A$ des Leiters** ist. (The electrical resistance is **smaller the larger the cross-section $A$ of the conductor** is).
- Es gilt die folgende Beziehung: $$R = \rho \cdot \frac{\ell}{A}.$$
### Spezifischer Widerstand ($\rho$) und Leitfähigkeit ($\sigma$) (Specific Resistance ($\rho$) and Conductivity ($\sigma$))
- Der Faktor **$\rho$** ist vom Leitermaterial abhängig und wird als **spezifischer Widerstand** bezeichnet. (The factor **$\rho$** depends on the conductor material and is called **specific resistance**).
- Die Einheit für $\rho$ ist **Ohm-Meter ($\Omega \cdot m$)**. (The unit for $\rho$ is **Ohm-meter ($\Omega \cdot m$)**). $$[\rho] = [R] \cdot \frac{[A]}{[\ell]} = \frac{\Omega \cdot m^2}{m} = \Omega \cdot m.$$
- Der Kehrwert $\sigma = 1/\rho$ wird als **elektrische Leitfähigkeit** bezeichnet. (The reciprocal $\sigma = 1/\rho$ is called **electrical conductivity**).
### Beispielrechnung (Example Calculation)
- **Aufgabe:** Wie lang muss ein Konstantandraht mit $A = 1 , mm^2$ und $\rho = 0,5 , \mu\Omega \cdot m$ sein, damit sein Widerstand $1 , \Omega$ beträgt?. (How long must a constantan wire with $A = 1 , mm^2$ and $\rho = 0,5 , \mu\Omega \cdot m$ be so that its resistance is $1 , \Omega$?).
- **Lösung:** Durch Auflösen der Gleichung nach $\ell$ erhält man: $$\ell = \frac{R \cdot A}{\rho} = \frac{1\Omega \cdot 10^{-6}m^2}{0,5 \cdot 10^{-6}\Omega \cdot m} = 2 , m.$$