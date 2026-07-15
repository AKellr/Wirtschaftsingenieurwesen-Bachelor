### 1. Statische Investitionsrechnung (Static Investment Calculation)

| **Concept**                      | **Formula / Calculation**                                      | **Decision Rule / Insight**                                                             | **Citation** |
| -------------------------------- | -------------------------------------------------------------- | --------------------------------------------------------------------------------------- | ------------ |
| **Kalkulatorische Abschreibung** | $\frac{A_0 - RW}{n}$                                           | Erfasst den jährlichen, linearen Wertverzehr.                                           |              |
| **Kalk. Zinsen (ohne Restwert)** | $z = \frac{A_0}{2} \cdot i$                                    | Durchschnittlich gebundenes Kapital halbiert sich über die Laufzeit.                    |              |
| **Kalk. Zinsen (mit Restwert)**  | $z = \frac{A_0 + L_n}{2} \cdot i$                              | Der Restwert bleibt als Kapital im Unternehmen gebunden.                                |              |
| **Kostenvergleich**              | $K = \text{kalk. AfA} + \text{kalk. Zinsen} + K_f + K_v$       | Bei unterschiedlicher Auslastung zwingend Stückkosten ($k = \frac{K}{x}$) vergleichen.  |              |
| **Gewinnvergleich**              | $G = E - K$                                                    | Wähle die Alternative mit dem höchsten Nettoüberschuss (Gewinn).                        |              |
| **Kritische Menge ($x_{krit}$)** | $G_A(x) = G_B(x)$                                              | Menge ermitteln, ab der ein höheres Fixkosten-Objekt vorteilhaft wird (Break-Even).     |              |
| **Rentabilität (Brutto)**        | $\frac{G + \text{kalk. Zinsen}}{\emptyset\text{ GK}}$          | Investition ist sinnvoll, wenn die Bruttorendite den Kalkulationszins ($i$) übersteigt. |              |
| **Amortisationsdauer**           | $\frac{\text{Anschaffungskosten}}{\text{Gewinn} + \text{AfA}}$ | Zeigt in Jahren an, wann das eingesetzte Kapital durch Rückflüsse gedeckt ist.          |              |

### 2. Dynamische Investitionsrechnung (Dynamic Investment Calculation)

|**Concept**|**Formula / Calculation**|**Decision Rule / Insight**|**Citation**|
|---|---|---|---|
|**Barwertfaktor (BWF)**|$(1 + i)^{-n}$|Diskontiert einen zukünftigen Zielwert auf den heutigen Tag ($t=0$).||
|**Kapitalwert ($K_0$ / NPV)**|$-A_0 + \sum_{t=1}^{n} \frac{Z_t}{(1+i)^t}$|Investition vorteilhaft, wenn $K_0 > 0$. Erwirtschaftet Mindestverzinsung + Zusatzwert.||
|**Annuität ($A$)**|$K_0 \cdot \frac{q^n \cdot (q-1)}{q^n - 1}$|Verteilt den Kapitalwert gleichmäßig als Rente über die Nutzungsdauer.||
|**Diskontierungssummenfaktor**|$\frac{q^n - 1}{q^n \cdot (q - 1)}$|Bestimmt den Barwert einer konstanten Rente in nur einem Rechenschritt.||
|**Endwertfaktor (EWF)**|$\frac{q^n - 1}{q - 1}$|Verdichtet den Zinseszins-Effekt nachschüssiger, konstanter Zahlungsreihen.||

### 3. Finanzierung, WACC & CAPM

| **Concept**           | **Formula / Calculation**                                                                  | **Decision Rule / Insight**                                                             | **Citation** |
| --------------------- | ------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------- | ------------ |
| **Leverage-Effekt**   | $r_{EK} = r_{GK} + \frac{FK}{EK} \cdot (r_{GK} - k)$                                       | Positiv, wenn Gesamtkapitalrendite ($r_{GK}$) höher ist als der FK-Zins ($k$).          |              |
| **CAPM ($r_{EK}$)**   | $r_f + \beta \cdot (r_m - r_f)$                                                            | Ermittelt die risikoadäquate Renditeforderung der Eigenkapitalgeber.                    |              |
| **WACC**              | $i_{EK} \cdot \frac{EK}{GK} + i_{FK} \cdot (1 - s) \cdot \frac{FK}{GK}$                    | Gesamtkapitalkosten. Dient als Mindestrendite (Hurdle Rate) für Investitionen.          |              |
| **Skontokosten p.a.**[[]] | $\frac{\text{Skonto}}{100\% - \text{Skonto}} \cdot \frac{360}{\text{Ziel} - \text{Frist}}$ | Ist dieser Satz höher als der Bankzins, lohnt sich ein Bankkredit, um Skonto zu ziehen. |              |
| **Zero-Bond Kurs**    | $\frac{N}{q^n}$                                                                            | Notiert bei positivem Marktzins immer unter pari. Rendite aus Kaufkursdifferenz.        |              |

