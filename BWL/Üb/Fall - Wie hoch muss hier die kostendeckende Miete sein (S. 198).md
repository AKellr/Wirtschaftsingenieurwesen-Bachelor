## 1. Konzeptioneller Hintergrund
Das Ziel dieses Falls ist die Ermittlung einer **kostendeckenden monatlichen Kaltmiete pro Quadratmeter** für ein kommunales Wohnungsbauprojekt der Stadt Koblenz. Bei dieser Rückwärtskalkulation wird der Zielkapitalwert der Investition exakt auf Null gesetzt ($K_0 = 0$). Damit die Investition wirtschaftlich die Waage hält, müssen die abgezinsten Mieteinnahmen (Barwert der Einzahlungen) exakt der Summe aller Anschaffungs- und laufenden Betriebskosten (Barwert der Auszahlungen) entsprechen.

---

## 2. Datenbasis & Ermittlung der Anfangsinvestition (Jahr 0)

### Flächenberechnung
* **Netto-Wohnfläche:** $100 \text{ Wohnungen} \times 100\ qm = 10.000\ qm$
* **Erforderliche Nutzfläche (15 %):** $1.500\ qm$
* **Gesamte Baufläche:** $11.500\ qm$

### Kostenblöcke im Jahr 0
* **Reine Baukosten:** $11.500\ qm \times 3.500/qm = \mathbf{40.250.000}$
* **Grundstückskosten (inkl. 10 % Nebenkosten):** $5.000\ qm \times 800\ €/qm \times 1,10 = \mathbf{4.400.000\ €}$
* **Gesamte Anfangsauszahlung ($I_0$):** $40.250.000 + 4.400.000 = \mathbf{44.650.000}$

---

## 3. Dynamisierung & Rentenbarwertberechnung (Jahre 1–60)

### Prämierte Finanzparameter
* **Nutzungsdauer ($n$):** $60 \text{ Jahre}$
* **Kalkulationszinssatz ($i$):** $4,0\ \%$
* **Dynamisierung der Instandhaltung ($g$):** $2,5\ \%$ p.a. ab Jahr 2
* **Instandhaltung Basis (Jahr 1):** $1,5\ \%$ der reinen Baukosten = $\mathbf{603.750\ €}$

### Berechnung des effektiven Zinssatzes ($i_{\text{eff}}$)
Aufgrund der fortlaufenden Preissteigerung ($g$) bei gleichzeitiger Abzinsung ($i$) wird mit dem realen Effektivzins kalkuliert:
$$i_{\text{eff}} = \frac{1 + i}{1 + g} - 1 = \frac{1,04}{1,025} - 1 \approx \mathbf{1,4634\ \%}$$

### Rentenbarwertfaktor ($RBF$)
Unter Verwendung von $i_{\text{eff}} \approx 1,4634\ \%$ und $n = 60$ ergibt sich der Barwertfaktor für die laufenden Kosten:
$$RBF = \frac{(1 + 0,014634)^{60} - 1}{(1 + 0,014634)^{60} \times 0,014634} \approx \mathbf{39,83}$$

---

## 4. Synthese & Kalkulation der Zielmiete

### Gesamtkapitalwert der Auszahlungen (Kostenbarwert)
1. **Anfangsinvestition (Jahr 0):** $44.650.000\ €$
2. **Barwert Instandhaltung (Jahre 1–60):** $603.750\ € \times 39,83 = 24.047.363\ €$
3. **Gesamte Auszahlungen (heutiger Wert):** $\mathbf{68.697.363\ €}$

### Target-Kalkulation der Mieteinnahmen
Damit $K_0 = 0$ aufgeht, muss der Barwert der Einzahlungen exakt dem Barwert der Auszahlungen entsprechen ($68.697.363\ €$).

1. **Erforderliche Netto-Mieteinnahmen pro Jahr:**
   $$\text{Miete p.a.} = \frac{\text{Gesamtauszahlungen}}{RBF} = \frac{68.697.363}{39,83} \approx \mathbf{1.724.764 / \text{Jahr}}$$

2. **Erforderliche monatliche Kaltmiete pro Quadratmeter ($10.000\ qm$):**
   $$\text{Miete pro } m^2 \text{ und Monat} = \frac{1.724.764}{10.000\ qm \times 12 \text{ Monate}} \approx \mathbf{14,37}$$

> [!NOTE]
> **Kaufmännisches Fazit:**
> Um eine vollständige Kostendeckung über den Lebenszyklus von 60 Jahren bei einem Verzinsungsanspruch von 4,0 % zu realisieren, muss die Stadt Koblenz eine monatliche Kaltmiete von mindestens **14,37 €/qm** ansetzen. Liegt der politisch gewollte Mietpreis für "sozialverträgliches Wohnen" darunter, verzeichnet das Projekt einen negativen Kapitalwert und muss dauerhaft kommunal bezuschusst werden.