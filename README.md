LANGKAH LANGKAH LAPORAN PRAKTIKUM 3


Program latihan1.py


Tujuan Program
Menampilkan sejumlah bilangan acak sesuai dengan jumlah yang dimasukkan pengguna menggunakan perulangan while.
Kode Program
from random import random

n = int(input("Masukkan nilai N: "))
i = 0
while i < n:
    r = random()
    print("Data ke-", i + 1, "=>", r)
    i += 1

print("Selesai")
Alur Algoritma
1.	Program mengimpor fungsi random() dari modul random.
2.	Pengguna diminta memasukkan nilai N sebagai batas jumlah data acak yang akan ditampilkan.
3.	Variabel penghitung i diinisialisasi dengan nilai 0.
4.	Program menjalankan perulangan while selama nilai i lebih kecil dari N.
5.	Dalam setiap iterasi:
o	Menghasilkan angka acak dengan random().
o	Menampilkan data ke-i beserta angka acak tersebut.
o	Nilai i ditambah 1 setiap kali loop dijalankan.
6.	Setelah perulangan selesai, program mencetak tulisan “Selesai”.
<img width="1366" height="768" alt="Screenshot (40)" src="https://github.com/user-attachments/assets/60c3f433-275e-42c9-8038-b9928aeecd3a" />


Program latihan2.py


Tujuan Program
Menghitung dan menampilkan laba per bulan selama 8 bulan berdasarkan ketentuan persentase yang berbeda di setiap periode.
Kode Program
modal = 100000000
laba = 0

for bulan in range(1, 9):
    if bulan in [1, 2]:
        laba_bulan = 0
    elif bulan in [3, 4]:
        laba_bulan = modal * 0.01
    elif bulan in [5, 6, 7]:
        laba_bulan = modal * 0.05
    elif bulan == 8:
        laba_bulan = modal * 0.03

    laba += laba_bulan
    print(f"Laba bulan ke-{bulan} sebesar: {int(laba_bulan)}")

print(f"\nTotal laba adalah: {int(laba)}")
Alur Algoritma
1.	Inisialisasi modal sebesar 100 juta dan laba awal 0.
2.	Gunakan perulangan for dari bulan ke-1 sampai bulan ke-8.
3.	Tentukan laba per bulan dengan aturan:
o	Bulan 1–2 → laba 0.
o	Bulan 3–4 → 1% dari modal.
o	Bulan 5–7 → 5% dari modal.
o	Bulan 8 → 3% dari modal.
4.	Hitung laba setiap bulan dan tambahkan ke total laba (laba += laba_bulan).
5.	Tampilkan laba setiap bulan.
6.	Setelah loop selesai, tampilkan total laba seluruh periode.
<img width="1366" height="768" alt="Screenshot (37)" src="https://github.com/user-attachments/assets/854559cf-99ee-459e-ba18-8df7f22de261" />


Program latihan3.py


Tujuan Program
Membuat simulasi mesin ATM sederhana dengan fitur penarikan uang dan keluar dari menu.
Kode Program
saldo = 1000000

while True:
    print("\nSaldo saat ini: Rp", saldo)
    print("1. Tarik Uang")
    print("2. Keluar")

    pilihan = input("Pilih menu (1/2): ")

    if pilihan == "1":
        tarik = int(input("Masukkan jumlah penarikan: "))
        if tarik <= saldo:
            saldo -= tarik
            print("Penarikan berhasil!")
        else:
            print("Saldo tidak cukup!")
    elif pilihan == "2":
        print("Terima kasih telah menggunakan ATM!")
        break
Alur Algoritma
1.	Inisialisasi saldo awal sebesar Rp 1.000.000.
2.	Jalankan loop while True agar menu terus berulang.

o	(1) Tarik uang.
o	(2) Keluar.
4.	Jika pengguna memilih 1:
o	Minta jumlah uang yang ingin ditarik.
o	Jika saldo mencukupi, kurangi saldo dan tampilkan pesan berhasil.
o	Jika tidak cukup, tampilkan pesan kesalahan.
5.	Jika pengguna memilih 2:
   <img width="1366" height="768" alt="Screenshot (38)" src="https://github.com/user-attachments/assets/647e6c60-ef84-413b-9ec5-0355acc2469f" />

o	Tampilkan pesan terima kasih dan keluar dari program dengan break.

