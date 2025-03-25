---
title: INVERS MATRIK

---

# INVERS MATRIK 
### Definisi Matriks Invers

Matriks invers adalah matriks yang jika dikalikan dengan matriks aslinya menghasilkan matriks identitas.

Secara matematis, jika ${A}$ adalah sebuah matriks persegi, maka inversnya, yang ditulis sebagai $A^{-1}$, memenuhi persamaan:

$$
A \times A^{-1}=A^{-1} \times A=I
$$

di mana $I$ adalah matriks identitas, yaitu matriks dengan angka 1 di diagonal utama dan $\mathbf{0}$ di tempat lainnya.
Contoh matriks identitas untuk ukuran $2 \times 2$ : 

$$
I=\left[\begin{array}{ll}
1 & 0 \\
0 & 1
\end{array}\right]
$$

dan untuk ukuran $3 \times 3$ : 

$$
I=\left[\begin{array}{lll}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{array}\right]
$$
### Syarat Suatu Matriks Memiliki Invers

Tidak semua matriks memiliki invers. Suatu matriks $A$ bisa memiliki invers $$ A^{-1} $$ jika memenuhi dua syarat berikut:
1. Matriks harus berbentuk persegi $$ \rightarrow $$ jumlah baris harus sama dengan jumlah kolom.
2. Determinan tidak boleh nol $$ \rightarrow|A| \neq 0 $$.

Jika determinannya nol $(|A|=0)$, maka matriks disebut singular dan tidak memiliki invers.



## MATRIK 3 PERSAMAAN

### Buat Persamaan 3x3    

Diberikan sistem persamaan linear:

$$ \begin{align*}
    2x - y + z &= 3 \\
    x + y - z &= 1 \\
    3x + 2y + z &= 4
\end{align*} $$

Bentuk matriks augmentasi:


$$
[A | B] = \left[ \begin{array}{ccc|c}
2 & -1 & 1 & 3 \\
1 & 1 & -1 & 1 \\
3 & 2 & 1 & 4
\end{array} \right]
$$

### Langkah-Langkah Penyelesaian

### Langkah 1: Bentuk Augmented Matrix $[A \mid I]$

$$
[A \mid I]=\left[ \begin{array}{ccc|ccc}
2 & -1 & 1 & 1 & 0 & 0 \\
1 & 1 & -1 & 0 & 1 & 0 \\
3 & 2 & 1 & 0 & 0 & 1
\end{array} \right]
$$

### Langkah 2: Buat Elemen (1,1) Menjadi 1

##### Bagi baris pertama dengan 2:

$$ R_1 \leftarrow \frac{1}{2} R_1 $$

Hasilnya:


$$
\left[ \begin{array}{ccc|ccc}
1 & -\frac{1}{2} & \frac{1}{2} & \frac{1}{2} & 0 & 0 \\
1 & 1 & -1 & 0 & 1 & 0 \\
3 & 2 & 1 & 0 & 0 & 1
\end{array} \right]
$$

### Langkah 3: Nol-kan Elemen di Bawah (1,1)


$$ R_2 \leftarrow R_2 - R_1, \quad R_3 \leftarrow R_3 - 3R_1 $$


Hasilnya:


$$
\left[ \begin{array}{ccc|ccc}
1 & -\frac{1}{2} & \frac{1}{2} & \frac{1}{2} & 0 & 0 \\
0 & \frac{3}{2} & -\frac{3}{2} & -\frac{1}{2} & 1 & 0 \\
0 & \frac{7}{2} & -\frac{1}{2} & -\frac{3}{2} & 0 & 1
\end{array} \right] 
$$

### Langkah 4: Buat Elemen (2,2) Menjadi 1

##### Bagi baris kedua dengan $\frac{3}{2}$ :

$$ R_2 \leftarrow \frac{2}{3} R_2 $$

Hasilnya:


$$
\left[ \begin{array}{ccc|ccc}
1 & -\frac{1}{2} & \frac{1}{2} & \frac{1}{2} & 0 & 0 \\
0 & 1 & -1 & -\frac{1}{3} & \frac{2}{3} & 0 \\
0 & \frac{7}{2} & -\frac{1}{2} & -\frac{3}{2} & 0 & 1
\end{array} \right]
$$

##### Langkah 5: Nol-kan Elemen di Bawah (2,2)


$$ R_3 \leftarrow R_3 - \frac{7}{2} R_2 $$

Hasilnya:


$$
\left[ \begin{array}{ccc|ccc}
1 & -\frac{1}{2} & \frac{1}{2} & \frac{1}{2} & 0 & 0 \\
0 & 1 & -1 & -\frac{1}{3} & \frac{2}{3} & 0 \\
0 & 0 & \frac{5}{2} & -\frac{4}{3} & -\frac{14}{6} & 1
\end{array} \right]
$$ 

#### Langkah 6: Buat Elemen (3,3) Menjadi 1

##### Bagi baris ketiga dengan $\frac{5}{2}$:

$$ R_3 \leftarrow \frac{2}{5} R_3 $$

Hasilnya:


$$
\left[ \begin{array}{ccc|ccc}
1 & -\frac{1}{2} & \frac{1}{2} & \frac{1}{2} & 0 & 0 \\
0 & 1 & -1 & -\frac{1}{3} & \frac{2}{3} & 0 \\
0 & 0 & 1 & -\frac{8}{15} & -\frac{28}{30} & \frac{2}{5}
\end{array} \right]
$$

#### Langkah 7: Nol-kan Elemen di Atas (3,3)


$$ R_1 \leftarrow R_1 - \frac{1}{2} R_3, \quad R_2 \leftarrow R_2 + R_3 $$

Hasil akhirnya:


$$
\left[ \begin{array}{ccc|ccc}
1 & 0 & 0 & \frac{8}{15} & -\frac{1}{5} & \frac{7}{20} \\
0 & 1 & 0 & -\frac{1}{5} & \frac{3}{5} & -\frac{7}{10} \\
0 & 0 & 1 & \frac{1}{15} & -\frac{2}{15} & \frac{7}{30}
\end{array} \right]
$$

#### Langkah 8: Matriks Identitas Diperoleh

Maka inversnya adalah:

$$
A^{-1} = \left[ \begin{array}{ccc}
\frac{8}{15} & -\frac{1}{5} & \frac{7}{20} \\
-\frac{1}{5} & \frac{3}{5} & -\frac{7}{10} \\
\frac{1}{15} & -\frac{2}{15} & \frac{7}{30}
\end{array} \right]
$$

#### Langkah 9: Hitung $A^{-1} \times B$

$$
A^{-1} \times B = \left[ \begin{array}{c}1 \\ 0 \\ 0\end{array} \right]
$$

Sehingga solusinya adalah:
$$
\begin{align*}
    x &= 1 \\
    y &= 0 \\
    z &= 0
\end{align*}
$$


