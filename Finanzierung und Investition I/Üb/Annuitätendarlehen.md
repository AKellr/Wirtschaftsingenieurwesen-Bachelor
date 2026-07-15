### 1. Theoretischer Hintergrund
Bei einem **Annuitätendarlehen** bleibt die periodische Gesamtzahlung (die **Annuität**) über die gesamte Vertragslaufzeit hinweg konstant. Sie setzt sich aus zwei Komponenten zusammen:
*   **Zinsanteil ($Z_t$):** Berechnet sich in jeder Periode neu auf Basis des aktuellen Restschuldenstands zu Beginn des Jahres ($S_{t-1} \cdot i$). Da die Schuld kontinuierlich sinkt, nimmt der Zinsanteil degressiv ab.
*   **Tilgungsanteil ($T_t$):** Da die Annuität konstant bleibt, während der Zinsanteil sinkt, steigt der Tilgungsanteil progressiv an ($T_t = A - Z_t$).

---

### 2. Berechnung der Ausgangswerte
Basierend auf den Falldaten aus `image_f9a55c.png`:
*   **Darlehensbetrag ($S_0$):** 250.000 EUR
*   **Zinssatz ($i$):** 4,2% p.a.
*   **Anfängliche Tilgung ($t_1$):** 2,0% p.a.

$$\text{Annuitätsfaktor} = i + t_1 = 4,2\% + 2,0\% = 6,2\%$$
$$A = S_0 \cdot (i + t_1) = 250.000 \text{ EUR} \cdot 0,062 = \mathbf{15.500 \text{ EUR}}$$

Die feste jährliche Annuität beträgt somit über die gesamte Laufzeit hinweg exakt **15.500 EUR**.

---

### 3. Tilgungsplan (Jahre 1 bis 5)
Entsprechend der Berechnungen und der Tabellenstruktur aus `image_fa37c5.png`:

| Jahr ($t$) | Schuldenstand 1.1. ($S_{t-1}$) | Zinsanteil ($Z_t = 4,2\%$) | Tilgungsanteil ($T_t = A - Z_t$) | Annuität ($A$) |
| :---: | :---: | :---: | :---: | :---: |
| **1** | 250.000,00 EUR | 10.500,00 EUR | 5.000,00 EUR | 15.500,00 EUR |
| **2** | 245.000,00 EUR | 10.290,00 EUR | 5.210,00 EUR | 15.500,00 EUR |
| **3** | 239.790,00 EUR | 10.071,18 EUR | 5.428,82 EUR | 15.500,00 EUR |
| **4** | 234.361,18 EUR | 9.843,17 EUR | 5.656,83 EUR | 15.500,00 EUR |
| **5** | 228.704,34 EUR | 9.605,58 EUR | 5.894,42 EUR | 15.500,00 EUR |

*Hinweis zu Jahr 5:* Der verbleibende Schuldenstand zum 31.12. des 5. Jahres (bzw. zum 1.1. des 6. Jahres) beträgt nach Abzug der letzten Tilgung genau **222.809,92 EUR**.