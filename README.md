# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Alumno: Venus Getsemaní Semino Alemán
## Actividad #- Resolución de sistemas de ecuaciones lineales
  

---

##  Objetivo de la Documentación
El propósito de este documento es **registrar la resolución de ecuacines lineares utilizando matrices**. Los métodos que se implementaron son: **Gauss,Gauss-Jordan, matriz inversa y regla de Cremer**.

---

##  Ejercicios Realizados

---

#  Matriz (3x3)


$$
\begin{cases}
x + y + z = 6\\
2x - y + z = 3\\
x + 2y - z = 2
\end{cases}
$$

En forma matricial:

$$
A =
\begin{pmatrix}
1 & 1 & 1\\
2 & -1 & 1\\
1 & 2 & -1
\end{pmatrix},
\qquad
\mathbf{x} =
\begin{pmatrix}
x\\y\\z
\end{pmatrix},
\qquad
\mathbf{b} =
\begin{pmatrix}
6\\3\\2
\end{pmatrix},
\qquad
A\mathbf{x} = \mathbf{b}.
$$


---

###  Resolución por método de Gauss

#### Matriz aumentada:
$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6\\
2 & -1 & 1 & 3\\
1 & 2 & -1 & 2
\end{array}
\right]
$$

1. Eliminar la \(x\) de las filas 2 y 3:

$$
R_2 \leftarrow R_2 - 2R_1,\quad
R_3 \leftarrow R_3 - R_1
$$

$$
\longrightarrow
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6\\
0 & -3 & -1 & -9\\
0 & 1 & -2 & -4
\end{array}
\right]
$$

2. Intercambio en la segunda fila:

$$
R_2 \leftrightarrow R_3
\Longrightarrow
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6\\
0 & 1 & -2 & -4\\
0 & -3 & -1 & -9
\end{array}
\right]
$$

3. Eliminar la \(y\) de la fila 3:

$$
R_3 \leftarrow R_3 + 3R_2
$$

$$
\longrightarrow
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6\\
0 & 1 & -2 & -4\\
0 & 0 & -7 & -21
\end{array}
\right]
$$

A partir de la forma escalonada:

$$
-7z = -21 \Rightarrow z = 3,
$$

$$
y - 2z = -4 \Rightarrow y - 6 = -4 \Rightarrow y = 2,
$$

$$
x + y + z = 6 \Rightarrow x + 2 + 3 = 6 \Rightarrow x = 1.
$$

Por tanto:

$$
(x,y,z) = (1,2,3).
$$

---
#### Resolución por Gauss-Jordan
$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6\\
0 & 1 & -2 & -4\\
0 & 0 & -7 & -21
\end{array}
\right]
$$

1. Tercera fila:

$$
R_3 \leftarrow -\frac{1}{7} R_3
\Longrightarrow
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6\\
0 & 1 & -2 & -4\\
0 & 0 & 1 & 3
\end{array}
\right]
$$

2. Eliminar la variable \(z\) en filas 1 y 2:

$$
R_2 \leftarrow R_2 + 2R_3,\quad
R_1 \leftarrow R_1 - R_3
$$

$$
\longrightarrow
\left[
\begin{array}{ccc|c}
1 & 1 & 0 & 3\\
0 & 1 & 0 & 2\\
0 & 0 & 1 & 3
\end{array}
\right]
$$

3. Eliminar \(y\) de la primera fila:

$$
R_1 \leftarrow R_1 - R_2
$$

$$
\Longrightarrow
\left[
\begin{array}{ccc|c}
1 & 0 & 0 & 1\\
0 & 1 & 0 & 2\\
0 & 0 & 1 & 3
\end{array}
\right]
$$

Solución final:

$$
x = 1,\quad y = 2,\quad z = 3.
$$

---
#### Resolución por matriz inversa
Matirz:
$$
A =
\begin{pmatrix}
1 & 1 & 1\\
2 & -1 & 1\\
1 & 2 & -1
\end{pmatrix}.
$$

