[[Physics]]

> [!SUMMARY] Zusammenfassung
> Dieses Kapitel behandelt die Skalargrößen der Mechanik. Die **Arbeit** ($W$) wird als Prozessgröße definiert, die den Energiezustand eines Systems ändert. Die **Energie** ($E$) ist die gespeicherte Fähigkeit, Arbeit zu verrichten.  Es werden die Erhaltungssätze für konservative und dissipative Systeme eingeführt und der Begriff der **Leistung** ($P$) als Arbeit pro Zeit definiert [cite: 701-707, 729-730].

---

## 5.1 Arbeit (Work)

Arbeit ist der Energietransfer auf einen Körper durch eine Kraft, die entlang eines Weges wirkt.  Im Gegensatz zur Vektorgröße "Kraft" ist Arbeit ein **Skalar**.

### Definitionen

1.  **Konstante Kraft:**
    Wenn die Kraft $\vec{F}$ konstant ist, gilt das Skalarprodukt:
    $$W = \vec{F} \cdot \vec{s} = |\vec{F}| \cdot |\vec{s}| \cdot \cos(\varphi)$$
    * $\varphi$: Winkel zwischen Kraftvektor und Wegvektor.
    *  *Hinweis:* Nur die Kraftkomponente in Wegrichtung verrichtet Arbeit ($F \cos \varphi$)

2.  **Veränderliche Kraft / Krummliniger Weg:**
    Ändert sich die Kraft oder der Weg, muss über infinitesimale Wegstücke $d\vec{s}$ integriert werden:
    $$W = \int_{1}^{2} dW = \int_{1}^{2} \vec{F} d\vec{s}$$

> [!INFO] Einheiten
>  $[W] = N \cdot m = J \text{ (Joule)} = W \cdot s$[cite: 705].

---

## 5.2 Energie (Energy)

Energie ist eine **Zustandsgröße**.  Ein Körper, an dem Arbeit verrichtet wurde (z.B. Beschleunigung), hat Energie gespeichert.

### Energieformen

#### 1. Kinetische Energie ($E_{kin}$)
Auch Bewegungsenergie genannt. Ein Körper der Masse $m$ mit Geschwindigkeit $v$ besitzt die Energie:
$$E_{kin} = \frac{1}{2} m v^2$$
*  **Herleitung:** Folgt aus $W=Fs$, $F=ma$ und $s=\frac{1}{2}at^2$.

#### 2. Potenzielle Energie ($E_{pot}$)
Auch Lageenergie genannt. Fähigkeit, aufgrund der Position im Gravitationsfeld Arbeit zu verrichten. Sie entspricht der **Hubarbeit**:
$$E_{pot} = m g h$$
*  $g$: Erdbeschleunigung ($9,81 m/s^2$)

#### 3. Elastische Energie ($E_{e}$)
Energie, die durch elastische Deformation (z.B. Feder) gespeichert wird.
$$E_{e} = \int_{0}^{s} F ds = \frac{1}{2} c s^2$$
* $c$: Federkonstante (manchmal auch $k$ oder $D$).
*  Basiert auf dem Hookesches Gesetz ($F \sim s$) 

---

## 5.3 Leistung (Power)

 Die Leistung $P$ gibt an, wie schnell Arbeit verrichtet wird

$$P = \frac{dW}{dt}$$

Für konstante Leistung gilt:
$$P = \frac{\Delta W}{\Delta t}$$

> [!TIP] Zusammenhang mit Geschwindigkeit
> Da $W = F \cdot s$ und $v = s/t$, kann die Leistung auch durch Kraft und Geschwindigkeit ausgedrückt werden:
> $$P = \vec{F} \cdot \vec{v}$$


 **Einheit:** $[P] = W \text{ (Watt)} = J/s$.

---

## 5.4 Energieerhaltung

 Der **Energieerhaltungssatz** besagt, dass Energie in einem abgeschlossenen System weder erzeugt noch vernichtet, sondern nur umgewandelt werden kann.

### 1. Konservative Systeme (Reibungsfrei)
Nur konservative Kräfte (Gravitation, Federkraft) wirken. Mechanische Energie bleibt konstant.
$$E_{kin} + E_{pot} = E_{gesamt} = \text{konst.}$$

### 2. Dissipative Systeme (Mit Reibung)
Nicht-konservative Kräfte (Reibung) wandeln mechanische Energie in Wärme ($E_r$) um.
$$E_{kin} + E_{pot} + E_{r} = E_{gesamt} = \text{konst.}$$

> [!EXAMPLE] Beispiel: Hybridauto
> Ein Hybridfahrzeug nutzt den Energieerhaltungssatz beim Bremsen.  Statt kinetische Energie nur durch Reibung in nutzlose Wärme umzuwandeln (dissipativ), wird sie in elektrische Energie umgewandelt und in der Batterie gespeichert (rekuperiert) [cite: 783-787].

---

## Exkurs: Impuls (Einführung)

Der Impuls $\vec{p}$ ist eng mit der Kraft verknüpft (Newton II).

* **Definition:** $\vec{p} = m \vec{v}$
* **Kraftstoß:** $\vec{F} = \frac{d\vec{p}}{dt}$ (Kraft entspricht der zeitlichen Änderung des Impulses).
* **Einheit:** $[p] = kg \cdot \frac{m}{s} = Ns$

> [!QUESTION] Übungsaufgabe: Boot abstoßen
> **Gegeben:**
> * Masse Boot $m = 500 \, kg$
> * Kraft $F = 75 \, N$
> * Zeit $t = 5 \, s$
>
> **Gesucht:** Impuls $p$ und Geschwindigkeit $v$.
>
> **Lösung:**
> 1.  Zusammenhang nutzen: $F = p/t \Rightarrow p = F \cdot t$
>     $$p = 75 \, N \cdot 5 \, s = 375 \, Ns$$
> 2.  Geschwindigkeit berechnen: $v = p/m$
>     $$v = \frac{375 \, Ns}{500 \, kg} = 0,75 \, m/s$$
>  [cite: 804-807]

---

## Formelsammlung Kapitel 5

| Größe | Formel | Einheit |
| :--- | :--- | :--- |
| **Arbeit** | $W = \vec{F} \cdot \vec{s}$ | $J$ |
| **Kinetische Energie** | $E_{kin} = \frac{1}{2}mv^2$ | $J$ |
| **Potenzielle Energie** | $E_{pot} = mgh$ | $J$ |
| **Elastische Energie** | $E_{e} = \frac{1}{2}cs^2$ | $J$ |
| **Leistung** | $P = \frac{dW}{dt} = F \cdot v$ | $W$ |