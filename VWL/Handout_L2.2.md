# Die Optimale Konsumentenentscheidung

![[Pasted image 20260508143353.png]]
## 1. Was der Konsument möchte: Präferenzen
Der Konsument strebt nach der Maximierung seines persönlichen Wohlbefindens bzw. Nutzens.
* ***Indifferenzkurven* ($U_1, U_2, U_3$):** Diese Kurven stellen Güterbündel dar, die dem Konsumenten den gleichen Nutzen stiften.
* ***Nutzenmaximierung*:** Kurven, die weiter vom Ursprung entfernt liegen, repräsentieren ein höheres Nutzniveau ($U_3 > U_2 > U_1$).
* ***Ziel*:** Das Erreichen der höchstmöglichen Indifferenzkurve.
## 2. Was der Konsument sich leisten kann: Die Budgetbeschränkung
Die finanziellen Mittel und die Marktpreise setzen der Konsumfreiheit Grenzen.
* ***Budgetlinie*:** Sie zeigt alle Kombinationen von Gut A und Gut B, für die der Konsument sein gesamtes Budget ausgibt.
* ***Formel*:** $P_A \cdot A + P_B \cdot B = \text{Budget}$
* ***Bereiche*:**
	* **Leistbarer Bereich:** Alles auf oder unterhalb der Budgetlinie.
	* **Nicht leistbarer Bereich:** Alle Punkte oberhalb der Linie überschreiten die verfügbaren Ressourcen.
## 3. Die Optimale Entscheidung (Das Optimum)
Die optimale Konsumentenentscheidung wird im Punkt **$E$** (Optimum) erreicht, an dem sich Wünsche und Möglichkeiten treffen.
### Definition des Optimums
Ein rationaler Konsument (**Homo Oeconomicus**) wählt das Güterbündel auf der höchsten erreichbaren Indifferenzkurve, das exakt das Budget ausschöpft.

> [!IMPORTANT] **Mathematische Bedingung**
> Im Optimum ist die Budgetlinie eine **Tangente** zur Indifferenzkurve. Das bedeutet, die Steigung der Budgetlinie entspricht der Grenzrate der Substitution.
### Komponenten des Optimums
| Merkmal | Beschreibung |
| :--- | :--- |
| **Optimale Menge Gut A ($A^*$)** | Die Menge von Gut A, die im Gleichgewicht konsumiert wird. |
| **Optimale Menge Gut B ($B^*$)** | Die Menge von Gut B, die im Gleichgewicht konsumiert wird. |
| **Budgetstatus** | Das Budget ist im Punkt $E$ vollständig ausgeschöpft. |
| **Nutzenstatus** | Erreicht das höchste für dieses Budget realisierbare Niveau ($U_2$). |
# Die Optimale Konsumentenentscheidung: Das Tangentialpunkt-Kriterium

![[Pasted image 20260508143900.png]]
## 1. Die Kernkomponenten der Steigung
Um das Optimum zu verstehen, müssen die Steigungen der beiden Kurven betrachtet werden:
* **Steigung der Indifferenzkurve ($IC$):** Entspricht der **Grenzrate der Substitution ($GRS$)**. Sie stellt den *subjektiven Tauschwillen* dar – also wie viel von Gut A der Konsument bereit ist aufzugeben, um eine zusätzliche Einheit von Gut B zu erhalten.
* **Steigung der Budgetgeraden ($BC$):** Entspricht dem **Preisverhältnis ($\frac{p_1}{p_2}$)**. Sie stellt das *objektive Markttauschverhältnis* dar – also wie viel von Gut A der Konsument tatsächlich aufgeben muss, um am Markt eine Einheit von Gut B zu kaufen.
## 2. Das Optimum (Punkt E)
Das Optimum wird dort erreicht, wo die Budgetlinie die höchstmögliche Indifferenzkurve ($IC_2$) gerade noch berührt. In diesem **Tangentialpunkt** stimmen beide Steigungen exakt überein.
### Die Gleichgewichtsbedingung
$$GRS = \frac{p_1}{p_2}$$

