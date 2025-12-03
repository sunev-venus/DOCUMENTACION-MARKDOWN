# Documentación de Ejercicios - Juan José Zapata Buenfil

## Información General
- **Materia:** Fundamentos de Álgebra
- **Tema:** Operaciones con Matrices
- **Fecha:** 17 de Noviembre 2024
- **Estudiante:** Juan José Zapata Buenfil
- **Grupo:** B

## Objetivo de la Documentación
El propósito de este documento es registrar y explicar los ejercicios realizados en la Actividad #16, enfocada en la identificación, clasificación y operaciones básicas con matrices. Se documenta el proceso de resolución paso a paso para cada ejercicio.

---

## Ejercicios Realizados

### Ejercicio 1: Cálculo de Determinantes 2×2

#### Enunciado del Problema
Calcular los determinantes de las siguientes matrices 2×2:

$$
A = \left(\begin{array}{cc}
5 & 2 \\
3 & 1 \\
\end{array}\right), \quad 
B = \left(\begin{array}{cc}
-1 & 4 \\
2 & -8 \\
\end{array}\right), \quad 
C = \left(\begin{array}{cc}
6 & 9 \\
2 & 3 \\
\end{array}\right), \quad 
D = \left(\begin{array}{cc}
0 & 5 \\
-5 & 0 \\
\end{array}\right)
$$

#### Respuesta
- **Determinante de A:** -1
- **Determinante de B:** 0
- **Determinante de C:** 0
- **Determinante de D:** 25

#### Procedimiento
1. **Fórmula del determinante 2×2:** Para una matriz \( \left(\begin{array}{cc} a & b \\ c & d \end{array}\right) \), el determinante es \( ad - bc \)

<ol start="2">
  <li><strong>Cálculo para matriz A:</strong> $\det(A) = (5 \times 1) - (2 \times 3) = 5 - 6 = -1$</li>
  <li><strong>Cálculo para matriz B:</strong> $\det(B) = (-1 \times -8) - (4 \times 2) = 8 - 8 = 0$</li>
  <li><strong>Cálculo para matriz C:</strong> $\det(C) = (6 \times 3) - (9 \times 2) = 18 - 18 = 0$</li>
  <li><strong>Cálculo para matriz D:</strong> $\det(D) = (0 \times 0) - (5 \times -5) = 0 - (-25) = 0 + 25 = 25$</li>
</ol>

---

### Ejercicio 2: Regla de Sarrus para Determinantes 3×3

#### Enunciado del Problema
Usar la regla de Sarrus para calcular los determinantes de las matrices 3×3:

$$
E = \left(\begin{array}{ccc}
1 & 2 & 3 \\
0 & 1 & 4 \\
5 & 6 & 0 \\
\end{array}\right), \quad 
F = \left(\begin{array}{ccc}
2 & -1 & 3 \\
1 & 4 & 0 \\
3 & 2 & -2 \\
\end{array}\right)
$$

#### Respuesta
- **Determinante de E:** 1
- **Determinante de F:** -48

#### Procedimiento

## Cálculo para la Matriz E

Para calcular el determinante de E, $\det(E)$, aumentamos la matriz repitiendo las primeras dos columnas:

$$
\det(E) = \left| \begin{array}{ccc|cc}
1 & 2 & 3 & 1 & 2 \\
0 & 1 & 4 & 0 & 1 \\
5 & 6 & 0 & 5 & 6
\end{array} \right|
$$

**1. Suma de diagonales positivas:**
$(1 \times 1 \times 0) + (2 \times 4 \times 5) + (3 \times 0 \times 6) = 0 + 40 + 0 = 40$

**2. Suma de diagonales negativas:**
$(3 \times 1 \times 5) + (1 \times 4 \times 6) + (2 \times 0 \times 0) = 15 + 24 + 0 = 39$

**3. Resultado:**
$\det(E) = (\text{Suma positiva}) - (\text{Suma negativa}) = 40 - 39 = 1$


## Cálculo para la Matriz F

Para calcular el determinante de F, $\det(F)$, repetimos el proceso:

$$
\det(F) = \left| \begin{array}{ccc|cc}
2 & -1 & 3 & 2 & -1 \\
1 & 4 & 0 & 1 & 4 \\
3 & 2 & -2 & 3 & 2
\end{array} \right|
$$

**1. Suma de diagonales positivas :**
$(2 \times 4 \times -2) + (-1 \times 0 \times 3) + (3 \times 1 \times 2) = -16 + 0 + 6 = -10$

**2. Suma de diagonales negativas :**
$(3 \times 4 \times 3) + (2 \times 0 \times 2) + (-1 \times 1 \times -2) = 36 + 0 + 2 = 38$

**3. Resultado:**
$\det(F) = (\text{Suma positiva}) - (\text{Suma negativa}) = -10 - 38 = -48$

---

### Ejercicio 3: Método de Cofactores para Determinantes 3×3

#### Enunciado del Problema
Calcular el determinante usando el método de cofactores (expandir por la fila o columna más conveniente):

