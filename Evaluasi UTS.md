---
title: Evaluasi UTS

---

# Evaluasi UTS
## Soal
### A. Menghitung Nilai Determinan Matriks Dengan Rumus Ekspansi Baris 
$$\sum_{k=1}^n (-1)^{i+k} a_{ik} M_{ik} $$
### B. Menghitung Invers matriks dengan rumus adjoin
$$\sum_{k=1}^n (-1)^{i+k} a_{ik} M_{ik}$$
$$M_{ij} = \det A_{ij}.$$
### C. Matriks:
#### 1. $A = \begin{bmatrix} -7 & -5 \\ 1 & 4 \end{bmatrix}$
#### 2. $A = \begin{bmatrix} 0 & 2 & -3 \\ 1 & -2 & -1 \\ 0 & 0 & 1 \end{bmatrix}$
#### 3. $A = \begin{bmatrix} 1 & -3 & 1 & 1 \\ -3 & 1 & 1 & 1 \\ 1 & 1 & -3 & 1 \\ 1 & 1 & 1 & -3 \end{bmatrix}.$


## Jawaban
### A. Menghitung Nilai Determinan Matriks Dengan Rumus Ekspansi Baris 
#### 1. Matriks ke-1
$$A = \begin{bmatrix} -7 & -5 \\ 1 & 4 \end{bmatrix}$$
Rumus:
$$(-1)^{1+1} a_{11} M_{11} + (-1)^{1+2} a_{12} M_{12}$$
$$(-1)^{1+1} -7 M_{11} + (-1)^{1+2} -5 M_{12}$$
$$-7 M_{11} + 5 M_{12}$$
$$(-7 \times[4]) + (5 \times[1])$$
$$(-7 \times4) + (5 \times1)$$
$$-28 + 5 = -23$$
Maka Determinan dari Matriksnya adalah -23.
#### 2. Matriks ke-2
$$A = \begin{bmatrix} 0 & 2 & -3 \\ 1 & -2 & -1 \\ 0 & 0 & 1 \end{bmatrix}$$
Rumus:
$$a_{31} M_{31} - a_{32} M_{32} + a_{33} M_{33}$$

$$0 M_{31} - 0 M_{32} + 1 M_{33}$$
$$0 \times \begin{bmatrix} 2 & -3 \\ -2 & -1 \end{bmatrix} - 0 \times \begin{bmatrix} 0 & -3 \\ 1 & -1 \end{bmatrix} + 1 \times \begin{bmatrix} 0 & 2 \\ 1 & -2 \end{bmatrix}$$


$$M_{33} = \begin{bmatrix} 0 & 2 \\ 1 & -2 \end{bmatrix}$$
$$ad - bc$$
$$(0\times−2)−(2\times1) = -2$$

$$det(A)=1\times(−2)=−2$$

Maka determinan matriksnya adalah -2.
#### 3. Matriks ke-3
$$A = \begin{bmatrix} 1 & -3 & 1 & 1 \\ -3 & 1 & 1 & 1 \\ 1 & 1 & -3 & 1 \\ 1 & 1 & 1 & -3 \end{bmatrix}.$$

Rumus:

$$det(A) = a_{11}M_{11} - a_{12}M_{12} + a_{13}M_{13} - a_{14}M_{14}$$
$$1 \times M_{11} - (-3) \times M_{12} + 1 \times M_{13} - 1 \times M_{14}$$
$$M_{11} + 3M_{12} + M_{13} - M_{14}$$

Minor matriks:
$$a(ei-fh)-b(di-fg)+c(dh-eg)$$
Dengan rumus di atas bisa mendapatkan determinan dari minor sub matriks nya.
$$M_{11} = 
\begin{bmatrix} 
1 & 1 & 1 \\ 
1 & -3 & 1 \\ 
1 & 1 & -3 
\end{bmatrix}
$$

$$1\times(1(−3)−1\times1)+1(1\times1−(−3)\times1)$$
$$1(9−1)−1(−3−1)+1(1+3)$$
$$8−(−4)+4=16$$

$$M_{12} = 
\begin{bmatrix} 
-3 & 1 & 1 \\ 
1 & 1 & 1 \\ 
1 & 1 & -3 
\end{bmatrix}
$$
$$−3(9−1)−1(−3−1)+1(1+3)$$
$$−3(8)−(−4)+4=−24+4+4=−16$$

$$M_{13} = 
\begin{bmatrix} 
-3 & 1 & 1 \\ 
1 & 1 & 1 \\ 
1 & 1 & -3 
\end{bmatrix}
$$

$$−3(−3−1)−1(−3−1)+1(1−1)$$
$$−3(−4)−(−4)+0=12+4=16$$

