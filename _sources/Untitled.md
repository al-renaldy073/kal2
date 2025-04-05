---
title: Untitled

---

###  Mencari Determinan dengan konsep Minor dan Confactor matrik. Beri contoh matrik 3x3 4x4 dan 

1. **Determinan Matrik 3×3**

    $A = \begin{bmatrix}  
1 & 2 & 3\\
4 & 5 & 6\\ 
7 & 8 & 9
\end{bmatrix}$

    **Menentukan Minor dan Cofaktor**
    
     **Langkah 1: Pilih Baris atau Kolom untuk Ekspansi**
Kita akan melakukan ekspansi sepanjang baris pertama.
     **Langkah 2: Hitung Minor dan Kofaktor**
     Minor $M_{ij}$ adalah determinan dari submatriks yang diperoleh dengan menghilangkan baris ke-$i$ dan kolom ke-$j$. Kofaktor $C_{ij}$ didefinisikan sebagai $C_{ij} = (-1)^{i+j} \cdot M_{ij}$.
    1. Elemen $a_{11}$ = $1$
        * Minor $M_{11} = \left| \begin{array}{cc}  
5 & 6 \\
8 & 9   
\end{array} \right| = (5 \cdot 9) - (6 \cdot 8) = 45 - 48 = -3$ 
        * Konfaktor $C_{11} = (-1)^{1+1} \cdot M_{11} = 1 \cdot (-3) = -3$
    1. Elemen $a_{12}$ = $2$
        * Minor $M_{12} =  \begin{vmatrix} 4 & 6 \\ 7 & 9 \end{vmatrix} = (4 \cdot 9) - (6 \cdot 7) = 36 - 42 = -6$ 
        * Konfaktor $C_{12} = (-1)^{1+2} \cdot M_{12} = -1 \cdot (-6) = 6$
    1. Elemen $a_{13}$ = $3$
        * Minor $M_{13} = \begin{vmatrix} 4 & 5 \\ 7 & 8 \end{vmatrix} = (4 \cdot 8) - (5 \cdot 7) = 32 - 35 = -3$ 
        * Konfaktor $C_{13} = (-1)^{1+3} \cdot M_{13} = 1 \cdot (-3) = -3$
        
    **Langkah 3: Hitung Determinan**
Determinan dihitung dengan menjumlahkan hasil kali elemen-elemen baris pertama dengan kofaktor masing-masing:

    $\det(A) = a_{11} \cdot C_{11} + a_{12} \cdot C_{12} + a_{13} \cdot C_{13}$
$\det(A) = 1 \cdot (-3) + 2 \cdot 6 + 3 \cdot (-3) = -3 + 12 - 9 = 0$ 

    **Hasil**
Determinan dari matriks $A$ adalah: $0$

1. **Determinan Matrik 4×4**
   
   $A =
\begin{bmatrix} 
1 & 2 & 3 & 4 \\ 
5 & 6 & 7 & 8 \\ 
9 & 10 & 11 & 12 \\ 
13 & 14 & 15 & 16 
\end{bmatrix}$

    **Langkah 1: Pilih Baris/Kolom untuk Ekspansi**
Kita akan melakukan ekspansi sepanjang baris pertama karena mengandung angka yang relatif kecil, sehingga memudahkan perhitungan.

    Baris pertama: $[1,2,3,4]$.
    
    Rumus determinan:
    
    $\text{det}(A) = \sum_{j=1}^{4} (-1)^{1+j} \cdot a_{1j} \cdot M_{1j}$
    
    di mana $M_{ij}$ adalah minor dari elemen  $a_{ij}$

    **Langkah 2: Hitung Setiap Kofaktor untuk Baris Pertama**
    1. Elemen $a_{11}$ = $1:$
        * Kofaktor: $C_{11} = (-1)^{1+1} \cdot 1 \cdot M_{11} = 1 \cdot M_{11}$
        * Minor $M_{11}$:
    Hilangkan baris 1 dan kolom 1:
    
            $M_{11} = \begin{vmatrix}  
6 & 7 & 8 \\
10 & 11 & 12 \\
14 & 15 & 16  
\end{vmatrix}$
    
            Hitung determinan $3×3$ ini dengan ekspansi:
        
            $M_{11} = 6 \cdot \begin{vmatrix}  
11 & 12 \\
15 & 16  
\end{vmatrix} - 7 \cdot \begin{vmatrix}  
10 & 12 \\
14 & 16  
\end{vmatrix} + 8 \cdot \begin{vmatrix}  
10 & 11 \\
14 & 15  
\end{vmatrix}$
        
            $= 6 \cdot (11 \cdot 16 - 12 \cdot 15) - 7 \cdot (10 \cdot 16 - 12 \cdot 14) + 8 \cdot (10 \cdot 15 - 11 \cdot 14)$
