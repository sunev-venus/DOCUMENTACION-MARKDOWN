# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Alumno: Venus Getsemaní Semino Alemán
## Actividad \#16 - Matrices doc

---
### Identificación de matrices

Matriz identidad, porque la diagonal está compuestos por solo unos y los elementos fuera de la diagonal son ceros.

$$ A =
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
$$

MUESTRA

Calcula la suma de A y B

$$ A =
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
\end{pmatrix}
$$

$$ B =
\begin{pmatrix}
9 & 10 & 11 \\
12 & 13 & 14 \\
\end{pmatrix}
$$

$$ A + B =
\begin{pmatrix}
1 + 9 & 2 + 10 & 3 + 11 \\
4 + 12 & 5 + 13 & 6 + 14 \\
\end{pmatrix}
$$

$$ A + B =
\begin{pmatrix}
10 & 12 & 14 \\
16 & 18 & 20 \\
\end{pmatrix}
$$

---
# EJERCICIO 1: Clasificar matrices
 
### Identifica el tipo de cada matriz:

$$ A =
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
$$

MATRÍZ IDENTIDAD: Los elementos de la diagonal son uno y los demás son ceros.

$$ B =
\begin{pmatrix}
3 & 0 & 0 \\
0 & -2 & 0 \\
0 & 0 & 5 \\
\end{pmatrix}
$$

MATRÍz DIAGONAL: Los elementos fuera de la diaonal son cero.

$$ C =
\begin{pmatrix}
2 & 1 & 4 \\
1 & 3 & 5 \\
4 & 5 & 6 \\
\end{pmatrix}
$$

MATRÍZ SIMÉTRICA: Los elementos son sipétricos entre sí, la diagona hace un espejo entre ellos.

$$ D =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 4 & 5 \\
0 & 0 & 6 \\
\end{pmatrix}
$$

MATRÍZ TRIANGULAR SUPERIOR: Elementos debajo de la diagonal son cero.


---
# EJERCICIO 2: Operaciones básicas
 
### Dadas las marices:

$$ A =
\begin{pmatrix}
2 & -1 \\
3 & 4 \\
\end{pmatrix}
$$

$$ B =
\begin{pmatrix}
5 & 2 \\
-1 & 3 \\
\end{pmatrix}
$$

### Calcula
a) A + B

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

b) 2A + B

$$ K = 2
$$

$$ 2A =
\begin{pmatrix}
2(2) & 2(-1) \\
2(3) & 2(4) \\
\end{pmatrix}
$$

$$ 2A =
\begin{pmatrix}
4 & -2 \\
6 & 8 \\
\end{pmatrix}
$$

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

c) AB

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

d) BA

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

e) AT

$$ AT =
\begin{pmatrix}
2 & 3 \\
-1 & 4 \\
\end{pmatrix}
$$


---
# EJERCICIO 3: Multiplicacion de cadena
 
### Dadas:

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

Verifica que (AB)C = A(BC)

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

----

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

Verifica que (AB)C = A(BC) -> Cumple con la igualdad

---







