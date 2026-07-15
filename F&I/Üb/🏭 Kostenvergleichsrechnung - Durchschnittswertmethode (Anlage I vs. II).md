## 📥 Gegebene Basisdaten
Vergleich zweier Produktionsanlagen unter Anwendung der finanzmathematischen **Durchschnittswertmethode** bei einem kalkulatorischen Zinssatz von **8 % p.a.**

| Parameter | Anlage I | Anlage II |
| :--- | :---: | :---: |
| Anschaffungskosten ($A_0$) | 50.000 € | 80.000 € |
| Restwert ($RW$) | 5.000 € | 10.000 € |
| Nutzungsdauer ($n$) | 5 Jahre | 5 Jahre |
| Leistungseinheiten / Jahr ($x$) | 40.000 LE | 50.000 LE |

---

## 📐 Mathematische Formeln der Durchschnittswertmethode

### 1. Kalkulatorische Abschreibung (linear)
Erfasst den jährlichen, gleichmäßigen Wertverzehr der Anlage über die Nutzungsdauer:
$$\text{kalk. Abschreibung} = \frac{A_0 - RW}{n}$$

### 2. Kalkulatorische Zinsen
Erfassen die Opportunitätskosten des im Durchschnitt gebundenen Kapitals über die Laufzeit:
$$\text{kalk. Zinsen} = \frac{A_0 + RW}{2} \cdot i$$

---

## 🧩 Schritt-für-Schritt-Berechnung & Kostenaufstellung

| Kostenposition | Berechnung Anlage I | Anlage I | Berechnung Anlage II | Anlage II |
| :--- | :--- | :---: | :--- | :---: |
| **kalk. Abschreibung** | $\frac{50.000 - 5.000}{5}$ | 9.000 € | $\frac{80.000 - 10.000}{5}$ | 14.000 € |
| **kalk. Zinsen (8 %)** | $\frac{50.000 + 5.000}{2} \cdot 0{,}08$ | 2.200 € | $\frac{80.000 + 10.000}{2} \cdot 0{,}08$ | 3.600 € |
| Lohnkosten p.a. | *gegeben* | 8.000 € | *gegeben* | 6.000 € |
| Instandhaltung p.a. | *gegeben* | 3.500 € | *gegeben* | 2.000 € |
| Raumkosten p.a. | *gegeben* | 1.000 € | *gegeben* | 1.200 € |
| Energiekosten p.a. | *gegeben* | 2.500 € | *gegeben* | 2.000 € |
| **Gesamtkosten ($K$)** | **Summe** | **26.200 €** | **Summe** | **28.800 €** |

---

## 📐 Stückkostenanalyse ($k$)

Da die jährlichen Leistungsmengen ($x_{\text{I}} = 40.000\text{ LE}$ vs. $x_{\text{II}} = 50.000\text{ LE}$) voneinander abweichen, liefert nur die Berechnung der Stückkosten ($k = \frac{K}{x}$) eine valide Entscheidungsgrundlage:

* **Stückkosten Anlage I ($k_{\text{I}}$):**
  $$k_{\text{I}} = \frac{26.200\text{ €}}{40.000\text{ LE}} = \mathbf{0{,}655\text{ € / LE}}$$

* **Stückkosten Anlage II ($k_{\text{II}}$):**
  $$k_{\text{II}} = \frac{28.800\text{ €}}{50.000\text{ LE}} = \mathbf{0{,}576\text{ € / LE}}$$

---

## 🏛️ Investitionsentscheidung

> [!success] **Fazit**
> Nach Maßgabe der Kostenvergleichsrechnung ist **Anlage II vorteilhafter**. Obwohl sie mit $28.800\text{ €}$ höhere absolute Gesamtkosten pro Jahr verursacht als Anlage I ($26.200\text{ €}$), führt ihre höhere Produktionskapazität (Degressionseffekt der Fixkosten bei 50.000 LE) zu den geringeren Stückkosten von **0,576 € / LE** (Ersparnis von $0{,}079\text{ €}$ pro Leistungseinheit).