### 4. Liquidität, Kennzahlen & Controlling

|**Concept**|**Formula / Calculation**|**Decision Rule / Insight**|**Citation**|
|---|---|---|---|
|**Liquidität 2. Grades**|$\frac{\text{Liq. Mittel} + \text{Kurzfr. Forderungen}}{\text{Kurzfristiges FK}} \cdot 100\%$|Wert $>100\%$ zeigt an, dass kurzfristige Verbindlichkeiten gedeckt sind.||
|**Deckungsgrad B**|$\frac{EK + LFK}{AV} \cdot 100\%$|Goldene Bilanzregel im weiteren Sinne; Anlagevermögen muss langfristig finanziert sein.||
|**Dyn. Verschuldungsgrad**|$\frac{FK - \text{liquide Mittel}}{\text{Cashflow}}$|Dauer in Jahren, um Fremdkapital aus operativem Cashflow komplett zu tilgen.||
|**Risiko (Erwartungswert)**|$R_{i,t} = S_{i,t} \cdot p_i$|Gesamtrisiko ($S$) multipliziert mit der Eintrittswahrscheinlichkeit ($p$).||
|**Economic Value Added (EVA)**|$(\text{Geschäftsrendite} - WACC) \cdot \text{Geschäftsvermögen}$|Wenn positiv, wurde echter Mehrwert geschaffen (Rendite übertrifft Kapitalkosten).||
|**Sharpe-Ratio**|$\frac{R_p - R_f}{\sigma_p}$|Überrendite im Verhältnis zur Volatilität. Wert $> 1$ bedeutet attraktives Chance/Risiko-Profil.||

---

## 1. Rentabilitätskennzahlen
Diese Kennzahlen messen den finanziellen Erfolg eines Unternehmens im Verhältnis zum eingesetzten Kapital oder dem erzielten Umsatz.

* **Eigenkapitalrentabilität ($EkR$):** Measures profit in relation to equity.
    $$EkR = \frac{G}{Ek} \cdot 100$$
* **Gesamtkapitalrentabilität ($GKR$):** Measures profit plus debt interest in relation to total capital.
    $$GKR = \frac{G + FKZ}{Gk} \cdot 100$$
* **Umsatzrentabilität ($UR$):** Measures profit in relation to total sales.
    $$UR = \frac{G}{U} \cdot 100$$
* **Gewinn ($G$):** Total revenue minus total costs.
    $$G = U - K$$

---

### Leverage-Effekt (Hebelwirkung des Fremdkapitals)

> [!NOTE] **Definition & Funktionsweise**
> Der Leverage-Effekt beschreibt die Veränderung der Eigenkapitalrendite durch den Einsatz von Fremdkapital. Solange die Gesamtkapitalrentabilität ($i$) größer ist als der Fremdkapitalzins ($k$), steigt die Eigenkapitalrentabilität mit zunehmender Verschuldung.
> 
> **Formel:**
> $$r_{EK} = \left(i + \frac{Fk}{Ek} \cdot (i - k)\right) \cdot 100$$
> * $i$ = Gesamtkapitalrentabilität
> * $k$ = Fremdkapitalzins

---

### Kapitalbindung

* **Rentabilität des gebundenen Kapitals ($R_N$ / $R_B$):**
    $$R_N = \frac{G}{\emptyset GB.K} \cdot 100 \quad \text{bzw.} \quad R_B = \frac{G + \text{kalk. } Z}{\emptyset GB.K} \cdot 100$$
* **Durchschnittlich gebundenes Kapital ($\emptyset GBK$):** Anfangsinvestition plus Restwert geteilt durch 2.
    $$\emptyset GBK = \frac{A_0 + Res}{2} \quad \text{oder} \quad \frac{A_0}{2}$$

---

## 2. Liquidität & Deckungsgrade
Diese Kennzahlen geben Aufschluss über die Zahlungsfähigkeit eines Unternehmens und zeigen, wie stabil das Anlagevermögen finanziert ist.

### Liquiditätsgrade (Kurzfristige Zahlungsfähigkeit)

