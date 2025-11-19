## 📂 Kontributor

* **RAFI UBAYDILLAH** - *Mahasiswa UPB - 312410542.*

# 💻 Praktikum 8: PHP dan Database MySQL (CRUD Sederhana)

**Project CRUD (Create, Read, Update, Delete) sederhana menggunakan PHP Native dan database MySQL (dengan MySQLi).**

Praktikum ini bertujuan untuk memahami konsep dasar interaksi antara bahasa pemrograman PHP dengan database untuk mengelola data.

<br>

## ✨ Tampilan Aplikasi (Tema Modern Blue UI)

Tampilan aplikasi ini telah dimodifikasi menggunakan CSS dengan tema **Modern Biru Elegan** seperti aplikasi E-Learning (mobile app style) untuk meningkatkan *user experience*.

### Halaman Data Barang (READ)


### Halaman Tambah Barang (CREATE)


### Halaman Ubah Barang (UPDATE)


<br>

---

## 🛠️ Persiapan dan Instalasi

Ikuti langkah-langkah berikut untuk menjalankan project ini di komputer Anda:

### 1. Prasyarat
* **Web Server:** XAMPP, WAMP, atau sejenisnya.
* **Browser:** Google Chrome, Firefox, atau sejenisnya.
* **Text Editor:** VSCode, Sublime Text, atau sejenisnya.

### 2. Konfigurasi XAMPP
1.  Pastikan **Apache** dan **MySQL** sudah di-Start/Running melalui XAMPP Control Panel.

### 3. Struktur Project
1.  Buat folder project di `C:\xampp\htdocs\` dengan nama **`lab8_php_database`**.
2.  Di dalam folder tersebut, buat file-file PHP dan CSS berikut:
    * `koneksi.php`
    * `index.php`
    * `tambah.php`
    * `ubah.php`
    * `hapus.php`
    * `style.css` (Style Modern Blue UI yang sudah kita buat)
3.  Buat satu folder lagi untuk menyimpan gambar:
    * **`gambar/`**

### 4. Setup Database
1.  Buka `http://localhost/phpmyadmin` di browser.
2.  Buat database baru dengan nama: **`latihan1`**.
3.  Di dalam database `latihan1`, jalankan query SQL ini untuk membuat tabel `data_barang`:

```sql
CREATE TABLE data_barang (
    id_barang INT(10) AUTO_INCREMENT PRIMARY KEY,
    kategori VARCHAR(30),
    nama VARCHAR(30),
    gambar VARCHAR(100),
    harga_beli DECIMAL(10,0),
    harga_jual DECIMAL(10,0),
    stok INT(4)
);
