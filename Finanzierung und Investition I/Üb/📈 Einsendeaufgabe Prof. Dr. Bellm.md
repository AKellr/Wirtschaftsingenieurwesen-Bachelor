## 📥 Gegebene Basisdaten
* **Anschaffungskosten (AK):** 200.000 € (für Objekt A und B)
* **Nutzungsdauer (n):** 10 Jahre
* **Absatzmenge (x_b):** 10.000 Stück p.a. (für Aufgabenteil b)

| Parameter | Investitionsobjekt A | Investitionsobjekt B |
| :--- | :---: | :---: |
| **Preis je Stück (p)** | 13,000 € | 13,500 € |
| **Fixe Kosten / Periode (K_fix)** | 3.500 € | 5.000 € |
| **Variable Kosten / Stück (k_v)** | 10,50 € | 10,50 € |

---

## 🔢 Aufgabe 1a: Kritische Auslastung (Gewinnvergleichsrechnung)
Die kritische Menge (x_krit) markiert den Punkt, an dem beide Investitionsobjekte den exakt gleichen Gewinn erzielen.

### 1. Aufstellen der Gewinnfunktionen
Allgemein: G(x) = (p - k_v) * x - K_fix

* **Objekt A:** G_A(x) = (13,00 - 10,50) * x - 3.500 = 2,5x - 3.500
* **Objekt B:** G_B(x) = (13,50 - 10,50) * x - 5.000 = 3x - 5.000

### 2. Gleichsetzen und Auflösen (G_A = G_B)
2,5x - 3.500 = 3x - 5.000
1.500 = 0,5x
x_krit = 3.000 Stück

> [!success] **Entscheidungsregel für die Klausur**
> * **Menge < 3.000 Stück:** Objekt A ist vorteilhafter (geringere Fixkostenbelastung).
> * **Menge > 3.000 Stück:** Objekt B ist vorteilhafter (höhere Deckungsspanne pro Stück kompensiert die Fixkosten).

---

## 🔢 Aufgabe 1b: Amortisationsdauer (Payback-Periode)
Die Amortisationszeit gibt an, nach wie vielen Jahren die Anschaffungskosten durch die jährlichen Rückflüsse (Cashflows) wiedergewonnen sind.

Formel: Amortisationsdauer = Anschaffungskosten / Jährlicher Rückfluss
Wobei: Jährlicher Rückfluss = Gewinn + Abschreibung (AfA)

### 1. Berechnung der linearen Abschreibung (AfA)
* AfA = Anschaffungskosten / Nutzungsdauer
* AfA = 200.000 € / 10 Jahre = 20.000 € p.a. (identisch für A und B)

### 2. Berechnung für Investitionsobjekt A (bei x = 10.000)
* **Gewinn A:** G_A(10.000) = 2,5 * 10.000 - 3.500 = 21.500 €
* **Rückfluss A:** 21.500 € (Gewinn) + 20.000 € (AfA) = 41.500 €
* **Amortisationsdauer A:** 200.000 € / 41.500 € = 4,82 Jahre

### 3. Berechnung für Investitionsobjekt B (bei x = 10.000)
* **Gewinn B:** G_B(10.000) = 3 * 10.000 - 5.000 = 25.000 €
* **Rückfluss B:** 25.000 € (Gewinn) + 20.000 € (AfA) = 45.000 €
* **Amortisationsdauer B:** 200.000 € / 45.000 € = 4,44 Jahre

> [!info] **Fazit & Empfehlung**
> Da die geplante Absatzmenge von 10.000 Stück über der kritischen Menge (3.000) liegt, erwirtschaftet **Objekt B** den höheren Rückfluss pro Jahr. Das investierte Kapital amortisiert sich bei Objekt B mit **4,44 Jahren** schneller als bei Objekt A (4,82 Jahre). Objekt B ist vorzuziehen.

# 📈 Dynamische Investitionsrechnung: Pizzaofen-Fallstudie

## 📥 Gegebene Basisdaten
* **Anschaffungsauszahlung ($I_0$):** 30.000 €
* **Nutzungsdauer ($n$):** 4 Jahre
* **Zahlungsüberschüsse ($Z_t$):**
  - Jahr 1 ($Z_1$): 7.500 €
  - Jahr 2 ($Z_2$): 8.500 €
  - Jahr 3 ($Z_3$): 10.000 €
  - Jahr 4 ($Z_4$): 11.000 €