| Kennzahl | Formel | Zielwert / Richtwert | Beschreibung |
| :--- | :--- | :--- | :--- |
| **Liquidität 1. Grades** (Barliquidität) | $\frac{\text{Liq.M}}{\text{kurzfr. FK}} \cdot 100$ | $10 - 30\%$ | Liquide Mittel im Verhältnis zu den kurzfristigen Verbindlichkeiten. |
| **Liquidität 2. Grades** (Einzugsbedingte Liq.) | $\frac{\text{Liq.M} + \text{kurzfr. Ford.}}{\text{kurzfr. FK}} \cdot 100$ | $\approx 100\%$ | Einbeziehung kurzfristiger Forderungen zur Deckung des kurzfristigen Fremdkapitals. |
| **Liquidität 3. Grades** (Umsatzbedingte Liq.) | $\frac{\text{kurzfr. UML}}{\text{kurzfr. FK}} \cdot 100$ | $\approx 200\%$ | Gesamtes kurzfristiges Umlaufvermögen im Verhältnis zum kurzfristigen Fremdkapital. |

### Anlagendeckungsgrade (Goldene Bilanzregel)

| Kennzahl | Formel | Zielwert / Richtwert | Beschreibung |
| :--- | :--- | :--- | :--- |
| **Deckungsgrad A (1)** | $\frac{Ek}{AV} \cdot 100$ | $70 - 100\%$ | Deckung des Anlagevermögens durch das Eigenkapital. |
| **Deckungsgrad B (2)** | $\frac{Ek + \text{langfr. FK}}{AV} \cdot 100$ | $110 - 150\%$ | Deckung des Anlagevermögens durch langfristiges Kapital (Goldene Bilanzregel). |
| **Deckungsgrad C (3)** | $\frac{Ek + \text{langfr. FK}}{AV + \text{langfr. UV}}$ | - | Verhältnis von langfristigem Kapital zu langfristig gebundenem Vermögen. |

### Verschuldungskennzahlen

* **Verschuldungsgrad:**
    $$\text{ver.g} = \frac{Fk}{Ek}$$
* **Dynamischer Verschuldungsgrad:** Zeigt an, in wie vielen Jahren die Verbindlichkeiten theoretisch durch den Cashflow getilgt werden können.
    $$\text{dyn.v.g} = \frac{\text{verb.} - L_0}{CF}$$
    * $\text{verb.}$ = Verbindlichkeiten
    * $L_0$ = Liquide Mittel
    * $CF$ = Cashflow

---

## 3. Unternehmenssteuerung & Wertorientierung
Moderne Steuerungskennzahlen zur Ermittlung des operativen Erfolgs, des generierten Unternehmenswertes und der gewichteten Kapitalkosten.

* **EBIT (Earnings Before Interest and Taxes):** Operatives Ergebnis vor Zinsen und Steuern.
    $$EBIT = U - \text{Aufw.}$$
    $$EBIT = \text{Über.} + i + s$$
    * $\text{Über.}$ = Jahresüberschuss
    * $i$ = Zinsen
    * $s$ = Steuern
* **NOPAT (Net Operating Profit After Taxes):** Operativer Gewinn nach Steuern.
    $$NOPAT = EBIT - \text{ErSt}$$
    * $\text{ErSt}$ = Ertragsteuern

> [!INFO] **EVA (Economic Value Added)**
> Der EVA misst den geschaffenen Übergewinn eines Unternehmens, der nach Abzug der kalkulatorischen Kapitalkosten verbleibt. Ein **EVA > 0** bedeutet, dass echter Wert für die Kapitalgeber geschaffen wurde.
> 
> **Formeln:**
> $$EVA = NOPAT - (Ek \cdot WACC)$$
> $$EVA = \text{inv. K} \cdot (ROIC - WACC)$$
> * $\text{inv. K}$ = Investiertes Kapital

* **WACC (Weighted Average Cost of Capital):** Gewichteter Gesamtkapitalkostensatz.
    $$\text{Ohne Steuern:} \quad WACC = \left(r_{EK} \cdot \frac{EK}{GK}\right) + \left(r_{FK} \cdot \frac{FK}{GK}\right)$$
    $$\text{Mit Tax Shield (s):} \quad WACC = \left(r_{EK} \cdot \frac{EK}{GK}\right) + r_{FK} \cdot (1-s) \cdot \frac{FK}{GK}$$
* **Gordon Growth Model (Ewige Rente):** Bestimmung des Unternehmenswertes basierend auf dem zukünftigen Free Cashflow und einer konstanten Wachstumsrate.
    $$Gr.f = \frac{FCF}{WACC - \text{WachR}}$$
