# VWL I: Mikroökonomik - Klausurvorbereitung
## Aufgaben 1 & 2: Grundlagen & Konsumententheorie

### 1. Aufgabe 1: Wirtschaftswissenschaftliche Grundlagen

#### 1.1. Begriffszuordnungen & Kernkonzepte
* **Mautpflichtige Straßennutzung:** Allmendegüter. Eine Maut reguliert die Rivalität im Konsum und verhindert die Übernutzung.
* **Volkswirtschaftlicher Nutzen durch Bildung:** Positive Externalität. Schafft unkompensierten Zusatznutzen für unbeteiligte Dritte.
* **Modelltheoretisches Axiom:** Annahme. Ein Sachverhalt, der als wahr akzeptiert wird, ohne bewiesen werden zu müssen, um Komplexität zu reduzieren.
* **Rationaler Akteur:** Homo Oeconomicus. Fiktives Subjekt, das vollständig rational handelt und konstante Kosten-Nutzen-Abwägungen trifft.

#### 1.2. Zeithorizonte in der Mikroökonomik
* **Kurze Frist:** Mindestens ein Produktionsfaktor ist starr (fix). Daraus resultiert die Existenz von Fixkosten ($FC$).
* **Lange Frist:** Zeitraum, in dem alle Produktionsfaktoren vollständig variabel sind. Daraus folgt: Gesamtkosten enthalten keine Fixkosten ($FC = 0$), alle Kosten sind variabel ($VC$).

#### 1.3. Buchhalterischer vs. Ökonomischer Gewinn
* **Explizite Kosten:** Tatsächliche monetäre Ausgaben ($650.000\$ + 155.000\$ + 185.000\$ = 990.000\$$).
* **Implizite Kosten / Opportunitätskosten:** Entgangener Nutzen der nächstbesten Alternative (Mieteinnahmen: $35.000\$$).

$$\text{Buchhalterischer Gewinn} = \text{Umsatz} - \text{Explizite Kosten} = 1.000.000\$ - 990.000\$ = 10.000\$$$
$$\text{Ökonomischer Gewinn} = \text{Buchhalterischer Gewinn} - \text{Implizite Kosten} = 10.000\$ - 35.000\$ = -25.000\$$$

##### Ökonomische Handlungsempfehlung
Da der ökonomische Gewinn negativ ist ($\pi_{ök} < 0$), ist die Fortführung der Produktion ineffizient. Das Unternehmen sollte die Produktion einstellen und das Grundstück vermieten, da die Opportunitätskosten der Eigennutzung zu hoch sind.

#### 1.4. Allmendegüter-Problematik
* **Zentrale Problematik:** Fluch der Allmendegüter (Tragedy of the Commons).
* **Ursache:** Fehlen von exklusiven Eigentumsrechten gepaart mit Nicht-Ausschließbarkeit bei gleichzeitiger Rivalität im Konsum. Dies führt unreguliert zur vollständigen Degradierung/Übernutzung der Ressource.

---

### 2. Aufgabe 2: Konsumententheorie (Nutzenmaximierung)

#### 2.1. Gegebene Parameter
* **Budget ($I$):** $800\text{ €}$
* **Preise:** $p_1 = 25\text{ €}$, $p_2 = 40\text{ €}$
* **Nutzenfunktion ($U$):** $U(q_1, q_2) = q_1^2 \cdot q_2$

#### 2.2. Analytische Bestimmung des Haushaltsoptimums via Lagrange

##### Schritt 1: Formulierung der Budgetbeschränkung (BC)
$$25q_1 + 40q_2 = 800 \implies 800 - 25q_1 - 40q_2 = 0$$

##### Schritt 2: Aufstellen der Lagrange-Funktion ($\mathcal{L}$)
$$\mathcal{L}(q_1, q_2, \lambda) = q_1^2 \cdot q_2 + \lambda(800 - 25q_1 - 40q_2)$$

##### Schritt 3: Bedingungen erster Ordnung (FOC)
$$\text{(I)} \quad \frac{\partial \mathcal{L}}{\partial q_1} = 2q_1q_2 - 25\lambda \stackrel{!}{=} 0 \implies 2q_1q_2 = 25\lambda$$
$$\text{(II)} \quad \frac{\partial \mathcal{L}}{\partial q_2} = q_1^2 - 40\lambda \stackrel{!}{=} 0 \implies q_1^2 = 40\lambda$$
$$\text{(III)} \quad \frac{\partial \mathcal{L}}{\partial \lambda} = 800 - 25q_1 - 40q_2 \stackrel{!}{=} 0$$

