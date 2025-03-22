---
title: Determinan Matriks

---

## Determinan Matriks
Determinan matriks adalah sebuah nilai skalar yang dihitung dari elemen-elemen suatu matriks persegi (matriks dengan jumlah baris dan kolom yang sama). Determinan digunakan dalam berbagai aplikasi matematika, seperti dalam mencari invers matriks, menyelesaikan sistem persamaan linear, dan menentukan apakah suatu matriks memiliki solusi unik.
Determinan matriks A ditulis sebagai $Det(A)$ atau $[A]$

Jika kita memiliki matriks A berukuran 2×2:

$A = \begin{bmatrix}  
a & b \\
c & d  
\end{bmatrix}$

Maka rumus determinannya adalah:

$\text{det}(A) = (a \times d) - (b \times c)$

**Contoh Perhitungan**

$A = \begin{bmatrix}  
1 & 2 \\
3 & 4  
\end{bmatrix}$

$\text{det}(A) = (1 \times 4) - (2 \times 3) = 4 - 6 = -2$

### Metode Sarrus (Hanya untuk Matriks 3×3)
Metode ini hanya berlaku untuk matriks berukuran 3×3.
Langkah-langkah:
1. Tuliskan ulang dua kolom pertama di sebelah kanan matriks.
2. Jumlahkan hasil perkalian diagonal utama, lalu kurangi hasil perkalian diagonal sekunder.
Rumus

    $\text{det}(A) = (a_{11}a_{22}a_{33} + a_{12}a_{23}a_{31} + a_{13}a_{21}a_{32}) - (a_{13}a_{22}a_{31} + a_{11}a_{23}a_{32} + a_{12}a_{21}a_{33})$

    **Contoh**
    
    $A = \begin{bmatrix} 
1 & 2 & 3 \\ 
4 & 5 & 6 \\ 
7 & 8 & 9 
\end{bmatrix}$

    Menggunakan metode Sarrus:
    
    $det(𝐴 )=(1⋅5⋅9+2⋅6⋅7+3⋅4⋅8)−(3⋅5⋅7+1⋅6⋅8+2⋅4⋅9)$
    
    $det(𝐴)= (45+84+96)−(105+48+72)=225−225=0$

### Sifat-Sifat Determinan
**Sifat Penting Determinan**
1. **Determinan Matriks Identitas:**
    det(𝐼)=1, di mana 𝐼 adalah matriks identitas.
1. **Baris atau Kolom Nol:**
    Jika ada baris atau kolom yang semuanya nol, maka det(𝐴)=0.
1. **Pertukaran Baris/Kolom:**
Jika dua baris atau kolom dipertukarkan, determinan berubah tanda.
1. **Kelipatan Baris/Kolom:**
Jika satu baris atau kolom dikalikan dengan skalar 𝑘, maka determinan menjadi 𝑘⋅det(𝐴).
1. **Matriks Singular:**
Jika det(𝐴)=0, maka matriks 𝐴 disebut singular (tidak memiliki invers).

**Mengapa Determinan Penting?**
* Digunakan untuk menentukan apakah suatu matriks memiliki invers $(det(𝐴)≠0)$.
* Digunakan dalam perhitungan invers matriks melalui rumus:

    $A^{-1} = \frac{1}{\det(A)} \cdot \text{adj}(A)$


### Minor Matriks
Minor dari suatu elemen $A_{ij}$ dalam matriks adalah determinan dari submatriks yang diperoleh dengan menghapus **baris ke-$i$ dan kolom ke-$j$** dari matriks asal.

Contoh Perhitungan Minor Matriks: Misalkan kita memiliki matriks $A$ berukuran 3×3:

$A = \begin{bmatrix}  
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9  
\end{bmatrix}$

Jika kita ingin mencari **Minor** $M_{11}$ (Minor dari elemen $A_{11}$ yaitu angka 1), maka **kita hapus baris pertama dan kolom pertama**, sehingga diperoleh submatriks:

$M_{11} = \begin{bmatrix}  
5 & 6 \\
8 & 9  
\end{bmatrix}$

Determinan dari submatriks ini adalah:

$\text{det}(M_{11}) = (5 \times 9) - (6 \times 8) = 45 - 48 = -3$

