## 1. Theoretisches Fundament & Prämisse
* **Kontenausgleichsverbot:** Eine strikte, laufzeitübergreifende Trennung von Finanzierungssphäre (Soll) und Investitionssphäre (Haben). 
* **Verwendungsbeschränkung:** Operative Einzahlungsüberschüsse (EZÜ) verbleiben zwingend auf dem Guthabenkonto und dürfen *nicht* zur vorzeitigen Rückzahlung/Tilgung des Kredits herangezogen werden.
* **Kalkulationszinsdifferenzierung:** Unvollkommener Kapitalmarkt mit asymmetrischen Zinssätzen: Sollzinssatz (`i_Soll`) > Habenzinssatz (`i_Haben`).

---

## 2. Mathematische Berechnungsverfahren

### Ansatz A: Iterative Kontenfortführung (Endogen)
Rekursive Ermittlung der Perioden-Endbestände beider Kontoinstanzen:
* **Fremdkapital-/Kreditkonto:**
  * Anfangsbestand ($t=0$): `Kreditbestand_0 = Anschaffungsauszahlung`
  * Zinsbelastung ($t$): `Sollzins_t = Kreditbestand_{t-1} * i_Soll`
  * Fortschreibung: `Kreditbestand_t = Kreditbestand_{t-1} + Sollzins_t`
* **Guthabenkonto:**
  * Anfangsbestand ($t=0$): `Guthaben_0 = 0`
  * Zinszufluss ($t$): `Habenzins_t = Guthaben_{t-1} * i_Haben`
  * Fortschreibung: `Guthaben_t = Guthaben_{t-1} + Habenzins_t + EZÜ_t`
* **Finaler Kontenausgleich ($t=n$):** `VEW = Guthaben_n - Kreditbestand_n`

### Ansatz B: Formelgestützte Direktaufzinsung (Exogen)
Ausnutzung der mathematischen Unabhängigkeit der Zahlungsströme bei Kontenausgleichsverbot:

$$\text{VEW} = -A_0 \cdot (1 + i_{\text{Soll}})^n + \sum_{t=1}^n \text{EZÜ}_t \cdot (1 + i_{\text{Haben}})^{n-t}$$

---

## 3. Klausurrelevante Berechnungsmatrix (Fallbeispiel)
* **Eingangsdaten:** $A_0 = 3.500.000\text{ €}$, $n = 4\text{ Jahre}$, $i_{\text{Soll}} = 10\,\%$, $i_{\text{Haben}} = 5\,\%$, $\text{EZÜ} = [700k / 1,2M / 1,4M / 1,4M]$.

| Komponente | Basiswert | Periode ($t$) | Restlaufzeit ($n-t$) | Aufzinsungsfaktor | Endwert ($t=4$) |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Kreditbasis** | -3.500.000 € | 0 | 4 | 1,4641 | -5.124.350 € |
| **EZÜ 1** | 700.000 € | 1 | 3 | 1,157625 | 810.337,50 € |
| **EZÜ 2** | 1.200.000 € | 2 | 2 | 1,1025 | 1.323.000 € |
| **EZÜ 3** | 1.400.000 € | 3 | 1 | 1,0500 | 1.470.000 € |
| **EZÜ 4** | 1.400.000 € | 4 | 0 | 1,0000 | 1.400.000 € |
| **Exakter VEW** | | | | | **-121.012,50 €** |

---

## 4. Kritische Fehlerquellen & Klausurtaktik (Moschinski-Falle)

* **Rundungsdifferenzen durch Tabellenabrundung:** Wird der Aufzinsungsfaktor für $t=1$ fälschlicherweise auf 4 Nachkommastellen abgeschnitten (`1,1576` statt `1,157625`), resultiert ein ungenauer Wert von $810.320\text{ €}$ und ein verfälschter Vermögensendwert von $-121.030\text{ €}$.
* **Klausur-Vorgabe:** Faktoren stets mit allen Nachkommastellen im Rechner halten und Zwischenergebnisse nicht verkürzt neu eintippen.
* **Entscheidungskriterium:**
  * $\text{VEW} \geq 0$: Das Investitionsvorhaben generiert eine Vermögensmehrung gegenüber der Fristenkongruenten Unterlassungsalternative am Kapitalmarkt. Vorteilhafthaut gegeben.
  * $\text{VEW} < 0$: Das Vorhaben mindert das Endvermögen. **Investition ist strikt abzulehnen**.