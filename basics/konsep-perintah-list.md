---
icon: ellipsis-stroke
---

# Konsep Perintah List

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

## **List dalam Python**

**List** adalah salah satu tipe data koleksi di Python yang digunakan untuk menyimpan banyak item dalam satu variabel. List adalah struktur data yang paling umum digunakan karena fleksibilitasnya.

***

## **Ciri-Ciri List**

1. **Terurut**: Elemen dalam list memiliki indeks yang dimulai dari 0.
2. **Dapat diubah (mutable)**: Elemen dalam list dapat ditambahkan, diubah, atau dihapus setelah list dibuat.
3. **Mendukung berbagai tipe data**: List dapat menyimpan elemen dengan tipe data yang berbeda (misalnya, integer, string, bahkan list lain).
4. **Ditandai dengan tanda kurung siku (`[]`)**.

***

## **Cara Membuat List**

```python
# List kosong
my_list = []

# List dengan elemen
my_list = [1, 2, 3, 4, 5]

# List dengan berbagai tipe data
my_list = [1, "Hello", 3.14, True]

# List bersarang (list di dalam list)
nested_list = [[1, 2, 3], ["a", "b", "c"]]
```

***

## **Operasi Dasar pada List**

1.  **Mengakses Elemen**

    * Gunakan indeks untuk mengakses elemen (indeks mulai dari `0`).

    ```python
    my_list = [10, 20, 30, 40]
    print(my_list[0])  # Output: 10
    print(my_list[-1])  # Output: 40 (indeks negatif untuk elemen terakhir)
    ```
2.  **Menambah Elemen**

    * `append()`: Menambahkan elemen di akhir list.
    * `insert()`: Menyisipkan elemen di posisi tertentu.

    ```python
    my_list = [1, 2, 3]
    my_list.append(4)  # [1, 2, 3, 4]
    my_list.insert(1, 10)  # [1, 10, 2, 3, 4]
    ```
3.  **Menghapus Elemen**

    * `remove()`: Menghapus elemen berdasarkan nilai.
    * `pop()`: Menghapus elemen berdasarkan indeks (jika tidak ada indeks, elemen terakhir dihapus).
    * `clear()`: Menghapus semua elemen dalam list.

    ```python
    my_list = [1, 2, 3, 4]
    my_list.remove(2)  # [1, 3, 4]
    my_list.pop(1)  # [1, 4]
    my_list.clear()  # []
    ```
4.  **Mengubah Elemen**

    ```python
    my_list = [1, 2, 3]
    my_list[1] = 20  # [1, 20, 3]
    ```
5.  **Menggabungkan List**

    * Dengan `+` operator.
    * Menggunakan `extend()`.

    ```python
    list1 = [1, 2, 3]
    list2 = [4, 5, 6]
    combined = list1 + list2  # [1, 2, 3, 4, 5, 6]
    list1.extend(list2)  # list1 menjadi [1, 2, 3, 4, 5, 6]
    ```
6.  **Memeriksa Elemen**

    ```python
    my_list = [1, 2, 3, 4]
    print(3 in my_list)  # Output: True
    print(5 not in my_list)  # Output: True
    ```

***

## **Fungsi dan Metode List**

| **Metode**     | **Deskripsi**                                                |
| -------------- | ------------------------------------------------------------ |
| `append(x)`    | Menambahkan elemen `x` di akhir list.                        |
| `insert(i, x)` | Menyisipkan elemen `x` pada indeks `i`.                      |
| `remove(x)`    | Menghapus elemen pertama dengan nilai `x`.                   |
| `pop(i)`       | Menghapus elemen pada indeks `i` (default: elemen terakhir). |
| `clear()`      | Menghapus semua elemen dalam list.                           |
| `index(x)`     | Mengembalikan indeks pertama dari elemen `x`.                |
| `count(x)`     | Menghitung jumlah elemen `x` dalam list.                     |
| `sort()`       | Mengurutkan elemen dalam list secara ascending (default).    |
| `reverse()`    | Membalik urutan elemen dalam list.                           |
| `copy()`       | Mengembalikan salinan dari list.                             |

***

## **Contoh Lengkap**

```python
# Membuat list
fruits = ["apple", "banana", "cherry"]

# Menambah elemen
fruits.append("orange")
print(fruits)  # ['apple', 'banana', 'cherry', 'orange']

# Mengubah elemen
fruits[1] = "blueberry"
print(fruits)  # ['apple', 'blueberry', 'cherry', 'orange']

# Menghapus elemen
fruits.remove("cherry")
print(fruits)  # ['apple', 'blueberry', 'orange']

# Menggabungkan list
more_fruits = ["grape", "mango"]
fruits.extend(more_fruits)
print(fruits)  # ['apple', 'blueberry', 'orange', 'grape', 'mango']

# Mengurutkan list
fruits.sort()
print(fruits)  # ['apple', 'blueberry', 'grape', 'mango', 'orange']
```

Jika ada hal lain yang ingin dijelaskan lebih lanjut, beri tahu saya! 😊