Jadi, Minor $M_{11} = -3$

### Cofaktor Matriks
Cofaktor dari elemen $A_{ij}$ Adalah **minor** $M_{ij}$ **dikalikan dengan tanda** $(-1)^{i+j}$

$C_{ij} = (-1)^{i+j} \times M_{ij}$

**Contoh Perhitungan Cofaktor Matriks:** Dari contoh sebelumnya, kita sudah menghitung **Minor** $M_{11} = -3.$

Sekarang, kita cari **Cofaktor** $C_{11}$

$C_{11} = (-1)^{1+1} \times (-3) = (1) \times (-3) = -3$

Sekarang, coba kita cari **Cofaktor** $C_{12}$ (elemen di baris ke-1, kolom ke-2, yaitu 2):
1. Hapus baris pertama dan kolom kedua, diperoleh submatriks:

    $M_{12} = \begin{bmatrix}  
4 & 6 \\
7 & 9  
\end{bmatrix}$

2. Hitung determinan:

    $\text{det}(M_{12}) = (4 \times 9) - (6 \times 7) = 36 - 42 = -6$
3. Hitung Cofaktor:

    $C_{12} = (-1)^{1+2} \times (-6) = (-1) \times (-6) = 6$
    
    Jadi, **Cofaktor** $C_{12}= 6$
###  Mencari Determinan dengan konsep Minor dan Confactor matrik. Beri contoh matrik 3x3 4x4 dan 5x5
1. **Determinan Matriks 3×3**

    $A = \begin{bmatrix}  
2 & 3 & 1\\
4 & 5 & 6\\ 
7 & 8 & 9
\end{bmatrix}$

    Rumus ekspansi kofaktor pada baris pertama:

    $\det(A) = a_{11}C_{11} + a_{12}C_{12} + a_{13}C_{13}$
$= 2C_{11} - 3C_{12} + 1C_{13}$

    Menghitung Minor dan Kofaktor:

    $M_{11} =
\begin{vmatrix} 5 & 6 \\ 8 & 9 \end{vmatrix}
= (5 \times 9 - 6 \times 8) = 45 - 48 = -3$

    $C_{11} = (-1)^{1+1} M_{11} = (-1)^2 (-3) = -3$

    $M_{12} =\begin{vmatrix} 4 & 6 \\ 7 & 9 \end{vmatrix}
= (4 \times 9 - 6 \times 7) = 36 - 42 = -6$

    $C_{12} = (-1)^{1+2} M_{12} = (-1)^3 (-6) = 6$

    $M_{13} = \begin{vmatrix} 4 & 5 \\ 7 & 8 \end{vmatrix}= (4 \times 8 - 5 \times 7) = 32 - 35 = -3$

    $C_{13} = (-1)^{1+3} M_{13} = (-1)^4 (-3) = -3$

    Menghitung Determinan:

    $\det(A) = (2 \times -3) + (-3 \times 6) + (1 \times -3)$

    $= -6 - 18 - 3 = \mathbf{-27}$

2. **Determinan Matriks 4×4**

    $B =
\begin{bmatrix} 
1 & 2 & 3 & 4 \\ 
5 & 6 & 7 & 8 \\ 
9 & 10 & 11 & 12 \\ 
13 & 14 & 15 & 16 
\end{bmatrix}$

    Rumus ekspansi kofaktor pada baris pertama:

    $\det(B) = 1C_{11} - 2C_{12} + 3C_{13} - 4C_{14}$

    * **Langkah 1: Hitung Minor dan Kofaktor**

        * Hitung $C_{11}$ (Minor dari elemen $B_{11} = 1)

            $M_{11} =
\begin{vmatrix} 
6 & 7 & 8 \\ 
10 & 11 & 12 \\ 
14 & 15 & 16 
\end{vmatrix}$

            Gunakan ekspansi kofaktor kembali untuk menentukan determinan $M_{11}$ dengan cara yang sama seperti contoh matriks 3×3.

            $M_{11} = (6 \times (11 \times 16 - 12 \times 15)) - (7 \times (10 \times 16 - 12 \times 14)) + (8 \times (10 \times 15 - 11 \times 14))$
    
            Hitung determinan matriks 3×3 dengan ekspansi kofaktor pada baris pertama:
    
            $\det(M_{11}) = 6 
