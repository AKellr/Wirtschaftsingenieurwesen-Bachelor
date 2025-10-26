Unter dem **Binomialkoeffizienten** $\binom{n}{k}$ (gelesen als „$n$ über $k$“) versteht man den Bruch $$ \binom{n}{k} = \frac{n(n-1)(n-2) \cdots (n-k+2)(n-k+1)}{k!} $$ Zusätzlich definiert man: $$ \binom{n}{0} = 1. $$
**Hinweise zur Definition**
Es gilt $k \in \mathbb{N}$. Es ist sofort klar, dass im Nenner $k$ Faktoren stehen (Produkt der $k$ natürlichen Zahlen von 1 bis $k$). Es gilt $n \in \mathbb{R}^1$. $n$ gibt den ersten Faktor im Zähler an. Alle weiteren Faktoren werden jeweils um eins kleiner. Man kann sich leicht davon überzeugen, dass auch im Zähler insgesamt $k$ Faktoren vorhanden sind ($\text{Ü}2$).

Für $n \ge k$ gilt:
$$ \binom{n}{k} = \frac{n!}{k!(n-k)!} = \binom{n}{n-k} $$

**Beweis**
**a) Linker Teil der Gleichung** $\binom{n}{k} = \frac{n!}{k!(n-k)!}$:

Erweitern der Definition des Binomialkoeffizienten mit $\frac{(n-k)!}{(n-k)!}$ liefert:
$$ \binom{n}{k} = \frac{n(n-1)\cdots(n-k+1)}{k!} \cdot \frac{(n-k)!}{(n-k)!} = \frac{n(n-1)\cdots(n-k+1) \cdot 1 \cdot 2 \cdots (n-k-1)(n-k)}{k! \cdot (n-k)!} $$
Im Zähler treten alle natürlichen Zahlen von $1$ bis $n$ jeweils genau einmal als Faktor auf, nur in einer anderen Reihenfolge:
$$ \binom{n}{k} = \frac{1 \cdot 2 \cdots (n-k-1)(n-k)(n-k+1) \cdots (n-1)n}{k!(n-k)!} $$
**b) Rechter Teil der Gleichung** $\binom{n}{n-k} = \frac{n!}{k!(n-k)!}$:

Das in a) gezeigte Resultat wenden wir auf den rechts stehenden Binomialkoeffizienten
$$ \binom{n}{n-k} $$
an und ersetzen jeweils $k$ durch $n-k$:
$$ \binom{n}{n-k} = \frac{n!}{(n-k)! \cdot (n - (n-k))!} = \frac{n!}{(n-k)! \cdot k!} $$
Damit ist die Behauptung bewiesen.

**Es gilt:** $$ \binom{n}{k} + \binom{n}{k+1} = \binom{n+1}{k+1} $$
$$ \binom{n}{k} + \binom{n}{k+1} = \binom{n+1}{k+1} $$
$$ \binom{n}{k} + \binom{n}{k+1} = \frac{n(n-1)\cdots(n-k+1)}{k!} + \frac{n(n-1)\cdots(n-k+1)(n-k)}{(k+1)!} $$
$$ = \frac{n(n-1)\cdots(n-k+1)(k+1) + n(n-1)\cdots(n-k+1)(n-k)}{(k+1)!} $$
$$ = \frac{n(n-1)\cdots(n-k+1)[(k+1) + (n-k)]}{(k+1)!} $$
$$ = \frac{n(n-1)\cdots(n-k+1)(n+1)}{(k+1)!} $$
$$ = \binom{n+1}{k+1} $$
![[Pasted image 20250928162847.png]]

Das Pascalsche Dreieck besitzt folgende Eigenschaften:
- Es ist **symmetrisch zur Mittelachse**.
- Ausgehend von den Randwerten 1 werden alle anderen Werte als **Summe der beiden darüber stehenden** gebildet.

