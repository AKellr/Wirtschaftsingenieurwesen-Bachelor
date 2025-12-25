[[GDE]]

### 9.1 Mesh Analysis (Maschenanalyse)

**Concept:** Uses **Kirchhoff's Voltage Law (KVL)**. We calculate circulating "Mesh Currents" ($I_1, I_2...$) in the "windows" of the circuit1111.

- **Best for:** Circuits with many voltage sources and few loops.
    
- **Restriction:** Only works for "planar" networks (circuits that can be drawn without wires crossing)2.
    

#### The Matrix Equation

$$[R] \cdot (I) = (U_q)$$

Where $[R]$ is the Resistance Matrix, $(I)$ is the Mesh Current Vector, and $(U_q)$ is the Source Voltage Vector3.

#### Procedure (Vorgehensweise)

1. **Draw Meshes:** Draw a loop current for every "window". **Convention:** Draw all loops **Clockwise**4.
    
2. **Fill Matrix $[R]$ (Left Side):**
    
    - **Diagonal Elements ($R_{11}, R_{22}$):** Sum of **ALL** resistors in that specific mesh 5.
        
    - **Off-Diagonal Elements ($R_{12}, R_{21}$):** Resistance shared between meshes.
        
        - **Negative (-):** If mesh currents flow in **opposite** directions through the shared resistor (Standard case for clockwise loops) 6.
            
        - **Positive (+):** If mesh currents flow in the **same** direction.
            
3. **Fill Vector $(U_q)$ (Right Side):**
    
    - Sum of all voltage sources in that mesh.
        
    - **Positive (+):** Source arrow is **OPPOSITE** to mesh current direction (Head-to-Head) 7.
        
    - **Negative (-):** Source arrow is in the **SAME** direction as mesh current8.
        

> **Critical Note:** Ideal **Current Sources** cannot be put directly into the matrix. You must convert them into equivalent Voltage Sources ($U_{eq} = I_q \cdot R_p$) first 9.

---

### 9.3 Nodal Analysis (Knotenanalyse)

**Concept:** Uses **Kirchhoff's Current Law (KCL)**. We calculate the **Voltage Potential** at each node relative to a reference node (Ground)10101010.

- **Best for:** Circuits with many parallel branches or current sources.
    

#### The Matrix Equation

$$[G] \cdot (U) = (I_q)$$

Where $[G]$ is the Conductance Matrix ($G=1/R$), $(U)$ is the Node Voltage Vector, and $(I_q)$ is the Source Current Vector11.

#### Procedure (Vorgehensweise)

1. **Pick Reference:** Choose one node as "Ground" (0 V). Usually the bottom wire12.
    
2. **Fill Matrix $[G]$ (Left Side):**
    
    - **Diagonal Elements ($G_{11}, G_{22}$):** Sum of **ALL** conductances connected directly to that node13.
        
        - _Remember:_ $G = \frac{1}{R}$.
            
    - **Off-Diagonal Elements ($G_{12}, G_{21}$):** Sum of conductances connecting the two nodes. These are **always Negative (-)**14.
        
3. **Fill Vector $(I_q)$ (Right Side):**
    
    - Sum of all current sources connected to that node.
        
    - **Positive (+):** Current flows **INTO** the node (Incoming/Zufließend)15.
        
    - **Negative (-):** Current flows **AWAY** from the node (Outgoing/Abfließend)16.
        

> **Critical Note:** Ideal **Voltage Sources** cannot be put directly into the matrix. You must convert them into equivalent Current Sources ($I_{eq} = U_q / R_s$) first 17.

---

### Comparison Cheat Sheet

| **Feature**         | **Mesh Analysis**              | **Nodal Analysis**             |
| ------------------- | ------------------------------ | ------------------------------ |
| **Law Used**        | KVL (Voltage Loop)             | KCL (Current Node)             |
| **Variable Solved** | Loop Currents ($I$)            | Node Voltages ($U$)            |
| **Matrix Values**   | Resistance ($R$)               | Conductance ($G = 1/R$)        |
| **Off-Diagonals**   | Shared $R$ (Usually Negative)  | Shared $G$ (Always Negative)   |
| **Source Vector**   | Voltage Sources ($U_q$)        | Current Sources ($I_q$)        |
| **Problem Source**  | Current Sources (Must Convert) | Voltage Sources (Must Convert) |