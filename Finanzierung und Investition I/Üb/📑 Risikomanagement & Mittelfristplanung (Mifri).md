## 1. Mathematische Grundlagen & Definitionen
Im operativen Controlling wird das Risiko eines Sachverhalts über den mathematischen Erwartungswert (Risikowert) quantifiziert. Dieser dient als stochastischer Korrekturposten für die deterministische Mittelfristplanung ($Mifri$).

### Kernformel
$$R_{i,t} = S_{i,t} \cdot p_i$$

Wobei:
- $R_{i,t}$: Risikowert (Erwartungswert) des Risikos $i$ im Planjahr $t$
- $S_{i,t}$: Quantifiziertes Schadensausmaß (Gesamtrisiko) des Risikos $i$ im Planjahr $t$
- $p_i$: Stationäre Eintrittswahrscheinlichkeit des Risikos $i$ ($konstant$ über den Planungshorizont $T$)

### Bestimmung des relevanten Schadensausmaßes ($S_{i,t}$)
1. **Inkrementelles Risiko (Differenzbetrachtung):** Steigen bestehende Kostenpositionen (z. B. Energiebeschaffung), ist nur der *zusätzliche* finanzielle Mehrschaden als Risiko anzusetzen, da die Basis bereits im Budget enthalten ist:
   $$S_{t} = K_{\text{neu}, t} - K_{\text{Basis}, t}$$
2. **Variables Exposure (Prozentuales Risiko):** Bei Währungs- oder Marktpreisrisiken bezieht sich das Schadensausmaß oft nur auf einen volatilen Prozentsatz ($\alpha$) eines Gesamtvolumens ($V_t$):
   $$S_{t} = V_t \cdot \alpha$$

---

## 2. Strukturierte Zerlegung der Risikosachverhalte

### (1) Einkauf (Symmetrisches Mehrebenen-Risiko)
- **Basisaufwand:** $1{,}8\text{ Mio. € } p.a.$
- **Szenario:** Verdopplung in $t \in \{2, 3, 4, 5\}$ $\implies K_{\text{neu}} = 3{,}6\text{ Mio. €}$
- **Inkrementeller Schaden ($S$):** $3{,}6\text{ Mio. €} - 1{,}8\text{ Mio. €} = 1{,}8\text{ Mio. €}$
- **Erwartungswert ($R$):** $1{,}8\text{ Mio. €} \cdot 0{,}30 = 540.000\text{ € } p.a.$

### (2) Personal (Punktuelles Umsatzrisiko)
- **Szenario:** Kapazitätsengpass führt zu Umsatzunterlassung in $t=4$.
- **Schadenshöhe ($S$):** $2{,}3\text{ Mio. €}$
- **Erwartungswert ($R$):** $2{,}3\text{ Mio. €} \cdot 0{,}80 = 1.840.000\text{ €}$

### (3) Recht (Punktuelles Haftungsrisiko)
- **Szenario:** Produkthaftungsanspruch (USA) in $t=2$.
- **Schadenshöhe ($S$):** $4{,}6\text{ Mio. €}$
- **Erwartungswert ($R$):** $4{,}6\text{ Mio. €} \cdot 0{,}10 = 460.000\text{ €}$

### (4) Produktion (Asymmetrisches Periodenrisiko)
- **Szenario:** Technischer Anlagenausfall in $t=1$ und $t=2$.
- **Schadenshöhe ($S$):** $S_1 = 1{,}2\text{ Mio. €}$; $S_2 = 0{,}5\text{ Mio. €}$
- **Erwartungswert ($R$):**
  - $R_1 = 1{,}2\text{ Mio. €} \cdot 0{,}40 = 480.000\text{ €}$
  - $R_2 = 0{,}5\text{ Mio. €} \cdot 0{,}40 = 200.000\text{ €}$

### (5) Finanzen/Controlling (Währungs-Exposure)
- **Basisvolumen ($V$):** $65\text{ Mio. € } p.a.$ in $t \in \{3, 4\}$
- **Wechselkursrisiko ($\alpha$):** $10\%$
- **Schadenshöhe ($S$):** $65\text{ Mio. €} \cdot 0{,}10 = 6{,}5\text{ Mio. €}$
- **Erwartungswert ($R$):** $6{,}5\text{ Mio. €} \cdot 0{,}40 = 2.600.000\text{ € } p.a.$

---

## 3. Aggregationslogik im Risikobericht (Risk Matrix)

Die quantitative Risikoberichterstattung erfolgt über eine zweidimensionale Aggregation:

1. **Vertikale Aggregation (Jahresscheiben / Spaltensummen):** Identifiziert zeitliche Risikokonzentrationen innerhalb einer Planungsperiode.
   $$R_{\text{Gesamt}, t} = \sum_{i=1}^{n} R_{i,t}$$
2. **Horizontale Aggregation (Risikokategorien / Zeilensummen):** Kumuliert das Gesamtrisiko eines spezifischen Sachverhalts über den gesamten Zeithorizont $T$.
   $$R_{\text{Gesamt}, i} = \sum_{t=1}^{T} R_{i,t}$$

### Risikomatrix (Zusammenfassung in €)
| Kategorie ($i$) | Jahr 1 | Jahr 2 | Jahr 3 | Jahr 4 | Jahr 5 | $\sum$ Zeile ($R_{\text{Gesamt}, i}$) |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| **(1) Einkauf** | 0 | 540.000 | 540.000 | 540.000 | 540.000 | **2.160.000** |
| **(2) Personal** | 0 | 0 | 0 | 1.840.000 | 0 | **1.840.000** |
| **(3) Recht** | 0 | 460.000 | 0 | 0 | 0 | **460.000** |
| **(4) Produktion** | 480.000 | 200.000 | 0 | 0 | 0 | **680.000** |
| **(5) Finanzen** | 0 | 0 | 2.600.000 | 2.600.000 | 0 | **5.200.000** |
| **$\sum$ Spalte ($R_{\text{Gesamt}, t}$)** | **480.000** | **1.200.000** | **3.140.000** | **4.980.000** | **540.000** | 🎯 **10.340.000** |

---

## 4. Controlling-Implikationen & Risikosteuerung

> [!warning] **Risikoballung (Risk Concentration) in $t=4$**
> Mit einem kumulierten Risikowert von **4.980.000 €** weist das Jahr 4 die höchste Volatilität auf. Ursächlich ist das synchrone Zusammentreffen des makroökonomischen Währungsrisikos (Finanzen) und des operativen Kapazitätsrisikos (Personal). Die Liquiditätsreserve bzw. Risikopositionen in der Planbilanz für $t=4$ müssen asymmetrisch erhöht werden.

> [!danger] **Top-Risiko: Währungsrisiko China**
> Das FX-Risiko stellt mit einem Gesamtwert von **5,2 Mio. €** ($50{,}28\%$ des Gesamtrisikovolumens) das dominierende Einzelrisiko des Unternehmens dar. 
> *Mitigationsmaßnahme:* Implementierung von derivativen Sicherungsinstrumenten (z. B. Devisentermingeschäfte / FX Forwards), um den stochastischen Erwartungswert in eine deterministische, fixe Planungsgröße zu überführen.