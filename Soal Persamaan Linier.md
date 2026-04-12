---
title: UTS Determinan

---

# Soal Persamaan Linier
$$
\begin{cases} 
x_1 + x_2 + x_3 + x_4 + x_5 = 15 \\
2x_1 + 3x_2 + x_3 + x_4 + x_5 = 23 \\
x_1 + 2x_2 + 3x_3 + x_4 + x_5 = 25 \\
x_1 + x_2 + 2x_3 + 3x_4 + x_5 = 27 \\
x_1 + x_2 + x_3 + 2x_4 + 3x_5 = 29
\end{cases}
$$

$$
\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 1 & 15 \\
2 & 3 & 1 & 1 & 1 & 23 \\
1 & 2 & 3 & 1 & 1 & 25 \\
1 & 1 & 2 & 3 & 1 & 27 \\
1 & 1 & 1 & 2 & 3 & 29
\end{array}
$$

# Jawaban

## a. Diketahui:

$$
A= 
\begin{bmatrix}
1 & 1 & 1 & 1 & 1  \\
2 & 3 & 1 & 1 & 1  \\
1 & 2 & 3 & 1 & 1  \\
1 & 1 & 2 & 3 & 1  \\
1 & 1 & 1 & 2 & 3
\end{bmatrix}
$$

$$
X= 
\begin{bmatrix}
x_1 \\
x_2 \\
x_3 \\
x_4 \\
x_5
\end{bmatrix}
, \quad
 B= 
\begin{bmatrix}
15 \\
23 \\
25 \\
27 \\
29
\end{bmatrix}
$$

## b. Mencari Determinan A
Untuk Mencari determinan A bisa memakai rumus Determinan yaitu:
$$
\det(A)=\sum_{j=1}^{n}(-1)^{1+j} a_{1j}\,\det(A_{1j})
$$
Tetapi dengan rumus itu untuk menghitung matriks 5x5 akan sangat panjang dan memakan waktu lama, contohnya untuk rumus 4x4 saja seperti ini.

##### Contoh Matriks:
$$
\begin{bmatrix}
a & b & c & d \\
e & f & g & h \\
i & j & k & l \\
m & n & o & p
\end{bmatrix}
$$
##### Rumus:
$$
\begin{aligned}
& a(f(kp - lo) - g(jp - ln) + h(jo - kn)) \\
& - b(e(kp - lo) - g(ip - lm) + h(io - km)) \\
& + c(e(jp - ln) - f(ip - lm) + h(in - jm)) \\
& - d(e(jo - kn) - f(io - km) + g(in - jm))
\end{aligned}
$$

Rumus di atas masih 4x4 dan untuk 5x5 akan jauh lebih panjang. Dengan seperti itu untuk mencari determinan dari matriks 5x5 lebih baik dengan cara lain, salah satunya bisa dengan mengubah matriks nya menjadi matriks segita dengan cara seperti dalam operasi eleminasi gauss. Setelah matriks nya sudah menjadi matriks segitiga kita tinggal mengkalikan angka angka di garis diagonalnya untuk mendapatkan determinannya.

##### 1. Operasi ke-1:

##### $\quad$Operasi :
$$
\begin{matrix}
R_2 = R_2-2R_1 \\
R_3 = R_3-R_1 \\
R_4 = R_4-R_1 \\
R_5 = R_5-R_1 
\end{matrix}
$$
##### $\quad$Hasil :
$$
\begin{bmatrix}
1 & 1 & 1 & 1 & 1 \\
0 & 1 & -1 & -1 & -1 \\
0 & 1 & 2 & 0 & 0 \\
0 & 0 & 1 & 2 & 0 \\
0 & 0 & 0 & 1 & 2
\end{bmatrix}
$$

##### 2. Operasi ke-2:

##### $\quad$Operasi :
$$
\begin{matrix}
R_3 = R_3-R_2
\end{matrix}
$$
##### $\quad$Hasil :
$$
\begin{bmatrix}
1 & 1 & 1 & 1 & 1 \\
0 & 1 & -1 & -1 & -1 \\
0 & 0 & 3 & 1 & 1 \\
0 & 0 & 1 & 2 & 0 \\
0 & 0 & 0 & 1 & 2
\end{bmatrix}
$$

