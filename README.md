## **1. Bilangan Terbesar** ##

**Penjelasan Code**

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
Kita mendefinisikan function mencari_bilangan_terbesar yang mengambil tiga parameter (a,b,c).
function tersebut menggunakan nested if-else statement untuk membandingkan angka yang di inputkan
Kemudian akan menampilkan Mana bilangan terbesar
Lalu di Program utamanya kita masukkan angka yang harus dimasukkan oleh user
Lalu kita panggil kembali function mencari_biilangan_terbesar
Lalu Output bilangan terbesar dari ketiga bilangan yang di input akan muncul

2. Bilangan N
Penjelasan code

# Input number of elements
N = int(input("Masukkan jumlah bilangan: "))

# Initialize maximum value to 0
max_val = 0

# Loop through N times to get the numbers
for i in range(1, N + 1):
    bilangan = int(input(f"Masukkan bilangan ke-{i}: "))
    
    # Check if the current number is greater than max_val
    if bilangan > max_val:
        max_val = bilangan

# Display the maximum number
print(f"Bilangan terbesar adalah: {max_val}")

Penjelasan: Di sini, kita membuat variabel max_val dan menginisialisasinya dengan nilai 0. Variabel ini akan digunakan untuk menyimpan nilai terbesar dari semua angka yang akan dibandingkan nanti. Kita mulai dengan nilai 0 karena kita belum membandingkan dengan angka apa pun.
Penjelasan: Bagian ini adalah sebuah loop (perulangan). Loop akan berjalan sebanyak N kali (sesuai dengan nilai yang dimasukkan pengguna sebelumnya).
for i in range(1, N + 1):: Baris ini memulai sebuah loop dengan variabel i yang akan mengambil nilai dari 1 hingga N. Setiap iterasi loop, nilai i akan bertambah 1.
bilangan = int(input(f"Masukkan bilangan ke-{i}: ")): Pada setiap iterasi, program akan meminta pengguna untuk memasukkan sebuah bilangan bulat. Bilangan yang dimasukkan akan disimpan dalam variabel bilangan. Format f"Masukkan bilangan ke-{i}: " digunakan untuk menampilkan pesan yang dinamis, di mana nilai i akan diganti dengan nomor urutan bilangan yang sedang diminta.
Setelah loop selesai berjalan, program akan mencetak hasil akhir, yaitu nilai terbesar yang ditemukan. Format f"Bilangan terbesar adalah: {max_val}" digunakan untuk menampilkan pesan yang disertai dengan nilai max_val.
