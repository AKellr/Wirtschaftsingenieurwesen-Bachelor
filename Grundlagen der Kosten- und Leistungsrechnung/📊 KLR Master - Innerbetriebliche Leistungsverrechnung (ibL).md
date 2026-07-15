## 🎯 1. Das BAB-Umfeld & Ziel
- **Ziel:** Vollständige Entlastung der **Vorkostenstellen** (Hilfskostenstellen wie IT, Strom, Werkstatt) durch Weiterverteilung ihrer Kosten auf die Verbraucher, bis ihr Saldo im Betriebsabrechnungsbogen exakt **0,00 €** beträgt.
- **Empfänger:** Hauptsächlich **Endkostenstellen** (Hauptkostenstellen wie Material, Fertigung, Vertrieb), die direkt an den Produkten arbeiten.

## 🪜 2. Die drei Abrechnungsverfahren
1. **Anbauverfahren (Blockverfahren):** Ignoriert wechselseitige Beziehungen zwischen Vorkostenstellen komplett. Kosten fließen direkt an Endkostenstellen.
2. **Stufenleiterverfahren:** Rechnet Vorkostenstellen nacheinander in einer festgelegten Reihenfolge ab. Einmal geschlossene Stufen können keine Kosten mehr empfangen.
3. **Simultanverfahren (Mathematisches Verfahren):** Berücksichtigt den gegenseitigen Leistungsaustausch exakt über ein lineares Gleichungssystem (LGS). *Absoluter Klausur-Klassiker!*

## 🧮 3. Das Simultanverfahren (Unser Berechnungsbeispiel)
* **Basisdaten:**
  - Strom ($X_1$): 20.000 € primäre Kosten, erhält 10 Std. von Reparatur ($X_2$). Gesamtleistung: 2.000 kWh.
  - Reparatur ($X_2$): 30.000 € primäre Kosten, erhält 500 kWh von Strom ($X_1$). Gesamtleistung: 100 Std.

* **Gleichungssystem aufstellen:**
  1) $2.000 \cdot q_1 = 20.000 + 10 \cdot q_2$
  2) $100 \cdot q_2 = 30.000 + 500 \cdot q_1$

* **Wichtige Klausurregel:** Bei fortlaufenden Operationen und Zwischenschritten immer mit **vier Nachkommastellen** im Taschenrechner rechnen, um Rundungsfehler zu vermeiden!
  - Gleichung (2) nach $q_2$ auflösen: $q_2 = 300 + 5 \cdot q_1$
  - Einsetzen in (1) führt zu: $1.950 \cdot q_1 = 23.000$

* **Ergebnisse (Interne Verrechnungssätze):**
  - ⚡ **Strom ($q_1$):** `11,7949 € / kWh`
  - 🛠️ **Reparatur ($q_2$):** `358,9744 € / Std.`

## 🔄 4. Sekundärkostenverrechnung
- Die ermittelten Sätze ($q$) werden im BAB mit den verbrauchten Einheiten der Hauptkostenstellen multipliziert.
- *Beispiel Fertigung:* Verbrauch von 1.200 kWh Strom $\rightarrow 1.200 \times 11,7949 € = 14.153,88 €$ (bzw. exakt ungerundet über den TR-Zwischenspeicher: $14.153,85 €$).