##### 3. Operasi ke-3:

##### $\quad$Operasi :
$$
\begin{matrix}
R_4 = 3R_4-R_3
\end{matrix}
$$
##### $\quad$Hasil :
$$
\begin{bmatrix}
1 & 1 & 1 & 1 & 1 \\
0 & 1 & -1 & -1 & -1 \\
0 & 0 & 3 & 1 & 1 \\
0 & 0 & 0 & 5 & -1 \\
0 & 0 & 0 & 1 & 2
\end{bmatrix}
$$

##### 4. Operasi ke-4:

##### $\quad$Operasi :
$$
\begin{matrix}
R_5 = 5R_5-R_4
\end{matrix}
$$
##### $\quad$Hasil :
$$
\begin{bmatrix}
1 & 1 & 1 & 1 & 1 \\
0 & 1 & -1 & -1 & -1 \\
0 & 0 & 3 & 1 & 1 \\
0 & 0 & 0 & 5 & -1 \\
0 & 0 & 0 & 0 & 11
\end{bmatrix}
$$

$$\quad$$

Hasil dari merubah matriks A tadi menjadi matriks segitiga maka akan mendapatkan hasil matrik seperti berikut:

$$
\begin{bmatrix}
1 & 1 & 1 & 1 & 1 \\
0 & 1 & -1 & -1 & -1 \\
0 & 0 & 3 & 1 & 1 \\
0 & 0 & 0 & 5 & -1 \\
0 & 0 & 0 & 0 & 11
\end{bmatrix}
$$

$$\quad$$

Setelah mendapatkan matriks segitanya sekarang tinggal mengambil angka angka di garis diagonalnya yaitu:

$$ 1 \times 1 \times 3 \times 5 \times 11 = 165 $$

Sekarang kita mendapatkan hasilnya, tetapi 165 masih belum akhir karena tadi untuk mengubah matriks awal menjadi matriks segitiga kita menggunakan operasi perkalian konstanta maka hasil yang kita dapatkan tidak determinan yang asli tetapi masih perlu di ubah lagi dengan cara membagi hasil determinan sekarang dengan hasil perkalian semua konstanta yang kita pakai sebelumnya maka akan membentuk rumus:

$$det(A) = \frac {165} {3 \times 5}$$

$$det(A) = \frac {165} {15} = 11$$

Maka Determinan asli dari matriks A adalah 11.



## c. Mencari Adjoin A
Untuk mendapatkan adjoin dari matriks A kita bisa menggunakan rumus adjoin berikut:
##### Rumus Adjoin:
$$(adjA)_{ij} = (-1)^{i+j} M_{ji}$$
Rumus adjoin di atas berasal dari rumus rumus berikut:

##### Rumus Kufaktor:
$$C_{ij} = (-1)^{i+j} \cdot M_{ij}$$

##### Transpose Matriks Kofaktor:
$$Adj(A) = C^T$$ 

##### Hasil dari rumus di atas menjadi: 
$$Adj(A) = C_{ji}$$ 
###### Atau 
$$(adjA)_{ij} = (-1)^{i+j} M_{ji}$$

Dengan rumus di atas kita harus mendapatkan adjoin dari matriks A, dengan rumus di atas kita bisa mulai menghitung adjoin dari matriks A.

Pertama kita harus mendapatkan minor matriks A terlebih dahulu, rumus yang bisa di gunakan seperti berikut:
##### Rumus Minor 5x5:
$$
\begin{bmatrix}
M_{11} & M_{12} & M_{13} & M_{14} & M_{15} \\
M_{21} & M_{22} & M_{23} & M_{24} & M_{25} \\
M_{31} & M_{32} & M_{33} & M_{34} & M_{35} \\
M_{41} & M_{42} & M_{43} & M_{44} & M_{45} \\
M_{51} & M_{52} & M_{53} & M_{54} & M_{55}
\end{bmatrix}
$$

