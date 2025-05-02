# **🔢 MINGGU 10 MATRIX AND ARRAY**

## No. 1
```python
matrix = [[1, 2, 3, 4], 
          [5, 6, 7, 8],
          [9, 10, 11, 12]]

print("Matrix =", matrix)
```
---
`matrix =` list dalam vector.

## No. 2

```python
Row = int(input("Enter the number of rows: "))
Column = int(input("Enter the number of columns: "))

# Initialize matrix
matrix = []
print("Enter the entries row wise:")

# For user input
# A for loop for row entries
for row in range(Row):
    a = []
    # A for loop for column entries
    for column in range(Column):
        a.append(int(input()))
    matrix.append(a)

# For printing the matrix
for row in range(Row):
    for column in range(Column):
        print(matrix[row][column], end=" ")
    print()
```

---

### 📌 Penjelasan :

* `input()` digunakan untuk menerima input dari pengguna dalam bentuk string.
* `int()` mengubah input string menjadi bilangan bulat (integer).
* `matrix = []` membuat list kosong yang akan diisi dengan data dari pengguna.
* `a.append()` menambahkan value ke variable a.


