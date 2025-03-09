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
1. samakan koefisien salah satu variabel

* pilih variabel yang akan dieliminasi (misalnya, $x$ atau $y$ ).

* Kalikan salah satu atau kedua persamaan dengan bilangan tertentu sehingga koefisien variabel tersebut menjadi sama.

2. Kurangkan atau jumlahkan kedua persamaan

* Jika koefisien variabel yang akan dieliminasi sama, gunakan operasi pengurangan atau penjumlahan untuk menghilangkannya.

* Ini akan menghasilkan persamaan baru dengan satu variabel saja.