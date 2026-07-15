## 📥 Gegebene Basisdaten
* **Gesamtkapital ($GK$):** 40.000 €
* **Eigenkapital ($EK$):** 20.000 € (Anteil: $\frac{EK}{GK} = 0{,}5 \implies 50\%$)
* **Fremdkapital ($FK$):** 20.000 € (Anteil: $\frac{FK}{GK} = 0{,}5 \implies 50\%$)
* **Basiszinssatz (Bundesanleihen):** 5,4 %
* **Risikozuschlag EK:** 5 %-Punkte
* **Fremdkapitalzinssatz ($i_{FK}$):** 8 %
* **Ertragsteuersatz ($s$):** 30 % ($0{,}3$)

---

## 🧮 Mathematische Kernformel (WACC-Ansatz)
$$i = i_{EK} \cdot \frac{EK}{GK} + i_{FK} \cdot (1 - s) \cdot \frac{FK}{GK}$$

Wobei:
- $i$: Gewichteter Gesamtkapitalkostensatz (Weighted Average Cost of Capital)
- $i_{EK}$: Renditeerwartung der Eigenkapitalgeber
- $i_{FK}$: Nominaler Fremdkapitalzinssatz
- $s$: Ertragsteuersatz (bewirkt den Steuereffekt / *Tax Shield*)

---

## 🔢 Schritt-für-Schritt-Berechnung

### Schritt 1: Ermittlung der Eigenkapitalkosten ($i_{EK}$)
Die Eigenkapitalkosten setzen sich additiv aus dem risikofreien Basiszins und einer risikoadäquaten Prämie zusammen:
$$i_{EK} = \text{Basiszins} + \text{Risikozuschlag}$$
$$i_{EK} = 5{,}4\% + 5\% = \mathbf{10{,}4\%} \quad (\text{bzw. } 0{,}104)$$

### Schritt 2: Ermittlung der Fremdkapitalkosten nach Steuern
Da Fremdkapitalzinsen steuerlich als Betriebsausgaben abziehbar sind, mindern sie die Ertragsteuerlast des Unternehmens. Die effektiven Kosten sinken um das *Tax Shield*:
$$i_{FK, \text{nach Steuern}} = i_{FK} \cdot (1 - s)$$
$$i_{FK, \text{nach Steuern}} = 8\% \cdot (1 - 0{,}3) = 8\% \cdot 0{,}7 = \mathbf{5{,}6\%} \quad (\text{bzw. } 0{,}056)$$

### Schritt 3: Gewichtung und finale Aggregationsrechnung
Einsetzen aller Teilkomponenten in die WACC-Gleichung:
$$i = 0{,}104 \cdot \frac{20.000}{40.000} + 0{,}08 \cdot (1 - 0{,}3) \cdot \frac{20.000}{40.000}$$
$$i = 0{,}104 \cdot 0{,}5 + 0{,}056 \cdot 0{,}5$$
$$i = 0{,}052 + 0{,}028 = \mathbf{0{,}08} \implies \mathbf{8\%}$$

---

## 💡 Controlling-Interpretation & Klausur-Fazit

> [!info] **Das Konzept des Tax Shields**
> Der Ausdruck $(1 - s)$ korrigiert die nominellen Fremdkapitalkosten nach unten. Im konkreten Fall zahlt das Unternehmen zwar nominal 8 % Zinsen an die Bank, per Saldo betragen die effektiven Kosten aufgrund der Steuerersparnis jedoch nur **5,6 %**. Dies erklärt, warum eine moderate Fremdfinanzierung oft eine kapitalsenkende Wirkung auf die Gesamtkapitalkosten hat.

> [!warning] **Mindestrendite für Investitionen (Hurdle Rate)**
> Der ermittelte Mischzinssatz von **8 %** fungiert als kalkulatorische Mindestrendite (*Hurdle Rate*) für das geplante Projekt. 
> * **Entscheidungsregel:** Das Investitionsobjekt ist nur dann absolut vorteilhaft, wenn seine interne Verzinsung oder die geplante Gesamtkapitalrendite **über 8 %** liegt. Liegt sie darunter, wird trotz eines eventuell positiven Buchgewinns der Wert für die Eigenkapitalgeber vernichtet.