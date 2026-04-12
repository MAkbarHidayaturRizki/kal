---
title: Sistem Persamaan Linier

---


# Sistem Persamaan Linier
Sistem Persamaan Linear (SPL) adalah kumpulan dua atau lebih persamaan linear yang memiliki variabel yang sama dan diselesaikan secara bersamaan.

Persamaan linear sendiri adalah persamaan aljabar dengan setiap variabel berpangkat satu.

Bentuk umum SPL dengan 𝑛 variabel:

$$
\begin{aligned}
a_{11}x_1 + a_{12}x_2 + \dots + a_{1n}x_n &= b_1 \\
a_{21}x_1 + a_{22}x_2 + \dots + a_{2n}x_n &= b_2 \\
\vdots \\
a_{m1}x_1 + a_{m2}x_2 + \dots + a_{mn}x_n &= b_m
\end{aligned}
$$


### a. Solusi Persamaan Linier
Solusi SPL adalah nilai variabel yang memenuhi semua persamaan dalam sistem tersebut.

Kemungkinan solusi:

1. Solusi tunggal (unik) → hanya satu solusi.
2. Tak hingga banyak solusi → ada variabel bebas.
3. Tidak ada solusi → sistem tidak konsisten.

### a. Contoh Sistem Persamaan Linier Dua Variabel (SPLDV)


\begin{cases}
x + y = 5 \\
x - y = 1
\end{cases}

**Penyelesaian:**

Jumlahkan kedua persamaan:

$$ (x+y) + (x-y) = 5 + 1 $$

$$ 2x = 6 $$

$$ x = 3 $$

Substitusi ke persamaan pertama:

$$ 3 + y = 5 $$

$$ y = 2 $$

**Solusi:**

$$ (x,y) = (3,2) $$

---

### c. Contoh Sistem Persamaan Linier Tiga Variabel (SPLTV)

$$
\begin{cases}
x + y + z = 6 \\
x + y = 4 \\
z = 2
\end{cases}
$$


Dari persamaan ketiga:


$$ z = 2 $$

Substitusi ke persamaan pertama:

$$ x + y + 2 = 6 $$

$$ x + y = 4 $$

Misalnya ambil:


$$ x = 2, \quad y = 2 $$

**Salah satu solusi:**

$$ (x,y,z) = (2,2,2) $$


### d. Matriks Augmentas
Matriks augmentasi adalah matriks yang diperoleh dengan menggabungkan matriks koefisien suatu sistem persamaan linear dengan vektor konstanta (ruas kanan).

Jika sistem ditulis dalam bentuk:
$$ Ax = b $$

maka matriks augmentasinya ditulis sebagai:
$$ [A \mid b] $$