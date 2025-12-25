[[Physics]]
**3.1. Eindimensionale Kinetik der Punktmasse**
Die Bewegung eines Punktes ist eindimensional, wenn sie auf einer vorgegebenen Bahn erfolgt ("Spurgeführt"). Zur eindeutigen Bestimmung des Ortes ist dann nur eine Koordinate nötig. Das Objekt kann dabei als Massepunkt mit einem Freiheitsgrad beschrieben werden.

Das **Weg-Zeit-Gesetz** beschreibt den Ort des Punktes in Abhängigkeit von der Zeit: $$x = x(t)$$
**3.1.1. Geschwindigkeit**
Die Änderung des Ortes mit der Zeit wird durch die Geschwindigkeit beschrieben.
1. **Mittlere Geschwindigkeit ($\bar{v}$):** Der Quotient aus $\Delta x$ und $\Delta t$ beschreibt die mittlere Geschwindigkeit. $$\bar{v} = \frac{s_1(t_1) - s_0(t_0)}{t_1 - t_0} = \frac{\Delta s}{\Delta t}$$ Die Fahrstrecke $\Delta s$ ergibt sich als: $$\Delta s = \bar{v} \cdot \Delta t$$
2. **Momentangeschwindigkeit ($v(t)$):** Bei nicht-gleichförmigen Bewegungen ist die Momentangeschwindigkeit gleich der ersten Ableitung des Weges nach der Zeit. $$v(t) = \lim_{\Delta t \to 0} \frac{\Delta s}{\Delta t} = \frac{ds}{dt} = \dot{s}$$
3. **Einheit:** Die Einheit der Geschwindigkeit ist: $$[v] = \frac{[s]}{[t]} = \frac{m}{s}$$
4. **Weg-Zeit-Gesetz für gleichförmige Bewegungen:** Bei gleichförmigen Bewegungen ist die Geschwindigkeit konstant ($v = \text{konst.}$) und entspricht der mittleren Geschwindigkeit. $$x(t) = v \cdot t + s_0$$ Eine gleichförmige Bewegung bedeutet, dass in gleichen Zeiten gleiche Wege zurückgelegt werden.

**3.1.2. Beschleunigung**
Bewegungen, bei denen sich die Geschwindigkeit ändert, werden als beschleunigt bezeichnet.
1. **Mittlere Beschleunigung ($\bar{a}$):** Der Quotient aus der Geschwindigkeitsänderung $\Delta v$ und der dafür benötigten Zeit $\Delta t$ beschreibt die mittlere Beschleunigung. $$\bar{a} = \frac{v_1(t_1) - v_0(t_0)}{t_1 - t_0} = \frac{\Delta v}{\Delta t}$$
2. **Momentanbeschleunigung ($a(t)$):** Dies ist die zeitliche Änderung der Geschwindigkeit und somit die erste Ableitung der Momentangeschwindigkeit nach der Zeit. $$a(t) = \lim_{\Delta t \to 0} \frac{\Delta v}{\Delta t} = \frac{dv}{dt} = \dot{v}$$
3. **Zweite Ableitung:** Die Beschleunigung ist auch die zweite Ableitung des Weges nach der Zeit: $$a = \frac{d\vec{v}}{dt} = \frac{d^2x}{dt^2} = \ddot{x}$$
4. **Einheit:** Die Einheit der Beschleunigung ist: $$[a] = \frac{[v]}{[t]} = \frac{m}{s^2}$$
5. **Gleichmäßig beschleunigte Bewegung:** Eine Bewegung mit konstanter Beschleunigung ($a = \text{konst.}$) wird gleichmäßig beschleunigt genannt. Die momentane Beschleunigung entspricht hier der mittleren Beschleunigung.
	    ◦ **Geschwindigkeit ($v(t)$) bei konstanter Beschleunigung:** Die Berechnung erfolgt durch Integration der konstanten Beschleunigung. $$v(t) = a \cdot t + v_0$$
	    ◦ **Weg-Zeit-Gesetz ($x(t)$) bei konstanter Beschleunigung:** Die Berechnung erfolgt durch zweimalige Integration. $$x(t) = \frac{a}{2} \cdot t^2 + v_0 \cdot t + x_0$$ Diese Gleichung beschreibt die Überlagerung einer Bewegung mit konstanter Geschwindigkeit $v$ und konstanter Beschleunigung $a$.

6. **Integration (Umkehrfunktion):** Man kann von der Beschleunigung $a(t)$ ausgehen und daraus Geschwindigkeit $v$ und Weg $s$ berechnen, indem man die Integralrechnung nutzt.
	    ◦ **Geschwindigkeit durch Integration:** $$v = \int_0^t a,dt + v_0$$ Die Größe $v_0$ ist die Integrationskonstante (Anfangsgeschwindigkeit bei $t=0$). Das Integral stellt die Fläche unter der entsprechenden Kurve dar. Die während der Beschleunigung gewonnene Geschwindigkeitsänderung $\Delta v$ entspricht der Fläche im $a$-$t$-Diagramm.
	    ◦ **Ort/Weg durch Integration:** $$x = \int_0^t v,dt + x_0$$ Die Größe $x_0$ ist die Integrationskonstante (Anfangsort bei $t=0$). Der zurückgelegte Weg $\Delta s = x - x_0$ stellt die Fläche unter der Geschwindigkeit-Zeit-Kurve $v(t)$ dar.
	    
7. **Abbremsen und schneller werden:**
	    ◦ **Bremsvorgänge** sind beschleunigte Bewegungen (Verzögerungen), bei denen die Geschwindigkeit und Beschleunigung unterschiedliche Vorzeichen haben.
	    ◦ Ein Körper wird **schneller**, wenn Beschleunigung und Geschwindigkeit beide positiv oder beide negativ sind.
	    ◦ Die Beschleunigung wird Null, wenn ein Körper zum Stehen gekommen ist.