##### Schritt 4: Bestimmung der Optimalitätsbedingung (GRS = relatives Preisverhältnis)
Division von $\text{(I)}$ durch $\text{(II)}$:
$$\frac{2q_1q_2}{q_1^2} = \frac{25\lambda}{40\lambda} \implies \frac{2q_2}{q_1} = \frac{25}{40} \implies \frac{2q_2}{q_1} = \frac{5}{8}$$
$$16q_2 = 5q_1 \implies q_2 = \frac{5}{16}q_1$$

##### Schritt 5: Substitution in die Budgetbeschränkung $\text{(III)}$
$$25q_1 + 40 \left(\frac{5}{16}q_1\right) = 800$$
$$25q_1 + 12.5q_1 = 800 \implies 37.5q_1 = 800$$
$$q_1^* = \frac{800}{37.5} \approx \mathbf{21.33}$$

##### Schritt 6: Berechnung der optimalen Menge $q_2^*$
$$q_2^* = \frac{5}{16} \cdot 21.3333 \approx \mathbf{6.67}$$

##### Schritt 7: Berechnung des optimalen Lagrange-Multiplikators $\lambda^*$
Nutze umgestellte Gleichung $\text{(II)}$:
$$\lambda^* = \frac{q_1^2}{40} = \frac{(21.3333)^2}{40} \approx \mathbf{11.38}$$

#### 2.3. Berechnung des maximalen Nutzenniveaus ($U^*$)
$$U^*(q_1^*, q_2^*) = (21.33)^2 \cdot 6.67 \approx \mathbf{3034.64}$$

## Aufgabe 3: Preiselastizität der Nachfrage

## 3. Preiselastizität am Beispiel des Weihnachtsbaummarktes

### 3.1. Mathematische Bestimmung der Elastizität

#### Gegebene Parameter
* **Nachfragefunktion ($q$):** $q = 200 - 5p$
* **Aktuelles Preisniveau ($p$):** $p = 30$
* **Elastizitätsformel ($\epsilon$):** $\epsilon = \frac{\partial q}{\partial p} \cdot \frac{p}{q}$

#### Schritt 1: Berechnung der nachgefragten Menge ($q$)
Einsetzen des Preisniveaus $p = 30$ in die Nachfragefunktion:
$$q = 200 - 5 \cdot 30 = 200 - 150 = \mathbf{50}$$

#### Schritt 2: Partielle Ableitung nach dem Preis ($\frac{\partial q}{\partial p}$)
$$\frac{\partial q}{\partial p} = -5$$

#### Schritt 3: Berechnung des Elastizitätswerts ($\epsilon$)
Einsetzen der berechneten Komponenten in die Elastizitätsformel:
$$\epsilon = -5 \cdot \frac{30}{50} = -5 \cdot 0,6 = \mathbf{-3}$$

---

### 3.2. Ökonomische Interpretation und Klassifikation

* **Elastizitätsklassifikation:** Da der Betrag der Preiselastizität größer als 1 ist ($|\epsilon| = 3 > 1$), ist die Nachfrage als **elastisch** einzustufen. Die prozentuale Änderung der nachgefragten Menge ist demnach größer als die prozentuale Änderung des Preises.
* **Kausalität:** Eine Preiserhöhung um $1\,\%$ induziert eine Verringerung der nachgefragten Menge um exakt $3\,\%$.

---

### 3.3. Determinanten der Preiselastizität der Nachfrage

Die Reagibilität der Nachfrage auf Preisänderungen wird primär durch folgende strukturelle Faktoren beeinflusst:

* **Verfügbarkeit von Substituten:** Je mehr Substitutionsgüter (Ersatzprodukte) existieren, desto elastischer reagiert die Nachfrage, da Konsumenten bei Preissteigerungen effizient ausweichen können.
* **Dringlichkeit des Bedarfs (Lebensnotwendige vs. Luxusgüter):** Lebensnotwendige Güter weisen eine unelastische Nachfrage auf, da auf sie kaum verzichtet werden kann. Bei Luxusgütern ist die Nachfrage elastisch, da der Konsum optional ist oder aufgeschoben werden kann.
* **Einkommensanteil für das Produkt:** Beansprucht ein Gut einen großen Anteil des verfügbaren Budgets, reagieren Konsumenten preissensibler (elastische Nachfrage) als bei Gütern mit einem marginalen Einkommensanteil.

