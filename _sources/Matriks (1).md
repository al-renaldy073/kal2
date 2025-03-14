---
title: Matriks

---

# Matriks
## Pendahulaun
Matriks adalah susunan angka atau objek matematika lainnya yang disusun dalam bentuk baris dan kolom, dimana operasi seperti penjumlahan dan perkalian dapat didefinisikan. Umumnya, matriks di atas medan 
$F$ berisi elemen-elemen dari $F$. Sebagian besar artikel ini berfokus pada matriks riil dan kompleks, yaitu matriks yang masing-masing elemennya berupa bilangan riil atau bilangan kompleks. Jenis elemen matriks yang umum akan dibahas di bawah. Sebagai contoh, ini adalah sebuah matriks riil:

$\mathbf{A} =
\begin{bmatrix}
-1.3 & 0.6 \\
20.4 & 5.5 \\
9.7 & -6.2
\end{bmatrix}
.$

## Apa itu matriks
Matriks adalah **sekumpulan bilangan yang disusun berdasarkan baris dan kolom, serta ditempatkan di dalam tanda kurung.** Nah, tanda kurungnya ini bisa berupa kurung biasa “( )” atau kurung siku “[ ]”, ya. Suatu matriks diberi nama dengan huruf kapital, seperti A, B, C, dan seterusnya.

Oh iya, kamu tau kan bedanya baris dan kolom? Baris itu susunannya horizontal atau ke samping, sedangkan kolom susunannya vertikal atau dari atas ke bawah.

Misalnya nih, matriks di atas tadi, kita beri nama matriks A. Maka,

