[[GDE]]
## Chapter 7: Ersatzschaltungen (Equivalent Circuits)

### 7.1 Ersatz-Spannungsquelle (Thévenin Equivalent)

Any linear DC network with two terminals can be replaced by a single voltage source in series with a resistor.

- **Concept:** Simplifies complex circuits into a "Black Box" model.
    
- **Components:**
    
    - $U_{q,eq}$ (or $U_{Th}$): **Leerlaufspannung** (Open Circuit Voltage).
        
    - $R_i$ (or $R_{Th}$): **Innenwiderstand** (Internal Resistance).
        
### 7.2 Transformation Steps (Umformung)

**Step 1: Calculate $U_{q,eq}$ (Voltage)**

- **Action:** Leave terminals A-B **OPEN** (_Leerlauf_).
    
- **Math:** Calculate the voltage potential difference between A and B.
    

**Step 2: Calculate $R_i$ (Resistance)**

- **Action:** "Kill" all independent sources inside the network and calculate the equivalent resistance looking into A-B.
    
- **The "Killing" Rules:**
    
    - **Voltage Source ($U$):** Replace with **Short Circuit** (_Kurzschluss_ / Wire).
        
    - **Current Source ($I$):** Replace with **Open Circuit** (_Leerlauf_ / Cut Wire).
        

### 7.3 & 7.4 Ersatz-Stromquelle (Norton Equivalent)

Any linear DC network can also be replaced by a single current source in parallel with a resistor.

- **Components:**
    
    - $I_k$ (or $I_N$): **Kurzschlussstrom** (Short-Circuit Current).
        
    - $R_i$ (or $R_N$): **Innenwiderstand** (Internal Resistance) - _Same value as Thévenin!_
        

**Step 1: Calculate $I_k$ (Current)**

- **Action:** **SHORT** terminals A-B with a wire.
    
- **Math:** Calculate the current flowing through that shorting wire.
    

### 7.5 Equivalence (Äquivalenz)

You can convert between Thévenin and Norton using Ohm's Law.

$$U_{q,eq} = I_k \cdot R_i$$

- **Thévenin:** $R_i$ is in **Series**.
    
- **Norton:** $R_i$ is in **Parallel**.
    

---

## Chapter 8: Leistung an Zweipolen (Power)

### 8.1 Leistungsbilanz (Power Balance)

Energy cannot be created or destroyed. In any closed circuit:

$$\sum P_{generated} = \sum P_{consumed}$$

- **Generator (_Erzeuger_):** $U$ and $I$ arrows point in **Opposite** directions.
    
- **Consumer (_Verbraucher_):** $U$ and $I$ arrows point in **Same** direction.
    

### 8.2 Wirkungsgrad (Efficiency)

Describes how much input power is converted to useful output power.

$$\eta = \frac{P_{out}}{P_{total}}$$

- At Maximum Power Transfer, $\eta = 50\%$.
    

### 8.3 Leistungsanpassung (Maximum Power Transfer)

To transfer the maximum possible power from a real source to a load ($R_a$):

Condition:

The load resistance must equal the internal resistance.

$$R_a = R_i$$

**Key Characteristics at Max Power:**

1. $P_{out}$ is at its peak (Hochpunkt).
    
2. Half the power is dissipated in the source ($R_i$), half in the load ($R_a$).
    
3. Efficiency is exactly **50%**.
    

---

### Summary of "Killing" Sources

|**Component**|**Action (English)**|**Action (German)**|**Replacement**|
|---|---|---|---|
|**Voltage Source**|Short Circuit|_Kurzschluss_|Wire (0 $\Omega$)|
|**Current Source**|Open Circuit|_Leerlauf_|Broken Wire ($\infty \Omega$)|

---

Now that you have these notes secured, do you feel ready to test yourself on a combined problem, or is there a specific concept you want to double-check first?