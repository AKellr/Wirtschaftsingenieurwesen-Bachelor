## 📥 Projektparameter (Basisdaten)
Ermittlung der effektiven Rendite (Interner Zinsfuß) einer Maschineninvestition mittels linearer Interpolation (Näherungsverfahren), da unregelmäßige Einzahlungsüberschüsse über die Laufzeit vorliegen.

* **Anschaffungskosten (A0):** 114.000 € (Auszahlung bei t = 0)
* **Nutzungsdauer (n):** 4 Jahre
* **Geforderte Mindestverzinsung (i):** 6 % p.a.

### Zahlungsstromübersicht (Zt)
* **Jahr 0 (t = 0):** -114.000 €
* **Jahr 1 (t = 1):** +30.000 €
* **Jahr 2 (t = 2):** +30.000 €
* **Jahr 3 (t = 3):** +30.000 €
* **Jahr 4 (t = 4):** +45.000 €

---

## 📐 Mathematische Auswertung & Lineare Interpolation

Das Verfahren benötigt zwei Versuchszinssätze, die das Ergebnis (Kapitalwert = 0) einschließen: einen positiven Kapitalwert (K1) und einen negativen Kapitalwert (K2).

### 1. Ermittelte Wertepaare
* **Zinssatz 1 (i1):** 6 % (0,06)  --> **Kapitalwert 1 (K1):** +1.832 €
* **Zinssatz 2 (i2):** 7 % (0,07)  --> **Kapitalwert 2 (K2):** -940 €

### 2. Berechnung des Internen Zinsfußes (r)
Formel für das Näherungsverfahren:
r = i1 - K1 * ((i2 - i1) / (K2 - K1))

**Einsetzen der berechneten Werte:**
r = 0,06 - 1.832 * ((0,07 - 0,06) / (-940 - 1.832))
r = 0,06 - 1.832 * (0,01 / -2.772)
r = 0,06 - (18,32 / -2.772)
r = 0,06 + 0,0066089
r ≈ 0,06661 --> **6,66 % p.a.**

---

## 🏛️ Ökonomische Beurteilung & Interpretation

> [!success] **Entscheidungsregel: Investition ist vorteilhaft (r > i)**
> Da die tatsächliche interne Verzinsung des Projekts mit **6,66 %** über den geforderten Kapitalkosten von **6,00 %** liegt, generiert die Maschine einen ökonomischen Mehrwert. Die Investition sollte durchgeführt werden.
