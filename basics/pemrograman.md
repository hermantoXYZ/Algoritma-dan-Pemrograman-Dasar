---
icon: elevator
---

# Pemrograman: perintah seleksi (if... else)

Perintah seleksi **`if...else`** dalam Python digunakan untuk melakukan pengambilan keputusan berdasarkan kondisi tertentu. Berikut adalah penjelasan dan contoh penggunaan **`if...else`**:

#### **Sintaks Dasar**

{% code lineNumbers="true" %}
```python
if kondisi:
    # blok kode jika kondisi benar (True)
else:
    # blok kode jika kondisi salah (False)
```
{% endcode %}

#### **Contoh 1: Penggunaan Sederhana**

{% code lineNumbers="true" %}
```python
angka = 10

if angka > 0:
    print("Angka adalah bilangan positif.")
else:
    print("Angka adalah bilangan nol atau negatif.")
```
{% endcode %}

**Penjelasan:**

* Jika kondisi `angka > 0` bernilai **True**, maka program mencetak "Angka adalah bilangan positif."
* Jika kondisi **False**, program mencetak "Angka adalah bilangan nol atau negatif."

#### **Contoh 2: Dengan Percabangan Lebih dari Satu (if...elif...else)**

{% code lineNumbers="true" %}
```python
nilai = 75

if nilai >= 85:
    print("Nilai Anda: A")
elif nilai >= 70:
    print("Nilai Anda: B")
elif nilai >= 55:
    print("Nilai Anda: C")
else:
    print("Nilai Anda: D")
```
{% endcode %}

**Penjelasan:**

* Program akan mengevaluasi setiap kondisi `if` dan `elif` dari atas ke bawah.
* Jika kondisi pertama **True**, maka blok kode tersebut dijalankan, dan program berhenti mengevaluasi kondisi lainnya.
* Jika semua kondisi tidak terpenuhi, blok `else` akan dijalankan.

#### **Contoh 3: Seleksi Bersarang (Nested if)**

{% code lineNumbers="true" %}
```python
umur = 20
status_pelajar = True

if umur >= 18:
    if status_pelajar:
        print("Anda pelajar dewasa.")
    else:
        print("Anda bukan pelajar.")
else:
    print("Anda masih di bawah umur.")
```
{% endcode %}

**Penjelasan:**

* **Seleksi bersarang** adalah ketika sebuah perintah `if` berada di dalam blok `if` atau `else`.
* Dalam contoh ini, kondisi pertama memeriksa apakah `umur >= 18`. Jika benar, maka memeriksa kondisi `status_pelajar`.

#### **Penggunaan If Tanpa Else**

Blok `else` bersifat opsional. Jika hanya ingin mengeksekusi sesuatu ketika kondisi tertentu terpenuhi, Anda bisa hanya menggunakan `if`:

```python
angka = 10

if angka > 0:
    print("Angka positif.")
```

#### **Penggunaan Sederhana dengan Operator Ternary**

Python juga mendukung operator ternary untuk seleksi sederhana:

```python
angka = 10
pesan = "Angka positif" if angka > 0 else "Angka nol atau negatif"
print(pesan)
```

#### Catatan

* Pastikan indentasi blok kode pada Python benar, karena indentasi menentukan struktur kode.
* Gunakan **`elif`** jika memiliki lebih dari dua kondisi.
