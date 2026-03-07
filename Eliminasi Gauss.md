---
title: Eleminasi Gauss

---


# Soal
###  1. Sistem Persamaan Linear
$$
\begin{cases} 
x_1 + x_2 + x_3 + x_4 + x_5 = 15 \\
2x_1 + 3x_2 + 2x_3 + 2x_4 + 2x_5 = 31 \\
0x_1 + x_2 + 2x_3 + x_4 + x_5 = 10 \\
x_1 + x_2 + x_3 + 2x_4 + 2x_5 = 21 \\
0x_1 + 0x_2 + 0x_3 + 0x_4 + 2x_5 = 4 
\end{cases}
$$


### 2. Matriks Augmentasi Awal
$$
\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 1 & 15 \\
2 & 3 & 2 & 2 & 2 & 31 \\
0 & 1 & 2 & 1 & 1 & 10 \\
1 & 1 & 1 & 2 & 2 & 21 \\
0 & 0 & 0 & 0 & 2 & 4
\end{array}
$$

# Penyelesaian

### 1. Membersihkan Kolom 1 (Bawah Pivot $x_1$)
#### Operasi :
$$
\begin{matrix}
R_2 = R_2-2R_1\\
R_4 = R_4-R_1 
\end{matrix}
$$

#### Hasil :
$$
\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 1 & 15 \\
0 & 1 & 0 & 0 & 0 & 1 \\
0 & 1 & 2 & 1 & 1 & 10 \\
0 & 0 & 0 & 1 & 1 & 6 \\
0 & 0 & 0 & 0 & 2 & 4
\end{array}
$$

### 2. Membersihkan Kolom 2 (Bawah Pivot $x_2$)
#### Operasi :
$$
\begin{matrix}
R_3 = R_3-R_2
\end{matrix}
$$

#### Hasil :
$$
\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 1 & 15 \\
0 & 1 & 0 & 0 & 0 & 1 \\
0 & 0 & 2 & 1 & 1 & 9 \\
0 & 0 & 0 & 1 & 1 & 6 \\
0 & 0 & 0 & 0 & 2 & 4
\end{array}
$$

### 3. Jawaban akhir
#### a. Dari Baris ke-5
$$
\begin{matrix}
2x_5 = 4 \\
x_5 = \frac{4} {2} = 2\\
x_5 = 2
\end{matrix}
$$
#### b. Dari Baris ke-4
$$
\begin{matrix}
1x_4+1x_5 = 6\\
x_4 + 2 = 6\\
x_4 = 6 - 2 = 4\\
x_4 = 4
\end{matrix}
$$

#### c. Dari Baris ke-3
$$
\begin{matrix}
2x_3 + 1x_4 + 1x_5 = 9\\
2x_3 + 4 + 2 = 9\\
2x_3 + 6 = 9\\
2x_3 = 3\\
x_3 = \frac{3}{2} = 1.5\\
x_3 = 1.5
\end{matrix}
$$
#### d. Dari Baris ke-2 
$$
\begin{matrix}
1x_2 = 1\\
x_2 = 1
\end{matrix}
$$

#### e. Dari Baris ke-1
$$
\begin{matrix}
x_1 + x_2 + x_3 + x_4 + x_5 = 15\\
x_1 + 1 + 1.5 + 4 + 2 = 15\\
x_1 + 8.5 = 15\\
x_1 = 15 - 8.5 = 6.5\\
x_1 = 6.5
\end{matrix}
$$
#### f. Hasil Akhir
$$(x_1 = 6.5, x_2 = 1, x_3 = 1.5,x_4 = 4, x_5 = 2 )$$