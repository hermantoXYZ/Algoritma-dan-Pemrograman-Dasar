---
icon: atom
---

# Tipe Data, Operator dan Operasi

## Tipe Data

Tipe data adalah suatu media atau memori pada komputer yang digunakan untuk menampung informasi.

Berikut adalah tipe data dari bahasa pemrograman Python yang umum digunakan, perhatikan dengan seksama ya:(&#x20;

***

* **Integer (`int`)**: Untuk angka bulat.
  * Contoh: `10`, `-5`, `2023`
* **Float (`float`)**: Untuk angka desimal.
  * Contoh: `3.14`, `-0.75`, `10.0`
* **String (`str`)**: Untuk teks.
  * Contoh: `"Halo Dunia"`, `'Python'`
* **Boolean (`bool`)**: Untuk logika benar/salah.
  * Contoh: `True`, `False`

***

* **List (`list`)**: Koleksi data yang terurut dan bisa diubah. Sering digunakan karena fleksibilitasnya.
  * Contoh: `[1, 2, 3]`, `['apel', 'jeruk', 'mangga']`
* **Tuple (`tuple`)**: Koleksi data yang terurut tetapi tidak dapat diubah. Digunakan untuk data tetap.
  * Contoh: `(1, 2, 3)`, `('Senin', 'Selasa', 'Rabu')`
* **Dictionary (`dict`)**: Koleksi pasangan kunci-nilai. Sering digunakan untuk data yang membutuhkan pengelompokan dengan label.
  * Contoh: `{'nama': 'Ali', 'usia': 25}`, `{'id': 101, 'status': 'aktif'}`
* **Set (`set`)**: Koleksi data unik yang tidak terurut. Digunakan untuk memastikan tidak ada duplikasi.
  * Contoh: `{1, 2, 3}`, `{'a', 'b', 'c'}`

***

* **NoneType (`None`)**: Menunjukkan ketiadaan nilai. Sering digunakan sebagai nilai awal atau default.
  * Contoh: `None`

## Operator Aritmatika & Operator Pembanding

Berikut adalah tabel yang mencakup **operator aritmatika** dan **operator pembanding** di Python:

| **Kategori**   | **Operator** | **Deskripsi**                | **Contoh** | **Hasil** |
| -------------- | ------------ | ---------------------------- | ---------- | --------- |
| **Aritmatika** | `+`          | Penjumlahan                  | `3 + 5`    | `8`       |
|                | `-`          | Pengurangan                  | `10 - 7`   | `3`       |
|                | `*`          | Perkalian                    | `4 * 6`    | `24`      |
|                | `/`          | Pembagian                    | `8 / 2`    | `4.0`     |
|                | `%`          | Sisa bagi (modulus)          | `10 % 3`   | `1`       |
|                | `//`         | Pembagian bulat              | `7 // 2`   | `3`       |
|                | `**`         | Perpangkatan                 | `2 ** 3`   | `8`       |
| **Pembanding** | `==`         | Sama dengan                  | `5 == 5`   | `True`    |
|                | `!=`         | Tidak sama dengan            | `5 != 3`   | `True`    |
|                | `>`          | Lebih besar                  | `7 > 3`    | `True`    |
|                | `<`          | Lebih kecil                  | `2 < 4`    | `True`    |
|                | `>=`         | Lebih besar atau sama dengan | `5 >= 5`   | `True`    |
|                | `<=`         | Lebih kecil atau sama dengan | `3 <= 4`   | `True`    |



{% embed url="https://colab.research.google.com/drive/1cSLZjM97a1ssis_SfqLuraWdahRYZ0PX?usp=sharing" %}
Berikut file dari Google Colab, silahkan diakses..
{% endembed %}

## Contoh Code Aritmatika

{% code overflow="wrap" lineNumbers="true" %}
```python
# Penjumlahan
a = 10
b = 3
print("Penjumlahan (a + b):", a + b)  # Output: 13

# Pengurangan
print("Pengurangan (a - b):", a - b)  # Output: 7

# Perkalian
print("Perkalian (a * b):", a * b)  # Output: 30

# Pembagian
print("Pembagian (a / b):", a / b)  # Output: 3.333...

# Modulus
print("Modulus (a % b):", a % b)  # Output: 1

# Pembagian bulat
print("Pembagian bulat (a // b):", a // b)  # Output: 3

# Pangkat
print("Pangkat (a ** b):", a ** b)  # Output: 1000

```
{% endcode %}

***

## Contoh Code Pembanding

{% code overflow="wrap" %}
```python
# Sama dengan
x = 5
y = 10
print("Sama dengan (x == y):", x == y)  # Output: False

# Tidak sama dengan
print("Tidak sama dengan (x != y):", x != y)  # Output: True

# Lebih besar
print("Lebih besar (x > y):", x > y)  # Output: False

# Lebih kecil
print("Lebih kecil (x < y):", x < y)  # Output: True

# Lebih besar atau sama dengan
print("Lebih besar atau sama dengan (x >= y):", x >= y)  # Output: False

# Lebih kecil atau sama dengan
print("Lebih kecil atau sama dengan (x <= y):", x <= y)  # Output: True
```
{% endcode %}