---

## 📐 Teil a) Kapitalwertverfahren (bei $i = 8\%$)

### Mathematischer Ansatz
Der Kapitalwert ($K_0$) berechnet sich durch die Summe aller auf den Zeitpunkt $t=0$ abgezinsten Zahlungsüberschüsse abzüglich der Anschaffungsauszahlung ($q = 1{,}08$):

$$K_0 = -I_0 + \sum_{t=1}^{n} \frac{Z_t}{q^t}$$

### Berechnung der Barwerte
* **Jahr 1:** $\frac{7.500}{(1{,}08)^1} = 6.944,44\text{ €}$
* **Jahr 2:** $\frac{8.500}{(1{,}08)^2} = 7.287,38\text{ €}$
* **Jahr 3:** $\frac{10.000}{(1{,}08)^3} = 7.938,32\text{ €}$
* **Jahr 4:** $\frac{11.000}{(1{,}08)^4} = 8.085,33\text{ €}$

$$\text{Summe der Barwerte} = 30.255,47\text{ €}$$
$$K_0 = -30.000\text{ €} + 30.255,47\text{ €} = \mathbf{255{,}47\text{ €}}$$

> [!success] **Entscheidung**
> Da $K_0 > 0$ ist, ist die Investition **vorteilhaft**. Das Restaurant sollte den Pizzaofen kaufen, da die Mindestverzinsung von 8 % übertroffen wird.

---

## 📐 Teil b) Risikoanpassung & Mindestpreisnachlass (bei $i = 10\%$)

Bei einem gestiegenen Zinssatz von $10\%$ ($q = 1{,}10$) sinken die Barwerte der Rückflüsse:
* **Summe der Barwerte (neu):** $6.818,18\text{ €} + 7.024,79\text{ €} + 7.513,15\text{ €} + 7.513,15\text{ €} = \mathbf{28.869{,}27\text{ €}}$
* **Kapitalwert (neu):** $K_0 = 28.869,27\text{ €} - 30.000\text{ €} = \mathbf{-1.130{,}73\text{ €}}$

### Ermittlung des Preisnachlasses
Damit die Investition bei erhöhtem Risiko wieder vorteilhaft ($K_0 = 0$) wird, muss die Anschaffungsauszahlung sinken.
$$\text{Mindest-Preisnachlass} = |K_0| = \mathbf{1.130{,}73\text{ €}}$$

---

## 📐 Teil c) Annuitätenmethode (bei $i = 8\%$)

Die Annuität ($A$) transformiert den einmaligen Kapitalwert in gleichmäßige jährliche Zahlungsströme. Dazu wird der Kapitalwert mit dem Wiedergewinnungsfaktor (WGF) multipliziert:

$$A = K_0 \cdot \frac{q^n \cdot (q-1)}{q^n - 1}$$

* **Berechnung des WGF:** $\frac{1{,}08^4 \cdot 0{,}08}{1{,}08^4 - 1} = \mathbf{0{,}30192}$
* **Berechnung der Annuität:** $A = 255,47\text{ €} \cdot 0{,}030192 = \mathbf{77{,}13\text{ € p.a.}}$

> [!info] **Bedeutung**
> Der Pizzaofen generiert über die 4 Jahre hinweg einen jährlichen Netto-Ertrag von 77,13 € (nach Deckung der Anschaffungskosten und der 8%-Mindestverzinsung).

---

## 📐 Teil d) Interner Zinsfuß ($i_{int}$)

Der interne Zinsfuß ist der Zinssatz, bei dem der Kapitalwert exakt Null beträgt ($K_0 = 0$). Die Ermittlung erfolgt über die lineare Interpolation (Näherungsverfahren):

$$\text{interner Zins} = i_1 - K_1 \cdot \frac{i_2 - i_1}{K_2 - K_1}$$

### Eingesetzte Werte:
* $i_1 = 0{,}08 \implies K_1 = 255,47\text{ €}$
* $i_2 = 0{,}10 \implies K_2 = -1.130,73\text{ €}$

