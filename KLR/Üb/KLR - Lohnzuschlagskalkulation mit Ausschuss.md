### 1. Theoretischer Hintergrund & Logik
Die **Lohnzuschlagskalkulation** ist ein traditionelles Verfahren der Zuschlagskalkulation. Sie nutzt die **Fertigungseinzelkosten (FEK / Fertigungslöhne)** als vertikale Zuschlagsbasis, um die **Fertigungsgemeinkosten (FGK)** (z. B. Abschreibungen auf Maschinen, Hallenmiete, Meistergehälter) proportional auf die Produkte zu verteilen.

Tritt in der Fertigung **Ausschuss** (Fehlproduktion) auf, müssen die gesamten Fertigungskosten der produzierten Menge auf die verbleibenden, tatsächlich *verkäuflichen* Einheiten umgelegt werden. Dies führt zu steigenden Stückkosten.

---

### 2. Mathematische Formeln & Ablauf-Schema

#### Schritt 1: Verteilung der Fertigungseinzelkosten (FEK)
Ist nur die Gesamtsumme der Lohnkosten gegeben, erfolgt die Aufteilung über die gesamten Arbeitsstunden:
$$\text{Lohnsatz (€/Std.)} = \frac{\text{Gesamte Lohnkosten (€)}}{\text{Gesamte Arbeitszeit aller Produkte (Std.)}}$$
$$\text{FEK}_{\text{Produkt}} = \text{Arbeitsstunden}_{\text{Produkt}} \cdot \text{Lohnsatz}$$

#### Schritt 2: Ermittlung des FGK-Zuschlagssatzes
$$\text{FGK-Zuschlagssatz (\%)} = \frac{\text{Gesamte Fertigungsgemeinkosten (€)}}{\text{Gesamte Fertigungseinzelkosten (€)}} \cdot 100$$

#### Schritt 3: Berechnung der Gesamtfertigungskosten
$$\text{Fertigungskosten}_{\text{Gesamt}} = \text{FEK} + \text{FGK} = \text{FEK} \cdot (1 + \text{Zuschlagssatz})$$

#### Schritt 4: Stückkostenberechnung unter Berücksichtigung des Ausschusses
$$\text{Verkäufliche Menge} = \text{Produktionsmenge} \cdot (1 - \text{Ausschussquote})$$
$$\text{Fertigungskosten pro Stück (€/Stck.)} = \frac{\text{Gesamtfertigungskosten des Produkts (€)}}{\text{Verkäufliche Menge (Stck.)}}$$

---

### 3. Konkretes Klausurbeispiel (gemäß image_17befb.jpg)

#### Gegebene Basisdaten:
* **Gesamte Lohnkosten (FEK):** $500.000\ \text{€}$
* **Gesamte Fertigungsgemeinkosten (FGK):** $350.000\ \text{€}$

| Produkt | Arbeitszeit (Std./Stck.) | Produktionsmenge | Ausschussquote | Verkaufspreis (€/Stck.) |
| :--- | :--- | :--- | :--- | :--- |
| **A** | $0,1$ | $1.000\ \text{Stck.}$ | $15\ \%$ | $400\ \text{€}$ |
| **B** | $0,05$ | $10.000\ \text{Stck.}$ | $15\ \%$ | $100\ \text{€}$ |
| **C** | $0,1$ | $4.000\ \text{Stck.}$ | $20\ \%$ | $500\ \text{€}$ |

#### Schritt-für-Schritt-Lösung:

##### 3.1 Fertigungseinzelkosten (FEK)
* **Gesamte Stunden:** $(1.000 \cdot 0,1) + (10.000 \cdot 0,05) + (4.000 \cdot 0,1) = 100 + 500 + 400 = 1.000\ \text{Std.}$
* **Lohnsatz:** $500.000\ \text{€} / 1.000\ \text{Std.} = 500\ \text{€ / Std.}$
* **FEK A:** $100\ \text{Std.} \cdot 500\ \text{€} = \mathbf{50.000\ \text{€}}$
* **FEK B:** $500\ \text{Std.} \cdot 500\ \text{€} = \mathbf{250.000\ \text{€}}$
* **FEK C:** $400\ \text{Std.} \cdot 500\ \text{€} = \mathbf{200.000\ \text{€}}$

##### 3.2 Zuschlagssatz & Gesamtfertigungskosten
* **Zuschlagssatz:** $350.000\ \text{€} / 500.000\ \text{€} = \mathbf{70\ \%}$ (Faktor $1,7$)
* **Fertigungskosten A:** $50.000\ \text{€} \cdot 1,7 = \mathbf{85.000\ \text{€}}$
* **Fertigungskosten B:** $250.000\ \text{€} \cdot 1,7 = \mathbf{425.000\ \text{€}}$
* **Fertigungskosten C:** $200.000\ \text{€} \cdot 1,7 = \mathbf{340.000\ \text{€}}$
*(Kontrolle: $85.000 + 425.000 + 340.000 = 850.000\ \text{€}$)*

##### 3.3 Fertigungskosten pro Stück (inkl. Ausschuss)
* **Produkt A:** $1.000\ \text{Stck.} - 15\ \% = 850\ \text{verkäufliche Stck.} \rightarrow 85.000\ \text{€} / 850 = \mathbf{100\ \text{€ / Stck.}}$
* **Produkt B:** $10.000\ \text{Stck.} - 15\ \% = 8.500\ \text{verkäufliche Stck.} \rightarrow 425.000\ \text{€} / 8.500 = \mathbf{50\ \text{€ / Stck.}}$
* **Produkt C:** $4.000\ \text{Stck.} - 20\ \% = 3.200\ \text{verkäufliche Stck.} \rightarrow 340.000\ \text{€} / 3.200 = \mathbf{106,25\ \text{€ / Stck.}}$

##### 3.4 Gesamtumsatz des Unternehmens
$$\text{Umsatz} = \sum (\text{Verkäufliche Menge} \cdot \text{Verkaufspreis})$$
* **Umsatz A:** $850\ \text{Stck.} \cdot 400\ \text{€} = 340.000\ \text{€}$
* **Umsatz B:** $8.500\ \text{Stck.} \cdot 100\ \text{€} = 850.000\ \text{€}$
* **Umsatz C:** $3.200\ \text{Stck.} \cdot 500\ \text{€} = 1.600.000\ \text{€}$
* **Gesamtumsatz:** $340.000 + 850.000 + 1.600.000 = \mathbf{2.790.000\ \text{€}}$

---

### 4. Klausur-Zusammenfassung & Fehlerquellen

> ⚠️ **Klausurfalle 1 (Basiswechsel):** Achte genau darauf, worauf sich der Ausschuss bezieht. Meistens ist es die *Produktionsmenge*. Die Multiplikation für den Umsatz darf dann **nur** mit der fehlerfreien Restmenge erfolgen.
> 
> ⚠️ **Klausurfalle 2 (Gemeinkostenbasis):** Die FGK werden im Rahmen der Lohnzuschlagskalkulation immer auf die **Lohnkosten (FEK)** aufgeschlagen, niemals direkt auf die Stunden oder die Stückzahlen.