Determinante por Sarrus:

$$
\det(A) = 1(-1)(-1) + 1(1)(1) + 1(2)(2)
          - 1(-1)(1) - 1(2)(-1) - 1(1)(2)
        = 7.
$$

Como \(\det(A)\neq 0\), si hay inversa:

$$
A^{-1} = \frac{1}{7}
\begin{pmatrix}
-1 & 3 & 2\\
3 & -2 & 1\\
5 & -1 & -3
\end{pmatrix}.
$$

Multiplicamos \(A^{-1}\mathbf{b}\):

$$
A^{-1}\mathbf{b}
= \frac{1}{7}
\begin{pmatrix}
-1 & 3 & 2\\
3 & -2 & 1\\
5 & -1 & -3
\end{pmatrix}
\begin{pmatrix}
6\\3\\2
\end{pmatrix}.
$$

Resultado:

$$
\begin{pmatrix}
7\\14\\21
\end{pmatrix}
$$

Aplicamos \(\tfrac{1}{7}\):

$$
\mathbf{x}=
\begin{pmatrix}
1\\2\\3
\end{pmatrix}.
$$

---

#### Resolución por regla de Cramer

Matrices:

$$
A =
\begin{pmatrix}
1 & 1 & 1\\
2 & -1 & 1\\
1 & 2 & -1
\end{pmatrix},\quad
\mathbf{b} =
\begin{pmatrix}
6\\3\\2
\end{pmatrix},
$$

Determinante:

$$
D = 7
$$

Matrices modificadas:

$$
A_x =
\begin{pmatrix}
6 & 1 & 1\\
3 & -1 & 1\\
2 & 2 & -1
\end{pmatrix},
$$

$$
A_y =
\begin{pmatrix}
1 & 6 & 1\\
2 & 3 & 1\\
1 & 2 & -1
\end{pmatrix},
$$

$$
A_z =
\begin{pmatrix}
1 & 1 & 6\\
2 & -1 & 3\\
1 & 2 & 2
\end{pmatrix}.
$$

Determinantes:

$$
D_x=7,\quad D_y=14,\quad D_z=21
$$

Solución:

$$
x=1,\quad y=2,\quad z=3.
$$

---

###  Proceso / Procedimiento
1. Se observa cada matriz.
2. Se identifica la posición de los ceros y los valores distintos.
3. Se comparan los elementos con las propiedades de cada tipo de matriz.
4. Se clasifica según corresponda: identidad, diagonal, simétrica o triangular.

---

#  EJERCICIO 2: Operaciones Básicas

###  Enunciado del Problema
Realizar operaciones básicas con las siguientes matrices:

$$
A =
\begin{pmatrix}
2 & -1 \\
3 & 4 \\
\end{pmatrix}
$$


$$
B =
\begin{pmatrix}
5 & 2 \\
-1 & 3 \\
\end{pmatrix}
$$

---

###  Solución / Respuesta

#### a) Suma de matrices A + B

$$ A + B =
\begin{pmatrix}
2 + 5 & -1 + 2 \\
3 + (-1) & 4 + 3 \\
\end{pmatrix}
$$

$$ A + B =
\begin{pmatrix}
7 & 1 \\
2 & 7 \\
\end{pmatrix}
$$

---

#### b) Operación 2A - B

1. Multiplicamos la matriz A por el escalar 2:

  $$ K = 2
  $$

  $$ 2A =
  \begin{pmatrix}
  2(2) & 2(-1) \\
  2(3) & 2(4) \\
  \end{pmatrix}
  $$


2. Restamos la matriz B:

$$ 2A - B =
\begin{pmatrix}
4 - 5 & -2 - 2 \\
6 - (-1) & 8 - 3 \\
\end{pmatrix}
$$

   $$ 2A - B =
\begin{pmatrix}
-1 & -4 \\
7 & 5 \\
\end{pmatrix}
$$

---

#### c) Producto de matrices AB

