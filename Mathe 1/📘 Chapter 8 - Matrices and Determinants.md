[[Math]]

## 8.1 Matrices (Matrizen)

### 🔹 Definition
A **matrix (Matrix)** is a rectangular arrangement of real numbers with $m$ rows (Zeilen) and $n$ columns (Spalten):

$$
A =
\begin{pmatrix}
a_{11} & a_{12} & \dots & a_{1n} \\
a_{21} & a_{22} & \dots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{m1} & a_{m2} & \dots & a_{mn}
\end{pmatrix}
$$

- The element $a_{ij}$ is in the *i-th row* and *j-th column* (i-te Zeile, j-te Spalte).

---

### 🔹 Special Matrices (spezielle Matrizen)

1. **Column vector (Spaltenvektor):**
   $$
   A =
   \begin{pmatrix}
   a_{11} \\ a_{21} \\ \vdots \\ a_{m1}
   \end{pmatrix}
   $$

2. **Row vector (Zeilenvektor):**
   $$
   A = (a_{11}, a_{12}, \dots, a_{1n})
   $$

3. **Square matrix (quadratische Matrix):** $m = n$

4. **Upper triangular matrix (obere Dreiecksmatrix):**
   $$
   A =
   \begin{pmatrix}
   a_{11} & a_{12} & a_{13} & \dots & a_{1n} \\
   0 & a_{22} & a_{23} & \dots & a_{2n} \\
   0 & 0 & a_{33} & \dots & a_{3n} \\
   \vdots & \vdots & \vdots & \ddots & a_{nn}
   \end{pmatrix}
   $$
   (analogous: lower triangular matrix – *untere Dreiecksmatrix*)

---

### 🔹 Matrix-Vector Product (Matrix-Vektor-Produkt)

Definition:
The product of an $(m,n)$-matrix $A$ with a vector $\vec{b}$ having $n$ entries is a new vector $\vec{c}$ with $m$ entries:

$$
\vec{c} = A \cdot \vec{b} =
\begin{pmatrix}
a_{11} & a_{12} & \dots & a_{1n} \\
a_{21} & a_{22} & \dots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{m1} & a_{m2} & \dots & a_{mn}
\end{pmatrix}
\begin{pmatrix}
b_1 \\ b_2 \\ \vdots \\ b_n
\end{pmatrix}
$$

$$
\Rightarrow c_i = a_{i1}b_1 + a_{i2}b_2 + \dots + a_{in}b_n
$$

Each entry of $\vec{c}$ is the **scalar product (Skalarprodukt)** of a row of $A$ with $\vec{b}$.

---
	
### 🔹 Matrix Product (Matrixprodukt)

If $A$ is a $(p, m)$-matrix and $B$ an $(m, n)$-matrix, the product $C = A \cdot B$ is defined as:

$$
c_{ij} = a_{i1}b_{1j} + a_{i2}b_{2j} + \dots + a_{im}b_{mj}
$$

- $C$ is a $(p, n)$-matrix.  
- The number of columns of $A$ must equal the number of rows of $B$.  
- In general: $A \cdot B \neq B \cdot A$ (**not commutative – nicht kommutativ**).

---

## 8.2 Determinants (Determinanten)

### 🔹 2×2 Determinant
For a $(2,2)$-matrix:

$$
A =
\begin{pmatrix}
a_{11} & a_{12} \\
a_{21} & a_{22}
\end{pmatrix}
$$

the determinant is:

$$
\det(A) = a_{11}a_{22} - a_{12}a_{21}
$$

Rule: **Main diagonal minus secondary diagonal**  
(Diagonale minus Nebendiagonale)

---

### 🔹 Properties of the Determinant (Eigenschaften der Determinante)

1. Swapping rows or columns changes the **sign (Vorzeichen)**.  
2. Multiplying a row/column by a scalar multiplies the determinant by that scalar.  
3. If two rows/columns are identical or proportional → $\det(A) = 0$.  
4. Adding a multiple of one row/column to another does **not** change $\det(A)$.  
5. $\det(A) = 0$ if $A$ has a zero row (Nullzeile) or column (Nullspalte).

---

### 🔹 3×3 Determinant — Sarrus’ Rule (Regel von Sarrus)

$$
\det(A) =
\begin{vmatrix}
a_{11} & a_{12} & a_{13} \\
a_{21} & a_{22} & a_{23} \\
a_{31} & a_{32} & a_{33}
\end{vmatrix}
$$

