# Kelompok 7 ->  Aplikasi Skor Bola Basket Sederhana Berbasis Tkinter

Naufal hisyam Attosy (2457051019)

Nicholah deva Yaman (2457051010)

M.Sultan Chaniago (2457051003)

Althaf zabran (2417053003)

# 🏀 Deskripsi Proyek

penjelasan:

project ini adalah menampilkan nilai score bola basket sederhana yang dibuat menggunakan bahasa pemrograman Python dengan pustaka Tkinter.
Aplikasi ini dirancang untuk mencatat, mengatur, dan menyimpan skor pertandingan bola basket antara dua tim. Pengguna dapat memasukkan nama tim, memperbarui skor secara manual selama pertandingan, serta menyimpan dan menampilkan riwayat pertandingan sebelumnya.

    tkinter: Membuat tampilan antarmuka (GUI)

    messagebox: Menampilkan dialog informasi

    PIL.Image, ImageTk: Untuk menampilkan gambar (background)

    csv: Menulis dan membaca data skor ke/dari file .csv

    os: Mengecek keberadaan file

    base64, BytesIO: Menangani gambar dalam format base64


# struktur dan penjelasan kode

    class AplikasiTkinter:

        def __init__(self, root):
    
    def tampilkan_halaman_awal(self):

- Membuat jendela utama (root) ukuran 600x500
- Menambahkan Canvas untuk gambar background
- Mengatur default skor dan nama tim
- Membuat dua Frame:
- frame_skor → Menampilkan & mengatur skor
- frame_developer → Menampilkan nama developer
- Menampilkan halaman awal

# 🔧 Fungsi-Fungsi Utama Aplikasi

1.Halaman Awal (Welcome Page)

~ Menampilkan sambutan "Welcome to Our Project"

~ Input untuk nama Tim A dan Tim B

~ Tombol navigasi:

- START → Masuk ke halaman pengaturan skor

- SCORE → Melihat riwayat skor pertandingan dari file CSV

- DEVELOPER → Menampilkan nama pembuat aplikasi

- QUIT → Menutup aplikasi

2.Halaman Skor (Score Page)

~ Menampilkan nama tim dan skor masing-masing

~ Tombol-tombol kendali untuk menambah/mengurangi poin:

+1, +3 → Tambah poin

-1, -3 → Kurangi poin (tidak bisa jika skor < nilai pengurangan)

~ Tombol tambahan:

- Reset → Mengatur ulang skor ke nol

- Simpan Skor → Menyimpan data pertandingan ke file CSV (basketball_scores.csv)

- Kembali → Kembali ke halaman awal

3.Riwayat Skor (Score History)
   
Menampilkan seluruh skor pertandingan yang pernah disimpan dalam file .csv

Format tampilan riwayat:

less
Copy
Edit
Team A: 12  vs  Team B: 8
Jika belum ada data: muncul notifikasi bahwa riwayat kosong

5.Sistem Penyimpanan File (CSV)

~ File basketball_scores.csv digunakan untuk menyimpan hasil pertandingan

~ Baris pertama adalah header (Nama Tim A, Skor A, Nama Tim B, Skor B)

~ Data disimpan setiap kali tombol "Simpan Skor" ditekan

6.Background Gambar

~ Tampilan latar belakang menggunakan gambar berbasis data base64 

~ Memberikan kesan visual yang lebih menarik dan profesional

# 🎯 Tujuan Proyek
- Membuat sistem pencatatan skor sederhana namun fungsional

- Melatih kemampuan menggunakan Tkinter, event-driven programming, dan file handling (CSV)

- Menyediakan tampilan antarmuka yang user-friendly untuk kegiatan olahraga informal atau presentasi tugas