> [!NOTE] **Bedeutung**
> Im Optimum entspricht der individuelle **Tauschwille** des Konsumenten exakt der **Tauschmöglichkeit** (Realität) des Marktes.
## 3. Analyse der Indifferenzkurven

| Kurve | Status | Beschreibung |
| :--- | :--- | :--- |
| **$IC_1$** | Ineffizient | Die Kurve wird an zwei Stellen geschnitten. Der Konsument könnte durch Umverteilung ein höheres Nutzniveau erreichen. |
| **$IC_2$** | **Optimal** | Tangentialpunkt zur Budgetlinie. Das maximale Nutzniveau innerhalb des Budgets ist erreicht. |
| **$IC_3$** | Nicht leistbar | Diese Kurve liegt vollständig außerhalb des durch die Budgetbeschränkung ($BC$) definierten Bereichs. |

> [!TIP] **Zusammenfassung**
> Ein rationaler Konsument passt seinen Konsum so lange an, bis sein persönliches Grenznutzenverhältnis dem Verhältnis der Marktpreise entspricht. Jede Abweichung von diesem Punkt würde entweder das Budget überschreiten oder ein geringeres Nutzniveau bedeuten.

# Die Lagrange-Methode: Eine Optimierungsmaschine

![[Pasted image 20260508144254.png]]
## 1. Der Input: Die Bausteine
Bevor die "Maschine" arbeiten kann, benötigt sie zwei grundlegende mathematische Eingaben:
* ***Nutzenfunktion* $U(q_1, q_2)$:** Beschreibt die Präferenzen des Konsumenten für verschiedene Mengen der Güter 1 und 2.
* ***Budgetbeschränkung* ($BC$):** Die Nebenbedingung, die meist in die Form Null gesetzt wird:
    $$I - q_1p_1 - q_2p_2 = 0$$
    *(Wobei $I$ das Einkommen, $q$ die Mengen und $p$ die Preise darstellen).*
## 2. Die Lagrange-Funktion
Die beiden Inputs werden in einer einzigen Funktion kombiniert:
$$\mathcal{L} = U(q_1, q_2) + \lambda(I - q_1p_1 - q_2p_2)$$

* **$\lambda$ (Lagrange-Multiplikator):** Eine Hilfsvariable, die den Grenznutzen des Geldes (Einkommens) repräsentiert.
## 3. Der Prozess: Ableitungen bilden (FOC)
Um das Maximum zu finden, müssen die partiellen Ableitungen der Lagrange-Funktion gebildet und gleich Null gesetzt werden (**Bedingungen erster Ordnung / First Order Conditions**):
1.  ***Ableitung nach* $q_1$:** $$\frac{\partial \mathcal{L}}{\partial q_1} = 0$$
2.  ***Ableitung nach* $q_2$:** $$\frac{\partial \mathcal{L}}{\partial q_2} = 0$$
3.  ***Ableitung nach* $\lambda$:** $$\frac{\partial \mathcal{L}}{\partial \lambda} = 0$$ 
    *(Dies stellt sicher, dass die Budgetbeschränkung exakt erfüllt ist).*
## 4. Der Output: Das Ergebnis
Durch das Lösen dieses Gleichungssystems erhält man die optimalen Verbrauchsmengen:

> [!ABSTRACT] **Optimales Güterbündel: $q_1^*, q_2^*$**
> Dies sind die Mengen der Güter 1 und 2, die dem Konsumenten unter Einhaltung seines Budgets den höchstmöglichen Nutzen liefern.

> [!INFO] **Vorteil der Methode**
> Die Lagrange-Methode verwandelt ein komplexes Optimierungsproblem mit Nebenbedingungen in ein einfacheres Problem ohne Nebenbedingungen, das durch Standard-Differentialrechnung gelöst werden kann.