### Berechnung:
$$i_{int} = 0{,}08 - 255,47 \cdot \frac{0{,}10 - 0{,}08}{-1.130,73 - 255,47}$$
$$i_{int} = 0{,}08 - 255,47 \cdot \frac{0{,}02}{-1.386,20} = 0{,}08 - (-0{,}003686) = \mathbf{0{,}08369} \implies \mathbf{8{,}37\%}$$

> [!success] **Fazit**
> Der exakte Effektivzins der Investition liegt bei **8,37%**. Da dieser Wert über den geforderten 8% liegt, ist das Projekt ökonomisch sinnvoll.

# 📈 Investitionsrechnung: Äquivalenz von Kapitalwert & Annuitätenbarwert

## 📥 Gegebene Basisdaten
* **Anschaffungsauszahlung ($I_0$):** 1.000.000 € (1 Mio. €)
* **Planungszeitraum ($n$):** 3 Jahre
* **Kalkulationszins ($i$):** 3 % ($q = 1{,}03$)
* **Zahlungsüberschüsse ($Z_t$):**
  - Jahr 1 ($Z_1$): 450.000 € (Basiswert)
  - Jahr 2 ($Z_2$): $450.000 \cdot 1{,}05 = \mathbf{472.500\text{ €}}$ (+5% p.a.)
  - Jahr 3 ($Z_3$): $472.500 \cdot 1{,}05 = \mathbf{496.125\text{ €}}$ (+5% p.a.)

---

## 📐 Schritt 1: Berechnung des Kapitalwerts ($K_0$)

Der Kapitalwert ermittelt sich durch Abzinsung der drei dynamischen Zahlungsüberschüsse:

$$K_0 = -1.000.000 + \frac{450.000}{(1{,}03)^1} + \frac{472.500}{(1{,}03)^2} + \frac{496.125}{(1{,}03)^3}$$

* **Barwert $Z_1$:** 436.893,20 €
* **Barwert $Z_2$:** 445.376,57 €
* **Barwert $Z_3$:** 454.024,64 €
* **Summe aller Barwerte:** 1.336.294,41 €

$$K_0 = 1.336.294,41\text{ €} - 1.000.000\text{ €} = \mathbf{336.294{,}41\text{ €}}$$

---

## 📐 Schritt 2: Berechnung der jährlichen Annuität ($A$)

Die Transformation des einmaligen Kapitalwerts in eine dreijährige, gleichbleibende Rente erfolgt über den Wiedergewinnungsfaktor (WGF):

$$A = K_0 \cdot \frac{q^n \cdot (q-1)}{q^n - 1}$$

* **Wiedergewinnungsfaktor:** $\frac{1{,}03^3 \cdot 0{,}03}{1{,}03^3 - 1} = \mathbf{0{,}35353036}$
* **Annuität ($A$):** $336.294{,}41\text{ €} \cdot 0{,}35353036 = \mathbf{118.890{,}13\text{ € p.a.}}$

---

## 🏛️ Schritt 3: Beweis der Äquivalenz (Barwert der Annuitäten)

Um zu zeigen, dass der Barwert der berechneten Annuitäten exakt dem Kapitalwert entspricht, werden die drei konstanten Zahlungen zurückgezinst:

$$\text{Barwert der Annuitäten} = \frac{118.890{,}13}{1{,}03^1} + \frac{118.890{,}13}{1{,}03^2} + \frac{118.890{,}13}{1{,}03^3}$$

$$\text{Barwert der Annuitäten} = 115.427,31\text{ €} + 112.065,35\text{ €} + 108.801,75\text{ €} = \mathbf{336.294{,}41\text{ €}}$$

$$\implies \text{Barwert der Annuitäten} = K_0$$

> [!success] **Fazit & Ökonomische Erkenntnis**
> Der mathematische Beweis ist erbracht. Die Annuitätenmethode führt zu derselben Investitionsentscheidung wie das Kapitalwertverfahren. Sie verteilt den totalen Vermögenszuwachs ($K_0$) unter Berücksichtigung von Zinseszinseffekten lediglich periodenreingeflasht auf die Nutzungsdauer.


# 📊 Derivateresumé: Call-Optionsschein auf Alibaba

