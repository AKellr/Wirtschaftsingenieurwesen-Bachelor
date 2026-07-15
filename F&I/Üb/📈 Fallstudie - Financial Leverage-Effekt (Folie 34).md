## 📊 1. Ausgangslage & Kerndaten
- **Gesamtkapital ($GK$):** 10.000.000 €
- **Operativer Gewinn ($GK$-Verzinsung):** 1.000.000 €
- **Gesamtkapitalrentabilität ($r_{GK}$):** 10 %

---

## 🧮 2. Mathematische Formeln
Die klassische Leverage-Formel zur direkten Berechnung lautet:
$$r_{EK} = r_{GK} + \frac{FK}{EK} \cdot (r_{GK} - k)$$

Alternativ über die schrittweise Ermittlung für die Tabellenklausur:
1. $\text{Zinszahlung} = FK \cdot k$
2. $\text{Restgewinn} = \text{Operativer Gewinn} - \text{Zinszahlung}$
3. $r_{EK} = \frac{\text{Restgewinn}}{EK} \cdot 100\%$

---

## 📋 3. Szenarien-Vergleich (Klausurmatrix)

| Teilaufgabe          | Eigenkapital ($EK$) | Fremdkapital ($FK$) | Verschuldungsgrad ($\frac{FK}{EK}$) | Zinssatz ($k$) | Zinszahlung | Restgewinn | Eigenkapitalrendite ($r_{EK}$) | Hebel-Wirkung              |
| :------------------- | :-----------------: | :-----------------: | :---------------------------------: | :------------: | :---------: | :--------: | :----------------------------: | :------------------------- |
| **a) Basis-Hebel**   |  5.000.000 € (50%)  |  5.000.000 € (50%)  |               **1,0**               |      8 %       |  400.000 €  | 600.000 €  |            **12 %**            | Positiver Leverage 📈      |
| **b) Maximal-Hebel** |  2.000.000 € (20%)  |  8.000.000 € (80%)  |               **4,0**               |      8 %       |  640.000 €  | 360.000 €  |            **18 %**            | Starker positiver Hebel 🚀 |
| **c) Hebel-Falle**   |  2.000.000 € (20%)  |  8.000.000 € (80%)  |               **4,0**               |      13 %      | 1.040.000 € | -40.000 €  |            **-2 %**            | Negativer Leverage 📉      |
|                      |                     |                     |                                     |                |             |            |                                |                            |
|                      |                     |                     |                                     |                |             |            |                                |                            |
	
---

## 💡 4. Klausur-Interpretation & Key Insights

> [!success] **Der positive Leverage-Effekt (Szenario a & b)**
> - **Kernbedingung:** $r_{GK} > k$ (Die Gesamtkapitalrendite ist *höher* als der Fremdkapitalzins; hier: $10\% > 8\%$).
> - **Effekt:** Unter dieser Bedingung führt jede Erhöhung des Fremdkapitalanteils (steigender Verschuldungsgrad $\frac{FK}{EK}$) zu einer **Erhöhung der Eigenkapitalrendite** ($r_{EK}$). Das Unternehmen verdient mit dem geliehenen Geld mehr, als es an Zinsen an die Bank zurückzahlen muss.

> [!danger] **Der negative Leverage-Effekt / Die Hebel-Falle (Szenario c)**
> - **Kernbedingung:** $r_{GK} < k$ (Die Gesamtkapitalrendite ist *niedriger* als der Fremdkapitalzins; hier: $10\% < 13\%$).
> - **Effekt:** Der Hebel schlägt gnadenlos ins Negative um. Erhöht man in dieser Situation den Fremdkapitalanteil, **sinkt die Eigenkapitalrendite drastisch** (hier auf **-2 %**). 
> - **Klausur-Fazit:** Obwohl das Unternehmen operativ absolut profitabel arbeitet (1 Mio. € Gewinn), rutschen die Eigentümer durch die Zinslast in die Verlustzone. Das finanzielle Risiko steigt bei hoher Verschuldung überproportional.