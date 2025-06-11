---
title: Untitled

---

# Hasil Kali Silang (Cross Product)

## **Definisi:** 
Hasil kali silang adalah operasi antara dua vektor dalam ruang tiga dimensi yang menghasilkan vektor baru yang tegak lurus terhadap kedua vektor tersebut.

Misalkan dua vektor:
$$ 
\vec{A} = \langle a_1, a_2, a_3 \rangle \quad \text{dan} \quad \vec{B} = \langle b_1, b_2, b_3 \rangle
$$
Maka hasil kali silang $\vec{A} \times \vec{B}$ adalah:
$$
\vec{A} \times \vec{B} =
\begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
a_1 & a_2 & a_3 \\
b_1 & b_2 & b_3 \\
\end{vmatrix}
=$$
$$
(a_2 b_3 - a_3 b_2)\hat{i} - (a_1 b_3 - a_3 b_1)\hat{j} + (a_1 b_2 - a_2 b_1)\hat{k}
$$

### Contoh:

Diberikan dua vektor:
$$
\vec{A} = \langle 2, 3, 4 \rangle, \quad \vec{B} = \langle 5, 6, 7 \rangle
$$

### Maka:
$$
\vec{A} \times \vec{B} =
\begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
2 & 3 & 4 \\
5 & 6 & 7 \\
\end{vmatrix}
$$

