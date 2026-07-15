## 1. Annuitätendarlehen & Tilgungsplan

### Mathematische Kernformeln

* **Kapitalwiedergewinnungsfaktor (ANF):**
    $$ANF = \frac{i \cdot (1 + i)^n}{(1 + i)^n - 1}$$
* **Konstante Annuität ($A$):**
    $$A = S_0 \cdot ANF$$
    *(wobei $S_0$ = Ursprüngliche Darlehenssumme)*
* **Zinsanteil der Periode $t$ ($Z_t$):**
    $$Z_t = S_{t-1} \cdot i$$
    *(wobei $S_{t-1}$ = Restschuld am Anfang der Periode $t$)*
* **Tilgungsanteil der Periode $t$ ($T_t$):**
    $$T_t = A - Z_t$$
* **Restschuld am Ende der Periode $t$ ($S_t$):**
    $$S_t = S_{t-1} - T_t$$

> [!WARNING] Klausurrelevante Besonderheit (Letzte Periode $n$)
> Aufgrund von **Rundungsdifferenzen** beim ANF (meist auf 4 Nachkommastellen) darf in der letzten Periode nicht starr mit der Standardannuität gerechnet werden. Es gelten folgende erzwungene Werte:
> * **Erzwungene Endrestschuld:** $S_n = 0$
> * **Erzwungene Tilgung:** $T_n = S_{n-1}$
> * **Modifizierte finale Annuität:** $A_n = Z_n + T_n$

### Klausur-Anwendungsbeispiel (Vollständiger Tilgungsplan)
**Gegebene Daten:**
* Darlehenssumme ($S_0$) = $10.000\ \text{€}$
* Laufzeit ($n$) = $3\ \text{Jahre}$
* Zinssatz ($i$) = $5\% = 0,05$

**Schritt 1: Berechnung des ANF (auf 4 Nachkommastellen gerundet)**
$$ANF = \frac{0,05 \cdot (1,05)^3}{(1,05)^3 - 1} = \frac{0,05 \cdot 1,157625}{0,157625} \approx 0,367209 \rightarrow \mathbf{0,3672}$$

**Schritt 2: Berechnung der Standard-Annuität ($A$)**
$$A = 10.000\ \text{€} \cdot 0,3672 = \mathbf{3.672,00\ \text{€}}$$

**Schritt 3: Periodenweise Berechnung & Finale Anpassung**
* **Periode 1:**
  * $Z_1 = 10.000 \cdot 0,05 = 500,00\ \text{€}$
  * $T_1 = 3.672,00 - 500,00 = 3.172,00\ \text{€}$
  * $S_1 = 10.000 - 3.172,00 = 6.828,00\ \text{€}$
* **Periode 2:**
  * $Z_2 = 6.828,00 \cdot 0,05 = 341,40\ \text{€}$
  * $T_2 = 3.672,00 - 341,40 = 3.330,60\ \text{€}$
  * $S_2 = 6.828,00 - 3.330,60 = 3.497,40\ \text{€}$
* **Periode 3 (Letzte Periode $\rightarrow$ Sonderlogik anwenden!):**
  * $Z_3 = 3.497,40 \cdot 0,05 = 174,87\ \text{€}$
  * $T_3 = S_2 = \mathbf{3.497,40\ \text{€}}$ *(erzwungen)*
  * $A_3 = 174,87 + 3.497,40 = \mathbf{3.672,27\ \text{€}}$ *(modifiziert wegen Rundung, +0,27 €)*
  * $S_3 = \mathbf{0,00\ \text{€}}$ *(erzwungen)*

| Periode ($t$) | Restschuld Anfang ($S_{t-1}$) | Annuität ($A_t$) | Zinsanteil ($Z_t$) | Tilgungsanteil ($T_t$) | Restschuld Ende ($S_t$) |
|:---:|:---:|:---:|:---:|:---:|:---:|
| **1** | $10.000,00\ \text{€}$ | $3.672,00\ \text{€}$ | $500,00\ \text{€}$ | $3.172,00\ \text{€}$ | $6.828,00\ \text{€}$ |
| **2** | $6.828,00\ \text{€}$ | $3.672,00\ \text{€}$ | $341,40\ \text{€}$ | $3.330,60\ \text{€}$ | $3.497,40\ \text{€}$ |
| **3** | $3.497,40\ \text{€}$ | $\mathbf{3.672,27\ \text{€}}$ | $174,87\ \text{€}$ | $\mathbf{3.497,40\ \text{€}}$ | $\mathbf{0,00\ \text{€}}$ |

---

## 2. Steuerparadoxon (Johansson-Mellgren-Effekt)

### Definition & Bedingung
Das **Steuerparadoxon** beschreibt den Zustand, bei dem der Kapitalwert einer Investition nach Steuern ($K_s$) höher ist als der Kapitalwert vor Steuern ($K_0$).

* **Mathematische Bedingung:** $$K_s > K_0$$

### Mechanismus & Stellschrauben
* **Anpassung des Kalkulationszinsfusses (Standard-Modell):**
    $$i_s = i \cdot (1 - s)$$
    *(wobei $s$ = Ertragsteuersatz, $i$ = Vorsteuer-Zinsfuss)*
