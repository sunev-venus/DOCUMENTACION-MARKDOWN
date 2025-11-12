# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Alumno: Venus Getsemaní Semino Alemán
## Actividad \#16 - Matrices doc
**Fecha:** 11 de noviembre de 2025 
  

---

##  Objetivo de la Documentación
El propósito de este documento es **registrar y explicar paso a paso** los ejercicios relacionados con el **tema de matrices**, abarcando su **clasificación, operaciones básicas y multiplicación de cadenas de matrices**, con el fin de reforzar los fundamentos de álgebra lineal aplicados en programación.

---

##  Ejercicios Realizados

A continuación, se documentan los ejercicios solicitados con su respectivo enunciado, solución y procedimiento. Estos fueron realizados en el salón de clase como asistencia del día.

---

#  EJERCICIO 1: Clasificar Matrices

###  Enunciado del Problema
Identificar el tipo de matriz según sus elementos y su posición dentro de la misma.

---

###  Solución / Respuesta

#### Matriz A:
$$
A =
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
$$

**Tipo:** *Matriz identidad*  
**Justificación:** Los elementos de la diagonal principal son **1** y los demás son **0**.

---

#### Matriz B:
$$
B =
\begin{pmatrix}
3 & 0 & 0 \\
0 & -2 & 0 \\
0 & 0 & 5 \\
\end{pmatrix}
$$

**Tipo:** *Matriz diagonal*  
**Justificación:** Todos los elementos fuera de la diagonal principal son **0**.

---

#### Matriz C:
$$
C =
\begin{pmatrix}
2 & 1 & 4 \\
1 & 3 & 5 \\
4 & 5 & 6 \\
\end{pmatrix}
$$

**Tipo:** *Matriz simétrica*  
**Justificación:** Los elementos están distribuidos de forma simétrica respecto a la diagonal principal.

---

#### Matriz D:
$$
D =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 4 & 5 \\
0 & 0 & 6 \\
\end{pmatrix}
$$

**Tipo:** *Matriz triangular superior*  
**Justificación:** Todos los elementos **debajo de la diagonal** son **0**.

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




