## 1. Konzeptioneller Hintergrund: CO₂-Kostenaufteilung
Die Fallstudie untersucht die ökonomische Lenkungswirkung von Umweltabgaben (hier: CO₂-Preis auf fossile Brennstoffe) im Mietwohnungsbestand. Nach der gesetzlichen Regelung bestimmt der **spezifische CO₂-Ausstoß pro Quadratmeter Wohnfläche und Jahr** ($kg\ CO_2 / m^2 \cdot a$), zu welchem Prozentsatz die CO₂-Kosten zwischen Mieter und Vermieter aufgeteilt werden.

* **Lenkungsziel:** Vermieter zu energetischen Sanierungen (z. B. Wärmedämmung) zu motivieren, um ihren prozentualen Kostenanteil zu senken.
* **Stufenmodell:** Je geringer der spezifische CO₂-Ausstoß des Gebäudes, desto geringer fällt der prozentuale Anteil aus, den der Vermieter tragen muss.

---

## 2. Empirische Datenbasis & Szenarienvergleich

### Rahmendaten des Objekts
* **Gesamte Wohnfläche:** $449\ m^2$ (Summe aller Mietparteien)
* **CO₂-Kostensatz (Jahr 1):** $30 EUR / \text{Tonne}$ (steigend auf bis zu $65EUR / \text{Tonne}$ in Folgeperioden)
* **Investitionsaufwand (Szenario II):** $40.000$ im Jahr 0 (Nutzungsdauer: 40 Jahre, Kalkulationszins: $3,5\ \%$)

### Systematischer Vergleich

| Parameter | Szenario I (Ist-Zustand) | Szenario II (Mit Wärmedämmung) |
| :--- | :--- | :--- |
| **Absoluter CO₂-Ausstoß** | $18.550\ kg / a$ | $14.840\ kg / a$ ($-20\ \%$ Einsparung) |
| **Spezifischer Ausstoß** | $\mathbf{41,31\ kg / m^2 \cdot a}$ | $\mathbf{33,05\ kg / m^2 \cdot a}$ |
| **Einstufung Gesetz** | Stufe: $> 42\ kg$ (bzw. oberer Bereich) | Stufe: $32 \text{ bis } < 37\ kg$ |
| **Verteilungsschlüssel** | **60 % Vermieter** / 40 % Mieter | **50 % Vermieter** / 50 % Mieter |

---

## 3. Mathematische Ermittlung der Vermieter-Ersparnis (Jahr 1)

1.  **Kostenbasis ohne Dämmung (Szenario I):**
    $$18,55t \times 30t = 556,50\ \implies \text{Anteil Vermieter } (60\ \%) = \mathbf{333,90}$$

2.  **Kostenbasis mit Dämmung (Szenario II):**
    $$14,84 t \times 30t = 445,20 \implies \text{Anteil Vermieter } (50\ \%) = \mathbf{222,60}$$

3.  **Netto-Ersparnis des Vermieters im Jahr 1:**
    $$\Delta \text{Kosten} = 333,90 - 222,60 = \mathbf{111,30}$$


## 4. Investitionsbewertung & Fazit

### Kapitalwertberechnung ($K_0$)
Wird die Anfangsauszahlung von $-40.000$€ mit den abgezinsten jährlichen CO₂-Kosteneinsparungen (unter Berücksichtigung des steigenden CO₂-Preispfades) über die 40-jährige Nutzungsdauer verrechnet, ergibt sich:

$$K_0 \approx \mathbf{-35.178,84}$$

### Ökonomische Interpretation

> [!CAUTION]
> **Kaufmännisches Fehlurteil & Staatsversagen:**
> 1. Die Investition in die Wärmedämmung ist für den Vermieter **massiv unvorteilhaft** ($K_0 \ll 0$). Die jährlichen Einsparungen bei der CO₂-Abgabe kompensieren das investierte Kapital bei weitem nicht.
> 2. **Versagen des Lenkungseffekts:** Die CO₂-Abgabe verfehlt in diesem Setup ihren klimapolitischen Zweck. Für den rational handelnden Vermieter ist es kaufmännisch deutlich günstiger, die CO₂-Strafzahlungen über 40 Jahre zu leisten, anstatt das Gebäude energetisch zu sanieren. Ohne zusätzliche Anreize (z. B. Modernisierungsumlage oder direkte Förderung) bleibt die Sanierungsquote aus Eigenantrieb null.