* **Ermittlung der steuerlichen Bemessungsgrundlage:**
    $$\text{Zu versteuerndes Einkommen} = \text{EZÜ} - \text{AfA} - \text{Fremdkapitalzinsen}$$
* **Einzahlungsüberschuss nach Steuern ($EZÜ_s$):**
    $$EZÜ_s = EZÜ - (\text{Zu versteuerndes Einkommen} \cdot s)$$

> [!INFO] Ökonomische Ursachenkette für die Klausurbegründung
> 1. Der **Abzinsungseffekt** durch den gesunkenen Kalkulationszinsfuß ($i_s < i$) wirkt kapitalwerterhöhend.
> 2. Die **steuerliche Absetzbarkeit** der Abschreibungen (AfA) mindert die Steuerbasis in frühen Perioden massiv.
> 3. Überwiegt der positive Zinseffekt den negativen Effekt der Steuerzahlungen auf die EZÜ, steigt der Gesamtkapitalwert an.

### Klausur-Anwendungsbeispiel (Nachweis des Paradoxons)
**Gegebene Daten:**
* Anschaffungsauszahlung ($I_0$) = $100\ \text{€}$
* $EZÜ_1 = 20\ \text{€}$ | $EZÜ_2 = 100\ \text{€}$
* Kalkulationszins vor Steuern ($i$) = $10\% = 0,10$
* Steuersatz ($s$) = $50\% = 0,50$
* Abschreibung ($AfA$): Linear über 2 Jahre ($50\ \text{€}/\text{Jahr}$)
* *Annahme:* Voller Verlustausgleich mit anderen Einkunftsarten im selben Jahr möglich.

**Schritt 1: Kapitalwert vor Steuern ($K_0$)**
$$K_0 = -100 + \frac{20}{1,10^1} + \frac{100}{1,10^2} = -100 + 18,18 + 82,64 = \mathbf{0,82\ \text{€}}$$

**Schritt 2: Ermittlung der Werte nach Steuern**
* Nachsteuer-Zinssatz: $i_s = 0,10 \cdot (1 - 0,50) = \mathbf{0,05\ (5\%)}$
* **Periode 1:**
  * Zu versteuerndes Einkommen = $20 - 50 = -30\ \text{€}$ (Steuerlicher Verlust)
  * Steuerzahlung = $-30 \cdot 0,50 = -15\ \text{€}$ (Steuererstattung / Steuerersparnis)
  * $EZÜ_{s,1} = 20 - (-15) = \mathbf{35\ \text{€}}$
* **Periode 2:**
  * Zu versteuerndes Einkommen = $100 - 50 = 50\ \text{€}$
  * Steuerzahlung = $50 \cdot 0,50 = 25\ \text{€}$
  * $EZÜ_{s,2} = 100 - 25 = \mathbf{75\ \text{€}}$

**Schritt 3: Kapitalwert nach Steuern ($K_s$)**
$$K_s = -100 + \frac{35}{1,05^1} + \frac{75}{1,05^2} = -100 + 33,33 + 68,03 = \mathbf{1,36\ \text{€}}$$

**Klausur-Fazit:**
Da $K_s\ (1,36\ \text{€}) > K_0\ (0,82\ \text{€})$, ist das **Steuerparadoxon mathematisch bewiesen**. Die Ursache liegt hier am massiven Zinseffekt (Sinken von $10\%$ auf $5\%$) kombiniert mit dem vorgezogenen Tax Shield in Periode 1.

---

## 3. Vollständiger Finanzplan (VOFI) & VOFI-Rendite

### Systematik
Der VOFI bildet die tatsächliche **Endvermögensentwicklung** unter expliziter Berücksichtigung der Finanzierungsstruktur (Eigenkapital- und Fremdkapitalkombination) sowie differenzierter Soll- und Habenzinssätze ab.

### Struktureller Tabellenaufbau (Klausurschema)

| Position | Periode 0 | Periode 1 bis n-1 | Periode n |
| :--- | :--- | :--- | :--- |
| **+ Operativer EZÜ** | 0 | $EZÜ_t$ | $EZÜ_n$ |
| **+ Kreditaufnahme** | $FK_0$ | 0 | 0 |
| **- Kredittilgung** | 0 | 0 oder Tilgungsrate | Gesamte Resttilgung |
| **= Kreditbestand (Ende)** | $FK_0$ | $FK_t$ | 0 |
| **+ Anfangskontostand** | 0 | $\text{Kontostand}_{t-1}$ | $\text{Kontostand}_{n-1}$ |
| **+/- Zinssaldo (Haben/Soll)** | 0 | $\text{Zins}_t$ | $\text{Zins}_n$ |
| **= Kontostand (Ende)** | 0 | $\text{Kontostand}_t$ | **Endvermögen (EV)** |

