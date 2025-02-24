---
title: 'Penyelesaian Sistem Persamaan '

---

## Penyelesaian Sistem Persamaan Linear


### Operasi Baris Elementer


### Eleminasi Gauss

Contoh Soal 1

\begin{aligned}
x_1 + 2x_2 + 3x_3 &= 6 \
2x_1 + 4x_2 + 6x_3 &= 12 \
x_3 - x_2 &= 2
\end{aligned}

Matriks augmented:

\begin{bmatrix}
1 & 2 & 3 & | 6 \\
2 & 4 & 6 & | 12 \\
0 & -1 & 1 & | 2
\end{bmatrix}

Baris kedua dikurangi 2 kali baris pertama:

\begin{bmatrix}
1 & 2 & 3 & | 6 \\
0 & 0 & 0 & | 0 \\
0 & -1 & 1 & | 2
\end{bmatrix}

Baris kedua menjadi nol, menunjukkan bahwa sistem memiliki solusi tak hingga.
Variabel bebas: , maka

$$x_2 = t - 2, \quad x_1 = -2x_2 - 3x_3 + 6 = -2(t-2) - 3t + 6 = -5t + 10.$$

\begin{aligned}
x_1 &= -5t + 10, \\
x_2 &= t - 2, \\
x_3 &= t, \quad t \in \mathbb{R}.
\end{aligned}


---

Contoh Soal 2

\begin{aligned}
x_1 + x_2 + x_3 &= 3 \\
2x_1 + 0x_2 + x_3 &= 5 \\
x_1 - 2x_2 + 0x_3 &= 3
\end{aligned}

Matriks augmented:

\begin{bmatrix}
1 & 1 & 1 & | 3 \\
2 & 0 & 1 & | 5 \\
1 & -2 & 0 & | 3
\end{bmatrix}

Eliminasi dengan mengurangi baris kedua dengan 2 kali baris pertama:

\begin{bmatrix}
1 & 1 & 1 & | 3 \\
0 & -2 & -1 & | -1 \\
1 & -2 & 0 & | 3
\end{bmatrix}

\begin{bmatrix}
1 & 1 & 1 & | 3 \\
0 & -2 & -1 & | -1 \\
0 & -3 & -1 & | 0
\end{bmatrix}

Eliminasi dengan mengubah baris ketiga:

$$B_3 = B_3 - \frac{3}{2} B_2$$

\begin{bmatrix} 1 & 1 & 1 & | 3 \ 0 & -2 & -1 & | -1 \ 0 & 0 & \frac{1}{2} & | -\frac{3}{2} \end{bmatrix}

Dari baris ketiga:

$$x_3 = -3.$$

$$-2x_2 -1(-3) = -1 \Rightarrow -2x_2 +3 = -1 \Rightarrow -2x_2 = -4 \Rightarrow x_2 = 2.$$

$$x_1 + 2 + (-3) = 3 \Rightarrow x_1 -1 = 3 \Rightarrow x_1 = 4.$$

$$(x_1, x_2, x_3) = (4, 2, -3).$$


---

Contoh Soal 3

\begin{aligned}
2x_1 + 2x_2 &= Y \\
x_1 + x_2 &= 2
\end{aligned}

Matriks augmented:

\begin{bmatrix}
2 & 2 & | Y \\
1 & 1 & | 2
\end{bmatrix}

Eliminasi dengan membagi baris pertama dengan 2:

\begin{bmatrix}
1 & 1 & | \frac{Y}{2} \\
1 & 1 & | 2
\end{bmatrix}

Kurangi baris kedua dengan baris pertama:

\begin{bmatrix}
1 & 1 & | \frac{Y}{2} \\
0 & 0 & | 2 - \frac{Y}{2}
\end{bmatrix}

Jika , baris kedua menjadi , sehingga ada solusi tak hingga:

$$x_1 = 2 - x_2.$$


Contoh Soal 4

\begin{aligned}
x_1 + x_2 &= 5 \\
x_1 + 2x_3 &= 6
\end{aligned}

Matriks augmented:

\begin{bmatrix}
1 & 1 & 0 & | 5 \\
1 & 0 & 2 & | 6
\end{bmatrix}

Eliminasi dengan mengurangi baris kedua dengan baris pertama:

\begin{bmatrix}
1 & 1 & 0 & | 5 \\
0 & -1 & 2 & | 1
\end{bmatrix}

Dari baris kedua:

$$- x_2 + 2x_3 = 1 \Rightarrow x_2 = 2x_3 - 1.$$

$$x_1 + (2x_3 - 1) = 5 \Rightarrow x_1 = 6 - 2x_3.$$

Solusi umum:

\begin{aligned}
x_1 &= 6 - 2t, \\
x_2 &= 2t - 1, \\
x_3 &= t, \quad t \in \mathbb{R}.
\end{aligned}

Sistem memiliki solusi tak hingga.