### 1. Theoretischer Hintergrund & Logik
Die **Kurzfristige Erfolgsrechnung (KER)** (auch betriebswirtschaftliche Auswertung / BWA genannt) ist ein zentrales Controlling-Instrument zur unterjährigen Überwachung des Betriebsergebnisses (meist monatlich oder quartalsweise). Im Gegensatz zur jährlichen Gewinn-und-Verlust-Rechnung (GuV) der Finanzbuchhaltung erlaubt sie eine zeitnahe Steuerung des Unternehmens.

Es existieren zwei mathematisch gleichwertige Verfahren, die zum **identischen Betriebsergebnis** führen, jedoch unterschiedliche Strukturen aufweisen:

* **Gesamtkostenverfahren (GKV):** Produktionsorientiert. Es erfasst die *gesamten* Kosten, die in der Periode für die Produktion angefallen sind, und stellt sie der gesamten erbrachten Leistung (Umsatz + Bestandsveränderungen) gegenüber.
* **Umsatzkostenverfahren (UKV):** Absatzorientiert. Es stellt den Umsatzerlösen der Periode ausschließlich die Kosten der tatsächlich *verkauften* Produkte (Umsatzkosten) gegenüber. Lagerveränderungen tauchen hier nicht explizit auf.

---

### 2. Das mathematische Struktur-Schema



#### Gesamtkostenverfahren (GKV)
$$\begin{aligned}
& \text{Umsatzerlöse (abgesetzte Menge } \cdot \text{Verkaufspreis)} \\
+ & \text{Bestandserhöhungen (unverkaufte, auf Lager produzierte Ware } \cdot \text{Herstellkosten)} \\
- & \text{Bestandsminderungen (aus dem Lager verkaufte Ware } \cdot \text{Herstellkosten)} \\
+ & \text{Andere aktivierte Eigenleistungen} \\
\hline
= & \mathbf{\text{Gesamtleistung der Periode}} \\
- & \text{Gesamte primäre Kosten der Periode (Material, Personal, Abschreibungen etc.)} \\
\hline
= & \mathbf{\text{Betriebsergebnis (Erfolg)}} \\
\hline
\end{aligned}$$

#### Umsatzkostenverfahren (UKV)
$$\begin{aligned}
& \text{Umsatzerlöse (abgesetzte Menge } \cdot \text{Verkaufspreis)} \\
- & \text{Herstellkosten der abgesetzten/verkauften Menge} \\
- & \text{Vertriebskosten der Periode} \\
- & \text{Verwaltungskosten der Periode} \\
\hline
= & \mathbf{\text{Betriebsergebnis (Erfolg)}} \\
\hline
\end{aligned}$$

---

### 3. Umfassendes Berechnungsbeispiel (mit Lagerveränderung)

#### Ausgangsdaten einer Periode:
* **Produktionsmenge ($x_p$):** $1.000\ \text{Stück}$
* **Verkaufsmenge ($x_v$):** $800\ \text{Stück}$ (folglich $\Delta \text{Lager} = +200\ \text{Stück}$ Bestandserhöhung)
* **Verkaufspreis ($p$):** $15\ \text{€ / Stück}$
* **Herstellkosten der Produktion ($HK_{\text{Stück}}$):** $10\ \text{€ / Stück}$ (Gesamte HK = $10.000\ \text{€}$)
* **Vertriebs- & Verwaltungskosten ($VwVtgK$):** $1.200\ \text{€}$ (fallen periodenbezogen an)

#### Berechnung nach dem GKV:
1.  **Umsatzerlöse:** $800\ \text{Stück} \cdot 15\ \text{€} = 12.000\ \text{€}$
2.  **Bestandserhöhung:** $+200\ \text{Stück} \cdot 10\ \text{€} = +2.000\ \text{€}$
3.  **Gesamtleistung:** $12.000\ \text{€} + 2.000\ \text{€} = \mathbf{14.000\ \text{€}}$
4.  **Gesamtkosten:** Herstellkosten ($10.000\ \text{€}$) + VwVtgK ($1.200\ \text{€}$) = $\mathbf{11.200\ \text{€}}$

$$\text{Betriebsergebnis}_{\text{GKV}} = 14.000\ \text{€} - 11.200\ \text{€} = \mathbf{2.800\ \text{€}}$$

#### Berechnung nach dem UKV:
1.  **Umsatzerlöse:** $800\ \text{Stück} \cdot 15\ \text{€} = \mathbf{12.000\ \text{€}}$
2.  **Umsatzkosten (HK der verkauften Menge):** $800\ \text{Stück} \cdot 10\ \text{€} = \mathbf{-8.000\ \text{€}}$
3.  **Vertriebs- & Verwaltungskosten:** $\mathbf{-1.200\ \text{€}}$

$$\text{Betriebsergebnis}_{\text{UKV}} = 12.000\ \text{€} - 8.000\ \text{€} - 1.200\ \text{€} = \mathbf{2.800\ \text{€}}$$

*Ergebnis:* Beide Verfahren liefern exakt denselben Gewinn von **2.800 €**.

---

### 4. Vor- und Nachteile im Klausur-Vergleich

| Kriterium | Gesamtkostenverfahren (GKV) | Umsatzkostenverfahren (UKV) |
| :--- | :--- | :--- |
| **Gliederung** | Nach **Kostenarten** (Material, Personal etc.) | Nach **Funktionsbereichen** (Produktion, Vertrieb, Admin) |
| **Vorteile** | • Einfache Datenübernahme aus der FiBu<br>• Zeigt die gesamte Produktionsleistung inklusive Lageraufbau | • Sehr intuitiv (Kosten stehen direkt dem Erlös gegenüber)<br>• Internationaler Standard (IFRS/US-GAAP)<br>• Ermöglicht schnelle Bruttomargen-Analysen |
| **Nachteile** | • Unübersichtlich bei hoher Produktvielfalt<br>• Erfordert zwingend eine Bestandsaufnahme (Inventur/Lagerbuch) | • Aufwendige Aufteilung der Kostenstellen nach Funktionen in der Kostenrechnung nötig |
