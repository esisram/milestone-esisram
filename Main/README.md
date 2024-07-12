# NihonTravel Website

[Fahima DayCare](https://www.fahimadaycare.site/)

<a href="https://www.fahimadaycare.site/" target="_blank">
<img src="../images/readme_picture/fahimadaycare_log.jpeg" alt="add relative path to image" 
width="200" height='250'/>
</a>

Website [**NihonTravel**](https://www.fahimadaycare.site/) adalah situs web yang menyediakan informasi tentang berbagai layanan dan produk yang terkait dengan perjalanan ke Jepang. Panduan ini menjelaskan langkah-langkah untuk membuat dan menjalankan website ini.

## Struktur Proyek

NihonTravel/
├── index.html
├── CSS/
│ └── style.css
└── README.md

## Langkah-langkah Membuat Website

### 1. Persiapan

Pastikan Anda memiliki struktur proyek seperti yang dijelaskan di atas. Buat folder utama bernama `NihonTravel`, di dalamnya buat folder `CSS` dan file `index.html` serta `style.css`.

### 2. HTML

File `index.html` berfungsi sebagai halaman utama dari website NihonTravel. Berikut adalah struktur utama dari file `index.html`:

- Bagian `<head>`: Mengandung metadata, judul halaman, dan link ke stylesheet serta font dari Google Fonts.
- Bagian `<body>`: Terdiri dari header, main content, dan footer.

#### Header

Header berisi navigasi dengan logo situs dan tombol "Sign In". Berikut adalah kode untuk header:

```html
<header class="navbar-container">
  <nav class="navbar">
    <h1 class="logo"><a href="./index.html">NihonTravel</a></h1>
    <ul class="nav-links">
      <li>Join now for an extra 10% Cash Back on purchases made in your first 7 days.*</li>
    </ul>
    <a href="#SignIn" class="header-btn">Sign In</a>
  </nav>
</header>
```

Main Content
Bagian utama berisi grid yang menampilkan berbagai kategori seperti "About Us", "Products", "Services", "Gallery", dan "Contact". Setiap item dalam grid ini adalah tautan ke halaman terkait.

```<main class="grid-container">
  <!-- Contoh item dalam grid -->
  <div id="items-1" class="grid-item">
    <a href="../1_about_us/index.html">
      <img src="about_us_image_url" alt="About Us" />
    </a>
    <p class="text-overlay">About Us</p>
  </div>
  <!-- Item lainnya mengikuti struktur yang sama -->
</main>
```

Footer
Footer tidak memiliki konten spesifik dan dapat diperluas sesuai kebutuhan
`<footer></footer>`

# tutorial custom domain :

## Persiapan:

1. Pastikan Anda memiliki akun Vercel dan Niagahoster:

- Daftar atau login ke akun Vercel di vercel.com.
- Daftar atau login ke akun Niagahoster di niagahoster.co.id.

2. Siapkan proyek Anda di Vercel:

- Buat proyek baru atau gunakan proyek yang sudah ada di Vercel.

## Langkah-Langkah:

1. Deploy Proyek Anda di Vercel:

- Jika belum, deploy proyek Anda di Vercel. Ikuti petunjuk pada dasbor Vercel untuk melakukan deploy.
- Setelah berhasil deploy, Anda akan mendapatkan URL default dari Vercel (misalnya your-project.vercel.app).

2. Konfigurasi Domain di Niagahoster:

- Login ke akun Niagahoster Anda.
- Masuk ke panel kontrol domain (misalnya cPanel atau Plesk).
- Pilih domain yang ingin Anda hubungkan ke Vercel.
  Tambahkan CNAME Record di Niagahoster:

Di panel kontrol domain, cari opsi untuk mengelola DNS (misalnya "Zone Editor" atau "DNS Management").
Tambahkan record CNAME baru dengan rincian sebagai berikut:
Name/Alias: Isi dengan subdomain yang ingin Anda gunakan (misalnya www atau kosongkan jika ingin menggunakan domain utama).
Type: Pilih CNAME.
Value/Target: Isi dengan URL default dari Vercel (misalnya your-project.vercel.app).
Simpan perubahan.
Konfigurasi Domain di Vercel:

Kembali ke dasbor Vercel.
Pilih proyek yang ingin Anda hubungkan dengan domain dari Niagahoster.
Masuk ke pengaturan proyek dan pilih "Domains".
Klik "Add Domain" dan masukkan domain yang sudah Anda tambahkan CNAME-nya di Niagahoster.
Vercel akan meminta Anda untuk melakukan verifikasi. Ikuti instruksi yang diberikan oleh Vercel untuk menyelesaikan verifikasi.
Verifikasi dan Propagasi:

Proses propagasi DNS bisa memakan waktu beberapa menit hingga 24 jam.
Setelah propagasi selesai, domain Anda akan terhubung ke proyek Vercel.
Troubleshooting:
Jika domain Anda tidak terhubung setelah 24 jam, periksa kembali pengaturan DNS di Niagahoster untuk memastikan record CNAME sudah benar.
Pastikan tidak ada konflik dengan record DNS lain yang mungkin sudah ada sebelumnya.