Dengan rumus di atas kita bisa mulai mencari nilai $M_{11}$ sampai $M_{55}$ dengan cara mengambil matriks 4x4 di setiap posisi $M_{11}$ sampai $M_{55}$ lalu matriksnya hitung untuk mendapatkan nilai determinan di setiap matriksnya dan hasilnya di taro di posisi $M_{11}$ sampai $M_{55}$ di tempat matriks 4x4 tadi berasal.
$\quad$
Selain dengan rumus tadi kita bisa menggunakan cara sebelumnya untuk mencari nilai determinan matriks 5x5 yaitu dengan cara seperti proses eleminasi gauss untuk mengubah matriksnya menjadi matriks segitiga lalu nilai di garis diagonalnya di kalikan dan akan mendapatkan nilai determinan 4x4 yang akan membentuk minor matriks A.

#### List Matriks 4x4 $M_{11}$ sampai $M_{55}$:

##### a. Matriks $M_{1j}$
$$
M_{11} =
\begin{bmatrix}
3 & 1 & 1 & 1 \\
2 & 3 & 1 & 1 \\
1 & 2 & 3 & 1 \\
1 & 1 & 2 & 3
\end{bmatrix}
= 39 
$$

$$
M_{12} =
\begin{bmatrix}
2 & 1 & 1 & 1 \\
1 & 3 & 1 & 1 \\
1 & 2 & 3 & 1 \\
1 & 1 & 2 & 3
\end{bmatrix}
= 25
$$

$$
M_{13} =
\begin{bmatrix}
2 & 3 & 1 & 1 \\
1 & 2 & 1 & 1 \\
1 & 1 & 3 & 1 \\
1 & 1 & 2 & 3
\end{bmatrix}
= 7
$$

$$
M_{14} =
\begin{bmatrix}
2 & 3 & 1 & 1 \\
1 & 2 & 3 & 1 \\
1 & 1 & 2 & 1 \\
1 & 1 & 1 & 3
\end{bmatrix}
= 9
$$

$$
M_{15} =
\begin{bmatrix}
2 & 3 & 1 & 1 \\
1 & 2 & 3 & 1 \\
1 & 1 & 2 & 3 \\
1 & 1 & 1 & 2
\end{bmatrix}
= -1
$$

##### b. Matriks $M_{2j}$

$$
M_{21} =
\begin{bmatrix}
1 & 1 & 1 & 1 \\
2 & 3 & 1 & 1 \\
1 & 2 & 3 & 1 \\
1 & 1 & 2 & 3
\end{bmatrix}
= 5
$$

$$
M_{22} =
\begin{bmatrix}
1 & 1 & 1 & 1 \\
1 & 3 & 1 & 1 \\
1 & 2 & 3 & 1 \\
1 & 1 & 2 & 3
\end{bmatrix}
= 8
$$

$$
M_{23} =
\begin{bmatrix}
1 & 1 & 1 & 1 \\
1 & 2 & 1 & 1 \\
1 & 1 & 3 & 1 \\
1 & 1 & 2 & 3
\end{bmatrix}
= 4
$$

$$
M_{24} =
\begin{bmatrix}
1 & 1 & 1 & 1 \\
1 & 2 & 3 & 1 \\
1 & 1 & 2 & 1 \\
1 & 1 & 1 & 3
\end{bmatrix}
= 2
$$

$$
M_{25} =
\begin{bmatrix}
1 & 1 & 1 & 1 \\
1 & 2 & 3 & 1 \\
1 & 1 & 2 & 3 \\
1 & 1 & 1 & 2
\end{bmatrix}
= 1
$$

##### c. Matriks $M_{3j}$

$$
M_{31} =
\begin{bmatrix}
1 & 1 & 1 & 1 \\
3 & 1 & 1 & 1 \\
1 & 2 & 3 & 1 \\
1 & 1 & 2 & 3
\end{bmatrix}
= -6
$$