$= 6 \cdot (176 - 180) - 7 \cdot (160 - 168) + 8 \cdot (150 - 154)$
$= 6 \cdot (-4) - 7 \cdot (-8) + 8 \cdot (-4) = -24 + 56 - 32 = 0$

    1. Elemen $a_{12}$ = $2:$
        * Kofaktor: $C_{12} = (-1)^{1+2} \cdot 2 \cdot M_{12} = -2 \cdot M_{12}$
        * Minor $M_{12}$:
        Hilangkan baris 1 dan kolom 2:
        
            $M_{12} =  
\begin{vmatrix}  
5 & 7 & 8 \\
9 & 11 & 12 \\
13 & 15 & 16  
\end{vmatrix}$

            Hitung dengan cara serupa:
                        $M_{12} = 5 \cdot \begin{vmatrix}  
11 & 12 \\
15 & 16  
\end{vmatrix} - 7 \cdot \begin{vmatrix}  
9 & 12 \\
13 & 16  
\end{vmatrix} + 8 \cdot \begin{vmatrix}  
9 & 11 \\
13 & 15  
\end{vmatrix}$


            $= 5 \cdot (-4) - 7 \cdot (-12) + 8 \cdot (-8) = -20 + 84 - 64 = 0$
        
    1. Elemen $a_{13}$ = $3:$
        * Kofaktor: $C_{13} = (-1)^{1+3} \cdot 3 \cdot M_{13} = 3 \cdot M_{13}$
        * Minor $M_{13}$:
        Hilangkan baris 1 dan kolom 3:
        
            $M_{13} =  
\begin{vmatrix}  
5 & 6 & 8 \\
9 & 10 & 12 \\
13 & 14 & 16  
\end{vmatrix}$

            Hasil perhitungan:
                              
            $M_{13} = 5 \cdot \begin{vmatrix}  
10 & 12 \\
14 & 16  
\end{vmatrix} - 6 \cdot \begin{vmatrix}  
9 & 12 \\
13 & 16  
\end{vmatrix} + 8 \cdot \begin{vmatrix}  
9 & 10 \\
13 & 14  
\end{vmatrix}$

            $= 5 \cdot (-8) - 6 \cdot (-12) + 8 \cdot (-4) = -40 + 72 - 32 = 0$
        
    1. Elemen $a_{14}$ = $1:$
        * Kofaktor: $C_{14} = (-1)^{1+4} \cdot 4 \cdot M_{14} = -4 \cdot M_{14}$
        * Minor $M_{14}$:
        
            $M_{14} =  
\begin{vmatrix}  
5 & 6 & 7 \\
9 & 10 & 11 \\
13 & 14 & 15  
\end{vmatrix}$

            Hasil perhitungan:
            
            $M_{14} = 5 \cdot \begin{vmatrix}  
10 & 11 \\
14 & 15  
\end{vmatrix} - 6 \cdot \begin{vmatrix}  
9 & 11 \\
13 & 15  
\end{vmatrix} + 7 \cdot \begin{vmatrix}  
9 & 10 \\
13 & 14  
\end{vmatrix}$

            $= 5 \cdot (-4) - 6 \cdot (-8) + 7 \cdot (-4) = -20 + 48 - 28 = 0$

    **Langkah 3: Gabungkan Hasil Kofaktor**
    $\det(A) = C_{11} + C_{12} + C_{13} + C_{14} = 1 \cdot 0 + (-2) \cdot 0 + 3 \cdot 0 + (-4) \cdot 0 = 0$
    
    **Verifikasi dengan Sifat Matriks:**
    * Baris/kolom linear dependen:
    Baris ke-4 $([13,14,15,16])$ adalah hasil dari baris ke-3 $([9,10,11,12])$ ditambah baris ke-1 $([1,2,3,4])$ dikali 4
    Artinya, matriks ini **singular** (tidak memiliki invers), sehingga determinannya **harus 0**.
    
    Kesimpulan:
Determinan matriks $A$ adalah $0$.
Hasil ini konsisten dengan sifat matriks yang memiliki baris/kolom saling bergantung linear.

3. **Determinan Matrik 5×5**

      $A =