# Die Langrange-Lösung

![[Pasted image 20260508144538.png]]

# Der Einkommensschock (Normale Güter)

![[Pasted image 20260508145325.png]]
## 1. Die Verschiebung der Budgetgerade
Wenn das Einkommen sinkt, verringert sich der Handlungsspielraum des Konsumenten linear.
* ***Parallele Verschiebung*:** Da sich die Preise ($p_1, p_2$) nicht ändern, bleibt die Steigung der Budgetgerade ($-\frac{p_1}{p_2}$) gleich. Die Gerade verschiebt sich parallel nach innen (von $BC$ zu $BC'$).
* ***Verengung des leistbaren Bereichs*:** Der Konsument kann sich nun von beiden Gütern weniger leisten. Die Achsenabschnitte rücken näher an den Ursprung.
## 2. Anpassung des Optimums
Die Senkung des Einkommens zwingt den Konsumenten, auf ein niedrigeres Nutzniveau auszuweichen.
* ***Vom alten zum neuen Optimum*:** Der Konsument muss das neue Optimum dort finden, wo die neue Budgetgerade $BC'$ die höchstmögliche (aber nun niedrigere) Indifferenzkurve $U_2$ tangiert.
* ***Nutzenverlust*:** Da das neue Optimum auf einer Indifferenzkurve näher am Ursprung liegt ($U_2 < U_1$), sinkt der Gesamtnutzen des Konsumenten.
## 3. Klassifizierung: Normale Güter
Das Diagramm zeigt die Reaktion für **normale Güter**.

> [!IMPORTANT] **Definition: Normales Gut**
> Ein Gut wird als "normal" bezeichnet, wenn die Nachfrage danach bei sinkendem Einkommen ebenfalls sinkt (und bei steigendem Einkommen steigt).

| Merkmal | Beobachtung im Diagramm |
| :--- | :--- |
| **Menge Gut 1 ($q_1$)** | Sinkt im Vergleich zum alten Optimum. |
| **Menge Gut 2 ($q_2$)** | Sinkt im Vergleich zum alten Optimum. |
| **Einkommenseffekt** | Positiv (Nachfrage folgt der Einkommensentwicklung). |


> [!INFO] **Kernbotschaft**
> Bei einem negativen Einkommensschock und ausschließlich normalen Gütern führt die parallele Innenverschiebung der Budgetbeschränkung zu einer Reduktion der Konsummenge beider Güter und einem Rückgang des Wohlbefindens.

# Der Preisschock: Rotation der Budgetgeraden

![[Pasted image 20260508145726.png]]
## 1. Mechanik der Rotation
Wenn der Preis eines Gutes (hier: Cola) sinkt, verändert sich das Austauschverhältnis zwischen den Gütern.
* ***Der Ankerpunkt (Pizza):*** Da sich weder das Einkommen noch der Preis für Pizza geändert haben, bleibt der maximale Achsenabschnitt für Pizza (hier bei 100 Einheiten) starr.
* ***Rotation nach außen*:** Die Kaufkraft für Cola steigt. Der Konsument könnte nun maximal 1000 statt 500 Einheiten Cola kaufen. Die Budgetgerade rotiert vom Ursprung aus gesehen nach außen ($BC \to BC'$).
* ***Relative Preise*:** Die Budgetgerade wird **flacher**, da das Preisverhältnis $p_{Cola} / p_{Pizza}$ gesunken ist.
## 2. Auswirkungen auf das Optimum
Durch die Preisänderung verschiebt sich das Gleichgewicht des Konsumenten hin zu einem neuen Konsumbündel.
* ***Nutzensteigerung*:** Da die neue Budgetgerade $BC'$ nun Indifferenzkurven erreicht, die weiter vom Ursprung entfernt liegen, steigt das Nutzniveau ($IC_1 \to IC_2$).
* ***Substitutions- und Einkommenseffekt*:**
    * Der Konsument tendiert dazu, mehr von dem nun relativ günstigeren Gut (Cola) zu konsumieren.
    * Die effektive Kaufkraft ist gestiegen, was den Konsum beider Güter beeinflussen kann (je nach Gutstyp).
## 3. Vergleich der Optima

| Merkmal | Altes Optimum | Neues Optimum |
| :--- | :--- | :--- |
| **Budgetgerade** | Steiler ($BC$) | Flacher ($BC'$) |
| **Indifferenzkurve** | Niedrigeres Niveau ($IC_1$) | Höheres Niveau ($IC_2$) |
| **Kaufkraft** | Begrenzt auf max. 500 Cola | Erweitert auf max. 1000 Cola |

> [!TIP] **Merksatz**
> Eine Preisänderung bewirkt immer eine **Rotation** der Budgetgeraden um den Achsenabschnitt des Gutes, dessen Preis **konstant** geblieben ist.

# Dekonstruktion: Substitutions- und Einkommenseffekt

![[Pasted image 20260508150104.png]]
## 1. Der Substitutionseffekt (SE)
Der SE isoliert die reine Änderung des relativen Preisverhältnisses, ohne die Änderung der Kaufkraft zu berücksichtigen.
* ***Mechanismus*:** Wenn Cola billiger wird, tauscht der Konsument das nun relativ teurer gewordene Gut (Pizza) gegen das günstigere Gut (Cola) aus.
* ***Grafische Darstellung*:** Bewegung entlang der ursprünglichen Indifferenzkurve ($IC_1$) bis zu einem "hypothetical point". Hier wird die Steigung der neuen Budgetgeraden ($BC'$) simuliert, während das reale Nutzniveau konstant bleibt.
* ***Richtung*:** Der SE wirkt immer entgegen der Preisänderung (Preis sinkt $\to$ Nachfrage durch SE steigt).
## 2. Der Einkommenseffekt (EE)
Der EE beschreibt die Reaktion auf die durch den Preisverfall gestiegene reale Kaufkraft.
* ***Mechanismus*:** Da Cola billiger geworden ist, bleibt dem Konsumenten beim Kauf der gleichen Menge mehr Geld übrig. Er ist "real reicher" geworden.
* ***Grafische Darstellung*:** Verschiebung vom "hypothetical point" auf der ursprünglichen Kurve zum endgültigen **neuen Optimum** auf der höheren Indifferenzkurve ($IC_2$).
* ***Richtung*:** Bei normalen Gütern verstärkt der EE den Substitutionseffekt (Nachfrage steigt weiter).
## 3. Die Gesamteffekte im Überblick

| Effekt | Ursache | Grafische Bewegung | Fokus |
| :--- | :--- | :--- | :--- |
| **Substitutionseffekt** | Neuer relativer Preis | Entlang der Kurve ($IC_1$) | Reiner Tauschwille |
| **Einkommenseffekt** | Höhere reale Kaufkraft | Auf eine höhere Kurve ($IC_2$) | Reale Kaufkraftänderung |
| **Gesamteffekt** | Preisänderung | Vom Ursprungs- zum Zieloptimum | Summe aus SE + EE |

> [!IMPORTANT] **Anatomie der Preisänderung**
> Jeder Preisschock besteht aus diesen zwei unsichtbaren Bewegungen. Während der **Substitutionseffekt** das Verhalten bei gleichbleibendem Wohlbefinden isoliert, zeigt der **Einkommenseffekt**, wie der Konsument von seinem gestiegenen Realeinkommen profitiert.

# Vergleichsmatrix: Substitutionseffekt vs. Einkommenseffekt

![[Pasted image 20260508150603.png]]
## Detaillierte Analyse
### Substitutionseffekt (SE)
* ***Mechanismus***: Der SE isoliert die Preisänderung von der Kaufkraftänderung.
* ***Verhalten***: Selbst wenn das reale Einkommen konstant gehalten würde, sorgt der SE dafür, dass der Konsument mehr vom günstigeren Gut nachfragt.
* ***Grafische Kennzeichnung***: Markiert durch eine Gleitbewegung auf der ursprünglichen Nutzenkurve, um das neue Preisverhältnis abzubilden.
### Einkommenseffekt (EE)
* ***Mechanismus***: Der Preisverfall eines Gutes wirkt wie eine Erhöhung des Realeinkommens.
* ***Verhalten***: Der Konsument nutzt diesen "Zuwachs", um ein höheres Nutzniveau zu erreichen.
* ***Grafische Kennzeichnung***: Sichtbar durch den Sprung von einer niedrigeren auf eine höhere Indifferenzkurve.

> [!INFO] **Zusammenfassung**
> Während der **Substitutionseffekt** beschreibt, wie wir Güter aufgrund ihres Preises gegeneinander **austauschen**, beschreibt der **Einkommenseffekt**, wie sich unser Konsumverhalten durch die Veränderung unseres **Wohlstandes** anpasst.

# Giffen-Güter: Wenn der Einkommenseffekt den Substitutionseffekt dominiert

![[Pasted image 20260508150755.png]]
## 1. Die Besonderheit des Giffen-Guts
Damit ein Gut als Giffen-Gut klassifiziert werden kann, müssen zwei Bedingungen erfüllt sein:
1.  Es handelt sich um ein **inferiores Gut** (bei steigendem Einkommen sinkt die Nachfrage).
2.  Der **Einkommenseffekt (EE)** ist so stark, dass er den **Substitutionseffekt (SE)** überlagert.
## 2. Analyse der Effekte im Diagramm
In der Grafik wird die Reaktion auf eine **Preissenkung** von Gut 1 (Cola) dargestellt:
* ***Substitutionseffekt (SE):*** Wie gewohnt führt der niedrigere Preis dazu, dass der Konsument Gut 2 durch Gut 1 ersetzt. Die Menge von Gut 1 steigt (Bewegung vom ursprünglichen Optimum zum hypothetischen Punkt).
* ***Einkommenseffekt (EE):*** Da Gut 1 hier ein extrem inferiores Gut ist, führt die gestiegene reale Kaufkraft dazu, dass der Konsument die Nachfrage nach diesem Gut drastisch reduziert (Bewegung vom hypothetischen Punkt zum neuen Optimum).
* ***Gesamteffekt*:** Da der EE (Pfeil nach links) größer ist als der SE (Pfeil nach rechts), liegt das neue Optimum links vom ursprünglichen Optimum. **Ergebnis:** Der Preis sinkt, aber die Nachfrage sinkt ebenfalls.
## 3. Zusammenfassung der Wirkungsrichtungen

| Effekt | Richtung (bei Preissenkung) | Auswirkung auf Menge |
| :--- | :--- | :--- |
| **Substitutionseffekt** | Positiv | Der Konsument möchte mehr vom billigeren Gut. |
| **Einkommenseffekt** | Negativ (stark) | Der Konsument fühlt sich reicher und meidet das "Arme-Leute-Gut". |
| **Gesamteffekt** | **Negativ** | Die Menge sinkt trotz niedrigerem Preis. |

> [!CAUTION] **Abgrenzung: Inferiores Gut vs. Giffen-Gut**
> Jedes Giffen-Gut ist ein inferiores Gut, aber nicht jedes inferiore Gut ist ein Giffen-Gut. Bei den meisten inferioren Gütern ist der Substitutionseffekt immer noch stärker als der Einkommenseffekt, sodass das Gesetz der Nachfrage (Preis runter $\to$ Menge hoch) bestehen bleibt.

![[Pasted image 20260508151115.png]]

![[Pasted image 20260508151419.png]]

![[Pasted image 20260508151513.png]]