## 📥 Gegebene Basisdaten
* **Aktueller Aktienkurs ($S_0$):** 193,00 €
* **Basispreis / Strike ($X$):** 190,00 €
* **Bezugsverhältnis:** 1:1
* **Laufzeit:** 12 Monate
* **Prämisse:** Der Optionsscheinpreis entspricht exakt dem inneren Wert.

---

## 📐 Teil a) Momentaner innerer Wert

Der innere Wert eines Call-Optionsscheins ($IW_{\text{Call}}$) beschreibt den rechnerischen Wert bei sofortiger Ausübung. Er kann niemals negativ werden ($\max[0; S_t - X]$).

$$IW_{\text{Call}} = S_0 - X$$
$$IW_{\text{Call}} = 193{,}00\text{ €} - 190{,}00\text{ €} = \mathbf{3{,}00\text{ €}}$$

> [!info] **Marktsituation**
> Da der Aktienkurs über dem Basispreis liegt ($S_0 > X$), notiert die Option **"im Geld"** (*in the money*).

---

## 📐 Teil b) Szenarioanalyse ($\pm$ 5% Kursänderung)

### Szenario (i): Aktienkurs steigt um 5%
* **Neuer Aktienkurs ($S_1$):** $193{,}00\text{ €} \cdot 1{,}05 = \mathbf{202{,}65\text{ €}}$
* **Neuer innerer Wert ($IW_1$):** $202{,}65\text{ €} - 190{,}00\text{ €} = \mathbf{12{,}65\text{ €}}$
* **Prozentuale Wertänderung des Scheins:**
  $$\Delta\% = \frac{12{,}65\text{ €} - 3{,}00\text{ €}}{3{,}00\text{ €}} \cdot 100\% = \mathbf{+321{,}67\%}$$

### Szenario (ii): Aktienkurs fällt um 5%
* **Neuer Aktienkurs ($S_2$):** $193{,}00\text{ €} \cdot 0{,}95 = \mathbf{183{,}35\text{ €}}$
* **Neuer innerer Wert ($IW_2$):** $\max[0; 183{,}35\text{ €} - 190{,}00\text{ €}] = \max[0; -6{,}65\text{ €}] = \mathbf{0{,}00\text{ €}}$
* **Prozentuale Wertänderung des Scheins:** **-100,00%** (Totalverlust des inneren Wertes)

> [!warning] **Asymmetrisches Risikoprofil**
> Während der Gewinn theoretisch unbegrenzt mit dem Aktienkurs steigt, ist der Verlust für den Käufer des Optionsscheins auf den eingesetzten Betrag (hier den anfänglichen inneren Wert von 3,00 €) begrenzt.

---

## 📐 Teil c) Relevante Kennzahlen zur Sensitivitätsbeurteilung

Um die Reaktionsstärke eines Optionsscheins auf Kursänderungen des Basiswerts zu messen, nutzt das Risikomanagement folgende Kennzahlen:

| Kennzahl                     |  Symbol  | Erklärung                                                                                                                                                                                                            |
| :--------------------------- | :------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Einfacher Hebel**          |   $H$    | Setzt den Aktienkurs ins Verhältnis zum Optionspreis (bereinigt um das Bezugsverhältnis). Zeigt das theoretische Investitionsverhältnis an.<br>$$H = \frac{S_0}{\text{Optionspreis} \cdot \text{Bezugsverhältnis}}$$ |
| **Delta**                    | $\Delta$ | Gibt an, um wie viel Euro sich der Optionspreis ändert, wenn die Aktie um **1,00 €** steigt. Bei weit im Geld liegenden Optionsscheinen geht das Delta gegen 1.                                                      |
| **Omega (Effektiver Hebel)** | $\Omega$ | Gibt an, um wie viel **Prozent** der Optionsschein steigt/fällt, wenn sich die Aktie um **1%** bewegt.<br>$$\Omega = \text{Hebel} \cdot \Delta$$                                                                     |
# 🏦 Anleihebewertung: Barwert von Kupon- und Nullkuponanleihen

## 📥 Gegebene Basisdaten
* **Marktzins ($i$):** 5 % p.a. ($\implies q = 1{,}05$)
* **Nominalwert ($N$):** 1.000 € (Rückzahlungswert für beide Anleihen)