\begin{bmatrix} 
2 & -3 & 1 & -5 & 4 \\ 
1 & 4 & 2 & 3 & 5 \\ 
3 & 1 & 5 & 2 & 4 \\ 
5 & 2 & 4 & 3 & 1 \\ 
4 & 5 & 3 & 2 & 1
\end{bmatrix}$

    * Minor $M_{11}$
    Hapus baris ke-1 dan kolom ke-1 dari $A$, diperoleh submatriks:
    
        $M_{11} = \begin{bmatrix}  
4 & 2 & 5\\
1 & 5 & 2\\ 
2 & 4 & 3\\ 
5 & 3 & 1
\end{bmatrix}$

        Hitung determinan $M_{11}$ dengan ekspansi baris pertama:

        $det(M_{11}) = 4 \cdot \begin{vmatrix}  
1 & 5 & 2 \\
2 & 4 & 3 \\
5 & 3 & 1 
\end{vmatrix} - 2 \cdot \begin{vmatrix}  
1 & 5 & 2 \\
2 & 4 & 3 \\
5 & 3 & 2  
\end{vmatrix} + 5 \cdot \begin{vmatrix}  
1 & 4 & 1 \\
2 & 4 & 1 \\
5 & 2 & 4 
\end{vmatrix}$

         Hitung masing-masing determinan matriks $3x3$ dengan metode Sarrus.
         
         Submatriks $M_{11}$ (setelah menghapus baris pertama dan kolom pertama dari $A$):
         
        $M_{11} = \begin{bmatrix}  
5 & 2 & 4\\
4 & 1 & 3\\ 
3 & 2 & 1
\end{bmatrix}$

        Menggunakan metode Sarrus:
        $\det(M_{11}) = (5 \times 1 \times 1) + (2 \times 3 \times 4) + (4 \times 4 \times 2) - [(3 \times 1 \times 4) + (2 \times 4 \times 5) + (1 \times 2 \times 3)]$
        
        $= (5 + 24 + 32) - (12 + 40 + 6)$
        
        $= 61 - 58 = 3$
        
        
        
    * Minor $M_{12}$
    Hapus baris ke-1 dan kolom ke-2 dari A, diperoleh submatriks:
    
        $M_{12} = \begin{bmatrix}  
4 & 2 & 5\\
1 & 5 & 2\\ 
2 & 4 & 3\\ 
5 & 3 & 1
\end{bmatrix}$

        Hitung determinan $M_{12}$ dengan ekspansi baris pertama:
        
        $det(M_{12}) = 4 \cdot \begin{vmatrix}  
1 & 5 & 2 \\
2 & 4 & 3 \\
5 & 3 & 1 
\end{vmatrix} - 2 \cdot \begin{vmatrix}  
1 & 5 & 2 \\
2 & 4 & 3 \\
5 & 3 & 2  
\end{vmatrix} + 5 \cdot \begin{vmatrix}  
1 & 4 & 1 \\
2 & 4 & 1 \\
5 & 2 & 4 
\end{vmatrix}$

        Submatriks $M_{12}$

        $M_{12} = \begin{bmatrix}  
3 & 2 & 4\\
5 & 1 & 3\\ 
4 & 2 & 1
\end{bmatrix}$

        Menggunakan metode Sarrus:
        
        $\det(M_{12}) = (3 \times 1 \times 1) + (2 \times 3 \times 4) + (4 \times 5 \times 2) - [(4 \times 1 \times 4) + (2 \times 5 \times 3) + (1 \times 2 \times 3)]$
        
        $= (3 + 24 + 40) - (16 + 30 + 6)$
        
        $= 67 - 52 = 15$
        
    * Minor $M_{13}$
    Hapus baris ke-1 dan kolom ke-3 dari $A$, diperoleh submatriks:
    
        $M_{13} = \begin{bmatrix}  
4 & 2 & 5\\
1 & 5 & 2\\ 
2 & 4 & 3\\ 
5 & 3 & 1
\end{bmatrix}$

        Hitung determinan $M_{13}$ dengan ekspansi baris pertama:
        
        $det(M_{13}) = 4 \cdot \begin{vmatrix}  
1 & 5 & 2 \\
2 & 4 & 3 \\
5 & 3 & 1 
\end{vmatrix} - 2 \cdot \begin{vmatrix}  
1 & 5 & 2 \\
2 & 4 & 3 \\
5 & 3 & 2  
\end{vmatrix} + 5 \cdot \begin{vmatrix}  
1 & 4 & 1 \\
2 & 4 & 1 \\
5 & 2 & 4 
\end{vmatrix}$

        Submatriks $(M_{13})$
        
        $M_{13} = \begin{bmatrix}  
