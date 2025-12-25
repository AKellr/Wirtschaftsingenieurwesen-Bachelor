[[GDE]]

## 1. Recap: Power & Sources (Chapters 7 & 8)
*Key Concepts & Formulas*

### Power Balance (Leistungsbilanz)
The fundamental rule of circuits:
> The sum of all generated power must equal the sum of all consumed power.

$$\sum P_{Erzeuger} = \sum P_{Verbraucher}$$

### Sign Convention (Zählpfeile)
* **Generator (Source):** Current ($I$) and Voltage ($U$) arrows point in **opposite** directions.
* **Consumer (Resistor/Load):** Current ($I$) and Voltage ($U$) arrows point in the **same** direction.

### Maximum Power Transfer (Leistungsanpassung)
*Question:* At what value of $R$ is the power transfer to the load maximal?

* **The Condition:** Maximum power occurs when load resistance equals internal resistance.
    $$R_a = R_i \quad (\text{or } R_L = R_i)$$
* **The Result:** At this exact point, the efficiency ($\eta$) is:
    $$\eta = 0.5 \quad (50\%)$$

---

## 2. Chapter 9: Mesh Analysis (Maschenanalyse)
*The Systematic Method for Loop Currents*

### The Concept
Instead of calculating current in every single wire, we calculate **"Loop Currents"** ($I_1, I_2, \dots$) that circulate in the "windows" of the circuit.

### The Matrix Equation
You are solving for a vector of currents $(I)$.
$$[R] \cdot (I) = (U_q)$$
* **$[R]$**: Resistance Matrix
* **$(I)$**: Mesh Current Vector (Unknowns)
* **$(U_q)$**: Voltage Source Vector (Knowns)

### Step-by-Step Procedure
1.  **Draw Meshes:** Define a loop current for every "window" (Fenstermasche). *Standard practice: Draw all clockwise.*
2.  **Fill the Matrix ($[R]$):**
    * **The Diagonal ($R_{11}, R_{22}$):** Sum of **all** resistors in that specific mesh.
        * *Example:* $R_{11} = R_1 + R_2 + \dots$
    * **The Off-Diagonals ($R_{12}, R_{21}$):** Resistors **shared** between two meshes.
        * *Rule:* If loop currents go in the same direction through the shared resistor $\rightarrow$ Positive.
        * *Standard Rule:* If all loops are clockwise, currents oppose each other $\rightarrow$ **Negative** ($-R_{shared}$).
3.  **Fill the Right Side ($(U_q)$):**
    * Sum of all voltage sources in that mesh.
    * *Sign Rule:*
        * Current flows **out** of positive terminal (pushes with source) $\rightarrow$ **Positive** ($+$).
        * Current flows **into** positive terminal (pushes against source) $\rightarrow$ **Negative** ($-$).

> [!WARNING] Problem: Current Sources
> If the circuit has an **Ideal Current Source**, you cannot write a voltage equation for it directly.
> **Solution:** Convert the Current Source + Parallel Resistor into an **Ersatz-Spannungsquelle** (Voltage Source + Series Resistor) *before* analysis.

---

## 3. Chapter 9: Nodal Analysis (Knotenanalyse)
*The Counterpart to Mesh Analysis*

### The Concept
Instead of loops, we look at junctions (Nodes). We calculate the **Voltage Potential** at each node relative to a reference (Ground).

### The Matrix Equation
You are solving for node voltages $(U)$ using Conductance ($G = 1/R$).
$$[G] \cdot (U) = (I_q)$$
* **$[G]$**: Conductance Matrix
* **$(U)$**: Node Voltage Vector (Unknowns)
* **$(I_q)$**: Current Source Vector (Knowns)

### Step-by-Step Procedure
1.  **Pick a Reference:** Choose one node to be **Ground (0V)**. *Usually the bottom wire.*
2.  **Fill the Matrix ($[G]$):**
    * **The Diagonal ($G_{11}, G_{22}$):** Sum of all Conductances connected **directly** to that node.
        * *Reminder:* $G = \frac{1}{R}$. Entry is $(\frac{1}{R_1} + \frac{1}{R_2})$.
    * **The Off-Diagonals ($G_{12}, G_{21}$):** Sum of conductances connecting the two nodes.
        * *Rule:* Always **Negative**.
        * *Example:* If Node 1 & 2 are connected by $R_3$, entry is $-\frac{1}{R_3}$.
3.  **Fill the Right Side ($(I_q)$):**
    * Sum of all current sources connected to that node.
    * *Sign Rule:*
        * Current flowing **INTO** the node $\rightarrow$ **Positive** ($+$).
        * Current flowing **OUT** of the node $\rightarrow$ **Negative** ($-$).

> [!WARNING] Problem: Voltage Sources
> If the circuit has an **Ideal Voltage Source**, you cannot sum currents easily.
> **Solution:** Convert the Voltage Source + Series Resistor into an **Ersatz-Stromquelle** (Current Source + Parallel Resistor) *before* analysis.