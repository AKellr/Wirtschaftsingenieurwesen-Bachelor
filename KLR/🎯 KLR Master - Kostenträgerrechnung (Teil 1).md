## 🏭 1. Fertigungsarten & Kalkulationsverfahren
- **Massenfertigung:** Ein einziges Produkt wird dauerhaft in Großserie hergestellt (z. B. Strom, Zement) $\rightarrow$ **Divisionskalkulation** 📑
- **Sortenfertigung:** Ähnliche Produkte aus dem gleichen Grundstoff, die sich leicht unterscheiden (z. B. Bier, Joghurt) $\rightarrow$ **Äquivalenzziffernrechnung** 🥤
- **Serien- oder Einzelfertigung:** Unterschiedliche Produkte nach Kundenauftrag oder in Chargen (z. B. Spezialmaschinen, Möbel) $\rightarrow$ **Zuschlagskalkulation** 🚗

## 🥤 2. Die Äquivalenzziffernrechnung
- **Ziel:** Kostenverteilung auf Produktvarianten über Gewichtungsfaktoren (Äquivalenzziffer $f$). Das festgelegte Basisprodukt erhält immer den Faktor $f = 1,0$.

### 🧮 Das mathematische Rechenschema (Unser Beispiel)
- **Basisdaten:**
  - 🍺 Sorte A (Helles - Basis): $x_1 = 1.000$ Liter | $f_1 = 1,0$
  - 🟤 Sorte B (Dunkles): $x_2 = 500$ Liter | $f_2 = 1,2$
  - 💰 Gesamtkosten ($K_{\text{ges}}$): 3.200 €

- **Schritt 1: Echte Mengen in Recheneinheiten (RE) umrechnen**
  - $\text{RE} = \text{Menge } (x) \times \text{Äquivalenzziffer } (f)$
  - Sorte A: $1.000 \times 1,0 = 1.000 \text{ RE}$
  - Sorte B: $500 \times 1,2 = 600 \text{ RE}$
  - **Gesamte Recheneinheiten ($\sum \text{RE}$):** $1.000 + 600 = 1.600 \text{ RE}$

- **Schritt 2: Kosten pro Recheneinheit ermitteln**
  - $\text{Kosten pro RE} = \frac{K_{\text{ges}}}{\sum \text{RE}} = \frac{3.200}{1.600 \text{ RE}} = 2,00 \text{ pro RE}$

- **Schritt 3: Finale Stückkosten pro Sorte berechnen**
  - $\text{Stückkosten} = \text{Kosten pro RE} \times f$
  - 🍺 Sorte A: $2,00 \times 1,0 = \mathbf{2,00 \text{ pro Liter}}$
  - 🟤 Sorte B: $2,00 \times 1,2 = \mathbf{2,40 \text{ pro Liter}}$

# 🎯 KLR Master: Kostenträgerrechnung (Teil 2)

## 🚗 1. Die Zuschlagskalkulation
- **Prinzip:** Trennung von Einzelkosten (direkt zuordenbar) und Gemeinkosten (über prozentuale Zuschlagsätze aus dem BAB aufgeschlagen).
- **Wichtig:** Verwaltungsgemeinkosten (VwGK) und Vertriebsgemeinkosten (VtGK) werden immer von den **Herstellkosten** berechnet!

### 🧮 Berechnungsbeispiel (Spezialmaschine)
- **Materialbereich:**
  - Materialeinzelkosten (MEK): `10.000 €`
  - + Materialgemeinkosten (MGK) (15 % von MEK): `1.500 €`
  - **= Materialkosten:** `11.500 €`
- **Fertigungsbereich:**
  - Fertigungseinzelkosten (FEK): `8.000 €`
  - + Fertigungsgemeinkosten (FGK) (125 % von FEK): `10.000 €`
  - **= Fertigungskosten:** `18.000 €`
- **Herstellkosten & Selbstkosten:**
  - **Herstellkosten (HK)** (Materialkosten + Fertigungskosten): `29.500 €`
  - + Verwaltungsgemeinkosten (VwGK) (10 % von HK): `2.950 €`
  - + Vertriebsgemeinkosten (VtGK) (5 % von HK): `1.475 €`
  - **= Selbstkosten (SK):** `33.925 €`

## 📑 2. Die Divisionskalkulation (Mehrstufig)
- **Prinzip:** Wird bei Massenfertigung angewendet. Bei Lagerveränderungen (Bestandserhöhung/-minderung) müssen Produktions- und Vertriebsmengen getrennt berechnet werden.
- **Formel:** $\text{Selbstkosten pro Stück} = \frac{\text{Herstellkosten}}{\text{Produktionsmenge}} + \frac{\text{Vertriebskosten}}{\text{Absatzmenge}}$
- **Beispiel:** 10.000 Stück produziert (50.000 € HK), 8.000 Stück verkauft (16.000 € VtK)
  - $5,00 \text{ HK/Stück} + 2,00 \text{ VtK/Stück} = \mathbf{7,00 \text{ Selbstkosten/Stück}}$

## 🛢️ 3. Die Kuppelkalkulation
- **Prinzip:** Kostenaufteilung bei Prozessen, bei denen zwangsläufig mehrere Produkte gleichzeitig entstehen (z. B. Raffinerie).
- **Restwertmethode:** Ein Hauptprodukt + Nebenprodukte. Erlöse der Nebenprodukte reduzieren die Kosten des Hauptprodukts.
- **Marktwertmethode:** Mehrere gleichwertige Hauptprodukte. Die Gesamtkosten werden proportional zum Marktwert (Verkaufserlös) der Produkte aufgeteilt.
# 🎯 KLR Master: Kostenträgerrechnung (Teil 3)

## 📈 1. Die Verkaufskalkulation (Vorwärtskalkulation)
- **Prinzip:** Rechnet von den Selbstkosten (SK) hoch zum Brutto-Listenverkaufspreis (Brutto-LVP), den der Endkunde im Laden oder laut Katalog sieht.
- **⚠️ Die Klausurfalle:** Während der Gewinn ein einfacher Aufschlag *vom Hundert* ist, werden Skonto und Rabatt bei der Vorwärtskalkulation *im Hundert* gerechnet. Der Grund: Der Kunde zieht diese Prozentsätze später vom jeweils höheren Listen- oder Zielpreis ab, weshalb diese die Basis (100 %) bilden!
  - $\text{Zielverkaufspreis (ZVP)} = \frac{\text{Barverkaufspreis (BVP)}}{100 - \text{Skonto}\%} \times 100$
  - $\text{Netto-LVP} = \frac{\text{Zielverkaufspreis (ZVP)}}{100 - \text{Rabatt}\%} \times 100$

### 🧮 Berechnungsbeispiel (Spezialmaschine)
- **Selbstkosten (SK):** `33.925,00 €` (Basis 100 %)
- + Gewinnzuschlag (10 % von SK): `3.392,50 €`
- **= Barverkaufspreis (BVP):** `37.317,50 €` *(entspricht 98 % des Folgeschritts)*
- + Kundenskonto (2 % im Hundert): `761,58 €`
- **= Zielverkaufspreis (ZVP):** `38.079,08 €` *(entspricht 90 % des Folgeschritts)*
- + Kundenrabatt (10 % im Hundert): `4.231,01 €`
- **= Netto-Listenverkaufspreis (Netto-LVP):** `42.310,09 €` *(Basis für USt / 100 %)*
- + Umsatzsteuer (19 % von Netto-LVP): `8.038,92 €`
- **= Brutto-Listenverkaufspreis (Brutto-LVP):** `50.349,01 €`