* **CAPM-Ansatz (Capital Asset Pricing Model):** Ermittlung der geforderten Eigenkapitalkosten unter Berücksichtigung eines Risikoprofils.
    $$i_{EK} = B.Z5 + Ris.Zu.$$
    * $B.Z5$ = Basiszinssatz
    * $Ris.Zu.$ = Risikozuschlag

---

## 4. Statische Investitionsrechnung
Verfahren der Investitionsrechnung, die den zeitlichen Anfall von Zahlungen (Zinseszins) vernachlässigen und stattdessen mit periodischen Durchschnittswerten kalkulieren.

* **Kalkulatorische Abschreibung ($KA$):**
    $$KA = \frac{A_0 - L_n}{n}$$
    * $A_0$ = Anschaffungskosten
    * $L_n$ = Restwert am Ende der Nutzungsdauer
    * $n$ = Nutzungsdauer
* **Kalkulatorische Zinsen ($KZ$):**
    $$\text{Ohne Restwert:} \quad KZ + Ab = \frac{A_0}{2} \cdot i$$
    $$\text{Mit Restwert:} \quad KZ + Ab = \frac{A_0 + L_n}{2} \cdot i$$
* **Amortisationsdauer ($AD$):** Zeitraum, in dem das eingesetzte Kapital wieder zurückfließt.
    $$\text{Kosten-Gewinn-Vergleich:} \quad AD = \frac{A_0 - L_n}{G + \text{Abs.}}$$
    $$\text{Cashflow-Vergleich:} \quad AD = \frac{A_0 - L_n}{EZ\ddot{U}}$$
    * $EZ\ddot{U}$ = Einzahlungsüberschuss (Cashflow)

---

## 5. Dynamische Investitionsrechnung
Finanzmathematische Methoden, die den exakten zeitlichen Anfall von Zahlungsströmen durch Aufzinsung (Endwert) oder Abzinsung (Barwert) berücksichtigen.

* **Rendite / Interne Verzinsung (Sonderfall bei genau 2 Zahlungen):**
    $$L = \left(\sqrt[n]{\frac{A_n}{A_0}} - 1\right) \cdot 100$$
    $$r = \left(\sqrt[n]{\frac{EZ\ddot{U}}{A_0}} - 1\right) \cdot 100$$
* **Endwertfaktor ($EWF$):** Wird genutzt, um den zukünftigen Endwert ($K_n$) einer regelmäßigen Rente ($g$) zu berechnen.
    $$EWF = \frac{(1+i)^n - 1}{i} \quad \rightarrow \quad K_n = g \cdot EWF$$
* **Diskontierungssummenfaktor ($DSF$ / Rentenbarwertfaktor):** Dient zur Ermittlung des heutigen Barwertes ($K_0$) einer zukünftigen, regelmäßigen Rente ($g$).
    $$DSF = \frac{(1+i)^n - 1}{i \cdot (1+i)^n} \quad \rightarrow \quad K_0 = g \cdot DSF$$
* **Kapitalwiedergewinnungsfaktor ($KWF$ / Annuitätenfaktor):** Der Kehrwert des DSF. Berechnet die jährliche, gleichbleibende Annuität ($a$) aus einem Barwert ($K_0$).
    $$KWF = \frac{i \cdot (1+i)^n}{(1+i)^n - 1} \quad \rightarrow \quad a = K_0 \cdot KWF$$

---

## 6. Sonderformeln & Finanzierung
Spezifische Berechnungsformeln für Kreditkonditionen, Effektivzinssätze und Fristenmodelle.

* **Effektivverzinsung des Lieferantenkredits:** Berechnet die impliziten Jahreskosten, wenn eine Skontofrist ungenutzt verstreicht.
    $$\text{Krd. Z} = \frac{Sk}{1-Sk} \cdot \frac{360}{Zf - \text{Sk. fris.}}$$
    * $Sk$ = Skontosatz
    * $Zf$ = Zahlungsziel
    * $\text{Sk. fris.}$ = Skontofrist
* **Näherungsformel für den Effektivzins (Anleihen):**
    $$\text{Ef.a.Z} = r = \frac{Z + \frac{D}{n}}{A \cdot B_{\%}} \cdot 100$$
    * $Z$ = Nominalzins
    * $D$ = Disagio
    * $n$ = Restlaufzeit
    * $A$ = Auszahlungsbetrag / Nennwert
    * $B_{\%}$ = Bezugskurs in Prozent
* **Mittlerer Zahlungstermin ($m$):**
    $$m = \frac{n+1}{2} \quad \text{oder} \quad m = t + \frac{(n-t)+1}{2}$$