$$
M_{32} =
\begin{bmatrix}
1 & 1 & 1 & 1 \\
2 & 1 & 1 & 1 \\
1 & 2 & 3 & 1 \\
1 & 1 & 2 & 3
\end{bmatrix}
= -3
$$

$$
M_{33} =
\begin{bmatrix}
1 & 1 & 1 & 1 \\
2 & 3 & 1 & 1 \\
1 & 1 & 3 & 1 \\
1 & 1 & 2 & 3
\end{bmatrix}
= 4
$$

$$
M_{34} =
\begin{bmatrix}
1 & 1 & 1 & 1 \\
2 & 3 & 1 & 1 \\
1 & 1 & 2 & 1 \\
1 & 1 & 1 & 3
\end{bmatrix}
= 2
$$

$$
M_{35} =
\begin{bmatrix}
1 & 1 & 1 & 1 \\
2 & 3 & 1 & 1 \\
1 & 1 & 2 & 3 \\
1 & 1 & 1 & 2
\end{bmatrix}
= 1
$$


##### d. Matriks $M_{4j}$
$$
M_{41} =
\begin{bmatrix}
 1 & 1 & 1 & 1 \\
 3 & 1 & 1 & 1 \\
 2 & 3 & 1 & 1 \\
 1 & 1 & 2 & 3
\end{bmatrix}
= 4
$$

$$
M_{42} =
\begin{bmatrix}
1 & 1 & 1 & 1 \\
2 & 1 & 1 & 1 \\
1 & 3 & 1 & 1 \\
1 & 1 & 2 & 3
\end{bmatrix}
= 2
$$
$$
M_{43} =
\begin{bmatrix}
1 & 1 & 1 & 1 \\
2 & 3 & 1 & 1 \\
1 & 2 & 1 & 1 \\
1 & 1 & 2 & 3
\end{bmatrix}
= 1
$$
$$
M_{44} =
\begin{bmatrix}
1 & 1 & 1 & 1 \\
2 & 3 & 1 & 1 \\
1 & 2 & 3 & 1 \\
1 & 1 & 1 & 3
\end{bmatrix}
= 6
$$
$$
M_{45} =
\begin{bmatrix}
1 & 1 & 1 & 1 \\
2 & 3 & 1 & 1 \\
1 & 2 & 3 & 1 \\
1 & 1 & 1 & 2
\end{bmatrix}
= 3
$$


##### e. Matriks $M_{5j}$
$$
M_{51} =
\begin{bmatrix}
1 & 1 & 1 & 1  \\
3 & 1 & 1 & 1  \\
2 & 3 & 1 & 1  \\
1 & 2 & 3 & 1
\end{bmatrix}
= -8
$$

$$
M_{52} =
\begin{bmatrix}
1 & 1 & 1 & 1  \\
2 & 1 & 1 & 1  \\
1 & 3 & 1 & 1  \\
1 & 2 & 3 & 1
\end{bmatrix}
= -4
$$

$$
M_{53} =
\begin{bmatrix}
1 & 1 & 1 & 1  \\
2 & 3 & 1 & 1  \\
1 & 2 & 1 & 1  \\
1 & 1 & 3 & 1
\end{bmatrix}
= -2
$$

$$
M_{54} =
\begin{bmatrix}
1 & 1 & 1 & 1  \\
2 & 3 & 1 & 1  \\
1 & 2 & 3 & 1  \\
1 & 1 & 2 & 1
\end{bmatrix}
= -1
$$

$$
M_{55} =
\begin{bmatrix}
1 & 1 & 1 & 1 \\
2 & 3 & 1 & 1 \\
1 & 2 & 3 & 1 \\
1 & 1 & 2 & 3
\end{bmatrix}
= 5
$$


#### Matriks Minor A:
$$
\begin{bmatrix}
39 & 25 & 7 & 9 & -1 \\
5 & 8 & 4 & 2 & 1 \\
-6 & -3 & 4 & 2 & 1 \\
4 & 2 & 1 & 6 & 3 \\
-8 & -4 & -2 & -1 & 5
\end{bmatrix}
$$

