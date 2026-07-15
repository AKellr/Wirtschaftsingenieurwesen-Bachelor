## 📥 Konzeptdefinition
Die Methode des **Internen Zinsfußes** (Internal Rate of Return) ermittelt den Zinssatz, bei dem der Kapitalwert einer Investition exakt Null ergibt ($K_0 = 0$). 

Bei Vorliegen von **genau zwei Zahlungsströmen** (einmalige Auszahlung zu Beginn, einmalige Rückzahlung am Ende; keine Zwischenzahlungen) vereinfacht sich das sonst komplexe iterative Näherungsverfahren zu einer geschlossenen mathematischen Wurzelformel. Dies entspricht der klassischen Zinseszinsrechnung (endfällige Investition/Nullkuponanleihe).

---

## 📐 Mathematisches Instrumentarium

### Die Effektivzinsformel
$$r = \left( \sqrt[n]{\frac{\text{EZÜ}_n}{A_0}} - 1 \right) \cdot 100$$

**Variablenbelegung:**
* **$r$:** Interner Zinssatz in Prozent (% p.a.)
* **$n$:** Laufzeit der Investition in Perioden (Jahre)
* **$\text{EZÜ}_n$:** Einzahlungsüberschuss (Endwert/Liquidationserlös) am Ende der Laufzeit im Jahr $n$
* **$A_0$:** Anschaffungsauszahlung (Anfangsinvestition) zum Zeitpunkt Null ($t = 0$)

---

## 🧮 Exemplarische Anwendung (Lebensversicherung)

### Datenbasis
* $A_0 = 50.000\text{ €}$
* $\text{EZÜ}_{10} = 80.000\text{ €}$
* $n = 10\text{ Jahre}$

### Rechenschritte
1. **Verhältnismethode (Gesamtwachstumsfaktor):**
   $$\frac{\text{EZÜ}_{10}}{A_0} = \frac{80.000\text{ €}}{50.000\text{ €}} = 1,60$$
2. **Periodisierung (Geometrisches Mittel über $n$ Jahre):**
   $$\sqrt[10]{1,60} = 1,60^{\frac{1}{10}} \approx 1,048122$$
3. **Isolierung des Zinssatzes (Abzug des Barwerts 100 %):**
   $$1,048122 - 1 = 0,048122$$
4. **Prozentuierung:**
   $$0,048122 \cdot 100 = \mathbf{4,81\,\% \text{ p.a.}}$$

---

## 🏛️ Ökonomische Interpretation

> [!success] **Entscheidungsregel der IRR-Methode**
> * **$r > i$ (Kalkulationszins):** Die Investition ist vorteilhaft, da die effektive Rentabilität über den Mindestkapitalkosten liegt.
> * **$r = i$:** Die Investition erreicht exakt die geforderte Mindestverzinsung ($K_0 = 0$).
> * **$r < i$:** Die Investition ist unvorteilhaft.