3 & 1 & 4\\
5 & 2 & 3\\ 
4 & 5 & 1
\end{bmatrix}$

        $\det(M_{13}) = (3 \times 2 \times 1) + (1 \times 3 \times 4) + (4 \times 5 \times 5) - [(4 \times 2 \times 4) + (1 \times 5 \times 3) + (1 \times 3 \times 5)]$
        
        $= (6 + 12 + 100) - (32 + 15 + 15)$
        
        $= 118 - 62 = 56$

    * Minor $M_{14}$
    Hapus baris ke-1 dan kolom ke-4 dari $A$, diperoleh submatriks:
    
        $M_{14} = \begin{bmatrix}  
4 & 2 & 5\\
1 & 5 & 2\\ 
2 & 4 & 3\\ 
5 & 3 & 1
\end{bmatrix}$

        Hitung determinan $M_{14}$ dengan ekspansi baris pertama:
        
        $det(M_{14}) = 4 \cdot \begin{vmatrix}  
1 & 5 & 2 \\
2 & 4 & 3 \\
5 & 3 & 1 
\end{vmatrix} - 2 \cdot \begin{vmatrix}  
1 & 5 & 2 \\
2 & 4 & 3 \\
5 & 3 & 2  
\end{vmatrix} + 5 \cdot \begin{vmatrix}  
1 & 4 & 1 \\
2 & 4 & 1 \\
5 & 2 & 4 
\end{vmatrix}$

        Submatriks $(M_{14})$
        
        $M_{14} =
\begin{bmatrix}
3 & 1 & 5 \\
5 & 2 & 4 \\
4 & 5 & 3
\end{bmatrix}$

        Menggunakan metode Sarrus:
        
        $\det(M_{14}) = (3 \times 2 \times 3) + (1 \times 4 \times 4) + (5 \times 5 \times 5) - [(5 \times 2 \times 5) + (1 \times 5 \times 3) + (3 \times 4 \times 4)]$
        
        $= (18 + 16 + 125) - (50 + 15 + 48)$
        
        $= 159 - 113 = 46$


    * Minor $M_{15}$
    Hapus baris ke-1 dan kolom ke-5:
    
        $M_{15} =
\begin{bmatrix}
1 & 4 & 2 & 3 \\
3 & 1 & 5 & 2 \\
5 & 2 & 4 & 1 \\
4 & 5 & 3 & 2
\end{bmatrix}$

        $det(M_{15}) = 1  \begin{vmatrix}  
1 & 5 & 2 \\
4 & 5 & 2 \\
5 & 2 & 4 
\end{vmatrix} - 4 \begin{vmatrix}  
3 & 5 & 2 \\
5 & 2 & 4 \\
4 & 5 & 3  
\end{vmatrix} + 2 \begin{vmatrix}  
3 & 1 & 5 \\
5 & 2 & 4 \\
4 & 5 & 3 
\end{vmatrix} + 3 \begin{vmatrix}  
3 & 1 & 5 \\
5 & 2 & 2 \\
4 & 5 & 2 
\end{vmatrix}$

        Submatriks $M_{15}$
        
        $M_{15} =
\begin{bmatrix}
 3 & 1 & 2 \\
5 & 2 & 1 \\
4 & 5 & 2
\end{bmatrix}$

        Menggunakan metode Sarrus:
        
        $\det(M_{15}) = (3 \times 2 \times 2) + (1 \times 1 \times 4) + (2 \times 5 \times 5) - [(4 \times 2 \times 2) + (5 \times 1 \times 3) + (2 \times 5 \times 5)]$
        
        $= (12 + 4 + 50) - (16 + 15 + 50)$
        
        $= 66 - 81 = -15$
        
        
    * Langkah Terakhir: Substitusi ke Determinan Matriks $(A)$
    Setelah mendapatkan semua minor, kita substitusi ke dalam ekspresi determinan utama:
    
        $\det(A) = 2M_{11} - 3M_{12} + 1M_{13} - 5M_{14} + 4M_{15}$
    
        Substitusi hasil:
        
        $\det(A) = 2(3) - 3(15) + 1(56) - 5(46) + 4(-15)$
        
        $= 6 - 45 + 56 - 230 - 60$
        
        $= \mathbf{-273}$
        
        
        **Kesimpulan :**

        Setelah melalui semua proses perhitungan dengan metode Sarrus, kita mendapatkan bahwa determinannya adalah:
        
        $\det(A) = 2(3) - 3(15) + 1(56) - 5(46) + 4(-15)$
        
        $= 6 - 45 + 56 - 230 - 60$
        
        $= \mathbf{-273}$
        
        Itulah perhitungan minor dan determinan matriks $(5 \times 5)$ secara rinci.





    
    