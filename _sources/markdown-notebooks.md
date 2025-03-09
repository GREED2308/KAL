---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.11.5
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# Eliminasi Persamaan Linear

Eliminasi dalam persamaan linear adalah salah satu metode untuk menyelesaikan sistem persamaan linear dengan menghilangkan salah satu variabel sehingga persamaan dapat disederhanakan menjadi satu variabel saja.

## Langkah-Langkah Metode Eliminasi

Misalkan kita memiliki sistem persamaan linear dua variabel berikut:

$$
\begin{aligned}
a_1x+b_1y = c_1\\
a_2x+b_2y = c_2
\end{aligned}
$$
1. Samakan koefisien salah satu variabel

* pilih variabel yang akan dieliminasi (misalnya, $x$ atau $y$ ).
* Kalikan salah satu atau kedua persamaan dengan bilangan tertentu sehingga koefisien variabel tersebut menjadi sama.

2. Kurangkan atau jumlahkan kedua persamaan

* Jika koefisien variabel yang akan dieliminasi sama, gunakan operasi pengurangan atau penjumlahan untuk menghilangkannya.
* Ini akan menghasilkan persamaan baru dengan satu variabel saja.

3. Selesaikan persamaan satu variabel

* Setelah didapat persamaan dengan satu variabel, selesaikan persamaan tersebut untuk menetukan nilai variabelnya.

4. Substitusi nilai variabel yang ditemukan

* Masukkan nilai variabel yang telah ditemukan ke salah satu persamaan awal untuk mendapatkan nilai variabel lainnya.

**Contoh:**

Selesaikan sistem persamaan berikut menggunakan metode eliminasi:

$$
\begin{aligned}
2_x + 3_y = 12\\
4_x - y = 5
\end{aligned}
$$

Langkah 1:

Samakan koefisien salah satu variabel. Kita pilih variabel $x$ untuk dieliminasi.Koefisien $x$ pada persamaan pertama adalah 2 dan pada persamaan kedua adalah 4. Agar sama, kalikan persamaan pertama dengan 2:

$$
\begin{aligned}
(2_x + 3_y = 12) \times 2 \\
4_x - y = 5
\end{aligned}
$$

Sekarang sistem persamaannya menjadi:

$$
\begin{aligned}
4_x + 6_y = 24\\
4_x - y = 5
\end{aligned}
$$

Langkah 2:

Kurangkan kedua persamaan:

$$
\begin{aligned}
(4_x + 6_y) - (4_x - y) = 24 - 5 \\
4_x + 6_y - 4_x - y = 19 \\
7_y = 19
\end{aligned}
$$

Langkah 3:

Selesaikan variabel $y$ :

$$
\begin{aligned}
y = \frac{19}{7}
\end{aligned}
$$