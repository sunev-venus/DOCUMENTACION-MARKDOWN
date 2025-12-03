# Tecnológico de Software
## Materia: Fundamentos de Álgebra
### Alumno: Venus Getsemaní Semino Alemán
### Actividad #16 - Documentación de Matrices

**Fecha:** 18 de noviembre de 2025

---

##  Objetivo de la Documentación
Registrar y explicar los ejercicios realizados sobre el cálculo de determinantes de matrices $2 \times 2$ y $3 \times 3$ usando diferentes métodos.

---

## 📝 Ejercicios Realizados

### Ejercicio 1: Cálculo de Determinantes $2 \times 2$

**Enunciado:** Calcular los determinantes de las siguientes matrices:

$$
A = \begin{pmatrix} 5 & 2 \\ 3 & 1 \end{pmatrix},\quad
B = \begin{pmatrix} -1 & 4 \\ 2 & -8 \end{pmatrix},\quad
C = \begin{pmatrix} 6 & 9 \\ 2 & 3 \end{pmatrix},\quad
D = \begin{pmatrix} 0 & 5 \\ -5 & 0 \end{pmatrix}
$$

**Resultados y Procedimiento:**

1.  **Matriz A:**
    $$\det(A) = (5 \cdot 1) - (2 \cdot 3) = 5 - 6 = -1$$
2.  **Matriz B:**
    $$\det(B) = (-1 \cdot -8) - (4 \cdot 2) = 8 - 8 = 0$$
3.  **Matriz C:**
    $$\det(C) = (6 \cdot 3) - (9 \cdot 2) = 18 - 18 = 0$$
4.  **Matriz D:**
    $$\det(D) = (0 \cdot 0) - (5 \cdot -5) = 0 - (-25) = 25$$

---

### Ejercicio 2: Determinante de Matriz $3 \times 3$

**Enunciado:**

$$
F = \begin{pmatrix}
2 & -1 & 3 \\
1 & 4 & 0 \\
3 & 2 & -2
\end{pmatrix}
$$

**Resultado:**
* $\det(F) = -51$

**Procedimiento:**
Método aplicado: *Regla de Sarrus o expansión por cofactores*.
$$-38 - 13 = -51$$

---

### Ejercicio 3: Método de Cofactores ($3 \times 3$)

**Enunciado:**

$$
G = \begin{pmatrix}
1 & 0 & 2 \\
-1 & 3 & 1 \\
2 & 0 & 1
\end{pmatrix}
$$

**Resultado:**
* $\det(G) = -9$

**Procedimiento (Expansión por primera fila):**

* **Término 1 ($G_{11}$):** 1 (Signo +)
    $$M_{11} = \det\begin{pmatrix} 3 & 1 \\ 0 & 1 \end{pmatrix} = 3 \quad \Rightarrow \quad (1)(3) = 3$$

* **Término 2 ($G_{12}$):** 0
    $$\text{El término es } 0$$

* **Término 3 ($G_{13}$):** 2 (Signo +)
    $$M_{13} = \det\begin{pmatrix} -1 & 3 \\ 2 & 0 \end{pmatrix} = -(3 \cdot 2) = -6 \quad \Rightarrow \quad (2)(-6) = -12$$

**Cálculo Final:**
$$\det(G) = 3 + 0 - 12 = -9$$

---

### Ejercicio 4: Propiedades de los Determinantes

**Matrices:**

$$
A = \begin{pmatrix} 2 & 1 \\ 1 & 3 \end{pmatrix},\quad
B = \begin{pmatrix} 1 & 2 \\ 3 & 1 \end{pmatrix}
$$

**Resultados:**
* $\det(A) = 5$
* $\det(B) = -5$
* $\det(AB) = -25$
* $\det(A^T) = 5$

**Verificación de Propiedades:**

1.  **Determinantes individuales:**
    * $\det(A) = (2 \cdot 3) - (1 \cdot 1) = 5$
    * $\det(B) = (1 \cdot 1) - (3 \cdot 2) = -5$

2.  **Propiedad de Multiplicación:** $\det(AB) = \det(A) \cdot \det(B)$
    $$\det(AB) = -25$$
    $$5 \cdot (-5) = -25$$
    *(Propiedad verificada)* 

3.  **Propiedad de la Transpuesta:** $\det(A^T) = \det(A)$
    $$5 = 5$$
    *(Propiedad verificada)* 

---

### Ejercicio 5: Área del Paralelogramo

**Vectores:** $U = (3, 2)$ y $V = (1, 4)$

**Resultado:**
* Área = 10 u²

**Procedimiento:**

1.  **Matriz formada por vectores:**
    $$A = \begin{pmatrix} 3 & 2 \\ 1 & 4 \end{pmatrix}$$

2.  **Cálculo del determinante:**
    $$\det(A) = (3 \cdot 4) - (2 \cdot 1) = 12 - 2 = 10$$

3.  **Interpretación:**
    El valor absoluto del determinante representa el área.
    Si cambiamos el orden de los vectores, el determinante sería $-10$, pero el área sigue siendo $|-10| = 10$.