can be calculated by:

$$
\det(A) = (a_{11}a_{22}a_{33} + a_{12}a_{23}a_{31} + a_{13}a_{21}a_{32})
- (a_{13}a_{22}a_{31} + a_{12}a_{21}a_{33} + a_{11}a_{23}a_{32})
$$

Mnemonic: **"Main diagonals minus secondary diagonals"**  
(Diagonalen minus Nebendiagonalen)

---

### 🔹 Determinant and Vector Operations (Determinanten und Vektoroperationen)

**Cross product (Vektorprodukt):**

$$
\vec{a} \times \vec{b} =
\begin{vmatrix}
\vec{e_x} & \vec{e_y} & \vec{e_z} \\
a_x & a_y & a_z \\
b_x & b_y & b_z
\end{vmatrix}
$$

**Scalar triple product (Spatprodukt):**

$$
[\vec{a}\vec{b}\vec{c}] = 
\begin{vmatrix}
a_x & b_x & c_x \\
a_y & b_y & c_y \\
a_z & b_z & c_z
\end{vmatrix}
$$

---

### 🔹 Laplace Expansion (Entwicklungssatz von Laplace)

For any $n \times n$ determinant $D$:

$$
D = \sum_{j=1}^{n} (-1)^{i+j} a_{ij} D_{ij}
$$

where $D_{ij}$ is the **minor determinant (Nebendeterminante)** obtained by removing row $i$ and column $j$.

The **signs follow a checkerboard pattern (Schachbrettmuster):**

$$
\begin{vmatrix}
+ & - & + & \dots \\
- & + & - & \dots \\
+ & - & + & \dots
\end{vmatrix}
$$

---

### 🔹 Practical Determinant Computation (Determinantenberechnung in der Praxis)

- For $2×2$ or $3×3$: use direct formula or Sarrus’ rule  
- For larger matrices: expand by rows or columns with many zeros  
- Computationally efficient form: **Triangular form (Dreiecksform)**

If $A$ is in upper triangular form:

$$
\det(A) = a_{11} \cdot a_{22} \cdot a_{33} \cdots a_{nn}
$$

---

### 🔹 Inverse Matrix (Inverse Matrix)

- $\det(A) = 0$ → **singular (singulär)** → not invertible  
- $\det(A) \neq 0$ → **regular (regulär)** → invertible

If $\vec{y} = A \cdot \vec{x}$, then:

$$
\vec{x} = A^{-1} \cdot \vec{y}
$$

---

### 🔹 Formula for Inverse Matrix (Formel für die inverse Matrix)

$$
A^{-1} = \frac{1}{\det(A)}
\begin{pmatrix}
D_{11} & -D_{21} & D_{31} & \dots \\
-D_{12} & D_{22} & -D_{32} & \dots \\
\vdots & \vdots & \ddots & \vdots \\
(-1)^{n+1}D_{1n} & (-1)^{n+2}D_{2n} & \dots & (-1)^{n+n}D_{nn}
\end{pmatrix}
$$

- $D_{ij}$ are **minor determinants (Nebendeterminanten)**.  
- Note: In $A^{-1}$, element $D_{ji}$ (transposed position) appears!  
- The sign pattern follows the **checkerboard (Schachbrettmuster)** rule.

---

## ✅ Summary Table (Überblick)

| Concept | German Term | Formula / Definition |
|----------|--------------|----------------------|
| Matrix | Matrix | rectangular array of numbers |
| Element $a_{ij}$ | Matrixelement | entry in row $i$, column $j$ |
| Determinant | Determinante | $\det(A)$ |
| 2×2 determinant | 2×2-Determinante | $a_{11}a_{22} - a_{12}a_{21}$ |
| 3×3 determinant | 3×3-Determinante | Rule of Sarrus |
| Minor | Nebendeterminante | determinant of submatrix |
| Laplace expansion | Entwicklungssatz von Laplace | $D = \sum (-1)^{i+j} a_{ij} D_{ij}$ |
| Inverse matrix | Inverse Matrix | $A^{-1} = \frac{1}{\det(A)} \text{Adj}(A)$ |
| Singular matrix | singuläre Matrix | $\det(A)=0$ |
| Regular matrix | reguläre Matrix | $\det(A)\neq0$ |

---
