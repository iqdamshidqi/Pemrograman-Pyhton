
# 🧑‍💻 **MINGGU 8 BASIC COMMAND**

## 1️⃣ **Menampilkan Output dengan `print()`**

Fungsi `print()` digunakan untuk menampilkan teks atau nilai di layar.

```python
print("Hello, world!")
```

🖨️ Output:

```
Hello, world!
```

---

## 2️⃣ **Variabel & Tipe Data**

### 📦 Menyimpan Nilai

Variabel menyimpan data seperti angka atau teks.

```python
hotel_room = 100
tax = hotel_room * 0.08
total = hotel_room + tax
```

---

### 👥 Membagi Biaya

Kita bisa hitung biaya per orang:

```python
room_guests = 5
share_per_person = total / room_guests
print("Each person needs to pay: " + str(share_per_person))
```

📌 Gunakan `str()` untuk mengubah angka menjadi teks agar bisa dicetak.

---

### 🔄 Konversi Tipe Data

| Fungsi    | Kegunaan                    |
| --------- | --------------------------- |
| `str()`   | Angka → String              |
| `int()`   | String atau float → Integer |
| `float()` | String atau integer → Float |

---

## 3️⃣ **Manipulasi String**

Gabungkan nama lengkap dengan tanda plus (`+`):

```python
salutation = 'Dr.'
first_name = 'Prisha'
middle_name = 'Jai'
last_name = 'Agarwal'
suffix = 'Ph.D.'

print(salutation + ' ' + first_name + ' ' + middle_name + ' ' + last_name + ' ' + suffix)
```

📌 Output: `Dr. Prisha Jai Agarwal Ph.D.`

---

## 4️⃣ **Operator Perbandingan dan Logika**

### 🔢 Perbandingan Angka

```python
x == y     # Sama dengan
x != y     # Tidak sama
x < y      # Lebih kecil
x >= y     # Lebih besar atau sama
```

---

### 🔤 Perbandingan String

```python
"apple" < "banana"  # True, karena 'a' < 'b'
"zoo" > "apple"     # True, karena 'z' > 'a'
```

📌 Perbandingan berdasarkan **urutan Unicode** huruf.

---

### 🧠 Fungsi `ord()` dan `chr()`

| Fungsi            | Kegunaan                         |
| ----------------- | -------------------------------- |
| `ord('A')` → `65` | Mengubah huruf jadi kode Unicode |
| `chr(65)` → `'A'` | Mengubah kode Unicode jadi huruf |

```python
print("tall" < "short")        # False
print(chr(116)+chr(97)+chr(108)+chr(108))  # tall
print('aab' < 'aac')           # True
```

---

## 5️⃣ **Percabangan: `if`, `elif`, `else`**

Gunakan untuk membuat keputusan berdasarkan kondisi.

```python
x = 3
if x == 0:
    print("Zero number")
elif x < 0:
    print("Negative number")
else:
    print("Positive number")
```

🧠 Python membaca dari atas ke bawah, dan hanya satu kondisi yang akan dijalankan.

---

## 6️⃣ **Fungsi (Function)**

### 🧮 Menghitung Total Hari

```python
def find_total_days(years, months, days):
    total = (years * 365) + (months * 30) + days
    return total

print(find_total_days(2, 6, 28))  # Output: 943
```

---

### 💧 Mengonversi Volume

```python
def convert_volume(fluid_ounce):
    ml = fluid_ounce * 29.5
    return ml

print(convert_volume(5))  # Output: 147.5
```

📌 Fungsi memudahkan kita untuk menghitung atau memproses sesuatu berulang kali.