**Binomischer Satz**
$$ (a+b)^n = \binom{n}{0}a^n + \binom{n}{1}a^{n-1}b + \binom{n}{2}a^{n-2}b^2 + \cdots + \binom{n}{n-1}ab^{n-1} + \binom{n}{n}b^n = \sum_{i=0}^{n} \binom{n}{i}a^{n-i}b^i $$

**Analog gilt für die Differenz**
$$ (a-b)^n = \binom{n}{0}a^n - \binom{n}{1}a^{n-1}b + \binom{n}{2}a^{n-2}b^2 - \binom{n}{3}a^{n-3}b^3 + \cdots \pm \binom{n}{n}b^n = \sum_{i=0}^{n} \binom{n}{i}a^{n-i}(-b)^i $$
**Permutationen**
**Definition:** Jede Anordnung von endlich vielen Elementen, in der jedes Element vorkommt, heißt **Permutation**.

**Permutation ohne Wiederholung**
**Definition:** Eine **Permutation von n Elementen (ohne Wiederholung)** ist jede Zusammenstellung von n verschiedenen Elementen in irgendeiner Anordnung. Unterschiedliche Anordnungen der n Elemente bedeuten stets verschiedene Permutationen.

**Beispiel:** Kehren wir zur eingangs gestellten Frage zurück: „Wie viele Möglichkeiten gibt es, vier Buchstaben anzuordnen?“ Nach der obigen Formel beträgt die Anzahl der Permutationen von 4 Elementen ohne Wiederholung P4​=4!=24.

**Definition:**
Seien die insgesamt $n$ Elemente in $k$ Gruppen mit je $n_1, n_2, \ldots, n_k$ gleichen Elementen, wobei $n_1 + n_2 + \cdots + n_k = n$ gilt, aufgeteilt. Eine \textbf{Permutation von $n$ Elementen (mit Wiederholung)} ist jede Zusammenstellung der $n$ Elemente in irgendeiner Anordnung. Dabei wird nicht zwischen den Elementen einer Gruppe unterschieden. Die Anzahl der Permutationen $P_{n}$ von $n$ Elementen mit Wiederholung beträgt $$ P_{n}^{(n_1, \ldots, n_k)} = \frac{n!}{n_1! n_2! \cdots n_k!} $$
**Beispiel**
In wie viel verschiedenen Reihenfolgen können 5 Personen (2 Männer und 3 Frauen) in einer Warteschlange stehen, wenn bei jedem einzelnen Standort nur zwischen Mann und Frau unterschieden wird? Im Gegensatz zum obigen Beispiel bei Permutationen ohne Wiederholung werden hier nicht mehr ausschließlich verschiedene Objekte betrachtet, sondern zwei Gruppen jeweils gleicher Elemente. Es gilt $n_1 = 2$ (2 Männer – zwischen ihnen soll nicht unterschieden werden) und $n_2 = 3$ (3 Frauen – zwischen ihnen soll ebenfalls nicht unterschieden werden). Insgesamt haben wir $n = n_1 + n_2 = 2 + 3 = 5$ Elemente. In die obige Formel eingesetzt ergeben sich insgesamt $$ P_{W,5}^{(2,3)} = \frac{5!}{2! \cdot 3!} = \frac{120}{2 \cdot 6} = 10 $$ Reihenfolgen in der Warteschlange.

Jede Zusammenstellung von $k$ aus $n$ Elementen, die ihre Anordnung nicht berücksichtigt, heißt **Kombination von** $n$ **Elementen zur Klasse** $k$ (je $k$ Stück; $1 \le k \le n$). 