#### Matriks Kufaktor:
$$
\begin{bmatrix}
39 & -25 & 7 & -9 & -1 \\
-5 & 8 & -4 & 2 & -1 \\
-6 & 3 & 4 & -2 & 1 \\
-4 & 2 & -1 & 6 & -3 \\
-8 & 4 & -2 & 1 & 5
\end{bmatrix}
$$

#### Matriks Adjoin(A) / Transpose Matriks Kufaktor:
$$
\begin{bmatrix}
39 & -5 & -6 & -4 & -8 \\
-25 & 8 & 3 & 2 & 4 \\
7 & -4 & 4 & -1 & -2 \\
-9 & 2 & -2 & 6 & 1 \\
-1 & -1 & 1 & -3 & 5
\end{bmatrix}
$$

Maka setelah mendapatkan Transpose dari matriks kufaktor A maka itulah matriks Adjoin A, karena adjoin sendiri itu matriks yang di buat dari kufaktor lalu di transpose.

## d.Mencari Solusi Matriks A

Untuk mencari solusi dari Sistem Persamaan Linier kita bisa menggunakan Eliminasi Gauss dan kita juga bisa menggunakan hasil dari perhitungan tadi yaitu dengan rumus:

$$X = A^{-1} B$$

Sebelum lanjut ke rumus di atas kita harus mendapatkan invers A dengan bantuan rumus berikut:

$$A^{-1} = \frac{1}{det(A)} Adj(A)$$

$$A^{-1} = \frac{1}{11}
\begin{bmatrix}
39 & -5 & -6 & -4 & -8 \\
-25 & 8 & 3 & 2 & 4 \\
7 & -4 & 4 & -1 & -2 \\
-9 & 2 & -2 & 6 & 1 \\
-1 & -1 & 1 & -3 & 5
\end{bmatrix}$$

$$A^{-1} = 
\begin{bmatrix}
\frac {39}{11} & \frac{-5}{11} & \frac{-6}{11} & \frac{-4}{11} & \frac{-8}{11} \\
\frac{-25}{11} & \frac{8}{11} & \frac{3}{11} & \frac{2}{11} & \frac{4}{11} \\
\frac{7}{11} & \frac{-4}{11} & \frac{4}{11} & \frac{-1}{11} & \frac{-2}{11} \\
\frac{-9}{11} & \frac{2}{11} & \frac{-2}{11} & \frac{6}{11} & \frac{1}{11} \\
\frac{-1}{11} & \frac{-1}{11} & \frac{1}{11} & \frac{-3}{11} & \frac{5}{11}
\end{bmatrix}$$

Setelah mendapatkan invers matriks A kita tinggal memakai rumus sebelumnya tinggal memasukkan invers matriks A ke rumusnya.

$$X = A^{-1} B$$

$$X = \begin{bmatrix}
\frac {39}{11} & \frac{-5}{11} & \frac{-6}{11} & \frac{-4}{11} & \frac{-8}{11} \\
\frac{-25}{11} & \frac{8}{11} & \frac{3}{11} & \frac{2}{11} & \frac{4}{11} \\
\frac{7}{11} & \frac{-4}{11} & \frac{4}{11} & \frac{-1}{11} & \frac{-2}{11} \\
\frac{-9}{11} & \frac{2}{11} & \frac{-2}{11} & \frac{6}{11} & \frac{1}{11} \\
\frac{-1}{11} & \frac{-1}{11} & \frac{1}{11} & \frac{-3}{11} & \frac{5}{11}
\end{bmatrix}
\times 
\begin{bmatrix}
15 \\
23 \\
25 \\
27 \\
29
\end{bmatrix}
$$

$$X = 
\begin{bmatrix}
\frac{-20}{11} \\
\frac{54}{11} \\
\frac{28}{11} \\
\frac{52}{11} \\
\frac{51}{11}
\end{bmatrix}
$$

Setelah mamakai rumus $X = A^{-1}B$ kita sudah mendapatkan solusi dari matriks A yaitu matrix X.

