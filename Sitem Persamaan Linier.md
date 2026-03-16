---
title: Soal

---


# Soal
###  1. Sistem Persamaan Linear
\begin{cases} 
x_1 + x_2 + x_3 + x_4 + x_5 = 15 \\
2x_1 + 3x_2 + 2x_3 + 2x_4 + 2x_5 = 31 \\
0x_1 + x_2 + 2x_3 + x_4 + x_5 = 10 \\
x_1 + x_2 + x_3 + 2x_4 + 2x_5 = 21 \\
0x_1 + 0x_2 + 0x_3 + 0x_4 + 2x_5 = 4 
\end{cases}


### 2. Matriks Augmentasi Awal

\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 1 & 15 \\
2 & 3 & 2 & 2 & 2 & 31 \\
0 & 1 & 2 & 1 & 1 & 10 \\
1 & 1 & 1 & 2 & 2 & 21 \\
0 & 0 & 0 & 0 & 2 & 4
\end{array}

# Penyelesaian

### 1. Membersihkan Kolom 1 (Bawah Pivot $x_1$)
#### Operasi :
\begin{matrix}
R_2 = R_2-2R_1\\
R_4 = R_4-R_1 
\end{matrix}

#### Hasil :
\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 1 & 15 \\
0 & 1 & 0 & 0 & 0 & 1 \\
0 & 1 & 2 & 1 & 1 & 10 \\
0 & 0 & 0 & 1 & 1 & 6 \\
0 & 0 & 0 & 0 & 2 & 4
\end{array}

### 2. Membersihkan Kolom 2 (Bawah Pivot $x_2$)
#### Operasi :
\begin{matrix}
R_3 = R_3-R_2
\end{matrix}

#### Hasil :
\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 1 & 15 \\
0 & 1 & 0 & 0 & 0 & 1 \\
0 & 0 & 2 & 1 & 1 & 9 \\
0 & 0 & 0 & 1 & 1 & 6 \\
0 & 0 & 0 & 0 & 2 & 4
\end{array}

### 3. Membuat pivot terakhir = 1
#### Operasi :
\begin{matrix}
R_5 = \frac{1}{2}R_5
\end{matrix}

#### Hasil :
\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 1 & 15 \\
0 & 1 & 0 & 0 & 0 & 1 \\
0 & 0 & 2 & 1 & 1 & 9 \\
0 & 0 & 0 & 1 & 1 & 6 \\
0 & 0 & 0 & 0 & 1 & 2
\end{array}

### 4. Menghilangkan angka di atas pivot $x_5$ 
#### Operasi :
\begin{matrix}
R_4 = R_4 - R_5\\
R_3 = R_3 - R_5\\
R_1 = R_1 - R_5
\end{matrix}

#### Hasil :
\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 0 & 13 \\
0 & 1 & 0 & 0 & 0 & 1 \\
0 & 0 & 2 & 1 & 0 & 7 \\
0 & 0 & 0 & 1 & 0 & 4 \\
0 & 0 & 0 & 0 & 1 & 2
\end{array}

### 5. Menghilangkan angka di atas pivot $x_4$
#### Operasi :
\begin{matrix}
R_1 = R_1 - R_4\\
R_3 = R_3 - R_4
\end{matrix}

#### Hasil :
\begin{array}{ccccc|c}
1 & 1 & 1 & 0 & 0 & 9 \\
0 & 1 & 0 & 0 & 0 & 1 \\
0 & 0 & 2 & 0 & 0 & 3 \\
0 & 0 & 0 & 1 & 0 & 4 \\
0 & 0 & 0 & 0 & 1 & 2
\end{array}

### 6. Membuat pivot $x_3$ = 1
#### Operasi :
\begin{matrix}
R_3 = \frac{1}{2}R_3
\end{matrix}

#### Hasil :
\begin{array}{ccccc|c}
1 & 1 & 1 & 0 & 0 & 9 \\
0 & 1 & 0 & 0 & 0 & 1 \\
0 & 0 & 1 & 0 & 0 & \frac{3}{2} \\
0 & 0 & 0 & 1 & 0 & 4 \\
0 & 0 & 0 & 0 & 1 & 2
\end{array}

### 7. Menghilangkan angka di atas pivot $x_3$
#### Operasi :
\begin{matrix}
R_1 = R_1 - R_3\\
\end{matrix}

#### Hasil :
\begin{array}{ccccc|c}
1 & 1 & 0 & 0 & 0 & \frac {15}{2} \\
0 & 1 & 0 & 0 & 0 & 1 \\
0 & 0 & 1 & 0 & 0 & \frac{3}{2} \\
0 & 0 & 0 & 1 & 0 & 4 \\
0 & 0 & 0 & 0 & 1 & 2
\end{array}
### 8. Menghilangkan angka di atas pivot $x_2$
#### Operasi :
\begin{matrix}
R_1 = R_1 - R_2
\end{matrix}

#### Hasil :
\begin{array}{ccccc|c}
1 & 0 & 0 & 0 & 0 & \frac {13}{2} \\
0 & 1 & 0 & 0 & 0 & 1 \\
0 & 0 & 1 & 0 & 0 & \frac {3}{2} \\
0 & 0 & 0 & 1 & 0 & 4 \\
0 & 0 & 0 & 0 & 1 & 2
\end{array}
### f. Hasil Akhir
$$(x_1 = \frac {13}{2}, x_2 = 1, x_3 = \frac {3}{2},x_4 = 4, x_5 = 2 )$$