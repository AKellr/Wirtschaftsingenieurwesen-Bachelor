### 1. Betriebsabrechnungsbogen (BAB)
Der BAB dient der Verteilung der Gemeinkosten auf die Hauptkostenstellen über spezifische Verteilungsschlüssel.

| Kto.    | Gemeinkostenart        | Buchhaltung (€) | Material (M) | Fertigung (F) | Verwaltung (Vw) | Vertrieb (Vt) | Verteilungsschlüssel / Basis |
| :------ | :--------------------- | :-------------- | :----------- | :------------ | :-------------- | :------------ | :--------------------------- |
| **41**  | Gemeinkostenmaterial   | 24.000          | 4.000        | 19.000        | 1.000           | --            | *Gegeben*                    |
| **42**  | Energie, Brennstoffe   | 36.000          | 6.000        | 18.000        | 6.000           | 6.000         | 1 : 3 : 1 : 1 (6 Anteile)    |
| **433** | Hilfslöhne             | 63.000          | 14.000       | 35.000        | 7.000           | 7.000         | 2 : 5 : 1 : 1 (9 Anteile)    |
| **439** | Gehälter               | 66.000          | --           | 6.000         | 30.000          | 30.000        | - : 1 : 5 : 5 (11 Anteile)   |
| **440** | Sozialkosten           | 40.000          | 4.000        | 20.000        | 12.000          | 4.000         | 2 : 10 : 6 : 2 (20 Anteile)  |
| **45**  | Instandsetzungen       | 22.000          | 2.000        | 18.000        | --              | 2.000         | 1 : 9 : - : 1 (11 Anteile)   |
| **46**  | Steuern                | 42.000          | 6.000        | 15.000        | 15.000          | 6.000         | 2 : 5 : 5 : 2 (14 Anteile)   |
| **47**  | Sonstige Kosten        | 144.000         | 12.000       | 12.000        | 96.000          | 24.000        | 1 : 1 : 8 : 2 (12 Anteile)   |
| **48**  | Kalkulatorische Kosten | 64.000          | 8.000        | 32.000        | 16.000          | 8.000         | 1 : 4 : 2 : 1 (8 Anteile)    |
| **Σ**   | **Summe Gemeinkosten** | **501.000**     | **56.000**   | **175.000**   | **183.000**     | **87.000**    | *Quersummenprüfung korrekt*  |

---

### 2. Berechnung der Gemeinkostenzuschlagssätze
Die Zuschlagssätze der Bereiche Material und Fertigung beziehen sich auf die jeweiligen Einzelkosten. Verwaltung und Vertrieb beziehen sich proportional auf die Herstellkosten (HK).

*   **Materialeinzelkosten (MEK):** 680.000 €
*   **Fertigungseinzelkosten (FEK):** 142.500 €

$$\text{MGK-Zuschlagssatz} = \frac{56.000}{680.000} \cdot 100\% \approx \mathbf{8{,}24\%}$$

$$\text{FGK-Zuschlagssatz} = \frac{175.000}{142.500} \cdot 100\% \approx \mathbf{122{,}81\%}$$

---

### 3. Kostenträgerblatt (Zuschlagskalkulation)

Die Kalkulation führt stufenweise von den Einzelkosten über die Herstellkosten bis hin zu den gesamten Selbstkosten des Auftrags.

$$\begin{aligned}
&\text{Materialeinzelkosten (MEK)} && \phantom{\cdot 100\%} & 680.000\ \text{€} \\
+\ &\text{Materialgemeinkosten (MGK)} && (\approx 8{,}24\% \text{ von MEK}) & 56.000\ \text{€} \\
+\ &\text{Fertigungseinzelkosten (FEK)} && & 142.500\ \text{€} \\
+\ &\text{Fertigungsgemeinkosten (FGK)} && (\approx 122{,}81\% \text{ von FEK}) & 175.000\ \text{€} \\
+\ &\text{Sondereinzelkosten der Fertigung (SEKf)} && & 198.500\ \text{€} \\
\hline
=\ &\mathbf{\text{Herstellkosten (HK)}} && & \mathbf{1.252.000\ \text{€}} \\
+\ &\text{Verwaltungsgemeinkosten (VwGK)} && (\approx 14{,}62\% \text{ von HK}) & 183.000\ \text{€} \\
+\ &\text{Vertriebsgemeinkosten (VtGK)} && (\approx 6{,}95\% \text{ von HK}) & 87.000\ \text{€} \\
\hline
=\ &\mathbf{\text{Selbstkosten (K}_s\mathbf{)}} && & \mathbf{1.522.000\ \text{€}}
\end{aligned}$$

