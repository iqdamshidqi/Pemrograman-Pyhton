# **🌀 MINGGU 9 LOOPING**

## ✅ Apa Itu Looping?

**Looping** adalah proses mengulang suatu perintah berkali-kali secara otomatis.

Misalnya: Kamu ingin mencetak “Halo!” sebanyak 5 kali, daripada mengetik `print("Halo!")` lima kali, kamu bisa menggunakan **loop**.

---

### 🧱 Jenis Loop di Python:

| Jenis Loop   | Keterangan                                                                 |
| ------------ | -------------------------------------------------------------------------- |
| `for` loop   | Digunakan ketika kita tahu **berapa kali** ingin mengulang.                |
| `while` loop | Digunakan ketika pengulangan dilakukan **selama suatu kondisi terpenuhi**. |

---

## 1. `for` Loop

### 🔹 Struktur Dasar:

```python
for variabel in range(banyak_perulangan):
    # perintah yang diulang
```

### 🔸 Contoh:

```python
for i in range(5):
    print("Halo!")
```

💡 `range(5)` artinya: angka dari 0 sampai 4 (total 5 kali).

**Output:**

```
Halo!
Halo!
Halo!
Halo!
Halo!
```

---

## 2. `while` Loop

### 🔹 Struktur Dasar:

```python
while kondisi:
    # perintah yang diulang
```

### 🔸 Contoh:

```python
x = 1
while x <= 3:
    print("Belajar Python")
    x += 1
```

**Output:**

```
Belajar Python
Belajar Python
Belajar Python
```

---

## 3. 🔁 Loop Bersarang (Nested Loop)

Kamu bisa menaruh loop di dalam loop, misalnya saat mencetak matriks:

```python
for i in range(3):        # baris
    for j in range(3):    # kolom
        print(j, end=" ")
    print()
```

**Output:**

```
0 1 2 
0 1 2 
0 1 2 
```

---

### 🛑 Menghentikan Loop

* `break` → menghentikan loop langsung
* `continue` → lompat ke iterasi berikutnya tanpa menjalankan baris setelahnya

```python
for i in range(5):
    if i == 3:
        break
    print(i)
```

**Output:**

```
0
1
2
```