![Cuplikan layar 2025-03-05 203614](https://hackmd.io/_uploads/rJodQ0Siyg.png)


Penamaan baris dan kolom dibuat urut, ya. Jadi, baris ke-1 dimulai dari atas, urut ke bawah. Sementara itu, kolom ke-1 dimulai dari kiri ke kanan.

## Operasi Aritmetika Matriks
### 1. Penjumlahan Matrik
**Konsep penjumalahan matriks:**

Penjumlahan matriks adalah operasi yang dilakukan dengan menjumlahkan elemen-elemen yang bersesuaian pada dua matriks yang memiliki ukuran yang sama.Penjumlahan matriks dapat dilakukan jika jumlah baris dan kolomnya sama.

Terdapat dua buah matriks yaitu matriks A dan matriks B yang memiliki ukuran baris dan kolom yang sama, maka penjumlahan matriks A + B akan menghasilkan matriks C = A + B

Dimana elemen 
 pada matriks hasil penjumlahan C adalah hasil penjumlahan elemen - elemen yang bersesuai pada matriks A dan B.
 
 $c_{ij} = a_{ij} + b_{ij}$
 
**Contoh penjumlahan matriks:**

Misal ada 2 matriks A dan B:

$A :
\begin{bmatrix}
1 & 3 \\
2 & 4
\end{bmatrix}$

$B :
\begin{bmatrix}
2 & 6 \\
4 & 8
\end{bmatrix}$

penjumlahan A + B adalah:

$A + B =
\begin{bmatrix}
1 + 2 & 3 + 6 \\
2 + 4 & 4 + 8
\end{bmatrix}$

Jadi hasil penjumlahan matriks A + B =

$C :
\begin{bmatrix}
3 & 9 \\
6 & 12
\end{bmatrix}$

### 2. Perkalian Matriks

**Konsep perkalian matriks:**

Perkalian matriks adalah operasi yang dilakukan antara dua matriks untuk menghasilkan matriks baru. Tidak semua matriks dapat diperkalikan, untuk dapat melakukan perkalian, jumlah kolom pada matriks pertama harus sama dengan jumlah baris pada matriks kedua.

Secara matematis, jika kita memiliki dua matriks A dan B, maka perkalian matriks $A \times B$ akan menghasilkan matriks $C$. Dengan syarat:

* Matriks $A$ memiliki ukuran $M \times P$ (m baris, n kolom)
* Matriks $B$ memiliki ukuran $N \times P$ (n baris, p kolom)

Maka hasil perkalian $C$ akan memiliki ukuran $M \times P$

**Cara melakukan perkalian matriks**

$A =
\begin{bmatrix}
a_{11} & a_{12} & \cdots & a_{1n} \\
a_{21} & a_{22} & \cdots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{m1} & a_{m2} & \cdots & a_{mn}
\end{bmatrix}$

$B =
\begin{bmatrix}
b_{11} & b_{12} & \cdots & b_{1n} \\
b_{21} & b_{22} & \cdots & b_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
b_{m1} & b_{m2} & \cdots & b_{mn}
\end{bmatrix}$

Dari perkalian matriks di atas akan menghasilkan matriks $C$ dengan ukuran $M \times P$

$C =
\begin{bmatrix}
c_{11} & c_{12} & \cdots & c_{1p} \\
c_{21} & c_{22} & \cdots & c_{2p} \\
\vdots & \vdots & \ddots & \vdots \\
c_{m1} & c_{m2} & \cdots & c_{mp}
\end{bmatrix}$

Setiap elemen $C_{ij}$ (elemen pada baris ke-i dan kolom ke-j dari matriks hasil) dihitung dengan cara mengalikan elemen baris ke-i dari matriks $A$ dengan elemen kolom ke-j dari matriks $B$, lalu menjumlahkan hasil perkalian tersebut. Secara matematis:

$c_{ij} = a_{i1} b_{1j} + a_{i2} b_{2j} + \dots + a_{in} b_{nj}$

ini berarti untuk setiap elemen yang dihasilkan dalam perkalian, dengan cara mengambil elemen-elemen dari baris tertentu matriks $A$ kemudian dikalikan dengan elemen-elemen dari kolom tertentu pada matriks $B$ dan menjumlahkan hasil perkalian tersebut.

**contoh perkalian matriks**

misal memiliki 2 matriks sebagai berikut:

$A : 
\begin{bmatrix}
2 & 3 & 4 \\
1 & 3 & 5 \\
4 & 3 & 6
\end{bmatrix}$

$B :
\begin{bmatrix}
1 & 4 & 2 \\
3 & 7 & 2 \\
5 & 1 & 4
\end{bmatrix}$

untuk menghitung matriks hasil, $C = A \times B =$

$C =
\begin{bmatrix}
c_{11} & c_{12} & c_{13} \\
c_{21} & c_{22} & c_{23} \\
c_{31} & c_{32} & c_{33}
\end{bmatrix}$

Dengan elemen-elemen yang dihitung sebagai berikut:

$c_{11} = (2 \times 1) + (3 \times 3) + (4 \times 5) = 31$

$c_{12} = (2 \times 4) + (3 \times 7) + (4 \times 1) = 33$

$c_{13} = (2 \times 2) + (3 \times 2) + (4 \times 4) = 26$

$c_{21} = (1 \times 1) + (3 \times 3) + (5 \times 5) = 35$

$c_{22} = (1 \times 4) + (3 \times 7) + (5 \times 1) = 30$

$c_{23} = (1 \times 2) + (3 \times 2) + (5 \times 4) = 28$

$c_{31} = (4 \times 1) + (3 \times 3) + (6 \times 5) = 43$

$c_{32} = (4 \times 4) + (3 \times 7) + (6 \times 1) = 43$

$c_{33} = (4 \times 2) + (3 \times 2) + (6 \times 4) = 38$

maka hasil matriks C adalah:

$C =
\begin{bmatrix}
31 & 33 & 26 \\
35 & 30 & 28 \\
43 & 43 & 38
\end{bmatrix}$

### 3. Perkalian Skalar Matriks
**Konsep perkalian skalar matriks:**

Perkalian skalar matriks berati mengalikan semua elemen yang ada pada matriks dengan bilangan skalarnya. Operasi ini tetap mempertahankan dimensi matriks atau tidak merubah dimensi matriks.

**cara melakukan perkalian skalar matriks:**

Misal ada matriks berukuran $M \times N$:

$A =
\begin{bmatrix}
a_{11} & a_{12} & \cdots & a_{1n} \\
a_{21} & a_{22} & \cdots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{m1} & a_{m2} & \cdots & a_{mn}
\end{bmatrix}$

dengan skalar $k_1$, maka perkalian matriks skalar adalah $KA$:

$kA =
\begin{bmatrix}
k \cdot a_{11} & k \cdot a_{12} & \cdots & k \cdot a_{1n} \\
k \cdot a_{21} & k \cdot a_{22} & \cdots & k \cdot a_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
k \cdot a_{m1} & k \cdot a_{m2} & \cdots & k \cdot a_{mn}
\end{bmatrix}$
 
**contoh perkalian skalar matriks:**

Terdapat matriks:

$A :
\begin{bmatrix}
1 & 6 & 5 \\
2 & 7 & 4 \\
3 & 8 & 3
\end{bmatrix}$

dan skalar $K =2$, maka hasil perkalian skalar matriks:


$3A = 3x =
\begin{bmatrix}
1 & 6 & 5 \\
2 & 7 & 4 \\
3 & 8 & 3
\end{bmatrix} =
\begin{bmatrix}
3 & 18 & 15 \\
6 & 21 & 12 \\
9 & 24 & 9
\end{bmatrix}$
 
 
Jadi, semua elemen yang ada pada matriks $A$ dikalikan dengan skalar yaitu $3$, dan akan memperoleh matriks tersebut.

# implementasi python perka

### Ordo dan Elemen Matriks
Matriks memiliki ukuran. Ukuran matriks disebut ordo. Ordo matriks ini berdasarkan dari banyaknya baris dikali banyaknya kolom pada matriks. Jadi, kalo suatu matriks A memiliki m baris dan n kolom, maka matriks A tersebut berukuran (berordo) m x n. Supaya lebih sederhana, kita bisa menulisnya dengan $\textit{Amxn.}$

Nah, masing-masing bilangan yang terdapat di dalam matriks disebut **elemen matriks.** Elemen-elemen matriks juga ada notasinya sendiri, lho. Kalo matriks dinotasikan dengan huruf kapital, maka elemen-elemen matriks dinotasikan dengan huruf kecil dan diberi indeks yang menyatakan **letak baris dan kolomnya.**

Misalnya nih, pada matriks A di atas, jumlah barisnya kan ada 5 dan jumlah kolomnya juga ada 5, maka ordonya adalah 5 x 5, atau bisa kita tulis A5×5. Lalu, untuk elemen-elemen matriks A bisa dinotasikan dengan aij, yang menyatakan elemen matriks A pada baris ke-i dan kolom ke-j.

Supaya tidak bingung simak contoh di bawah ini.
![Cuplikan layar 2025-03-05 203806](https://hackmd.io/_uploads/ry7q40Hi1x.png)

Kita ambil contoh $\textit{a11, a12}$ dan $\textit{a53}$, seperti pada gambar.

*  $\textit{a11.}$ menyatakan elemen matriks A pada baris ke-1 kolom ke-1, nilainya adalah 0.
* $\textit{a12.}$ menyatakan elemen matriks A pada baris ke-1 kolom ke-2, nilainya adalah 1.
* $\textit{a53.}$ menyatakan elemen matriks A pada baris ke-5 kolom ke-4, nilainya adalah 2.

### Jenis-jenis Materiks
Selain punya ukuran (ordo), matriks juga terbagi menjadi beberapa bentuk yang mempunyai sifat khusus. Nah, beberapa jenis matriks khusus yang perlu kamu ketahui di antaranya sebagai berikut:

1. **Matriks Baris**
Matriks baris adalah suatu matriks yang **terdiri dari satu baris aja**. Contoh matriks baris:

    $A = \begin{bmatrix} 0 & 3 & 4 \end{bmatrix}$
    $P = \begin{bmatrix} -2 & 5 & 5 & 4 \end{bmatrix}$
    $Q = \begin{bmatrix} 3 & 2 & -1 & 6 & 1 \end{bmatrix}$

    Kalo kita lihat, matriks A, matriks P, dan matriks Q, semuanya terdiri dari satu baris dan beberapa kolom. Untuk masing-masing ordonya, berarti $A_{1 \times 3}$, $A_{1 \times 4}$, $A_{1 \times 5}$.

2. **Matriks Kolom**
Kebalikannya dari matriks baris, matriks kolom adalah suatu matriks yang **terdiri dari satu kolom aja**. Contoh matriks kolom:

    $R = \begin{bmatrix} 1 \\ 2 \end{bmatrix}, \quad
S = \begin{bmatrix} 3 \\ 4 \\ -1 \end{bmatrix}, \quad
T = \begin{bmatrix} 5 \\ -7 \\ 2 \\ 3 \end{bmatrix}$

    Matriks R, matriks S, dan matriks T sama-sama terdiri dari satu kolom dan beberapa baris. Oleh karena itu, ordo matriksnya adalah  $A_{2 \times 1}$, $A_{3 \times 1}$, $A_{4 \times 1}$.

3. **Matriks Persegi**
Matriks persegi adalah suatu matriks yang **memiliki jumlah baris dan kolom sama.** Itu tandanya, m = n. Karena jumlah baris dan kolomnya sama, maka ordo matriksnya bisa kita tulis menjadi n x n, atau matriks ordo n.

    Pada matriks persegi, terdapat **diagonal utama**, yaitu elemen-elemen matriks yang letak barisnya sama dengan letak kolomnya. Selain diagonal utama, ada juga diagonal samping atau diagonal kedua. Kalo kita tarik garis di sepanjang diagonal utama matriks, maka diagonal samping ini berada di arah sebaliknya. Contoh matriks persegi:

    ![Cuplikan layar 2025-03-05 211438](https://hackmd.io/_uploads/SypvnCSi1g.png)
    
    ![Cuplikan layar 2025-03-05 211517](https://hackmd.io/_uploads/Hkz92ABsJe.png)

    berdasarkan contoh di atas, matriks A memiliki jumlah baris dan kolom yang sama karena matriks ini merupakan matriks persegi, yaitu sebanyak 2. Maka, matriks ini merupakan matriks berordo 2. Kemudian, elemen-elemen pada diagonal utamanya adalah 8 dan 7.
    
4. **Matriks Diagonal**
Matriks diagonal adalah **matriks persegi yang elemen-elemen selain diagonal utamanya bernilai nol.** Contoh matriks diagonal:

    ![Cuplikan layar 2025-03-05 211959](https://hackmd.io/_uploads/SkG66Criyg.png)
    
    ![Cuplikan layar 2025-03-05 212010](https://hackmd.io/_uploads/BkzT6Rri1g.png)
    
    ![Cuplikan layar 2025-03-05 212023](https://hackmd.io/_uploads/HkMaaRSoyg.png)

    Elemen-elemen pada diagonal utama matriks Q adalah 3, 8, dan 5. Nah, di luar diagonal utama, semua elemennya bernilai 0. Misalnya, elemen $Q_{2 1}$ adalah 0, lalu elemen $Q_{2 1}$ juga 0.
    
5. **Matriks Identitas**
Matriks identitas adalah **matriks persegi yang semua elemen pada diagonal utamanya bernilai satu, sedangkan elemen lainnya bernilai nol.** Umumnya, matriks identitas dinotasikan dengan I disertai dengan ordonya. Contoh matriks identitas:


    $I_2 =
\begin{bmatrix}
1 & 0 \\
0 & 1
\end{bmatrix} \quad
I_3 =
\begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{bmatrix} \quad
I_4 =
\begin{bmatrix}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1
\end{bmatrix}$

6. **Matriks Nol**
Sesuai namanya, matriks nol adalah **matriks yang semua elemennya bernilai nol.** Matriks nol biasanya dinotasikan dengan huruf O disertai ordonya. Contoh matriks nol:

    $O_{2 \times 1} =
\begin{bmatrix}
0  \\
0 
\end{bmatrix} \quad
O_{3 \times 2} =
\begin{bmatrix}
0 & 0  \\
0 & 0  \\
0 & 0 
\end{bmatrix} \quad
O_{2 \times 3} =
\begin{bmatrix}
0 & 0 & 0 \\
0 & 0 & 0
\end{bmatrix}$

### Transpose Matriks
Transpose matriks **adalah suatu matriks yang diperoleh dari hasil pertukaran antara elemen baris dan kolomnya.** Jadi, elemen-elemen pada baris akan kita tukar menjadi elemen-elemen pada kolom, atau sebaliknya. 

Misalnya, kita akan mentranspose matriks A dan B. Maka, matriks transposenya bisa dinotasikan dengan $A^t$ dan $B^t$.

![Cuplikan layar 2025-03-05 214817](https://hackmd.io/_uploads/S1ur4yUikg.png)

Nah, kalo kamu perhatikan kotak warna-warni pada matriks di atas, kamu pasti paham nih dengan polanya. Aku kasih contoh, ya. Coba kamu lihat matriks A dan $A^t$! Elemen-elemen baris ke-1 matriks $A^t$ (yang di kotak merah), itu merupakan pertukaran dari elemen-elemen kolom ke-1 matriks A. Begitu juga dengan elemen-elemen baris ke-2 matriks $A^t$ (yang di kotak biru), merupakan pertukaran dari elemen-elemen kolom ke-2 matriks A.

contoh soal di bawah ini. seperti yang di jalankan sebelumnya.

![Cuplikan layar 2025-03-05 215519](https://hackmd.io/_uploads/S1Ak8yUsJg.png)

 Sebetulnya, matriks itu materi yang mudah. Matriks bisa digunakan untuk menyelesaikan masalah sistem persamaan yang memiliki lebih dari dua variabel dengan cepat. Dibandingkan harus menggunakan metode substitusi atau eliminasi. Jadi, penting banget untuk memahami materi ini.
 
## sistem persamaan liear dengan menggunakan invers menggunakan obe (operasi baris elementer)
$\begin{align*}  
-7x_1 - 6x_2 - 12x_3 &= -33 \\
5x_1 + 5x_2 + 7x_3 &= 24 \\
x_1 + 4x_3 &= 5  
\end{align*}$

$A = \begin{bmatrix}  
-7 & -6 & -12 \\
5 & 5 & 7 \\
1 & 0 & 4  
\end{bmatrix}$

$x = \begin{bmatrix}  
x_1 \\
x_2 \\
x_3  
\end{bmatrix}$

$b = \begin{bmatrix}  
-33 \\
24 \\
5  
\end{bmatrix}$

Pertama Gabungkan matriks $\ [A]$ dengan matriks identitas $\ [I]$ untuk membentuk matriks augmented$\ [A | I]:$

$[A | I] = \begin{bmatrix}  
-7 & -6 & -12 & | & 1 & 0 & 0 \\
5 & 5 & 7 & | & 0 & 1 & 0 \\
1 & 0 & 4 & | & 0 & 0 & 1  
\end{bmatrix}$

pakai OBE jadi yang bagian kanan menjadi $(A^{-1}).$

Lalu kita Ubah Elemen (1,1) Menjadi 1 jadi Baris pertama dibagi dengan (-7):

$\begin{bmatrix}  
1 & \frac{6}{7} & \frac{12}{7} & \big| & -\frac{1}{7} & 0 & 0 \\
5 & 5 & 7 & \big| & 0 & 1 & 0 \\
1 & 0 & 4 & \big| & 0 & 0 & 1  
\end{bmatrix}$

Lalu Buat Elemen Kolom Pertama (2,1) dan (3,1) Menjadi 0

* Baris kedua: $( R_2 \to R_2 - 5R_1 )$
* Baris Ketiga: $( R_3 \to R_3 - R_1 )$

Hasilnya:

$\begin{bmatrix}  
1 & \frac{6}{7} & \frac{12}{7} & \big| & -\frac{1}{7} & 0 & 0 \\
0 & -\frac{1}{7} & -\frac{5}{7} & \big| & 1 & 0 & 0 \\
0 & -\frac{6}{7} & \frac{16}{7} & \big| & \frac{1}{7} & 0 & 1  
\end{bmatrix}$

Ubah Elemen (2,2) Menjadi 1 Kita bagi baris kedua dengan $( \frac{5}{7})$:

$\begin{bmatrix}  
1 & \frac{6}{7} & \frac{12}{7} & \big| & -\frac{1}{7} & 0 & 0 \\
0 & 1 & -\frac{1}{5} & \big| & 1 & \frac{7}{5} & 0 \\
0 & -\frac{6}{7} & \frac{16}{7} & \big| & \frac{1}{7} & 0 & 1  
\end{bmatrix}$

Setelah Itu Buat Elemen Kolom Kedua (1,2) dan (3,2) Menjadi 0

* Baris Pertama: $( R_1 \to R_1 - \frac{6}{7}R_2)$
* Baris Ketiga: $( R_3 \to R_3 + \frac{6}{7} R_2)$

Hasilnya:
$\begin{bmatrix}  
1 & 0 & \frac{18}{35} & \big| & -\frac{13}{35} & -\frac{42}{35} & 0 \\
0 & 1 & -\frac{1}{5} & \big| & 1 & \frac{7}{5} & 0 \\
0 & 0 & \frac{22}{35} & \big| & \frac{13}{22} & \frac{42}{22} & 1  
\end{bmatrix}$

Ubah Elemen (3,3) Menjadi 1 Kita bagi baris ketiga dengan $\left( \frac{22}{35} \right)$:

$\begin{bmatrix}  
1 & 0 & \frac{18}{35} & \big| & -\frac{13}{35} & -\frac{42}{35} & 0 \\
0 & 1 & -\frac{1}{5} & \big| & 1 & \frac{7}{5} & 0 \\
0 & 0 & 1 & \big| & \frac{13}{22} & \frac{42}{22} & \frac{35}{22}  
\end{bmatrix}$

Buat Elemen Kolom Ketiga (1,3) dan (2,3) Menjadi 0

* Baris Pertama: $( R_1 \to R_1 - \frac{18}{35}R_3)$
* Baris Kedua: $( R_2 \to R_2 + \frac{1}{5}R_3)$

Hasilnya:  

$\begin{bmatrix}  
1 & 0 & 0 & \big| & -3 & 5 & 2 \\
0 & 1 & 0 & \big| & 2 & 1 & 1 \\
0 & 0 & 1 & \big| & \frac{13}{22} & \frac{21}{11} & \frac{35}{22}  
\end{bmatrix}$  

Bagian kanan dari matriks ini adalah $( A^{-1} )$.  

Hitung $(x = A^{-1}b)$. Kita kalikan  $(A^{-1})$ dengan $(b)$:

$x = A^{-1}b = \begin{bmatrix}  
-3 \\
5 \\
2  
\end{bmatrix}$

Sehingga diperoleh:  
$x_1 = -3, \quad x_2 = 5, \quad x_3 = 2$

## Refrensi
https://id.wikipedia.org/wiki/Matriks_(matematika)

https://www.ruangguru.com/blog/mengenal-matriks-dalam-matematika-pengertian-jenis-dan-transpose