---

## 📐 Anleihe A: Nullkuponanleihe (Zero-Bond)

### Spezifikation
* **Zinskupon:** 0 % p.a.
* **Laufzeit ($n$):** 10 Jahre

### Mathematischer Ansatz & Berechnung
Da während der Laufzeit keine Kuponzahlungen fließen, entspricht der Kurs dem Barwert der endfälligen Tilgungszahlung am Ende des 10. Jahres:

$$\text{Kurs}_A = \frac{N}{q^n}$$
$$\text{Kurs}_A = \frac{1.000\text{ €}}{(1{,}05)^{10}} = \frac{1.000\text{ €}}{1{,}628895} = \mathbf{613{,}91\text{ €}}$$

> [!info] **Marktsituation**
> Ein Zero-Bond notiert während der Laufzeit bei positivem Marktzins immer **unter pari** (< 100%). Die Rendite des Anlegers resultiert ausschließlich aus der Differenz zwischen dem günstigeren Kaufkurs und dem Rückzahlungswert.

---

## 📐 Anleihe B: Kuponanleihe

### Spezifikation
* **Zinskupon:** 5 % p.a. ($\implies \text{Jährliche Zinszahlung } C = 1.000\text{ €} \cdot 5\% = 50\text{ €}$)
* **Laufzeit ($n$):** 2 Jahre

### Analytischer Lösungsweg (Paritätsregel)
Es gilt das finanzmathematische Theorem: Wenn der nominale Zinskupon einer Anleihe exakt dem geforderten Marktzins (Kalkulationszins) entspricht, entspricht der Barwert der Anleihe immer genau ihrem Nominalwert.

$$\text{Zinskupon} = \text{Marktzins} \implies \mathbf{\text{Kurs} = \text{Nominalwert} = 1.000\text{ €}}$$

### Rechnerischer Gegenbeweis (Abzinsung der Zahlungsströme)
$$\text{Kurs}_B = \frac{C}{q^1} + \frac{C + N}{q^2}$$
$$\text{Kurs}_B = \frac{50\text{ €}}{1{,}05^1} + \frac{1.050\text{ €}}{1{,}05^2}$$
$$\text{Kurs}_B = 47{,}62\text{ €} + 952{,}38\text{ €} = \mathbf{1.000{,}00\text{ €}}$$

> [!success] **Fazit**
> Anleihe B notiert exakt **zu pari** (100% des Nominalwerts).

# 💸 Kredit- und Liquiditätsmanagement: Berechnung von Skontokosten

## 📥 Gegebene Basisdaten
* **Gesamtes Zahlungsziel:** 90 Tage
* **Skontofrist:** 14 Tage
* **Skontosatz:** 2 %

---

## 📐 Mathematischer Ansatz (Lieferantenkredit-Formel)

Die Inanspruchnahme eines Lieferantenkredits durch Verzicht auf Skonto kommt einer Kreditaufnahme gleich. Die jährlichen Kosten dieses Kredits ($\text{Kosten p.a.}$) berechnen sich nach der kaufmännischen Zinsmethode (360 Tage):

$$\text{Skontokosten p.a.} = \frac{\text{Skontosatz}}{100\% - \text{Skontosatz}} \cdot \frac{360}{\text{Zahlungsziel} - \text{Skontofrist}}$$

---

## 🧩 Schritt-für-Schritt-Berechnung

### 1. Ermittlung des effektiven Kreditzeitraums
Der Kredit wird erst nach Ablauf der Skontofrist bis zum Ende des Zahlungsziels in Anspruch genommen:
$$t = 90\text{ Tage} - 14\text{ Tage} = \mathbf{76\text{ Tage}}$$

### 2. Berechnung des Periodenzinssatzes
Da der Skontoabzug vom Bruttorechnungsbetrag erfolgt, bezieht sich der Verzicht (2 %) auf den verminderten Auszahlungsbetrag (98 %):
$$\text{Zinssatz}_{76\text{ Tage}} = \frac{2}{100 - 2} = \frac{2}{98} \approx \mathbf{2{,}0408\%}$$

