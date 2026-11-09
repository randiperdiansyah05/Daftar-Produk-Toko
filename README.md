# Daftar-Produk-Toko

Project Pengantar JavaFX GUI – Level 2

1. Deskripsi Project

Aplikasi Daftar Produk Toko merupakan aplikasi desktop berbasis JavaFX yang dibuat untuk memenuhi tugas individu mata kuliah Pengantar JavaFX GUI – Level 2.

Aplikasi ini dikembangkan untuk membantu proses pencatatan dan pengelolaan data produk toko secara sederhana. Pengguna dapat menambahkan produk, melihat daftar produk, mencari produk berdasarkan nama, serta melihat informasi detail dari produk yang dipilih. Aplikasi menggunakan konsep Object-Oriented Programming (OOP) dengan pemisahan class Model, Controller, dan Data agar struktur program lebih terorganisasi dan mudah dikembangkan.

2. Teknologi yang Digunakan

Bahasa Pemrograman: Java 17
GUI Framework: JavaFX 21
Layout Interface: FXML
Styling: CSS
Build Management: Maven
IDE: NetBeans

3. Fitur Aplikasi

Aplikasi memiliki beberapa fitur utama:

1. Tambah Produk  
   Menambahkan produk baru dengan informasi kode produk, nama produk, kategori, dan harga.
2. Kode Produk Otomatis 
   Sistem menghasilkan kode produk secara otomatis dengan format P001, P002, P003, dan seterusnya.
3. Kategori Produk
   Menyediakan dua pilihan kategori, yaitu Makanan dan Minuman.
4. Upload Gambar Produk (Opsional)
   Pengguna dapat memilih gambar produk dari komputer untuk ditampilkan pada halaman detail.
5. Daftar Produk
   Menampilkan seluruh produk yang telah ditambahkan dalam bentuk tabel.
7. Pencarian Produk
   Memungkinkan pengguna mencari produk berdasarkan nama melalui tombol Cari.
8. Detail Produk
   Menampilkan informasi lengkap berdasarkan objek produk yang dipilih pada tabel.
9. Validasi Input
   Memastikan nama produk tidak kosong dan harga harus berupa angka dengan nilai lebih dari nol.
10. Navigasi Antarhalaman
   Menyediakan navigasi untuk berpindah antara halaman tambah produk, daftar produk, dan detail produk.

4. Struktur Tampilan Aplikasi
Aplikasi menggunakan tiga scene utama:
Scene 1 - Tambah Produk
Halaman untuk memasukkan data produk baru, meliputi kode produk otomatis, nama produk, kategori, harga, dan pilihan gambar produk.
Scene 2 - Daftar Produk
Halaman yang menampilkan seluruh produk dalam tabel serta menyediakan fitur pencarian dan tombol untuk melihat detail produk.
Scene 3 - Detail Produk
Halaman yang menampilkan informasi lengkap dari produk yang dipilih, termasuk gambar apabila tersedia.

6. Dokumentasi Screenshot
A. Halaman Tambah Produk
Menampilkan formulir untuk memasukkan data produk baru.
<img width="716" height="509" alt="Cuplikan layar 2026-11-09 202812" src="https://github.com/user-attachments/assets/225b201b-4fbd-459d-a837-4cc68c91954e" />
B. Halaman Daftar Produk
Menampilkan data produk yang telah berhasil ditambahkan ke dalam tabel.
<img width="686" height="509" alt="Cuplikan layar 2026-11-09 203024" src="https://github.com/user-attachments/assets/ccd3f616-0b9f-4229-8d08-78bb6adbb366" />
C. Halaman Detail Produk
Menampilkan informasi detail berdasarkan produk yang dipilih oleh pengguna.
<img width="677" height="507" alt="Cuplikan layar 2026-11-09 203102" src="https://github.com/user-attachments/assets/1377b886-1fbd-4bfc-812f-95c0c4bfba87" />

6. Struktur Folder Project

<img width="960" height="504" alt="image" src="https://github.com/user-attachments/assets/6207739d-9ad0-4d5b-81f3-33b80f863ab3" />

7. Konsep OOP yang Diterapkan

Class `Produk` digunakan sebagai model untuk merepresentasikan data setiap produk. Class ini memiliki atribut private, constructor, dan getter untuk mengakses informasi produk.

Pemisahan tanggung jawab class diterapkan sebagai berikut:

- **Produk:** Menyimpan atribut dan informasi produk.
- **DataProduk:** Mengelola penyimpanan data produk selama aplikasi berjalan.
- **FormController:** Mengelola proses input dan penambahan produk.
- **DaftarController:** Mengelola tabel dan pencarian produk.
- **DetailController:** Mengelola tampilan informasi produk yang dipilih.
- **Navigator:** Mengatur perpindahan antar-scene.

8. Penyimpanan Data
Data produk disimpan menggunakan `ObservableList` sehingga perubahan data dapat ditampilkan secara langsung pada tabel.
Aplikasi tidak menggunakan database. Data hanya tersimpan selama aplikasi berjalan dan akan hilang ketika aplikasi ditutup.

9. Cara Menjalankan Aplikasi
    1. Clone atau download repository GitHub.
    2. Buka project menggunakan NetBeans.
    3. Pastikan Java Development Kit (JDK) 17 sudah terpasang.
    4. Tunggu Maven mengunduh dependencies yang diperlukan.
    5. Lakukan Clean and Build.
    6. Jalankan project melalui NetBeans.

10. Pengujian Aplikasi

Pengujian dilakukan dengan beberapa skenario berikut:

- Menambahkan minimal tiga produk dengan kategori berbeda.
- Memastikan seluruh produk muncul pada tabel.
- Melakukan pencarian berdasarkan nama produk.
- Memilih produk dan membuka halaman detail.
- Memastikan tombol kembali dapat digunakan.
- Menguji validasi nama produk kosong.
- Menguji validasi harga kosong, bukan angka, atau bernilai nol maupun negatif.
