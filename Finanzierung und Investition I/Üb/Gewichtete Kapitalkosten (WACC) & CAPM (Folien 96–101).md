## 🧾 1. WACC mit Steuerschild (Tax Shield)
Der **WACC** (*Weighted Average Cost of Capital*) bildet die gewichteten Gesamtkapitalkosten eines Unternehmens ab. Da Fremdkapitalzinsen steuerlich absetzbar sind, mindern sie die Steuerlast. Das wird durch den Faktor $(1 - s)$ berücksichtigt.

$$\text{WACC} = r_{EK} \cdot \frac{EK}{GK} + r_{FK} \cdot (1 - s) \cdot \frac{FK}{GK}$$

> [!info] **Die Variablen:**
> - $r_{EK}$: Eigenkapitalkosten (Renditeforderung der Eigentümer)
> - $r_{FK}$: Fremdkapitalkosten (Nominalzins der Bank)
> - $s$: Ertragsteuersatz des Unternehmens
> - $\frac{EK}{GK}$: Eigenkapitalquote (Anteil am Gesamtkapital)
> - $\frac{FK}{GK}$: Fremdkapitalquote (Anteil am Gesamtkapital)

---

## 📊 2. CAPM (Capital Asset Pricing Model)
Das CAPM bestimmt die risikoadäquate Renditeforderung der Eigenkapitalgeber ($r_{EK}$), indem es das spezifische Risiko des Unternehmens ($\beta$) einrechnet.

$$r_{EK} = r_f + \beta \cdot (r_m - r_f)$$

> [!warning] **Die Variablen:**
> - $r_f$: Risikoloser Zinssatz (z. B. Rendite von Staatsanleihen)
> - $\beta$: Beta-Faktor (Risikomaß: $\beta > 1$ bedeutet riskanter als der Markt)
> - $(r_m - r_f)$: Marktrisikoprämie (Zusatzrendite des Aktienmarktes gegenüber dem risikolosen Zins)

# 📝 Rechenbeispiel: CAPM & WACC-Berechnung

## 📥 Gegebene Daten
- 📊 **Eigenkapitalquote ($\frac{EK}{GK}$):** 60 % (0,60)
- 🏦 **Fremdkapitalquote ($\frac{FK}{GK}$):** 40 % (0,40)
- 🛡️ **Risikoloser Zins ($r_f$):** 3 % (0,03)
- 📈 **Marktrendite ($r_m$):** 9 % (0,09)
- ⚖️ **Beta-Faktor ($\beta$):** 1,2
- 🏛️ **Fremdkapitalzins ($r_{FK}$):** 5 % (0,05)
- 💸 **Steuersatz ($s$):** 30 % (0,30)

---

## 🔢 Schritt 1: Eigenkapitalkosten ($r_{EK}$) via CAPM
$$\begin{aligned}
r_{EK} &= r_f + \beta \cdot (r_m - r_f) \\
r_{EK} &= 3\% + 1{,}2 \cdot (9\% - 3\%) \\
r_{EK} &= 3\% + 1{,}2 \cdot 6\% = \mathbf{10{,}2\%\ (0{,}102)}
\end{aligned}$$

---

## 🔢 Schritt 2: Gesamtkapitalkosten (WACC) mit Tax Shield
$$\begin{aligned}
\text{WACC} &= r_{EK} \cdot \frac{EK}{GK} + r_{FK} \cdot (1 - s) \cdot \frac{FK}{GK} \\
\text{WACC} &= 10{,}2\% \cdot 0{,}60 + 5\% \cdot (1 - 0{,}30) \cdot 0{,}40 \\
\text{WACC} &= 6{,}12\% + 5\% \cdot 0{,}70 \cdot 0{,}40 \\
\text{WACC} &= 6{,}12\% + 1{,}40\% = \mathbf{7{,}52\%\ (0{,}0752)}
\end{aligned}$$

> [!success] **Klausur-Fazit**
> Der steueradjustierte Mindestzinssatz (**WACC**) für dieses Unternehmen beträgt **7,52 %**. Investitionsprojekte müssen eine Rendite oberhalb dieser Grenze erwirtschaften, um den Wert des Unternehmens zu steigern.