$$
= (3 \cdot 7 - 4 \cdot 6)\hat{i} - (2 \cdot 7 - 4 \cdot 5)\hat{j} + (2 \cdot 6 - 3 \cdot 5)\hat{k}
\]
\[
= (21 - 24)\hat{i} - (14 - 20)\hat{j} + (12 - 15)\hat{k}
= -3\hat{i} + 6\hat{j} - 3\hat{k}
$$

Jadi hasilnya:
$$
\vec{A} \times \vec{B} = \langle -3, 6, -3 \rangle
$$


## Rumus Hasil Kali Silang Menggunakan Determinan

Misalkan dua vektor dalam ruang tiga dimensi:

$$
\vec{A} = \langle a_1, a_2, a_3 \rangle, \quad
\vec{B} = \langle b_1, b_2, b_3 \rangle
$$

Maka hasil kali silang $\vec{A} \times \vec{B}$ dapat dihitung menggunakan determinan sebagai berikut:

$$
\vec{A} \times \vec{B} =
\begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
a_1 & a_2 & a_3 \\
b_1 & b_2 & b_3 \\
\end{vmatrix}
$$

Nilai determinan tersebut dihitung sebagai:


$\vec{A} \times \vec{B} =
(a_2 b_3 - a_3 b_2)\hat{i}$
- $(a_1 b_3 - a_3 b_1)\hat{j}$
+ $(a_1 b_2 - a_2 b_1)\hat{k}$


atau dapat ditulis dalam notasi vektor:

$$
\vec{A} \times \vec{B} = 
\langle a_2 b_3 - a_3 b_2,\ 
-(a_1 b_3 - a_3 b_1),\ 
a_1 b_2 - a_2 b_1 \rangle
$$


## Soal: Hasil Kali Silang Dua Vektor

Diketahui dua vektor:

$$
\vec{u} = \langle 1, 1, 1 \rangle, \quad \vec{v} = \langle 2, 1, 1 \rangle
$$

### Langkah 1: Tulis dalam bentuk determinan 3x3

$$
\vec{u} \times \vec{v} =
\begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
1 & 1 & 1 \\
2 & 1 & 1 \\
\end{vmatrix}
$$

## Langkah 2: Hitung masing-masing komponen menggunakan ekspansi kofaktor}

Komponen arah $\hat{i}$:

$$\hat{i} \cdot
\begin{vmatrix}
1 & 1 \\
1 & 1 \\
\end{vmatrix} = \hat{i}(1 \cdot 1 - 1 \cdot 1) = \hat{i}(1 - 1) = 0\hat{i}$$


Komponen arah $\hat{j}$:

$$\hat{j} \cdot
\begin{vmatrix}
1 & 1 \\
2 & 1 \\
\end{vmatrix} = -\hat{j}(1 \cdot 1 - 1 \cdot 2) = -\hat{j}(1 - 2) = -\hat{j}(-1) = \hat{j}$$

Komponen arah $\hat{k}$:

$$ \hat{k} \cdot
\begin{vmatrix}
1 & 1 \\
2 & 1 \\
\end{vmatrix} = \hat{k}(1 \cdot 1 - 1 \cdot 2) = \hat{k}(1 - 2) = -\hat{k} $$


## Langkah 3: Gabungkan hasil}

$$
\vec{u} \times \vec{v} = 0\hat{i} + \hat{j} - \hat{k}
$$

Hasil Akhir dalam Notasi Vektor:

$$ 
\vec{u} \times \vec{v} = \langle 0,\ 1,\ -1 \rangle
$$ 


## hasil  dari soal di atas
<iframe src="https://www.geogebra.org/classic/wj7bkh8p?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

# Tugas Cross Dot
## Soal 1
1. Tentukan luas jajaran genjang yang ditentukan oleh vektor $\vec{u}=\left[\begin{array}{l}1 \\ 2\end{array}\right]$ dan $\vec{v}=\left[\begin{array}{l}2 \\ 1\end{array}\right]$.
2. Tentukan luas jajaran genjang yang ditentukan oleh vektor $\vec{u}=\left[\begin{array}{l}2 \\ 0\end{array}\right]$ dan $\vec{v}=\left[\begin{array}{l}0 \\ 3\end{array}\right]$.
3. Tentukan luas segitiga dengan titik-titik sudut $(0,0,0),(1,3,-1)$, dan $(2,1,1)$.
4. Tentukan luas segitiga dengan titik-titik sudut $(5,2,-1),(3,6,2)$, dan $(1,0,4)$.

## jawaban

### 1. Luas jajaran genjang dari velttor 

$$
\vec{u}=\left[\begin{array}{l}
1 \\
2
\end{array}\right], \quad \vec{v}=\left[\begin{array}{l}
2 \\
1
\end{array}\right]
$$

Untuk vektor 2D, luas jajaran genjang adalah nilai absolut dari determinan matriks 2x2: 

$$
\text { Luas }=|\vec{u} \times \vec{v}|=\left|\begin{array}{ll}
1 & 2 \\
2 & 1
\end{array}\right|=|(1)(1)-(2)(2)|=|1-4|=3
$$

Jawaban: Luas = 3

### 2. Luas jajaran genjang dari vektor

$$
\begin{gathered}
\vec{u}=\left[\begin{array}{l}
2 \\
0
\end{array}\right], \quad \vec{v}=\left[\begin{array}{l}
0 \\
3
\end{array}\right] \\
\text { Luas }=\left|\begin{array}{ll}
2 & 0 \\
0 & 3
\end{array}\right|=|(2)(3)-(0)(0)|=|6|=6
\end{gathered}
$$

Jawaban: Luas = 6

### 3. Luas segitiga dengan titik-titik sudut

$$
A=(0,0,0), \quad B=(1,3,-1), \quad C=(2,1,1)
$$

Hitung vektor.
$$
\overrightarrow{A B}=B-A=\left[\begin{array}{c}
1 \\
3 \\
-1
\end{array}\right], \quad \overrightarrow{A C}=C-A=\left[\begin{array}{l}
2 \\
1 \\
1
\end{array}\right]
$$

Hitung cross product

$$
\begin{gathered}
\overrightarrow{A B} \times \overrightarrow{A C}=\left|\begin{array}{ccc}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
1 & 3 & -1 \\
2 & 1 & 1
\end{array}\right|=\mathbf{i}(3 \cdot 1-(-1) \cdot 1)-\mathbf{j}(1 \cdot 1-(-1) \cdot 2)+\mathbf{k}(1 \cdot 1-3 \cdot 2) \\
=\mathbf{i}(3+1)-\mathbf{j}(1+2)+\mathbf{k}(1-6)=\left[\begin{array}{c}
4 \\
-3 \\
-5
\end{array}\right]
\end{gathered}
$$

Panjang vektor hasil cross: 

$$
|\overrightarrow{A B} \times \overrightarrow{A C}|=\sqrt{4^2+(-3)^2+(-5)^2}=\sqrt{16+9+25}=\sqrt{50}
$$

Luas segitiga $=1 / 2 \times \mid$ cross product:

$$
\text { Luas }=\frac{1}{2} \sqrt{50}=\frac{1}{2} \cdot 5 \sqrt{2}=\frac{5 \sqrt{2}}{2}
$$

Jawaban: Luas $=\frac{5 \sqrt{2}}{2}$

### 4. Luas segitiga dengan titik-titik sudut 

$$
A=(5,2,-1), \quad B=(3,6,2), \quad C=(1,0,4)
$$

Hitung vektor:

$$
\overrightarrow{A B}=B-A=\left[\begin{array}{c}
-2 \\
4 \\
3
\end{array}\right], \quad \overrightarrow{A C}=C-A=\left[\begin{array}{c}
-4 \\
-2 \\
5
\end{array}\right]
$$

Cross product

$$
\begin{gathered}
\overrightarrow{A B} \times \overrightarrow{A C}=\left|\begin{array}{ccc}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
-2 & 4 & 3 \\
-4 & -2 & 5
\end{array}\right|=\mathbf{i}(4 \cdot 5-3 \cdot(-2))-\mathbf{j}(-2 \cdot 5-3 \cdot(-4))+\mathbf{k}(-2 \cdot(-2)-4 \cdot(-4)) \\
=\mathbf{i}(20+6)-\mathbf{j}(-10+12)+\mathbf{k}(4+16)=\left[\begin{array}{c}
26 \\
-2 \\
20
\end{array}\right]
\end{gathered}
$$

Panjang:

$$
|\overrightarrow{A B} \times \overrightarrow{A C}|=\sqrt{26^2+(-2)^2+20^2}=\sqrt{676+4+400}=\sqrt{1080}
$$

Luas segitiga:

$$
\text { Luas }=\frac{1}{2} \sqrt{1080}=\frac{\sqrt{1080}}{2}
$$

Sederhanakan:

$$
\sqrt{1080}=\sqrt{36 \cdot 30}=6 \sqrt{30}
$$

Jawaban: Luas $=3 \sqrt{30}$