NAMA: M.RIDWAN ALMAHRI
NIM: (312510157)
KELAS: TI.25.A.2

Laporan Praktikum Python
1. Program latihan1.py
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

Program mengimpor fungsi random() dari modul random.

Pengguna diminta memasukkan nilai N sebagai batas jumlah data acak yang akan ditampilkan.

Variabel penghitung i diinisialisasi dengan nilai 0.

Program menjalankan perulangan while selama nilai i lebih kecil dari N.

Dalam setiap iterasi:

Menghasilkan angka acak dengan random().

Menampilkan data ke-i beserta angka acak tersebut.

Nilai i ditambah 1 setiap kali loop dijalankan.

Setelah perulangan selesai, program mencetak tulisan “Selesai”.

Screenshot Hasil Program

(Gambar dari file latihan1.py yang kamu kirim)
📸


2. Program latihan2.py
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

Inisialisasi modal sebesar 100 juta dan laba awal 0.

Gunakan perulangan for dari bulan ke-1 sampai bulan ke-8.

Tentukan laba per bulan dengan aturan:

Bulan 1–2 → laba 0.

Bulan 3–4 → 1% dari modal.

Bulan 5–7 → 5% dari modal.

Bulan 8 → 3% dari modal.

Hitung laba setiap bulan dan tambahkan ke total laba (laba += laba_bulan).

Tampilkan laba setiap bulan.

Setelah loop selesai, tampilkan total laba seluruh periode.

Screenshot Hasil Program

📸


3. Program latihan3.py
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

Inisialisasi saldo awal sebesar Rp 1.000.000.

Jalankan loop while True agar menu terus berulang.

Tampilkan menu:

(1) Tarik uang.

(2) Keluar.

Jika pengguna memilih 1:

Minta jumlah uang yang ingin ditarik.

Jika saldo mencukupi, kurangi saldo dan tampilkan pesan berhasil.

Jika tidak cukup, tampilkan pesan kesalahan.

Jika pengguna memilih 2:

Tampilkan pesan terima kasih dan keluar dari program dengan break.

Screenshot Hasil Program

📸


