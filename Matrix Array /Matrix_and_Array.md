# 🔢 **MINGGU 10: MATRIX AND ARRAY (Python Programming)**

> Pada minggu ini, kamu akan mempelajari dasar manipulasi matriks dan array menggunakan bahasa Python. Materi mencakup pembuatan, akses, modifikasi, serta operasi matematika pada matriks.

---

## 🧮 No. 1 – Membuat Matriks Manual

```python
matrix = [[1, 2, 3, 4], 
          [5, 6, 7, 8],
          [9, 10, 11, 12]]

print("Matrix =", matrix)
```

📝 **Penjelasan:**

* Matriks dibuat sebagai list berisi list lainnya.
* Ini disebut **nested list**, cocok untuk merepresentasikan array 2 dimensi.

🖨️ **Output:**

```
Matrix = [[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12]]
```

---

## ⌨️ No. 2 – Input Matriks dari Pengguna

```python
Row = int(input("Enter the number of rows: "))
Column = int(input("Enter the number of columns: "))

matrix = []
print("Enter the entries row wise:")

for row in range(Row):
    a = []
    for column in range(Column):
        a.append(int(input()))
    matrix.append(a)

for row in range(Row):
    for column in range(Column):
        print(matrix[row][column], end=" ")
    print()
```

📝 **Penjelasan:**

* `input()` → menerima input sebagai string.
* `int()` → mengubah ke bilangan bulat.
* Nested loop digunakan untuk membangun matriks dari input.
* Loop kedua mencetak matriks dengan format baris × kolom.

---

## 🧠 MATERI LANJUT: Operasi Dasar Matriks dalam Python

---

### 📌 1. Membuat Matriks dengan List Comprehension

```python
matrix = [[column for column in range(4)] for row in range(4)]
print(matrix)
```

📝 **Penjelasan:**

* Membuat matriks 4×4 dengan setiap baris berisi `[0, 1, 2, 3]`.

🖨️ **Output:**

```
[[0, 1, 2, 3],
 [0, 1, 2, 3],
 [0, 1, 2, 3],
 [0, 1, 2, 3]]
```

---

### ✏️ 2. Akses dan Modifikasi Elemen Matriks

```python
X = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
row = column = 1
X[row][column] = 11
print(X)
```

📝 **Penjelasan:**

* Mengubah elemen baris ke-1, kolom ke-1 dari 5 menjadi 11.

🖨️ **Output:**

```
[[1, 2, 3], [4, 11, 6], [7, 8, 9]]
```

---

### 🔁 3. Akses Menggunakan Indeks Negatif

```python
row = -2
column = -1
X[row][column] = 21
print(X)
```

📝 **Penjelasan:**

* `-2` menunjuk baris ke-2 dari belakang, yaitu `[4, 11, 6]`.
* `-1` menunjuk elemen terakhir (6) → diubah menjadi 21.

🖨️ **Output:**

```
[[1, 2, 3], [4, 11, 21], [7, 8, 9]]
```

---

### ➕ 4. Penjumlahan Matriks dengan Nested Loop

```python
X = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
Y = [[9, 8, 7], [6, 5, 4], [3, 2, 1]]
result = [[0, 0, 0], [0, 0, 0], [0, 0, 0]]

for row in range(len(X)):
    for column in range(len(X[0])):
        result[row][column] = X[row][column] + Y[row][column]

for r in result:
    print(r)
```

🖨️ **Output:**

```
[10, 10, 10]
[10, 10, 10]
[10, 10, 10]
```

---

### ➕➖ 5. Penjumlahan & Pengurangan Matriks Sekaligus

```python
Add_result = [[X[row][column] + Y[row][column] for column in range(len(X[0]))] for row in range(len(X))]
Sub_result = [[X[row][column] - Y[row][column] for column in range(len(X[0]))] for row in range(len(X))]

print("Matrix Addition")
for r in Add_result:
    print(r)

print("\nMatrix Subtraction")
for r in Sub_result:
    print(r)
```

🖨️ **Output:**

```
Matrix Addition
[10, 10, 10]
[10, 10, 10]
[10, 10, 10]

Matrix Subtraction
[-8, -6, -4]
[-2, 0, 2]
[4, 6, 8]
```

---

## 📚 Kesimpulan

| Topik              | Penjelasan                                                |
| ------------------ | --------------------------------------------------------- |
| List of Lists      | Digunakan untuk membuat matriks di Python                 |
| Nested Loop        | Cocok untuk iterasi baris dan kolom                       |
| List Comprehension | Cara ringkas membangun matriks                            |
| Operasi Matriks    | Tambah dan kurang bisa dilakukan manual (loop) atau NumPy |

