# Dokumentasi UI/UX Proyek: Aplikasi "SimpleNotes" (Catatan Saya)

Selamat datang di repositori dokumentasi UI/UX untuk aplikasi **SimpleNotes** (atau disebut juga **Catatan Saya**). Repositori ini memuat spesifikasi lengkap, rancangan antarmuka, prinsip desain, serta alur navigasi dari purwarupa aplikasi manajemen produktivitas harian berbasis mobile.

---

##  Spesifikasi Proyek 

Berikut adalah tabel spesifikasi proyek antarmuka sesuai dengan standar dokumentasi akademik yang telah ditentukan:

| FIELD | VALUE |
| :--- | :--- |
| **1. PROJECT** | Simple Notes Mobile App ("Catatan Saya") |
| **2. PURPOSE** | Desain aplikasi catatan dan checklist yang ramah pengguna dengan fitur pengkodean warna, pelacakan linimasa, deteksi lokasi & bahasa otomatis, serta asisten AI cerdas. |
| **3. VERSION** | 1.0 (Tahap Desain Awal) |
| **4. DATE** | 06/08/2026 |

---

## 🧭 Alur Utama & Arsitektur Aplikasi

Desain aplikasi ini berfokus pada kesederhanaan (*minimalism*) dan fungsionalitas tingkat tinggi tanpa mendistorsi ruang kerja utama pengguna. Alur sistem dibagi menjadi 5 komponen layar utama berikut:

### 1. Layar Pembuka (Splash Screen)
* **Fungsi:** Menampilkan logo identitas aplikasi saat pertama kali dijalankan sebagai layar transisi pembuka sebelum mengarahkan pengguna ke halaman utama.

### 2. Tampilan Beranda Catatan (Main Notes Screen)
Halaman utama yang berfungsi sebagai pusat manajemen seluruh berkas catatan pengguna.
* **Bilah Pencarian (Search Bar):** Terletak di bagian paling atas untuk mencari kata kunci judul atau isi catatan secara cepat.
* **Daftar Catatan (Notes List View):** Menampilkan deretan kartu catatan (*cards*) dinamis yang memuat judul, cuplikan teks konten, dan tanggal pembuatan.
* **Sematkan Catatan (Pin):** Fitur interaktif menggunakan **Logo Bintang** di sudut kanan untuk menaruh catatan krusial agar selalu berada di posisi teratas.
* **Hapus Catatan (Delete):** Fitur penghapusan cepat menggunakan **Logo Sampah** di pinggir hasil catatan untuk membuang berkas secara instan.
* **Tombol Aksi Mengambang (Floating Action Button):** Tombol bulat dengan **Logo Tambah (+)** di pojok kanan bawah untuk membuat dokumen catatan baru.
* **Navigasi Bawah (Bottom Navigation):** Menggunakan sistem 3 tab menu utama:
    * `Notes` (Logo Catatan)
    * `To-Do Timeline` (Logo Kalender)
    * `AI Generator` (Logo Bintang Berkilau)

### 3. Tampilan Buat & Edit Catatan (Note Creation/Editing Screen)
Halaman lembar kerja fleksibel yang terbuka ketika pengguna menekan tombol tambah (+).
* **Input Teks Utama:** Kolom khusus untuk menambahkan judul catatan beserta isi teks catatan panjang secara terpisah.
* **Daftar Ceklis / Belanjaan:** Modul interaktif di bawah teks utama untuk membuat daftar poin pekerjaan atau belanjaan.
* **Tambah Item Ceklis:** Tombol tekstual "+ TAMBAH ITEM CHECKLIST" yang membuka modal pop-up input untuk memasukkan baris tugas baru ke dalam daftar.
* **Pemilih Warna Latar (Note Background Color Picker):** Barisan palet warna berbentuk lingkaran di bagian bawah untuk mengubah warna latar belakang kartu catatan (kuning, merah muda, biru, ungu, cokelat, hijau pastel) sebagai alat kategorisasi visual.
* **Deteksi Lokasi & Bahasa:** Ikon kompas/navigasi pintar di sudut bawah yang berfungsi mendeteksi lokasi geografis pengguna (Contoh: Bandung) dan secara otomatis menyesuaikan konteks penyapaan bahasa daerah setempat (Contoh: *"Sampurasun!"* untuk Sunda atau *"Sugeng Enjang!"* untuk Jawa).
* **Tombol Simpan:** Menggunakan **Logo Disket** di sudut kanan atas dan bawah untuk mengunci perubahan ke dalam penyimpanan lokal (*Room Database / Persistent Data*).

### 4. Tampilan Asisten & Generator AI (AI Assistance & Generation Screen)
Modul pintar berbasis kecerdasan buatan cerdas yang dapat diakses melalui menu navigasi bawah berlogo bintang berkilau (✨).
* **Input Topik Pengguna (User Topic Input):** Pengguna menuliskan instruksi spesifik (Contoh alur: *"apa saja yang harus dibawa ke gunung"*).
* **Integrasi Konteks AI:** Mesin AI secara otomatis menyerap data sekunder berupa deteksi lokasi dan bahasa pengguna untuk menyusun jawaban.
* **Hasil Pembuatan AI (AI Generation Result):** AI akan menghasilkan draf teks rekomendasi yang terstruktur rapi, lengkap, detail, dan otomatis terintegrasi dengan konteks lingkungan sekitar pengguna secara real-time.

### 5. Tampilan Linimasa Tugas (To-Do Timeline Screen)
Halaman pemantauan progres tugas harian yang diakses melalui ikon menu kalender (📅).
* **Daftar Tugas Berbasis Waktu:** Menampilkan seluruh daftar tugas (*task items*) lengkap dengan kotak centang interaktif (*checkbox*) yang diurutkan kronologis berdasarkan linimasa waktu.
* **Tambah Tugas:** Tombol "+ TAMBAH TUGAS" di area bawah untuk memasukkan tenggat waktu atau agenda baru ke dalam manajemen linimasa.

---

## 🎨 Panduan Sistem Desain (Design System Guidelines)

Untuk menjaga konsistensi visual dan kenyamanan mata pengguna (*Material Design*), antarmuka ini menetapkan aturan baku berikut:
* **Tipografi:** Menggunakan rumpun font Sans-Serif bersih (*Alea Sanif / Clean Sanif*) yang memberikan keterbacaan tinggi pada layar gawai.
* **Warna Latar:** Berbasis warna latar belakang pastel cerah yang bersih dan netral, dikombinasikan dengan pengkodean warna dinamis pada setiap kartu dokumen.
* **Aturan Sudut Elemen:** Setiap kartu (*cards*), kolom input, dan tombol aksi wajib menerapkan aturan sudut membulat halus (*Rounded Corners*) sebesar `16px`.
* **Sistem Grid:** Konsistensi jarak antar elemen (*layout spacing*) dikontrol ketat menggunakan kelipatan sistem grid `8pt`.
