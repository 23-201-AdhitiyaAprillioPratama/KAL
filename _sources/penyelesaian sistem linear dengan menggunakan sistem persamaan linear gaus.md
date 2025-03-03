---
title: "penyelesaian sistem linear dengan menggunakan sistem persamaan\_linear\_gaus"

---

# penyelesaian sistem linear dengan menggunakan sistem persamaan linear gaus

## Sistem Persamaan Linear dengan 2 Persamaan dan 2 Variabel
saya memiliki sistem persamaan berikut:
 $3 x+4 y=10$
$5 x-2 y=8$

### Langkah 1: Membuat Matriks Augmented

Tulis sistem persamaan dalam bentuk matriks augmented:
$$
\left[\begin{array}{cc|c}
3 & 4 & 10 \\
5 & -2 & 8
\end{array}\right]
$$

### Langkah 2: Operasi Baris Elementer

#### Langkah 2.1: Membuat elemen pertama pada baris pertama menjadi 1.
Bagi baris pertama dengan 2:
$$\begin{gathered}R_1=R_1 \div 3 \\ {\left[\begin{array}{cc|c}1 & \frac{4}{3} & \frac{10}{3} \\ 5 & -2 & 8\end{array}\right]}\end{gathered}$$

#### Langkah 2.2: Eliminasi elemen di bawah pivot pertama.
Gunakan operasi baris: 
$$R_2=R_2-4 R_1 $$

perhitungan baris kedua:
- $5-5(1)=0$
- $-2-5\left(\frac{4}{3}\right)=-2-\frac{20}{3}=-\frac{26}{3}$
- $8-5\left(\frac{10}{3}\right)=8-\frac{50}{3}=-\frac{26}{3}$
matrix yang sekarang:
$$\left[\begin{array}{cc|c}1 & \frac{4}{3} & \frac{10}{3} \\ 0 & -\frac{26}{3} & -\frac{26}{3}\end{array}\right]$$

#### Langkah 2.3: Membuat elemen kedua pada baris kedua menjadi 1.
Bagi baris kedua $\left(R_2\right)$ dengan $-\frac{26}{3}$ :
$$
R_2=R_2 \div-\frac{26}{3}
$$

Perhitungan:
- $0 \div-\frac{26}{3}=0$
- $-\frac{26}{3} \div-\frac{26}{3}=1$
- $-\frac{26}{3} \div-\frac{26}{3}=1$

Matriks menjadi:
$$
\left[\begin{array}{cc|c}
1 & \frac{4}{3} & \frac{10}{3} \\
0 & 1 & 1
\end{array}\right]
$$

#### Langkah 2.4: Eliminasi elemen di atas pivot kedua.
Kurangi $\frac{4}{3}$ kali baris kedua dari baris pertama:
$$
R_1=R_1-\frac{4}{3} R_2
$$

Perhitungan baris pertama:
- $1-\frac{4}{3}(0)=1$
- $\frac{4}{3}-\frac{4}{3}(1)=0$
- $\frac{10}{3}-\frac{4}{3}(1)=\frac{6}{3}=2$

Matriks sekarang:
$$
\left[\begin{array}{ll|l}
1 & 0 & 2 \\
0 & 1 & 1
\end{array}\right]
$$

### Langkah 3: Solusi
Dari matriks terakhir, kita dapat membaca solusinya:
$$
x=2, \quad y=1
$$

Jadi, solusi dari sistem persamaan adalah:
$$
(x, y)=(2,1)
$$

### Geogebra Persamaan Linear dengan 2 Persamaan dan 2 Variabel

<iframe src="https://www.geogebra.org/calculator/mb3yhtr8?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

## Sistem Persamaan Linear dengan 3 Persamaan dan 3 Variabel

#### Sistem Persamaan Linear

$$
\begin{cases}2 x+3 y-z=5 & (\text { Persamaan } 1) \\ 4 x-y+2 z=6 & (\text { Persamaan } 2) \\ -3 x+2 y+4 z=7 & (\text { Persamaan } 3)\end{cases}
$$

