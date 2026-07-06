# Das 1. Gossensche Gesetz: Der abnehmende Grenznutzen
## 1. Grenznutzen (Marginal Utility)
Der **Grenznutzen (MU)** ist der zusätzliche Nutzen, den ein Konsument durch den Konsum einer weiteren Einheit eines Gutes (z. B. eines Kekses) erfährt.
* **Mathematische Definition:** $MU_1 = \frac{\Delta U}{\Delta q_1}$
* **Verlauf:** Während der Gesamtnutzen mit jeder konsumierten Einheit steigt, nimmt der *Zusatznutzen* (Grenznutzen) der jeweils nächsten Einheit immer weiter ab.
## 2. Die Nutzenfunktion $U = f(q_1)$
Die grafische Darstellung des Nutzens zeigt zwei wesentliche Eigenschaften:
* **Steigender Verlauf ($U' > 0$):** Mehr Konsum führt grundsätzlich zu mehr Gesamtnutzen.
* **Konkave Krümmung ($U'' < 0$):** Die Kurve flacht ab. Das bedeutet, der Zuwachs an Glücksempfinden wird immer kleiner.
    * *Beispiel:* Der erste Keks bei großem Hunger bringt einen enormen Nutzen. Der vierte Keks hingegen wird oft nur noch aus Gewohnheit gegessen und bietet kaum noch einen Mehrwert.
## 3. Mathematische Modellierung: Cobb-Douglas
Ein spezieller und häufig verwendeter Fall in der Mikroökonomie zur Darstellung dieses Verhaltens ist die **Cobb-Douglas-Funktion**:

$$U = q_1^\alpha q_2^{1-\alpha} \quad (\text{mit } 0 < \alpha < 1)$$

Diese Funktion stellt sicher, dass die Annahmen des abnehmenden Grenznutzens mathematisch konsistent abgebildet werden.

![[Pasted image 20260424074633.png]]

----

![[Pasted image 20260424075223.png]]

![[Pasted image 20260424075433.png]]

# Die Grenze der Realität: Die Budgetrestriktion
## 1. Die Budgetgleichung
Die ökonomische Grundregel lautet: Man kann nicht mehr ausgeben, als man hat. Das verfügbare Einkommen wird vollständig für den Konsum von Gütern aufgewendet.

$$I = q_1 p_1 + q_2 p_2$$

* **$I$ (Income):** Das verfügbare Einkommen.
* **$q_1, q_2$ (Quantities):** Die Mengen der konsumierten Güter 1 und 2.
* **$p_1, p_2$ (Prices):** Die Preise der jeweiligen Güter.
## 2. Grafische Darstellung: Die Budgetgerade
Die Budgetgerade trennt den leistbaren Bereich vom unleistbaren Bereich
* **Leistbarer Bereich:** Die Fläche unterhalb und auf der Budgetgeraden. Hier reicht das Einkommen aus.
* **Unleistbar:** Die Fläche oberhalb der Budgetgeraden. Diese Güterkombinationen übersteigen das Budget.
## 3. Die Steigung und Opportunitätskosten
Die Steigung der Budgetgeraden ist ein zentrales Maß für ökonomische Entscheidungen.

> [!IMPORTANT] Der relative Preis
> Die Steigung entspricht dem Preisverhältnis der beiden Güter: $-\frac{p_1}{p_2}$.
> Dies repräsentiert die **Opportunitätskosten**: Sie gibt an, auf wie viele Einheiten von Gut 2 man verzichten muss, um eine zusätzliche Einheit von Gut 1 zu erhalten.

![[Pasted image 20260424080031.png]]
# Das Optimum: Wo Wollen auf Können trifft
## 1. Die Komponenten des Modells
Um das Optimum zu bestimmen, werden zwei Konzepte zusammengeführt:
* **Indifferenzkurven (IC):** Repräsentieren das "Wollen". Höhere Kurven ($IC_3$) stehen für ein höheres Nutzenniveau.
* **Budgetgerade (BC):** Repräsentiert das "Können". Sie zeigt alle Kombinationen von Gut 1 und Gut 2, die mit dem vorhandenen Einkommen finanzierbar sind.
## 2. Analyse der verschiedenen Bereiche

| Bereich | Beschreibung | Ökonomische Einordnung |
| :--- | :--- | :--- |
| **Unerreichbar ($IC_3$)** | Höchster Nutzen, liegt aber außerhalb der Budgetgeraden. | Budget reicht nicht aus. |
| **Suboptimal ($IC_1$)** | Punkte auf der Budgetgeraden, die eine niedrigere Indifferenzkurve schneiden. | Leistbar, aber durch Umschichtung des Budgets kann ein höherer Nutzen erreicht werden. |
| **Das Optimum ($IC_2$)** | Der Punkt, an dem die Budgetgerade die höchstmögliche Indifferenzkurve gerade noch **tangiert**. | **Maximaler Nutzen** bei gegebenem Budget. |

## 3. Die Optimalitätsbedingung
Im Optimum entspricht die subjektive Austauschbereitschaft des Konsumenten genau dem objektiven Preisverhältnis am Markt.

> [!IMPORTANT] Die goldene Regel des Konsums
> **GRS = $p_1 / p_2$**
> *(Subjektives Tauschverhältnis = Objektives Markt-Tauschverhältnis)*

* **GRS (Grenzrate der Substitution):** Die Steigung der Indifferenzkurve. Sie gibt an, wie viel von Gut 2 man bereit ist aufzugeben, um eine Einheit mehr von Gut 1 zu erhalten.
* **$p_1 / p_2$:** Die Steigung der Budgetgeraden (Relativpreis).


![[Pasted image 20260424080558.png]]

# Die Mathematik der Entscheidung: Die Lagrange-Methode
## Der 3-Schritte-Prozes
### Step 1: Setup (Die Funktion aufstellen)
Die Lagrange-Funktion ($\mathcal{L}$) verbindet die Zielfunktion (Nutzen) mit der Nebenbedingung (Budget), multipliziert mit dem Lagrange-Multiplikator $\lambda$.

$$\mathcal{L} = U(q_1, q_2) + \lambda(I - q_1 p_1 - q_2 p_2)$$

* **Funktion:** Sie integriert das Budgetdefizit direkt in die zu optimierende Gleichung.
* **$\lambda$:** Der Multiplikator gibt den Grenznutzen des Einkommens an
### Step 2: Ableiten (Bedingungen 1. Ordnung)
Um das Maximum zu finden, werden die partiellen Ableitungen nach allen Variablen gebildet und Null gesetzt (FOC – First Order Conditions).

1.  $\frac{\partial \mathcal{L}}{\partial q_1} = 0$
2.  $\frac{\partial \mathcal{L}}{\partial q_2} = 0$
3.  $\frac{\partial \mathcal{L}}{\partial \lambda} = 0$
### Step 3: Lösen (Das Gleichungssystem)
Das resultierende System aus drei Gleichungen wird nun systematisch aufgelöst, um die optimalen Mengen ($q_1^*$ und $q_2^*$) zu bestimmen.
* **Vorgehensweise:** Meist werden die ersten beiden Gleichungen durcheinander dividiert, um $\lambda$ zu eliminieren.
* **Resultat:** Man erhält das optimale Verhältnis der Güter zueinander, welches dann in die Budgetbeschränkung (3. Gleichung) eingesetzt wird.
## Mathematische Zusammenfassung

| Schritt | Fokus | Mathematische Operation |
| :--- | :--- | :--- |
| **1. Modellierung** | Lagrange-Ansatz | $U + \lambda \cdot (\text{Budgetrestriktion})$ |
| **2. Optimierung** | Partielle Ableitungen | Gradient $\nabla \mathcal{L} = 0$ bilden |
| **3. Allokation** | Auflösen | Berechnung von $q_1^*$ und $q_2^*$ |

> [!TIP] Der ökonomische Kern
> Durch das Dividieren der Ableitungen nach $q_1$ und $q_2$ erhält man im Gleichgewicht die Bedingung:
> $$\frac{\partial U / \partial q_1}{\partial U / \partial q_2} = \frac{p_1}{p_2}$$
> Dies entspricht exakt der Bedingung **Grenznutzenverhältnis = Preisverhältnis**.

![[Pasted image 20260424082127.png]]

# Von der Entscheidung zur Nachfrage
## 1. Herleitung der Nachfragekurve
Die individuelle Nachfragekurve (D) ist die grafische Zusammenfassung aller optimalen Konsumentscheidungen, die ein Individuum bei variierenden Preisen eines Gutes trifft.
* **Variation des Preises:** Wenn der Preis von Gut 1 sinkt (z. B. von $2$ auf $1$), flacht die Budgetgerade ($BC_1 \rightarrow BC_2$) ab.
* **Neues Optimum:** Der Konsument erreicht eine höhere Indifferenzkurve ($IC_2$) und wählt eine neue optimale Menge (von 250 auf 750 Einheiten).
* **Übertragung:** Die Kombinationen aus Preis ($p$) und optimaler Menge ($q$) bilden die Punkte auf der Nachfragekurve im unteren Diagramm.
## 2. Das Gesetz der Nachfrage
Das Modell bestätigt eine fundamentale ökonomische Regel:

> [!IMPORTANT] Das Gesetz der Nachfrage
> Wenn der Preis eines Gutes fällt ($p \downarrow$), steigt die nachgefragte Menge ($q \uparrow$), vorausgesetzt, alle anderen Faktoren bleiben gleich (**ceteris paribus**).

Die Nachfragekurve hat daher im Standardfall eine **negative Steigung**.
## 3. Grafische Analyse im Vergleich

| Ebene                          | Achsen        | Darstellung                                                                           |
| :----------------------------- | :------------ | :------------------------------------------------------------------------------------ |
| **Obere Ebene (Entscheidung)** | Gut 2 / Gut 1 | Zeigt das ***Optimum*** durch Tangentialpunkte von Budgetgerade und Indifferenzkurve. |
| **Untere Ebene (Nachfrage)**   | Preis / Menge | Zeigt die ***Nachfragekurve (D)*** als direkte Korrelation zwischen Preis und Menge.  |

![[Pasted image 20260424082411.png]]

![[Pasted image 20260424082956.png]]

# Reaktionsfähigkeit: Die Preiselastizität der Nachfrage (PED)
## 1. Definition & Mathematische Basis
Die PED quantifiziert die prozentuale Änderung der Nachfragemenge als Reaktion auf eine Preisänderung von einem Prozent.

> [!MATH] Formel
> $$\epsilon \approx \frac{\partial q}{\partial p} \cdot \frac{p}{q}$$
## 2. Kategorisierung der Elastizität
Je nachdem, wie stark Konsumenten ihr Verhalten anpassen, unterscheidet man drei Hauptstufen. Diese lassen sich physikalisch durch den Widerstand eines Objekts gegen eine einwirkende Kraft veranschaulichen:
### $|\epsilon| < 1$: Unelastische Nachfrage
* **Charakteristik:** Die Mengenänderung ist proportional geringer als die Preisänderung.
* **Ursache:** Es handelt sich oft um lebensnotwendige Güter ohne nahe Substitute.
* **Beispiel:** Medikamente (Insulin), Grundnahrungsmittel, Treibstoff.
* **Visualisierung:** Ein massiver Block, der sich trotz starkem Druck (Preisänderung) kaum bewegt.
### $|\epsilon| = 1$: Proportionalelastische Nachfrage
* ***Charakteristik*:** Die Menge sinkt im exakt gleichen Verhältnis, in dem der Preis steigt.
* ***Bedeutung*:** Die Gesamtausgaben der Konsumenten (Umsatz der Anbieter) bleiben bei Preisänderungen konstant.
### $|\epsilon| > 1$: Elastische Nachfrage
* **Charakteristik:** Die Mengenänderung ist proportional stärker als die Preisänderung.
* **Ursache:** Luxusgüter, Güter mit vielen Substituten oder ein langer Beobachtungszeitraum.
* **Beispiel:** Urlaubsreisen, spezifische Markenprodukte (z. B. eine bestimmte Schokoladensorte).
* **Visualisierung:** Eine weiche Feder, die schon bei geringem Druck weit ausschlägt.
## 3. Bestimmungsfaktoren

| Faktor              | Auswirkung auf die Elastizität                                                                  |
| :------------------ | :---------------------------------------------------------------------------------------------- |
| ***Substitute***    | Je mehr Ersatzprodukte existieren, desto **höher** (elastischer) ist die PED.                   |
| ***Dringlichkeit*** | Je notwendiger das Gut, desto **niedriger** (unelastischer) ist die PED.                        |
| ***Budgetanteil***  | Je größer der Anteil am Einkommen, desto **elastischer** reagieren Käufer.                      |
| ***Zeithorizont***  | Langfristig ist die Nachfrage meist **elastischer**, da Konsumenten Alternativen finden können. |

# Die Matrix der Gütertypen: XED & Einkommenselastizität
## 1. Kreuzpreiselastizität (XED)
Die Kreuzpreiselastizität misst, wie die Nachfrage nach **Gut 1** reagiert, wenn sich der Preis von **Gut 2** ändert.

| Elastizität             | Gütertyp                | Dynamik                                                     | Beispiel                 |
| :---------------------- | :---------------------- | :---------------------------------------------------------- | :----------------------- |
| **$\epsilon_{12} > 0$** | ***Substitute***        | Preis Gut 2 $\uparrow \rightarrow$ Menge Gut 1 $\uparrow$   | Butter & Margarine       |
| **$\epsilon_{12} < 0$** | ***Komplementärgüter*** | Preis Gut 2 $\uparrow \rightarrow$ Menge Gut 1 $\downarrow$ | Drucker & Patronen       |
| **$\epsilon_{12} = 0$** | ***Unabhängig***        | Keine gegenseitige Beeinflussung.                           | Zahnbürsten & Autoreifen |
## 2. Einkommenselastizität
Die Einkommenselastizität misst, wie sich die Nachfrage nach einem Gut verändert, wenn das Einkommen des Konsumenten steigt oder sinkt.
### Normales (superiores) Gut ($\epsilon > 0$)
* **Reaktion:** Einkommen $\uparrow \rightarrow$ Nachfrage $\uparrow$.
* **Charakteristik:** Mit steigendem Wohlstand leisten sich Menschen mehr von diesen Gütern (z. B. Restaurantbesuche, Markenkleidung).

### Inferiores Gut ($\epsilon < 0$)
* **Reaktion:** Einkommen $\uparrow \rightarrow$ Nachfrage $\downarrow$.
* **Charakteristik:** Diese Güter werden bei steigendem Einkommen durch hochwertigere Alternativen ersetzt.
* **Beispiel:** Tütensuppen oder billige No-Name-Produkte werden durch frische Lebensmittel ersetzt.

> [!TIP] Merkregel
> * ***XED*** beantwortet: „In welcher Beziehung stehen zwei Produkte zueinander?“ (Ersatz oder Ergänzung)
> * ***Einkommenselastizität*** beantwortet: „Welchen Stellenwert hat das Produkt im Budget bei steigendem Wohlstand?“

![[Pasted image 20260424083936.png]]

![[Pasted image 20260424084139.png]]

