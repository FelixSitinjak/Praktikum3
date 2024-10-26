## **1. bilanganterbesar.py**

Program pertama yang akan dibuat adalah Program untuk menampilkan bilangan terbesar dari 3 Bilangan yang di Inputkan

Berikut flowchartnya

![image](https://github.com/user-attachments/assets/f58a00b8-cd7c-494f-b954-24809b793825)


**Program akan meminta kita untuk memasukkan 3 angka untuk dibandingkan :**

<img width="727" alt="Output 1" src="https://github.com/user-attachments/assets/a21a3911-a422-4fef-a6a8-cddb16b9d186">

**Penjelasan Code**

**1.**

```
def mencari_bilangan_terbesar(a, b, c):
    if a > b:
        if a > c:
            return a, "A adalah terbesar"
        else:
            return c, "C adalah terbesar"
    else:
        if b > c:
            return b, "B adalah terbesar"
        else:
            return c, "C adalah terbesar"

# Input bilangan A, B, C
print("Masukkan tiga bilangan:")
a = float(input("A: "))
b = float(input("B: "))
c = float(input("C: "))

# Menentukan bilangan terbesar
largest, message = mencari_bilangan_terbesar(a, b, c)

# Menampilkan hasil
print(f"\n{message}")
print(f"Bilangan terbesar adalah: {largest}")
```

1. Kita mendefinisikan function _mencari_bilangan_terbesar_ yang mengambil tiga parameter (a,b,c).
2. function tersebut menggunakan nested if-else statement untuk membandingkan angka yang di inputkan
3. Kemudian akan menampilkan Mana bilangan terbesar
4. Lalu di Program utamanya kita masukkan angka yang harus dimasukkan oleh user
5. Lalu kita panggil kembali function _mencari_biilangan_terbesar_
6. Lalu Output bilangan terbesar dari ketiga bilangan yang di input akan muncul
