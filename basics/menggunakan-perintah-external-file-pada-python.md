---
icon: folder-grid
---

# Menggunakan Perintah External File Pada Python

Python menyediakan fitur untuk bekerja dengan **file eksternal** seperti membaca, menulis, atau mengedit file teks (`.txt`), file CSV, file JSON, dan lainnya. Berikut adalah penjelasan dan contoh cara menggunakan file eksternal dalam Python.

***

#### **1. Membaca File Eksternal**

**a. Membaca File Teks**

Menggunakan mode `r` (read) untuk membaca file teks.

```python
# Membaca file teks
with open("contoh.txt", "r") as file:
    content = file.read()
    print(content)
```

**b. Membaca Baris per Baris**

```python
# Membaca file baris per baris
with open("contoh.txt", "r") as file:
    for line in file:
        print(line.strip())  # strip() untuk menghapus karakter newline
```

***

#### **2. Menulis ke File Eksternal**

**a. Menulis File Baru**

Menggunakan mode `w` (write) untuk menulis file baru (menghapus konten lama jika file sudah ada).

```python
# Menulis ke file
with open("contoh_baru.txt", "w") as file:
    file.write("Halo, ini adalah file baru!\n")
    file.write("Baris kedua dalam file.")
```

**b. Menambahkan ke File yang Sudah Ada**

Menggunakan mode `a` (append) untuk menambahkan konten ke file tanpa menghapus data lama.

```python
# Menambahkan data ke file
with open("contoh_baru.txt", "a") as file:
    file.write("\nBaris baru ditambahkan.")
```

***

#### **3. Membaca dan Menulis File CSV**

**Membaca File CSV**

Menggunakan modul `csv` untuk membaca file CSV.

```python
import csv

# Membaca file CSV
with open("data.csv", "r") as csv_file:
    reader = csv.reader(csv_file)
    for row in reader:
        print(row)
```

**Menulis File CSV**

```python
import csv

# Menulis ke file CSV
with open("data_baru.csv", "w", newline="") as csv_file:
    writer = csv.writer(csv_file)
    writer.writerow(["Nama", "Umur", "Kota"])  # Menulis header
    writer.writerow(["Ali", 25, "Jakarta"])
    writer.writerow(["Budi", 30, "Bandung"])
```

***

#### **4. Membaca dan Menulis File JSON**

**Membaca File JSON**

Menggunakan modul `json` untuk membaca file JSON.

```python
import json

# Membaca file JSON
with open("data.json", "r") as json_file:
    data = json.load(json_file)
    print(data)
```

**Menulis File JSON**

```python
import json

# Menulis ke file JSON
data = {"nama": "Ali", "umur": 25, "kota": "Jakarta"}

with open("data_baru.json", "w") as json_file:
    json.dump(data, json_file, indent=4)
```

***

#### **5. Contoh Lengkap**

**Membaca dan Menulis File Teks**

```python
# Menulis file teks
with open("example.txt", "w") as file:
    file.write("Ini adalah contoh file teks.\n")
    file.write("Python sangat seru!")

# Membaca file teks
with open("example.txt", "r") as file:
    content = file.read()
    print(content)
```

**Membaca dan Menulis File CSV**

```python
import csv

# Menulis file CSV
with open("example.csv", "w", newline="") as file:
    writer = csv.writer(file)
    writer.writerow(["ID", "Nama", "Usia"])
    writer.writerow([1, "Ali", 25])
    writer.writerow([2, "Budi", 30])

# Membaca file CSV
with open("example.csv", "r") as file:
    reader = csv.reader(file)
    for row in reader:
        print(row)
```

**Membaca dan Menulis File JSON**

```python
import json

# Menulis file JSON
data = {
    "siswa": [
        {"nama": "Ali", "usia": 25},
        {"nama": "Budi", "usia": 30}
    ]
}
with open("example.json", "w") as file:
    json.dump(data, file, indent=4)

# Membaca file JSON
with open("example.json", "r") as file:
    data = json.load(file)
    print(data)
```

***

#### **Mode Akses File**

| **Mode** | **Deskripsi**                                                 |
| -------- | ------------------------------------------------------------- |
| `r`      | Membuka file hanya untuk membaca.                             |
| `w`      | Membuka file untuk menulis (menghapus data lama jika ada).    |
| `a`      | Membuka file untuk menambah data di akhir file.               |
| `r+`     | Membuka file untuk membaca dan menulis.                       |
| `w+`     | Membuka file untuk menulis dan membaca (menghapus data lama). |
| `a+`     | Membuka file untuk menambah dan membaca.                      |