Langkah 1: Membuat Matriks Augmented
Tulis sistem persamaan dalam bentuk matriks augmented:
$$
\left[\begin{array}{ccc|c}
2 & 3 & -1 & 5 \\
4 & -1 & 2 & 6 \\
-3 & 2 & 4 & 7
\end{array}\right]
$$

Langkah 2: Eliminasi Gauss
Tujuan: Mengubah matriks menjadi bentuk eselon baris (row echelon form).
Langkah 2.1: Membuat elemen pertama pada baris pertama menjadi 1
Bagi baris pertama dengan 2:
$$
\left[\begin{array}{ccc|c}
1 & \frac{3}{2} & -\frac{1}{2} & \frac{5}{2} \\
4 & -1 & 2 & 6 \\
-3 & 2 & 4 & 7
\end{array}\right]
$$

Langkah 2.2: Eliminasi elemen di bawah pivot pertama
Gunakan operasi baris:
- $R_2=R_2-4 R_1$
- $R_3=R_3+3 R_1$

Hasilnya:
$$
\left[\begin{array}{ccc|c}
1 & \frac{3}{2} & -\frac{1}{2} & \frac{5}{2} \\
0 & -7 & 4 & -4 \\
0 & \frac{13}{2} & \frac{5}{2} & \frac{29}{2}
\end{array}\right]
$$

Langkah 2.3: Membuat elemen kedua pada baris kedua menjadi 1
Bagi baris kedua dengan -7 :
$$
\left[\begin{array}{ccc|c}
1 & \frac{3}{2} & -\frac{1}{2} & \frac{5}{2} \\
0 & 1 & -\frac{4}{7} & \frac{4}{7} \\
0 & \frac{13}{2} & \frac{5}{2} & \frac{29}{2}
\end{array}\right]
$$

Langkah 2.4: Eliminasi elemen di atas dan di bawah pivot kedua
Gunakan operasi baris:
- $R_1=R_1-\frac{3}{2} R_2$
- $R_3=R_3-\frac{13}{2} R_2$

Hasilnya:
$$
\left[\begin{array}{ccc|c}
1 & 0 & \frac{2}{7} & \frac{23}{14} \\
0 & 1 & -\frac{4}{7} & \frac{4}{7} \\
0 & 0 & \frac{27}{14} & \frac{41}{14}
\end{array}\right]
$$

Langkah 2.5: Membuat elemen ketiga pada baris ketiga menjadi 1
Bagi baris ketiga dengan $\frac{27}{14}$ :
$$
\left[\begin{array}{ccc|c}
1 & 0 & \frac{2}{7} & \frac{23}{14} \\
0 & 1 & -\frac{4}{7} & \frac{4}{7} \\
0 & 0 & 1 & \frac{41}{7} \times \frac{14}{27}=\frac{41}{27}
\end{array}\right]
$$

Langkah 2.6: Eliminasi elemen di atas pivot ketiga
Gunakan operasi baris:
- $R_1=R_1-\frac{2}{7} R_3$
- $R_2=R_2+\frac{4}{7} R_3$

Hasil akhirnya:
$$
\left[\begin{array}{lll|l}
1 & 0 & 0 & 2 \\
0 & 1 & 0 & 1 \\
0 & 0 & 1 & 3
\end{array}\right]
$$

Langkah 3: Solusi
Dari matriks terakhir, kita dapat membaca solusinya:
$$
x=2, \quad y=1, \quad z=3
$$

Verifikasi Solusi
Substitusikan nilai $x, y, z$ ke dalam persamaan asli untuk memverifikasi kebenaran solusi:

$$2 x+3 y-z=5$$

1. Persamaan 1:
$$
2(2)+3(1)-1(3)=4+3-3=5
$$

$$4 x-y+2 z=6$$

2. Persamaan 2:
$$
4(2)-1(1)+2(3)=8-1+6=6
$$

$$x+2 y+4 z=7$$

3. Persamaan 3:
$$
-3(2)+2(1)+4(3)=-6+2+12=7
$$

Kesimpulan
Solusi sistem persamaan linear ini adalah:
$$
x=2, \quad y=1, \quad z=3
$$

### Geogebra Persamaan Linear dengan 3 Persamaan dan 3 Variabel

[<iframe src="https://www.geogebra.org/calculator/deg5zxxg?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>]