$$M_{14} = 
\begin{bmatrix} 
-3 & 1 & 1 \\ 
1 & 1 & -3 \\ 
1 & 1 & 1 
\end{bmatrix}
$$

$$−3(1+3)−1(1+3)+1(1−1)$$
$$−3(4)−4+0=−12−4=−16$$

$$det(A)=16+3(−16)+16−(−16)$$
$$16−48+16+16 = 0$$

Maka Determinan matriksnya adalah 0.

### B. Menghitung Invers matriks dengan rumus adjoin
Rumus Invers:
$$A^{-1} = \frac{1}{det(A)} Adj(A)$$

#### 1. Matriks ke-1
$$A = \begin{bmatrix} -7 & -5 \\ 1 & 4 \end{bmatrix}$$

Determinan:
$$det(A)=(−7)(4)−(−5)(1)=−28+5=−23$$

Matriks Kufaktor:

$$
\begin{bmatrix}
M_{11} & -M_{12} \\
-M_{21} & M_{22}
\end{bmatrix}
$$
Minor:
$M_{11} = 4$
$M_{12} = 1$
$M_{13} = -5$
$M_{14} = -7$

$$
\begin{bmatrix}
4 & -1 \\
5 & -7
\end{bmatrix}
$$

Adjoin (Transpose dari matriks kufaktor di atas):

$$adj(A) = \begin{bmatrix}
4 & 5 \\
-1 & -7
\end{bmatrix}
$$

Maka Rumus inversnya adalah:

$$A^{-1} = \frac{1}{-23} \begin{bmatrix}
4 & 5 \\
-1 & -7
\end{bmatrix}$$

maka invers matriksnya adalah:
$$A^{-1} = \begin{bmatrix}
-\frac{4}{23} & -\frac{5}{23} \\
\frac{1}{23} & \frac{7}{23}
\end{bmatrix}
$$

#### 2. Matriks ke-2



$$A = \begin{bmatrix} 0 & 2 & -3 \\ 1 & -2 & -1 \\ 0 & 0 & 1 \end{bmatrix}$$

$$det(A) = -2$$

Selanjutnya mencari matriks Minor:

##### a. Matriks $M_{1j}$
$$
M_{11} =
\begin{bmatrix}
-2 & -1 \\
0 & 1 
\end{bmatrix}
= -2
$$
$$
M_{12} =
\begin{bmatrix}
1 & -1 \\
0 & 1 
\end{bmatrix}
= 1
$$
$$
M_{13} =
\begin{bmatrix}
1 & -2 \\
0 & 0
\end{bmatrix}
= 0
$$


##### b. Matriks $M_{2j}$

$$
M_{21} =
\begin{bmatrix}
2 & -3\\
0 & 1 
\end{bmatrix}
= 2
$$

$$
M_{22} =
\begin{bmatrix}
0 & -3 \\
0 & 1 
\end{bmatrix}
= 0
$$

$$
M_{23} =
\begin{bmatrix}
0 & 2 \\
0 & 0 
\end{bmatrix}
= 0
$$


##### c. Matriks $M_{3j}$
$$
M_{31} =
\begin{bmatrix}
2 & -3 \\
-2 & -1 
\end{bmatrix}
= -8
$$

$$
M_{32} =
\begin{bmatrix}
0 & -3 \\
1 & -1 
\end{bmatrix}
= 3
$$

$$
M_{33} =
\begin{bmatrix}
0 & 2 \\
1 & -2 
\end{bmatrix}
= -2
$$

Matriks Kufaktor:

$$
\begin{bmatrix}
-2 & -1 & 0 \\
-2 & 0 & 0 \\
-8 & -3 & -2
\end{bmatrix}
$$

Adjoin (Transpose dari matriks kufaktor di atas):

$$ adj(A) =
\begin{bmatrix}
-2 & -2 & -8 \\
-1 & 0 & -3 \\
0 & 0 & -2
\end{bmatrix}
$$



Maka Rumus inversnya adalah:
$$A^{-1} = \frac{1}{-2} \begin{bmatrix}
-2 & -2 & -8 \\
-1 & 0 & -3 \\
0 & 0 & -2
\end{bmatrix} = \begin{bmatrix}
\frac{-2}{-2} & \frac{-2}{-2} & \frac{-8}{-2}\\
\frac{-1}{-2} & \frac{0}{-2} & \frac{-3}{-2}  \\
\frac{0}{-2} & \frac{0}{-2} & -\frac{-2}{-2}
\end{bmatrix}$$

$$A^{-1} =  \begin{bmatrix}
1 & 1 & 4 \\
\frac{1}{2} & 0 & \frac {3}{2} \\
0 & 0 & 1
\end{bmatrix}$$


#### 3. Matriks ke-3

Karena determinan matriks ke-3 adalah 0 maka matriksnya tidak punya matriks invers