**Kombinationen ohne Wiederholungen** 
**Definition:** Treten in den Zusammenstellungen nur verschiedene Elemente auf, so spricht man von **Kombinationen ohne Wiederholung von $n$ Elementen zu je $k$**. Die Anzahl der Kombinationen ohne Wiederholung $C_n^k$ von $n$ Elementen zu je $k$ beträgt $$ C_n^k = \binom{n}{k} = \frac{n!}{k!(n-k)!}, \quad 1 \le k \le n $$
**Beispiel:**
Jetzt kommen wir zur spannenden Frage "Auf wie viele verschiedene Arten können aus
49 Zahlen 6 verschiedene Zahlen ausgewählt werden?" oder "Wie viel verschiedene
Sechserreihen gibt es beim Lotto (6 aus 49)"?
$$ C_{49}^6 = \binom{49}{6} = \frac{49 \cdot 48 \cdot 47 \cdot 46 \cdot 45 \cdot 44}{1 \cdot 2 \cdot 3 \cdot 4 \cdot 5 \cdot 6} = 13.983.816 $$

**Kombinationen mit Wiederholungen**
**Definition:** Sind in den Zusammenstellungen auch Wiederholungen zugelassen, so spricht man von **Kombinationen mit Wiederholung von n Elementen zu je k**.
Die Anzahl der Kombinationen mit Wiederholung $C_{W,n}^k$ von n Elementen zu je k beträgt
$$ C_{W,n}^k = \binom{n+k-1}{k}. $$
**Beispiel:** Gesucht ist die Anzahl verschiedener Würfe mit zwei nicht voneinander zu unterscheidenden Würfeln. Laut Aufgabenstellung ist es unerheblich, ob z. B. mit dem ersten Würfel eine 1 und mit dem zweiten eine 2 gewürfelt wird oder umgekehrt.
Mit $k=2$ und $n=6$ erhalten wir $$ C_6^2 = \binom{6+2-1}{2} = \binom{7}{2} = \frac{7!}{2!5!} = \frac{7 \cdot 6}{1 \cdot 2} = 21 $$ verschiedene Würfe.

**Variation**
**Definition:** Jede Zusammenstellung von $k$ aus $n$ Elementen, die ihre Anordnung berücksichtigt, heißt **Variation von $n$ Elementen zur Klasse $k$** (je $k$ Stück; $1 \le k \le n$).

**Variationen ohne Wiederholungen**
**Definition:** Treten in den Zusammenstellungen nur verschiedene Elemente auf, so spricht man von **Variationen ohne Wiederholung von** $n$ **Elementen zu je** $k$. 
Die Anzahl der Variationen ohne Wiederholung $V_n^k$ von $n$ Elementen zu je $k$ beträgt 
$$ V_n^k = \frac{n!}{(n-k)!}, \quad 1 \le k \le n. $$
**Beispiel**
Unter 5 Spielern soll der „Fußballer des Jahres“ ausgewählt werden. Wie viele Möglichkeiten gibt es für die richtige Reihenfolge der 3 Erstplatzierten? Es sind jeweils $k = 3$ aus $n = 5$ Spielern auszuwählen. Dabei ist nur die Reihenfolge der ersten drei zu berücksichtigen. Also handelt es sich um Variationen ohne Wiederholung und ihre Anzahl beträgt 
$$ V_5^3 = \frac{5!}{(5-3)!} = \frac{5!}{2!} = \frac{1 \cdot 2 \cdot 3 \cdot 4 \cdot 5}{1 \cdot 2} = 60. $$
**Variationen mit Wiederholungen**
**Definition:** Sind in den Zusammenstellungen auch Wiederholungen zugelassen, so spricht man von **Variationen mit Wiederholung von $n$ Elementen zu je $k$**. Die Anzahl der Variationen mit Wiederholung $V_{W,n}^k$ von $n$ Elementen zu je $k$ beträgt $$ V_{W,n}^k = n^k. $$
**Beispiel**
Wie viele „Wörter“ zu je 3 Buchstaben lassen sich aus den 26 Buchstaben des Alphabets bilden? (Dabei sind beliebige Folgen von 3 Buchstaben zugelassen.) Jeder der $n = 26$ Buchstaben kann $k = 3$ mal hintereinander gesetzt werden, also auch mit Wiederholungen. Somit handelt es sich beim gestellten Problem um Variationen mit Wiederholung; die Anzahl aller möglichen „Wörter“ beträgt $V_{26}^3 = 26^3 = 17576$.