$$ AB =
\begin{bmatrix}
10 & 4 \\
1 & -3 \\
--- & ---- \\
15 & 6 \\
-4 & 12 \\
\end{bmatrix}
$$

$$ AB =
\begin{pmatrix}
11 & 1 \\
11 & 18 \\
\end{pmatrix}
$$

---

#### d) Producto de matrices BA

$$ BA =
\begin{bmatrix}
10 & 5 \\
6 & 8 \\
---- & ---- \\
-2 & 1 \\
9 & 12 \\
\end{bmatrix}
$$

$$ BA =
\begin{bmatrix}
16 & 3 \\
7 & 13 \\
\end{bmatrix}
$$

---

#### e) Respuesta de A (Aᵀ)

$$ Aᵀ =
\begin{pmatrix}
2 & 3 \\
-1 & 4 \\
\end{pmatrix}
$$

---

###  Proceso / Procedimiento
- **Suma y resta:** se realizan elemento por elemento.  
- **Multiplicación:** se multiplica la fila de la primera matriz por la columna de la segunda.  
- **Transpuesta:** se intercambian filas por columnas.  

---

# EJERCICIO 3: Multiplicación de cadena

### Enunciado del Problema
Verificar que se cumple la propiedad asociativa de la multiplicación de matrices:  
**(AB)C = A(BC)**

Dadas las siguientes matrices:

$$ A =
\begin{pmatrix}
1 & 2 \\
3 & 4 \\
\end{pmatrix}
$$

$$ B =
\begin{pmatrix}
2 & 0 \\
1 & 3 \\
\end{pmatrix}
$$

$$ C =
\begin{pmatrix}
1 & 1 \\
0 & 2 \\
\end{pmatrix}
$$

---

### Solución / Respuesta

#### Cálculo de (AB)C

1. Primero, calculamos **AB**:

  $$ AB =
  \begin{bmatrix}
  2 & 0 \\
  2 & 6 \\
  ---- & ---- \\
  6 & 0 \\
  4 & 12 \\
  \end{bmatrix}
  $$

  $$ AB =
  \begin{pmatrix}
  4 & 6 \\
  10 & 12 \\
  \end{pmatrix}
  $$
   
2. Luego, multiplicamos el resultado por **C**:

  $$ (AB)C =
  \begin{bmatrix}
  4 & 4 \\
  0 & 12 \\
  ---- & ---- \\
  10 & 10 \\
  0 & 24 \\
  \end{bmatrix}
  $$

  $$ (AB)C =
  \begin{pmatrix}
  4 & 16 \\
  10 & 34 \\
  \end{pmatrix}
  $$

---

#### Cálculo de A(BC)

1. Primero, calculamos **BC**:

  $$ BC =
  \begin{bmatrix}
  2 & 2 \\
  0 & 0 \\
  ---- & ---- \\
  1 & 1 \\
  0 & 6 \\
  \end{bmatrix}
  $$

  $$ BC =
  \begin{pmatrix}
  2 & 2 \\
  1 & 7 \\
  \end{pmatrix}
  $$

3. Luego, multiplicamos **A** por el resultado:

  $$ a(BC) =
  \begin{bmatrix}
  2 & 2 \\
  2 & 14 \\
  ---- & ---- \\
  6 & 6 \\
  4 & 28 \\
  \end{bmatrix}
  $$

  $$ A(BC) =
  \begin{pmatrix}
  4 & 16 \\
  10 & 34 \\
  \end{pmatrix}
  $$

---

### Verificación
Como se puede observar:

$$
(AB)C = A(BC)
$$

Por lo tanto, **se cumple la propiedad asociativa** de la multiplicación de matrices.

---

## Conclusión
En esta práctica se aplicaron los conceptos fundamentales de **clasificación y operaciones con matrices**, comprobando propiedades importantes como la **asociatividad**.  
Esto permitió reforzar la lógica de operaciones elementales y mejorar la comprensión de los procesos de cálculo matricial que son base en programación y álgebra.

---