> [!NOTE] Zinsberechnungs-Logik
> * Wenn $\text{Anfangskontostand} > 0 \rightarrow \text{Habenzins} = \text{Anfangskontostand} \cdot i_{\text{Haben}}$ (Zinszufluss)
> * Unabhängig davon: $\text{Sollzins} = \text{Kreditbestand}_{t-1} \cdot i_{\text{Soll}}$ (Zinsabfluss)

### VOFI-Rentabilität (Eigenkapitalrendite $r_{\text{vofi}}$)
Berechnung des effektiven Zinssatzes des tatsächlich gebundenen Eigenkapitals ($EK_0$):
$$r_{\text{vofi}} = \left(\frac{EV}{EK_0}\right)^{\frac{1}{n}} - 1$$

### Klausur-Interpretation
* Ist $r_{\text{vofi}} > i_{\text{Haben}}$, ist die Investition inkl. Finanzierung vorteilhafter als eine reine Geldanlage am Kapitalmarkt zum Habenzins.
* Tritt ein **Hebeleffekt (Leverage-Effekt)** auf, liegt dies daran, dass die Gesamtrendite des Projekts über dem Sollzinssatz des Fremdkapitals ($i_{\text{Soll}}$) liegt.

### Klausur-Anwendungsbeispiel (VOFI-Erstellung)
**Gegebene Daten:**
* Anschaffungsauszahlung in $t=0$: $100\ \text{€}$
* Eigenkapitaleinsatz ($EK_0$): $40\ \text{€}$
* Kreditaufnahme ($FK_0$): $60\ \text{€}$
* Zinssätze: $i_{\text{Soll}} = 6\% = 0,06$ | $i_{\text{Haben}} = 3\% = 0,03$
* Operative Zahlungen: $EZÜ_1 = 50\ \text{€}$ | $EZÜ_2 = 70\ \text{€}$
* Tilgungsstruktur: Endfällige Tilgung des gesamten Kredits am Ende von Periode 2 ($T_2 = 60\ \text{€}$).

**Berechnungsschritte:**
* **Periode 1:**
  * Anfangs-Kreditbestand = $60\ \text{€}$ $\rightarrow$ Sollzins = $60 \cdot 0,06 = 3,60\ \text{€}$ (Abfluss)
  * Girokonto-Endstand = $0 + 50\ (\text{EZÜ}) - 3,60\ (\text{Sollzins}) = \mathbf{46,40\ \text{€}}$
* **Periode 2:**
  * Anfangskontostand Giro = $46,40\ \text{€}$ $\rightarrow$ Habenzins = $46,40 \cdot 0,03 = \mathbf{1,39\ \text{€}}$ (Zufluss)
  * Sollzins auf unveränderten Kreditbestand = $60 \cdot 0,06 = 3,60\ \text{€}$ (Abfluss)
  * Endfällige Kredittilgung = $60,00\ \text{€}$
  * Endvermögen ($EV$) auf Girokonto = $46,40 + 70,00\ (\text{EZÜ}) + 1,39\ (\text{Habenzins}) - 3,60\ (\text{Sollzins}) - 60,00\ (\text{Tilgung}) = \mathbf{54,19\ \text{€}}$

| Position | Periode 0 | Periode 1 | Periode 2 |
|:---|:---:|:---:|:---:|
| **Operativer EZÜ** | $-100,00\ \text{€}$ | $+50,00\ \text{€}$ | $+70,00\ \text{€}$ |
| **Kreditaufnahme (FK)** | $+60,00\ \text{€}$ | $0,00\ \text{€}$ | $0,00\ \text{€}$ |
| **Kredittilgung** | $0,00\ \text{€}$ | $0,00\ \text{€}$ | $-60,00\ \text{€}$ |
| **Kreditbestand (Ende)** | $60,00\ \text{€}$ | $60,00\ \text{€}$ | $0,00\ \text{€}$ |
| **Anfangskontostand Giro** | $0,00\ \text{€}$ | $0,00\ \text{€}$ | $+46,40\ \text{€}$ |
| **Zinssaldo (Haben + / Soll -)** | $0,00\ \text{€}$ | $-3,60\ \text{€}$ | $+1,39\ \text{€}\ (\text{Haben}) \\ -3,60\ \text{€}\ (\text{Soll})$ |
| **Kontostand Giro (Ende)** | $\mathbf{0,00\ \text{€}}$ | $\mathbf{+46,40\ \text{€}}$ | $\mathbf{+54,19\ \text{€} = EV}$ |

**Berechnung der VOFI-Rentabilität ($r_{\text{vofi}}$):**
$$r_{\text{vofi}} = \left(\frac{54,19\ \text{€}}{40,00\ \text{€}}\right)^{\frac{1}{2}} - 1 = \sqrt{1,35475} - 1 \approx 1,16394 - 1 = \mathbf{16,39\%}$$

**Interpretation für die Klausur:**
Die Investition erzielt unter Berücksichtigung der Mischfinanzierung eine Eigenkapitalrendite von **$16,39\%$**. Da dieser Wert weit über dem alternativen Habenzins ($3\%$) liegt, ist das Projekt absolut vorteilhaft. Zudem zeigt sich ein positiver Leverage-Effekt, da die Rendite über den Fremdkapitalkosten ($6\%$) liegt.