\begin{vmatrix} 
11 & 12 \\ 
15 & 16 
\end{vmatrix}$

            $- 7 
\begin{vmatrix} 
10 & 12 \\ 
14 & 16 
\end{vmatrix}$

            $+ 8 
\begin{vmatrix} 
10 & 11 \\ 
14 & 15 
\end{vmatrix}$

            $= 6(11 \times 16 - 12 \times 15) - 7(10 \times 16 - 12 \times 14) + 8(10 \times 15 - 11 \times 14)$
            $= 6(176 - 180) - 7(160 - 168) + 8(150 - 154)$
            $= 6(-4) - 7(-8) + 8(-4)$
            $= -24 + 56 - 32 = 0$

            Karena $M_{11} = 0,$ maka $C_{11} = (-1)^{1+1} (0) = 0.$
    
        * Hitung $C_{12}$ (Minor dari elemen $B_{12} = 2)$

            $M_{12} =
\begin{vmatrix}
5 & 7 & 8 \\
9 & 11 & 12 \\
13 & 15 & 16
\end{vmatrix}$
    
            Hitung determinan matriks 3×3 dengan cara yang sama:
    
            $\det(M_{12}) = 5(11 \times 16 - 12 \times 15) - 7(9 \times 16 - 12 \times 13) + 8(9 \times 15 - 11 \times 13)$
            $= 5(-4) - 7(-12) + 8(-6)$
            $= -20 + 84 - 48 = 16$
            $C_{12} = (-1)^{1+2} (16) = -16$
    
        * Hitung $C_{13}$
    
            $M_{13} =
\begin{vmatrix}
5 & 6 & 8 \\
9 & 10 & 12 \\
13 & 14 & 16
\end{vmatrix}$

            $\det(M_{13}) = 5(10 \times 16 - 12 \times 14) - 6(9 \times 16 - 12 \times 13) + 8(9 \times 14 - 10 \times 13)$
            $= 5(-8) - 6(-12) + 8(-4)$
            $= -40 + 72 - 32 = 0$
            $= -40 + 72 - 32 = 0$
    
        * Hitung $C_{14}$
    
            $M_{14} =
\begin{vmatrix}
5 & 6 & 7 \\
9 & 10 & 11 \\
13 & 14 & 15
\end{vmatrix}$

            $\det(M_{14}) = 5(10 \times 15 - 11 \times 14) - 6(9 \times 15 - 11 \times 13) + 7(9 \times 14 - 10 \times 13)$ 
            $= 5(-4) - 6(-12) + 7(-4)$
            $= -20 + 72 - 28 = 24$ 
            $C_{14} = (-1)^{1+4}(24) = 24$
    
    * **Langkah 2: Hitung Determinan**
    
        $\det(B) = 1(0) - 2(-16) + 3(0) - 4(24)$
        $= 0 + 32 + 0 - 96$
        $= -64$
    
3. **Determinan Matriks 5×5**
    Matriks:
    
    $C =
\begin{bmatrix} 
2 & 3 & 1 & 4 & 5 \\ 
6 & 7 & 8 & 9 & 10 \\ 
11 & 12 & 13 & 14 & 15 \\ 
16 & 17 & 18 & 19 & 20 \\ 
21 & 22 & 23 & 24 & 25
\end{bmatrix}$

    Gunakan ekspansi kofaktor pada baris pertama:

    $\det(C) = 2C_{11} - 3C_{12} + 1C_{13} - 4C_{14} + 5C_{15}$
    
    Untuk menghitung setiap $C_{1j}$, kita harus menentukan $M_{1j}$, yang merupakan determinan matriks 4×4. Prosesnya sama seperti sebelumnya, menggunakan ekspansi kofaktor lagi.
    
    $M_{11} =
\begin{vmatrix} 
7 & 8 & 9 & 10 \\ 
12 & 13 & 14 & 15 \\ 
17 & 18 & 19 & 20 \\ 
22 & 23 & 24 & 25 
\end{vmatrix}$
    
    Gunakan ekspansi kofaktor lagi untuk menghitung determinan matriks 4×4, lalu gunakan hasil tersebut untuk mendapatkan det(C).