### 1. Theoretischer Hintergrund & Grundprinzip
Die **Zuschlagskalkulation** dient der Ermittlung der Herstell- und Selbstkosten sowie des Verkaufspreises eines einzelnen Produkts (Kostenträgers). Sie trennt strikt zwischen direkt zurechenbaren Kosten und indirekten Kosten:

*   **Einzelkosten (Direkte Kosten):** Lassen sich direkt auf die einzelne Produkteinheit verbuchen (z. B. Fertigungsmaterial, Fertigungslohn).
*   **Gemeinkosten (Indirekte Kosten):** Fallen für den gesamten Betrieb oder Abteilungen an (z. B. Hallenmiete, Gehälter der Verwaltung). Sie werden im **Betriebsabrechnungsbogen (BAB)** gesammelt und über prozentuale **Zuschlagssätze** auf die Einzelkosten verrechnet.

---

### 2. Das Kalkulationsschema ("Kostentreppe")
In der Klausur wird die differenzierende Zuschlagskalkulation stufenweise von oben nach unten berechnet. Jeder Zuschlagssatz bezieht sich auf seine spezifische Basis.

| Kalkulationsstufe | Formel / Rechenweg | Basis für Zuschlagssatz |
| :--- | :--- | :--- |
|   Materialeinzelkosten (MEK) | *Direktwert aus Aufgabe* | - |
| + Materialgemeinkosten (MGK) | $+ \text{MEK} \cdot \text{MGK-Zuschlagssatz [\%]}$ | MEK |
| **= Materialkosten (MK)** | **= MEK + MGK** | - |
|   Fertigungseinzelkosten (FEK) | *Direktwert aus Aufgabe (Fertigungslohn)* | - |
| + Fertigungsgemeinkosten (FGK) | $+ \text{FEK} \cdot \text{FGK-Zuschlagssatz [\%]}$ | FEK |
| **= Fertigungskosten (FK)** | **= FEK + FGK** | - |
| **= Herstellkosten (HK)** | **= Materialkosten + Fertigungskosten** | **Basis für VwGK & VtGK** |
| + Verwaltungsgemeinkosten (VwGK) | $+ \text{HK} \cdot \text{VwGK-Zuschlagssatz [\%]}$ | Herstellkosten (HK) |
| + Vertriebsgemeinkosten (VtGK) | $+ \text{HK} \cdot \text{VtGK-Zuschlagssatz [\%]}$ | Herstellkosten (HK) |
| **= Selbstkosten (SK)** | **= HK + VwGK + VtGK** | **Basis für Gewinn** |
| + Gewinnzuschlag | $+ \text{SK} \cdot \text{Gewinnzuschlagsatz [\%]}$ | Selbstkosten (SK) |
| **= Barverkaufspreis (BVP)** | **= SK + Gewinn** | Netto-Verkaufspreis |

---

### 3. Mathematische Formeln der Zuschlagssätze (BAB-Schnittstelle)
Falls die Zuschlagssätze in der Klausur nicht gegeben sind, müssen sie zuerst mithilfe der Gesamtwerte aus dem Betriebsabrechnungsbogen (BAB) ermittelt werden:

*   **Materialgemeinkostensatz (MGK-Satz):**
    $$\text{MGK-Satz} = \frac{\text{Gesamte MGK}}{\text{Gesamte MEK}} \cdot 100\,\%$$
*   **Fertigungsgemeinkostensatz (FGK-Satz):**
    $$\text{FGK-Satz} = \frac{\text{Gesamte FGK}}{\text{Gesamte FEK}} \cdot 100\,\%$$
*   **Verwaltungsgemeinkostensatz (VwGK-Satz):**
    $$\text{VwGK-Satz} = \frac{\text{Gesamte VwGK}}{\text{Gesamte Herstellkosten der Periode}} \cdot 100\,\%$$
*   **Vertriebsgemeinkostensatz (VtGK-Satz):**
    $$\text{VtGK-Satz} = \frac{\text{Gesamte VtGK}}{\text{Gesamte Herstellkosten der Periode}} \cdot 100\,\%$$

> ⚠️ **Klausurfalle:** Die Zuschlagssätze für Verwaltung (VwGK) und Vertrieb (VtGK) beziehen sich in der differenzierenden Zuschlagskalkulation **immer** auf die Summe der Herstellkosten (HK) – niemals auf die jeweiligen Einzelkosten oder die reinen Fertigungskosten.