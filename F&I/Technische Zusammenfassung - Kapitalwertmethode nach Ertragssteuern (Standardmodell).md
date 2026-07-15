## 1. Konzeptionelles Fundament

Das steueradjustierte Standardmodell der Investitionsrechnung modifiziert die klassische Barwertberechnung, um den Einfluss von Ertragssteuern auf Unternehmensebene realitätsgetreu abzubilden. Steuern wirken dabei auf zwei Ebenen:

- **Zahlungsstromebene:** Reduktion der operativen Zuflüsse durch Ertragssteuerzahlungen, gemildert durch steuerliche Entlastungseffekte (_Tax Shields_) aus Abschreibungen.
    
- **Kapitalmarktebene:** Reduktion des Kalkulationszinssatzes, da auch die Opportunität am Kapitalmarkt einer Besteuerung unterliegt.
    

## 2. Mathematisches Instrumentarium

### Steuerliche Anpassung des Kalkulationszinssatzes

Der Mindestzinssatz vor Steuern ($i_{\text{vor}}$) wird um den Ertragssteuersatz ($s$) gekürzt:

$$i_{\text{nach}} = i_{\text{vor}} \cdot (1 - s)$$

> [!example] Beispiel
> 
> $$12\% \cdot (1 - 0,30) = 8,4\%$$

### Modifizierte lineare Abschreibung (AfA)

Die jährliche Abschreibung berücksichtigt den investitionsendogenen Restbuchwert ($\text{RBW}$) am Ende der Nutzungsdauer ($n$):

$$\text{AfA}_t = \frac{A_0 - \text{RBW}_n}{n}$$

> [!example] Beispiel
> 
> $$\frac{104.000\text{ €} - 4.000\text{ €}}{5} = 20.000\text{ € pro Jahr}$$

### Steuerbemessungsgrundlage & Zahlungsstromkomponenten

Für die Perioden $t = 1$ bis $n-1$ gilt:

- **Steuerbemessungsgrundlage:**
    
    $$\text{StBMG}_t = \text{EZÜ}_{\text{vor},t} - \text{AfA}_t$$
    
- **Ertragssteuer auf den operativen Überschuss:**
    
    $$S_t = \text{StBMG}_t \cdot s$$
    
- **Zahlungsüberschuss nach Steuern:**
    
    $$\text{EZÜ}_{\text{nach},t} = \text{EZÜ}_{\text{vor},t} - S_t$$
    

### Endperiodenmodifikation ($t = n$) bei Liquidation

In der finalen Periode kommt es zur Aufdeckung stiller Reserven, sofern der Liquidationserlös ($L_n$) vom Restbuchwert ($\text{RBW}_n$) abweicht:

- **Steuerpflichtiger Veräußerungsgewinn:**
    
    $$\text{Gewinn}_{\text{Liq}} = L_n - \text{RBW}_n$$
    
- **Liquide Endkondition nach Steuern:**
    
    $$\text{EZÜ}_{\text{nach},n} = \text{EZÜ}_{\text{vor},n} + L_n - (s \cdot (\text{EZÜ}_{\text{vor},n} - \text{AfA}_n)) - (s \cdot (L_n - \text{RBW}_n))$$
    

## 3. Strukturierte Berechnungsmatrix (Fallbeispiel)

### Parameter

- $A_0 = 104.000\text{ €}$
    
- $n = 5$
    
- $s = 30\%$
    
- $i_{\text{nach}} = 8,4\%$
    
- $\text{RBW}_5 = 4.000\text{ €}$
    
- $L_5 = 10.000\text{ €}$
    

|**Periode (t)**|**EZÜ vor St.**|**AfA**|**Steuerbasis**|**Steuer (30%)**|**Sonder-CF (Liq)**|**EZÜ nach St.**|**Abzinsungsf. (8,4%)**|**Barwert (BW)**|
|---|---|---|---|---|---|---|---|---|
|**0**|-104.000 €|—|—|—|—|-104.000 €|1,0000|-104.000,00 €|
|**1**|50.000 €|-20.000 €|30.000 €|-9.000 €|—|41.000 €|0,9225|37.823,00 €|
|**2**|40.000 €|-20.000 €|20.000 €|-6.000 €|—|34.000 €|0,8510|28.934,00 €|
|**3**|30.000 €|-20.000 €|10.000 €|-3.000 €|—|27.000 €|0,7851|21.198,00 €|
|**4**|20.000 €|-20.000 €|0 €|0 €|—|20.000 €|0,7242|14.484,00 €|
|**5**|20.000 €|-20.000 €|0 €|0 €|+8.200 € *|28.200 €|0,6681|18.840,42 €|
|**KW**||||||||**+17.279,42 €**|

> [!info] * Zusammensetzung Periode 5
> 
> Operativer $\text{EZÜ}$ ($20.000\text{ €}$) + Liquidationserlös ($10.000\text{ €}$) - Steuer auf Liquidationsgewinn ($30\%$ von $[10.000\text{ €} - 4.000\text{ €}] = 1.800\text{ €}$) = $28.200\text{ €}$.

## 4. Entscheidungspräferenz & Heuristik

- **Entscheidungskriterium:** Is $\text{KW}_{\text{nach}} > 0$, realisiert die Investition über die Deckung der Anschaffungskosten und der steueradjustierten Mindestverzinsung hinaus einen Vermögenszuwachs. Die Vorteilhaftigkeit ex post Besteuerung ist somit gegeben.
    

> [!warning] Klausurtaktischer Fokus
> 
> Der Liquidationserlös darf im finalen Jahr nicht einfach unbesteuert addiert werden. Liegt der Verkaufserlös über dem Buchwert, greift die fiskalische Gewinnbesteuerung und mindert den Cashflow der Abschlussperiode.