$$
G = \left(\begin{array}{ccc}
1 & 0 & 2 \\
-1 & 3 & 1 \\
2 & 0 & 1 \\
\end{array}\right)
$$

#### Respuesta
- **Determinante de G:** -9

#### Procedimiento

1. **Identificar los signos de los cofactores:**
$$
\left( \begin{array}{ccc}
+ & - & + \\
- & + & - \\
+ & - & +
\end{array} \right)
$$

**2. Fórmula de expansión (por Columna 2):**

$$
\det(G) = (G_{12} \times C_{12}) + (G_{22} \times C_{22}) + (G_{32} \times C_{32})
$$

**Cálculo de los términos:**

* **Término 1 ($G_{12}$):** $G_{12} = 0$, por lo tanto $0 \times C_{12} = 0$.
* **Término 3 ($G_{32}$):** $G_{32} = 0$, por lo tanto $0 \times C_{32} = 0$.
* **Término 2 ($G_{22}$):**
    * $G_{22} = 3$
    * El signo de la posición (2,2) es **Positivo** (+).
    * El menor $M_{22}$ se obtiene eliminando la fila 2 y la columna 2: $M_{22} = \det \left( \begin{array}{cc} 1 & 2 \\ 2 & 1 \end{array} \right)$
    * Se calcula el menor: $(1 \times 1) - (2 \times 2) = 1 - 4 = -3$.
    * El término completo es: $(\text{signo}) \times (\text{valor}) \times (\text{menor}) = (+) \times (3) \times (-3) = -9$.

**5. Resultado final:**

$$
\det(G) = 0 + (-9) + 0 = -9
$$

---

### Ejercicio 4: Verificar Propiedades de los Determinantes

#### Enunciado del Problema
Dadas las matrices A y B, verificar que:
- $\det(AB) = \det(A) \cdot \det(B)$
- $\det(A^T) = \det(A)$

$$
A = \left(\begin{array}{cc}
2 & 1 \\
1 & 3 \\
\end{array}\right), \quad 
B = \left(\begin{array}{cc}
1 & 2 \\
3 & 1 \\
\end{array}\right)
$$

#### Respuesta
- **$\det(A) = 5$**
- **$\det(B) = -5$**
- **$\det(AB) = -25$**
- **$\det(A^T) = 5$**

#### Procedimiento

** Cálculo de determinantes**

1. **Determinante de A:**
   
$$
\det(A) = (2 \times 3) - (1 \times 1) = 6 - 1 = 5
$$

3. **Determinante de B:**
   
$$
\det(B) = (1 \times 1) - (2 \times 3) = 1 - 6 = -5
$$

**Verificación de $\det(AB) = \det(A) \cdot \det(B)$**

3. **Calcular AB:**

AB = | 2 1 | × | 1 2 | = | (2×1)+(1×3) (2×2)+(1×1) | = | 2+3 4+1 | = | 5 5 |
| 1 3 | | 3 1 | | (1×1)+(3×3) (1×2)+(3×1) | | 1+9 2+3 | | 10 5 |

4. **Calcular $\det(AB)$:**

   det(AB) = (5 × 5) - (5 × 10) = 25 - 50 = -25

6. **Verificar la propiedad:**
   
det(A) × det(B) = 5 × (-5) = -25

7. **Calcular $A^T$:**
   
    | 2  1 |T    | 2  1 |
    A^T = | 1 3 | = | 1 3 |

8. **Calcular $\det(A^T)$:**
   
$$
\det(A^T) = (2 \times 3) - (1 \times 1) = 6 - 1 = 5
$$

10. **Verificar la propiedad:**

   **$\det(A^T) = 5 = \det(A)$**

---

### Ejercicio 5: Aplicación Geométrica de los Determinantes

#### Enunciado del Problema
Dados los vectores $\vec{u} = (3, 2)$ y $\vec{v} = (1, 4)$:
a) Calcula el área del paralelogramo que forman  
b) ¿Cambia el área si intercambias los vectores?  
c) ¿Qué representa el signo del determinante?

#### Solución o Respuesta
- **a) Área del paralelogramo: 10 unidades 
- **b) El área si cambia al intercambiar vectores
- **c) El signo indica la orientación de los vectores

#### Procedimiento

**Cálculo del área del paralelogramo**

1. **Matriz formada por los vectores:**

$$
M = \left(\begin{array}{cc}
3 & 2 \\
1 & 4 \\
\end{array}\right)
$$

2. **Cálculo del determinante:**

$$
\det(M) = (3 \times 4) - (2 \times 1) = 12 - 2 = 10
$$

3. **Matriz con vectores intercambiados:**

$$
M' = \left(\begin{array}{cc}
1 & 4 \\
3 & 2 \\
\end{array}\right)
$$

4. **Cálculo del nuevo determinante:**

$$
\det(M') = (1 \times 2) - (4 \times 3) = 2 - 12 = -10
$$

7. **Significado del signo:**
   - **Signo positivo (+10):** Los vectores están en orientación antihoraria (sentido positivo)
   - **Signo negativo (-10):** Los vectores están en orientación horaria (sentido negativo)
   - El *determinante* representa el área
   - El *signo* representa la orientación en el plano
