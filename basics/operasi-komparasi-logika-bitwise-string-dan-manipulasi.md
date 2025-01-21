---
icon: dna
---

# Operasi komparasi, logika, bitwise, string dan manipulasi

## Operasi logika

Python mendukung berbagai operasi logika yang dapat digunakan untuk menggabungkan dan memanipulasi nilai kebenaran (boolean) dalam program

1. **Operator Logika AND (and):**

Operator and mengembalikan True jika kedua ekspresi yang diberikan sama-sama True, dan mengembalikan False jika salah satu atau kedua ekspresi tersebut False.

{% code title="Operator Logika AND (and):" lineNumbers="true" %}
```python
// Some code
a = True
b = False
c = True
print(a and b)  # Output: False
print(a and c)  # Output: True
```
{% endcode %}

2. **Operator Logika OR (or)**

Operator or mengembalikan True jika salah satu atau kedua ekspresi yang diberikan True, dan mengembalikan False jika kedua ekspresi tersebut False.

<pre class="language-python" data-title="Operator Logika OR (or)" data-line-numbers><code class="lang-python">// Some code
<strong>a = True
</strong>b = False
c = True
print(a or b)  # Output: True
print(b or c)  # Output: True
</code></pre>

3. Operator Logika NOT (not)

Operator not digunakan untuk membalik nilai kebenaran (boolean) dari suatu ekspresi. Jika ekspresi bernilai True, maka not akan mengembalikan False, dan sebaliknya.

{% code lineNumbers="true" %}
```python
// Some code
a = True
b = False
print(not a)  # Output: False
print(not b)  # Output: True
```
{% endcode %}

4. Kombinasi Operator Logika

Dalam contoh ini, ekspresi (a and b) menghasilkan False, ekspresi (c and not d) menghasilkan True, dan karena menggunakan operator logika OR (or), hasil akhirnya adalah True.

{% code lineNumbers="true" %}
```python
// Some code
a = True
b = False
c = True
d = False
print((a and b) or (c and not d))  # Output: True
```
{% endcode %}

5. Penggunaan Operasi Logika dalam Pernyataan If

{% code lineNumbers="true" %}
```python
// Some code
a = True
b = False

if a and not b:
    print("Kondisi terpenuhi")
else:
    print("Kondisi tidak terpenuhi")
```
{% endcode %}
