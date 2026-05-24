---
title: Eigenface Menggunakan Singular Value Decomposition (SVD)

---

# Eigenface Menggunakan Singular Value Decomposition (SVD)

Eigenface adalah metode pengenalan wajah yang menggunakan konsep aljabar linear untuk mencari pola utama dari kumpulan wajah.

Metode ini bekerja dengan mengubah gambar wajah menjadi vector lalu mencari pola utama menggunakan Singular Value Decomposition (SVD).

<a href="https://drive.google.com/drive/folders/1gM5gq5yd2QXxmDMXwEalXzNJq9N0wPBc?usp=drive_link" target="_blank">Download Source Code</a>

Contoh Output:

<hr>

### PREPROCESSING IMAGE

Setelah itu gambar di ubah menjadi grayscale atau berwarna hitam putih.

Setelah itu hasil grayscale nya Semua diubah menjadi ukuran yang sama, misalnya 64×64 pixel.

Tujuan:
- Agar semua data memiliki jumlah pixel yang sama.
- Mempermudah proses matriks.

64×64 = 4096 pixel


Setelah mengubah gambarnyanya menjadi ukuran yang sama, matriks gambarnya akan di ubah yang awalnya 64x64 di ubah ke 4096 x 1 agar menjadi vector dan proses ini menggunakan flatten.

Proses di atas adalah proses mengubah suatu gambar menjadi suatu data matriks, proses ini di gunakan ke semua gambar dan akan menghasilkan suatu matriks 4096 x N atau jumlah gambarnya.

### CENTERING / NORMALIZATION

Rumus Mean Face:
$$\mu = \frac{1}{N}\sum_{i=1}^{N} x_i $$

Rumus Centered Matrix:
$$\Phi_i = x_i - \mu$$

Rumus di atas akan menghasilan matriks yang sudah di normalisasikan untuk mengatur skala nya dan agar numerik lebih stabil dan tidak ada nilai terlalu dominan, matriks nya akan berukuran 4096 x N atau jumlah data gambar yang ada.


Centering dilakukan agar sistem fokus pada perbedaan wajah terhadap rata-rata wajah.

### SINGULAR VALUE DECOMPOSITION

Rumus:
$$A = U\Sigma V^T$$

U (Eigenface) = Menyimpan pola utama wajah (eigenface).
$\Sigma$ (Singular Value= Menyimpan seberapa penting tiap pola.
$V^T$ = Menyimpan hubungan pola terhadap setiap wajah.


Rumus di atas adalah rumus inti yang di gunakan untuk Eigenface menggunakan SVD(Singular Value Decomposition).

Setiap kolom pada matriks U disebut eigenface.
Eigenface adalah pola utama wajah yang diperoleh dari seluruh dataset wajah.

### PROJECTION KE RUANG EIGENFACE
Rumus: 
$$\omega = U^Tx $$

Projection digunakan untuk mengubah wajah dari ruang pixel menjadi ruang pola eigenface.

Rumus di atas akan menghasilkan matriks seperti berikut:
$$
\omega=
\begin{bmatrix}
w_1\\
w_2\\
w_3
\end{bmatrix}
$$


$w_1$ = Kekuatan pola 1
$w_2$ = Kekuatan pola 2
$w_3$ = Kekuatan pola 3


Matriks diatas merupakan contoh matriks dari hasil projection ke ruang eigenface dan matriks itu adalah contoh dari 1 dataset atau gambar yang di projection dan berarti matriks keseluruhan dataset akan berukuran n x m, n adalah jumlah pola atau eigenface yang di pakai karena pengambilan eigenface bisa mengambil semua pola atau hanya pola pola yang dominan dan m adalah jumla dataset yang ada.


### FACE RECOGNITION

Setelah memproses semua dataset yang ada dengan mengubah ke matriks dan melakukan beberpa perhitungan maka setelah selesai bisa mencoba menguji data baru ke data yang sudah ada apakah data baru ada kemiripan terhadao data yang sudah ada atau sudah di analisa.

Data baru yang ingin di coba akan di proses dulu seperti proses sebelumnya dan akan menghasilkan matriks yang sudah di projection ke ruang pola U yang sudah ada sebelumnya .

Rumus:
$$
\omega_q = U^T x_q
$$

Rumus dia atas menguji data baru terhadap data lama yang ada ${U^T}$ adalah matriks U yang sudah di tranpose dan matriks $x_q$ adalah matrik data baru.

Setelah mendapatkan matriks nya, kita bisa mulai mencari matriks mana yang memiliki kemiripan terhadap matriks data baru.

Rumus:
$$d = \|\omega_q - \omega_i\|$$

Di rumus di atas terdahap $\omega_q$ yaitu matriks data baru setelah itu ada matriks $\omega_i$ itu adalah matriks dataset yang sudah di analisa tadi, maka data baru akan di proses dengan semua pola pola yang ada di matriks U dan akan menghasilkan nilai distance data baru terhadap data pola di dataset yang ada.

Semakin kecil distance maka wajah semakin mirip.




