# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Alumno: Venus Getsemaní Semino Alemán
## Actividad \#16 - Matrices doc
**Fecha:** 18 de noviembre de 2025 
  

---

## Objetivo de la Documentación
Registrar y explicar los ejercicios realizados sobre el cálculo de determinantes de matrices 2×2 y 3×3 usando diferentes métodos.

---

## Ejercicios Realizados

---

## Ejercicio 1: Cálculo de Determinantes 2×2

### Enunciado del Problema
Calcular los determinantes de las siguientes matrices 2×2:

math
A = \begin{pmatrix} 5 & 2 \\ 3 & 1 \end{pmatrix},\quad
B = \begin{pmatrix} -1 & 4 \\ 2 & -8 \end{pmatrix},\quad
C = \begin{pmatrix} 6 & 9 \\ 2 & 3 \end{pmatrix},\quad
D = \begin{pmatrix} 0 & 5 \\ -5 & 0 \end{pmatrix}


### Respuesta
- *det(A) = –1*  
- *det(B) = 0*  
- *det(C) = 0*  
- *det(D) = 25*

### Procedimiento

1. *Matriz A:*  
   det(A) = (5·1) – (2·3) = 5 – 6 = –1
2. *Matriz B:*  
   det(B) = (–1·–8) – (4·2) = 8 – 8 = 0
3. *Matriz C:*  
   det(C) = (6·3) – (9·2) = 18 – 18 = 0
4. *Matriz D:*  
   det(D) = (0·0) – (5·–5) = 0 – (–25) = 25

---

## Ejercicio 2: Determinante de Matriz 3×3

### Enunciado del Problema

math
F = \begin{pmatrix}
2 & -1 & 3 \\
1 & 4 & 0 \\
3 & 2 & -2
\end{pmatrix}


### Respuesta
- *det(F) = –51*

### Procedimiento
Método aplicado: *Regla de Sarrus o expansión por cofactores*.

math
-38 - 13 = -51


---

## Ejercicio 3: Método de Cofactores para Determinantes 3×3

### Enunciado del Problema

math
G = \begin{pmatrix}
1 & 0 & 2 \\
-1 & 3 & 1 \\
2 & 0 & 1
\end{pmatrix}


### Respuesta
- *det(G) = –9*

### Procedimiento

#### Expansión por cofactores (primera fila)

- *Término 1 (G₁₁):*  
  G₁₁ = 1  
  Signo: *+*  
  Menor:

  math
  M_{11} = \det\begin{pmatrix} 3 & 1 \\ 0 & 1 \end{pmatrix}
  = 3
  

  Término: (1)(3) = 3

- *Término 2 (G₁₂):*  
  G₁₂ = 0  
  → Término = *0*

- *Término 3 (G₁₃):*  
  G₁₃ = 2  
  Signo: *+*  
  Menor:

  math
  M_{13} = \det\begin{pmatrix} -1 & 3 \\ 2 & 0 \end{pmatrix}
  = - (3·2) = -6
  

  Término: (2)(–6) = –12

#### Resultado final

math
\det(G) = 3 + 0 - 12 = -9


---

## Ejercicio 4: Propiedades de los Determinantes

### Enunciado del Problema

math
A = \begin{pmatrix} 2 & 1 \\ 1 & 3 \end{pmatrix},\quad
B = \begin{pmatrix} 1 & 2 \\ 3 & 1 \end{pmatrix}


### Respuesta 
- *det(A) = 5*  
- *det(B) = –5*  
- *det(AB) = –25*  
- *det(Aᵀ) = 5*

### Procedimiento

#### Cálculo de determinantes reales

1. *Determinante de A*

math
\det(A) = (2·3) - (1·1) = 6 - 1 = 5



2. *Determinante de B*

math
\det(B) = (1·1) - (3·2) = - 6 + 1 = - 5



#### Verificación de la propiedad  
det(AB) = det(A)·det(B)


- det(AB) = –25  
- det(A)·det(B) = 5(–5) = –25

*Propiedad verificada* 

#### Verificación de det(Aᵀ) = det(A)

- det(Aᵀ) = 5  
- det(A) = 5  
  *Propiedad verificada* 

---

## Ejercicio 5: Área del Paralelogramo

### Enunciado del Problema
Vectores:

- U = (3, 2)  
- V = (1, 4)

### Respuesta
- *Área = 10*

### Procedimiento

1. *Matriz formada por los vectores*

math
A = \begin{pmatrix} 3 & 2 \\ 1 & 4 \end{pmatrix}


2. *Determinante*

math
\det(A) = 12 - 2 = 10


3. *Interpretación geométrica*  
El valor absoluto del determinante representa el área del paralelogramo.

4. *Cambio de orden*

math
\det\begin{pmatrix} 1 & 4 \\ 3 & 2 \end{pmatrix}
= 2 - 12 = -10


Área = |–10| = 10

---
