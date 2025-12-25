[[GDE]]
### The Core Concept

When a total current ($I_{total}$) splits into two parallel branches, it divides based on the resistance of each branch.

- **Low Resistance** $\rightarrow$ More Current.
    
- **High Resistance** $\rightarrow$ Less Current.
    

### The Formula

To find the current in one branch ($I_x$), you use the resistance of the **other** branch ($R_{other}$) in the numerator.

$$I_x = I_{total} \cdot \frac{R_{other}}{R_{total\_loop}}$$

Where:

- $R_{other}$: The resistance of the parallel branch you are **NOT** measuring.
    
- $R_{total\_loop}$: The sum of resistances in both parallel branches ($R_{this\_branch} + R_{other}$).
    

---

### 🌊 Intuition: The River Analogy

Think of current as water flowing down a river that splits into two channels.

1. **Channel A (Wide/Low R):** Easy path $\rightarrow$ Most water goes here.
    
2. **Channel B (Narrow/High R):** Hard path $\rightarrow$ Less water goes here.
    

The rule mathematically calculates exactly how much "water" chooses the easier vs. the harder path relative to each other.

---

### 🛑 Application: "Supply" vs. "Split"

Why did we ignore $R_4$ when calculating the split ratio in Question 1?

**1. The Supply (Upstream)**

- Components in **Series** with the source (like $R_4$) act as part of the "pump" assembly.
    
- They might make the source work harder (generate more voltage) to push the current, but they do not offer an alternative path.
    
- **Key Rule:** Current in a series wire is constant. The full $I_q$ flows through $R_4$ before reaching the junction.
    

**2. The Split (Downstream)**

- The Current Divider Rule only kicks in at the **Node** (Junction) where the path physically divides.
    
- It only cares about the **Parallel Options** available at that specific junction.
    
- Since $R_4$ is upstream (before the split), it does not affect the _ratio_ of how the current divides between the two downstream paths.