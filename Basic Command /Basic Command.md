## 1. Dasar-Dasar Python

### 👋 `print()` untuk Menampilkan Output

```python
print("Hello, world!")
```

---

## 2. Variabel dan Tipe Data

### 📦 Menyimpan Nilai

```python
hotel_room = 100
tax = hotel_room * 0.08
total = hotel_room + tax
```

### 👥 Membagi Biaya

```python
room_guests = 5
share_per_person = total / room_guests
print("Each person needs to pay: " + str(share_per_person))
```

### 🔄 Konversi Tipe Data

- `str()` → mengubah ke string
- `int()` → mengubah ke integer
- `float()` → mengubah ke float

---

## 3. Manipulasi String

```python
salutation = 'Dr.'
first_name = 'Prisha'
middle_name = 'Jai'
last_name = 'Agarwal'
suffix = 'Ph.D.'

print(salutation + ' ' + first_name + ' ' + middle_name + ' ' + last_name + ' ' + suffix)

```

---

## 4. Operator Perbandingan dan Logika

### 🔢 Perbandingan Numerik

```python
x == y     # sama dengan
x != y     # tidak sama
x < y      # lebih kecil
x >= y     # lebih besar atau sama
```

### 🔤 Perbandingan String

```python
"x" == "y" -> if words are the same, return True. Else, return false
"x" != "y" -> if words are not the same, return True. Else, return false
"x" < "y" -> if string "x" has smaller Unicode value than string "y", return True
"x" <= "y" -> if string "x" has smaller or equal Unicode value than string "y", return True
"x" > "y" -> if string "x" has larger Unicode value than string "y", return True
"x" >= "y" -> if string "x" has large or equal than string "y", return True
```
![Uploading image.png…]()


### 🧠 Fungsi `ord()` dan `chr()`

```python
print("tall" < "short")

print(chr(116)+chr(97)+chr(108)+chr(108))

print('aab' < 'aac')

ord('A')
```

---

## 5. Percabangan (`if`, `elif`, `else`)

```python
x = 3
if x == 0:
    print("Zero number")
elif x < 0:
    print("Negative number")
else:
    print("Positive number")
```

---

## 6. Fungsi (Function)

```python
def find_total_days(years, months, days):
    total = (years * 365) + (months * 30) + days
    return total

print(find_total_days(2, 6, 28))
```

```python
def convert_volume(fluid_ounce):
    ml = fluid_ounce * 29.5
    return ml
```
