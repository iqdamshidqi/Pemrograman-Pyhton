Berikut adalah **kode Python** yang ditampilkan pada gambar tersebut, saya salin ulang agar bisa kamu gunakan atau modifikasi:

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

### 📌 Penjelasan Singkat:

* Program ini meminta pengguna untuk memasukkan ukuran matriks (jumlah baris dan kolom).
* Kemudian, pengguna diminta mengisi setiap elemen satu per satu sesuai jumlah baris dan kolom.
* Setelah semua elemen dimasukkan, program mencetak matriks dalam format baris × kolom.

Ingin saya ubah ke versi NumPy atau tambahkan fitur seperti penjumlahan atau perkalian dua matriks?
