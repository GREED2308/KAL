---
title: 'Penyelesaian Sistem Persamaan '

---

## Penyelesaian Sistem Persamaan Linear

Penyelesaian Sistem Persamaan Linear (SPL) dapat dilakukan dengan beberapa metode, tergantung pada jumlah variabel dan karakteristik sistemnya.

* Metode Substitusi → Cocok untuk sistem dengan 2 variabel.
* Metode Eliminasi → Cocok untuk sistem dengan lebih dari 2 variabel.
* Metode Matriks → Efisien untuk sistem yang lebih besar.
* Metode Grafik → Hanya cocok untuk visualisasi pada sistem 2 variabel.

### Operasi Baris Elementer

Operasi Baris Elementer (OBE) adalah teknik yang digunakan dalam manipulasi matriks untuk menyelesaikan sistem persamaan linear, menemukan invers matriks, dan berbagai aplikasi lainnya.

* Operasi Baris Elementer (OBE) digunakan untuk menyelesaikan SPL, menghitung invers matriks, dan berbagai manipulasi matriks lainnya.
* Terdapat tiga operasi utama: pertukaran baris, perkalian baris dengan skalar, dan penjumlahan baris.
* OBE adalah dasar dari metode Eliminasi Gauss, Eliminasi Gauss-Jordan, dan metode matriks lainnya.

### Eleminasi Gauss

Metode Eliminasi Gauss adalah teknik penyelesaian Sistem Persamaan Linear (SPL) dengan mengubah matriks augmented ke bentuk segitiga atas menggunakan Operasi Baris Elementer (OBE).

* Eliminasi Gauss digunakan untuk mengubah matriks augmented menjadi bentuk segitiga atas
* Setelah bentuk segitiga atas diperoleh, digunakan substitusi balik untuk menyelesaikan sistem
* Metode ini lebih cepat dibanding substitusi biasa, terutama untuk sistem dengan banyak variabel

Contoh Soal 1

$$
\begin{array}{cc}
x_1+2x_2+3x_3=6\\
2x_1+4x_2+6x_3=12\\
x_3+x_2=2
\end{array}
$$

Penyelesaian:

$$
\begin{array}{cc}
x_1 + 2x_2 + 3x_3 = 6 \\
2x_1 + 4x_2 + 6x_3 = 12 \\
x_3 + x_2 = 2
\end{array}
$$

Matriks augmented:

$$
\begin{bmatrix}
1 & 2 & 3 & | & 6 \\
2 & 4 & 6 & | & 12 \\
0 & 1 & 1 & | & 2
\end{bmatrix}
$$

Baris kedua dikurangi 2 kali baris pertama:

$$
\begin{bmatrix}
1 & 2 & 3 & | & 6 \\
0 & 0 & 0 & | & 0 \\
0 & 1 & 1 & | & 2
\end{bmatrix}
$$

Maka,

$$
x_1 + 2x_2 + 3x_3 + 6 = x_1 + 2(2 - x_3) + 3x_3 = 6 \\
x_1+ 4 -2x_2 + 3x_3 = 6 \\
x_1+x_3 = 6 - 4 \\
x_1 = 2 - x_3
$$

Karna ada variabel bebas $$x_3 = t $$ Sehingga, solusi umum dari sistem persamaan tersebut adalah:

$$
\begin{aligned}
x_1 &= 2-t, \\
x_2 &= 2-t, \\
x_3 &= t, \quad t \in \mathbb{R}.
\end{aligned}
$$

---

Contoh Soal 2

$$
\begin{aligned}
x_1 + x_2 + x_3 = 3 \\
2x_1 + x_3 = 5 \\
x_1 + 2x_2 = 3
\end{aligned}
$$

Matriks augmented:

$$
\begin{bmatrix}
1 & 1 & 1 & | 3 \\
2 & 0 & 1 & | 5 \\
1 & -2 & 0 & | 3
\end{bmatrix}
$$

Eliminasi dengan mengurangi baris kedua dengan 2 kali baris pertama:

$$
\begin{bmatrix}
1 & 1 & 1 & | 3 \\
0 & -2 & -1 & | -1 \\
1 & -2 & 0 & | 3
\end{bmatrix}
$$

$$
\begin{bmatrix}
1 & 1 & 1 & | 3 \\
0 & -2 & -1 & | -1 \\
0 & -3 & -1 & | 0
\end{bmatrix}
$$

Eliminasi dengan mengubah baris ketiga:

$$B_3 = B_3 - \frac{3}{2} B_2$$

$$\begin{bmatrix}
1 & 1 & 1 & | 3 \\
0 & -2 & -1 & | -1 \\
0 & 0 & \frac{1}{2} & | -\frac{3}{2}
\end{bmatrix}$$

Dari baris ketiga:

$$x_3 = -3.$$

$$-2x_2 -1(-3) = -1 \Rightarrow -2x_2 +3 = -1 \Rightarrow -2x_2 = -4 \Rightarrow x_2 = 2.$$

$$x_1 + 2 + (-3) = 3 \Rightarrow x_1 -1 = 3 \Rightarrow x_1 = 4.$$

$$
x_1 = 4 \\
x_2 = 2 \\
x_3 = -3
$$


---

Contoh Soal 3

$$
\begin{aligned}
2x_1 + 2x_2 &= Y \\
x_1 + x_2 &= 2
\end{aligned}
$$

Matriks augmented:

$$
\begin{bmatrix}
2 & 2 & | Y \\
1 & 1 & | 2
\end{bmatrix}
$$

Eliminasi dengan membagi baris pertama dengan 2:

$$
\begin{bmatrix}
1 & 1 & | \frac{Y}{2} \\
1 & 1 & | 2
\end{bmatrix}
$$

Kurangi baris kedua dengan baris pertama:

$$
\begin{bmatrix}
1 & 1 & | \frac{Y}{2} \\
0 & 0 & | 2 - \frac{Y}{2}
\end{bmatrix}
$$

Jika , baris kedua menjadi , sehingga ada solusi tak hingga:

$$x_1 = 2 - x_2.$$


Contoh Soal 4

$$
\begin{aligned}
x_1 + x_2 &= 5 \\
x_1 + 2x_3 &= 6
\end{aligned}
$$

Matriks augmented:

$$
\begin{bmatrix}
1 & 1 & 0 & | 5 \\
1 & 0 & 2 & | 6
\end{bmatrix}
$$

Eliminasi dengan mengurangi baris kedua dengan baris pertama:

$$
\begin{bmatrix}
1 & 1 & 0 & | 5 \\
0 & -1 & 2 & | 1
\end{bmatrix}
$$

Dari baris kedua:

$$- x_2 + 2x_3 = 1 \Rightarrow x_2 = 2x_3 - 1.$$

$$x_1 + (2x_3 - 1) = 5 \Rightarrow x_1 = 6 - 2x_3.$$

Solusi umum:

$$
\begin{aligned}
x_1 &= 6 - 2t, \\
x_2 &= 2t - 1, \\
x_3 &= t, \quad t \in \mathbb{R}.
\end{aligned}
$$

Sistem memiliki solusi tak hingga.