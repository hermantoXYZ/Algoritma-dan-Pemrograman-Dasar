---
icon: atom
---

# Tipe Data, Operator dan Operasi

## Variabel

### 1. Apa itu Variabel?

Variabel adalah tempat untuk menyimpan data atau nilai di dalam program. Dalam Python, variabel dapat dibuat dengan memberikan nama variabel dan sebuah nilai, tanpa perlu mendeklarasikan tipe datanya terlebih dahulu. Python secara otomatis menentukan tipe data berdasarkan nilai yang diberikan.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdSEOOWHG7MeNwvGpSehX_BbtDumjUim4sJfG-HHYkaPXo6mhXlwz2ffDCZuif6WqYRvPmTfAfvpv173rcqEtCL_o7tMmE_NHMGxyWt3JvWpX4BMfYo4Ipg3oztfnkqY0ofdpmraKGuS0rqkkKhAirotYUK?key=CAmvbDG6f-5iZFMmcQosyw" alt=""><figcaption><p>Anggap saja variabel adalah sebuah keranjang, tempat di mana kita bisa memasukkan sesuatu di dalamnya, yaitu data.</p></figcaption></figure>

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcZ1aJFQ_AiKRK_1trowYd7RhSi6prB-0ggpN7Q1scF_ziHuKT2vRLbYyzaftwmYsCbr3LKRM1vj8A-DFq5Bg7ALE6VetIaSl0ewiAsDUo5xq5fqeALaVODrwfB0bbKOToP9DpxX1aGXhoLTId-OJyf9VKu?key=CAmvbDG6f-5iZFMmcQosyw" alt=""><figcaption></figcaption></figure>

{% hint style="danger" %}
`Kotak keranjang` merepresentasikan variabel. `Buah` merepresentasikan data.

Dan jenis-jenis buah tersebut `merepresentasikan tipe data`.
{% endhint %}

### **2. Cara Mendeklarasikan Variabel**

Sintaks dasar untuk mendeklarasikan variabel:

```python
pythonCopyEditnama_variabel = nilai
```

**Contoh:**

```python
pythonCopyEditnama = "Alice"       # String
umur = 25            # Integer
tinggi = 1.65        # Float
is_student = True    # Boolean
```

### **3. Aturan Penamaan Variabel**

* **Harus dimulai dengan huruf** atau **underscore (\_)**, tetapi **tidak boleh dimulai dengan angka**.
  * ✔️ `nama`
  * ❌ `1nama`
* Hanya boleh mengandung huruf, angka, atau underscore.
  * ✔️ `nama_saya`
  * ❌ `nama@saya`
* Bersifat case-sensitive (huruf besar dan kecil dianggap berbeda).
  * Contoh: `nama` dan `Nama` adalah dua variabel yang berbeda.
* Tidak boleh menggunakan kata kunci Python sebagai nama variabel (seperti `if`, `for`, `while`, dll.).



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
