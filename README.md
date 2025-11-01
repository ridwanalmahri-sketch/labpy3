NAMA: M.RIDWAN ALMAHRI
NIM: (312510157)
KELAS: TI.25.A.2


latihan1.py
Deskripsi Tugas
Program ini bertujuan untuk menampilkan N bilangan acak (random number) yang nilainya lebih kecil dari 0.5. Nilai N akan dimasukkan saat runtime. Program menggunakan kombinasi perulangan while dan fungsi random() dari modul random.
 Alur Algoritma
1.	Impor Modul: Mengimpor fungsi random dari modul random.
2.	Input N: Meminta pengguna memasukkan nilai integer untuk N (jumlah data yang akan ditampilkan).
3.	Inisialisasi: Mengatur counter perulangan (i) dimulai dari 0.
4.	Perulangan while: Perulangan akan terus berjalan selama i < N.
5.	Generate Angka Acak: Di dalam loop, fungsi random.random() dipanggil untuk menghasilkan bilangan acak (r) antara $0.0$ hingga $1.0$.
6.	Output: Bilangan acak tersebut dicetak bersama dengan nomor urut data ke-i + 1.
7.	Increment: Nilai counter i ditingkatkan (i = i + 1).
8.	Selesai: Setelah perulangan selesai, pesan "Selesai" ditampilkan.
 Hasil Eksekusi (latihan1.py)
latihan2.py
 Deskripsi Tugas
Program ini menghitung total laba usaha selama 8 bulan dengan modal awal Rp 100.000.000. Perhitungan laba didasarkan pada saldo bulan sebelumnya dan mengikuti skema persentase:
•	Bulan ke-1 dan ke-2: Laba 0%.
•	Bulan ke-3, ke-4, dan ke-5: Laba 1% dari saldo bulan sebelumnya.
•	Bulan ke-6, ke-7, dan ke-8: Laba 5% dari saldo bulan sebelumnya.
Alur Algoritma
1.	Inisialisasi: Variabel modal diatur ke 100.000.000.
2.	Perulangan for: Menggunakan perulangan for untuk iterasi dari bulan ke-1 hingga bulan ke-8 (range(1, 9)).
3.	Logika Laba: Di dalam loop, menggunakan struktur kondisional (if-elif) untuk menentukan persentase laba bulanan berdasarkan nomor bulan.
o	Jika bulan $\in \{1, 2\}$, laba_bulan = 0.
o	Jika bulan $\in \{3, 4, 5\}$, laba_bulan = modal * 0.01.
o	Jika bulan $\in \{6, 7, 8\}$, laba_bulan = modal * 0.05.
4.	Update Saldo: Saldo modal diperbarui dengan menambahkan laba_bulan (modal += laba_bulan).
5.	Output Bulanan: Mencetak laba yang diperoleh pada bulan tersebut.
6.	Total Laba: Mencetak total laba setelah 8 bulan (diasumsikan laba adalah variabel yang menyimpan total laba yang dihitung secara kumulatif atau dihitung dari perbedaan total saldo akhir dengan modal awal). Berdasarkan kode, variabel laba tampaknya diakumulasi untuk menyimpan total laba.
Hasil Eksekusi (latihan2.py)
latihan3.py
Deskripsi Tugas
Program ini mensimulasikan mesin ATM sederhana dengan saldo awal Rp 1.000.000. Pengguna dapat memilih untuk Tarik Uang atau Keluar dari sistem.
Alur Algoritma
1.	Inisialisasi: Variabel saldo diatur ke 1.000.000.
2.	Perulangan Utama while: Menggunakan while True untuk menampilkan menu ATM secara berulang hingga pengguna memilih untuk keluar.
3.	Tampilan Menu: Mencetak pilihan menu (1. Tarik Uang, 2. Keluar).
4.	Input Pilihan: Meminta pengguna memasukkan pilihan menu (pilihan).
5.	Logika Tarik Uang (Pilihan 1):
o	Meminta pengguna memasukkan jumlah_penarikan.
o	Pengecekan Saldo: Jika jumlah_penarikan $\le$ saldo, maka:
	saldo dikurangi dengan jumlah_penarikan.
	Menampilkan pesan "Penarikan berhasil!".
o	Saldo Tidak Cukup: Jika jumlah_penarikan $>$ saldo, menampilkan pesan "Saldo tidak cukup!".
6.	Logika Keluar (Pilihan 2):
o	Menampilkan pesan terima kasih.
o	Menggunakan break untuk keluar dari perulangan while True, mengakhiri program.