### 3. Lineare Hochrechnung auf ein Jahr (p.a.)
$$\text{Skontokosten p.a.} = 2{,}0408\% \cdot \frac{360\text{ Tage}}{76\text{ Tage}} = 0{,}020408 \cdot 4{,}7368 = \mathbf{9{,}67\%}$$

---

## 🏛️ Ökonomische Beurteilung (Opportunitätskosten-Vergleich)

Der Verzicht auf Skonto entspricht einem Zinssatz von **9,67 % p.a.** > [!success] **Finanzierungsregel**
> * **Skontokosten p.a. > Bankzinssatz:** Es lohnt sich, einen Bankkredit (z. B. Kontokorrentkredit zu 7 % p.a.) aufzunehmen, um die Rechnung innerhalb der 14 Tage mit Skonto zu begleichen.
> * **Skontokosten p.a. < Bankzinssatz:** Die Inanspruchnahme des Lieferantenkredits ist rational (nur bei extrem teuren Kreditlinien der Fall).

# 📚 Finanzglossar: Zentrale Kennzahlen der Anlageanalyse

## 📊 1. Sharpe-Ratio
Die **Sharpe-Ratio** ist eine Kennzahl zur Risikobeurteilung von Geldanlagen. Sie misst die **Überrendite** einer Anlage (die Rendite, die über den risikofreien Zinssatz hinausgeht) im Verhältnis zu ihrem Gesamtrisiko, dargestellt durch die Volatilität.

$$\text{Sharpe-Ratio} = \frac{R_p - R_f}{\sigma_p}$$

* $R_p$: Rendite des Portfolios / der Anlage
* $R_f$: Risikofreier Zinssatz (*Risk-free rate*)
* $\sigma_p$: Volatilität (Standardabweichung) der Anlage

> [!success] **Interpretation**
> * **$> 1$:** Die erzielte Rendite kompensiert das eingegangene Risiko überproportional gut (attraktive Anlage).
> * **$< 0$:** Die Anlage hat schlechter abgeschnitten als eine absolut risikofreie Geldanlage.

---

## 📉 2. Volatilität
Die **Volatilität** ist das finanzmathematische Maß für die **Schwankungsbreite** eines Wertpapierkurses oder Marktes innerhalb eines bestimmten Zeitraums. Sie wird statistisch meist als Standardabweichung der Renditen berechnet.

* **Hohe Volatilität:** Der Kurs schlägt stark nach oben und unten aus $\implies$ Hohes Risiko, aber auch hohe kurzfristige Gewinnchancen.
* **Geringe Volatilität:** Der Kurs verläuft relativ stabil und gleichmäßig $\implies$ Geringeres Risiko.

---

## 🏷️ 3. KGV (Kurs-Gewinn-Verhältnis)
Das **KGV** (*Price-Earnings Ratio, P/E*) ist eine klassische fundamentale Kennzahl zur Bewertung von Aktien. Es setzt den aktuellen Börsenkurs einer Aktie in Relation zum erzielten oder erwarteten Gewinn pro Aktie.

$$\text{KGV} = \frac{\text{Aktueller Aktienkurs}}{\text{Gewinn pro Aktie}}$$

> [!info] **Aussagekraft**
> * **Hohes KGV:** Der Markt hat hohe Wachstumserwartungen an das Unternehmen. Die Aktie kann jedoch auch überbewertet sein.
> * **Niedriges KGV:** Deutet auf ein reifes, langsam wachsendes Unternehmen hin oder signalisiert eine fundamentale Unterbewertung (günstige Aktie).

---

## 💰 4. Dividendenrendite
Die **Dividendenrendite** drückt die Ausschüttung eines Unternehmens an seine Aktionäre in Prozent des aktuellen Aktienkurses aus. Sie macht den Erfolg einer Aktienanlage unabhängig von reinen Kursgewinnen messbar.

$$\text{Dividendenrendite} = \frac{\text{Dividende pro Aktie}}{\text{Aktueller Aktienkurs}} \cdot 100\%$$

* Sie dient Anlegern als Maßstab für die "Verzinsung" ihres eingesetzten Kapitals durch direkte Gewinnausschüttungen.
* Besonders relevant für cashflow-orientierte Anlage- und Dividendenstrategien.