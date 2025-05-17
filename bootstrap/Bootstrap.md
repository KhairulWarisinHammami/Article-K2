### Bootstrap
Bootstrap adalah framework front-end paling populer di dunia yang membantu developer membangun situs web dan aplikasi yang intuitif, responsif, dan estetis dengan cepat. Dikembangkan pertama kali oleh para engineer dari Twitter pada tahun 2011, Bootstrap kini berada di versi 5.x dengan komunitas yang sangat aktif dan ekosistem yang kaya.

#### A. Pengantar

Pada dasarnya, Bootstrap menyederhanakan proses pembuatan antarmuka (UI) web dengan menyediakan komponen HTML, CSS, dan JavaScript siap pakai. Alih-alih menulis CSS dari nol untuk tombol, form, navbar, dan layout, Anda cukup mengimpor pustaka Bootstrap dan memanfaatkan kelas-kelas utilitas serta komponen yang telah dirancang secara konsisten. Hal ini memungkinkan tim developer fokus pada logika dan konten, tanpa harus khawatir tentang detail styling dan responsivitas.

Lebih jauh lagi, Bootstrap dibangun di atas sistem grid fleksibel yang memudahkan penataan elemen pada berbagai ukuran layar, mulai dari ponsel hingga desktop besar. Dengan demikian, Anda dapat menciptakan desain yang adaptif dan user-friendly tanpa harus menulis banyak media query secara manual. Selain itu, dokumentasi Bootstrap sangat komprehensif, lengkap dengan contoh kode dan animasi interaktif, sehingga baik pemula maupun developer berpengalaman dapat dengan mudah memahami dan menerapkan konsep-konsepnya.

#### B. Keunggulan
- Kemudahan Implementasi
- Responsivitas Otomatis
- Konsistensi Desain
- Variasi Komponen Lengkap
- Kustomisasi Mudah dengan SCSS
- Performance-Friendly
- Ecosystem dan Plugin

#### C. Instalasi Bootstrap

Panduan ini menjelaskan cara menginstal dan menggunakan **Bootstrap**, framework CSS populer untuk membuat antarmuka web yang responsif dan modern.


##### - Menggunakan CDN (Cara Termudah)

Jika Anda tidak ingin mengunduh file apa pun, Anda bisa menggunakan Bootstrap langsung dari CDN.

Tambahkan baris berikut di bagian `<head>` dan sebelum tag penutup `</body>` pada file HTML Anda:

```html
<!-- CSS Bootstrap -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">

<!-- JS Bootstrap (opsional, jika menggunakan komponen seperti modal, dropdown, dsb.) -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
```

 ##### - Instalasi via NPM (Node Package Manager) 
 
 Jika Anda menggunakan Node.js dan ingin mengelola dependensi menggunakan npm:  
 'npm install bootstrap'

 Kemudian, impor Bootstrap di file JavaScript atau SCSS Anda:  
 ```js
      // Jika menggunakan JavaScript
import 'bootstrap/dist/js/bootstrap.bundle.min.js';
import 'bootstrap/dist/css/bootstrap.min.css';
```

 ##### - Download Manual

 Jika Anda ingin menyimpan file Bootstrap secara lokal:  
 1. Kunjungi https://getbootstrap.com
 2. Klik tombol Download.
 3. Ekstrak file ZIP.
 4. Link file CSS dan JS ke HTML Anda:
```html
    <!-- CSS lokal -->
<link rel="stylesheet" href="path/to/bootstrap.min.css">

<!-- JS lokal -->
<script src="path/to/bootstrap.bundle.min.js"></script>
```
#### D. Sistem Grid di Bootstrap


Bootstrap menggunakan sistem grid berbasis 12 kolom yang sangat fleksibel. Grid ini memungkinkan Anda membuat layout responsif hanya dengan menambahkan class tertentu.
Contoh Struktur Grid  
```html
        <div class="container mt-4">
    <div class="row">
      <div class="col-md-4 bg-primary text-white p-3 border">Kolom 1</div>
      <div class="col-md-4 bg-success text-white p-3 border">Kolom 2</div>
    </div>
  </div>
```
- `.container`: Membuat padding horizontal dan mengatur lebar responsif.
- `.row`: Mengatur baris.
- Hasil:
  ![bootstrap Grid](https://github.com/KhairulWarisinHammami/Article-K2/blob/Bootstrap-fix/bootstrap/Grid%202.png)
  

  #### E. Komponen-Komponen Bootstrap

  Bootstrap menyediakan berbagai komponen UI siap pakai yang dapat digunakan langsung, Contohnya:
  - Tombol (Button)
    ```html
    <button class="btn btn-primary">Klik Saya</button>
    ```

    Hasil:
    
    ![Button](https://github.com/KhairulWarisinHammami/Article-K2/blob/Bootstrap-fix/bootstrap/BUTTON.png)

    
  - Navbar

```html
<nav class="navbar navbar-expand-lg navbar-dark bg-primary">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Brand</a>
    <button
      class="navbar-toggler"
      type="button"
      data-bs-toggle="collapse"
      data-bs-target="#navbarNav"
      aria-controls="navbarNav"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav ms-auto">
        <li class="nav-item">
          <a class="nav-link active" href="#">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Features</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Pricing</a>
        </li>
        <li class="nav-item">
          <a class="nav-link disabled">Disabled</a>
        </li>
      </ul>
    </div>
  </div>
</nav>
```
Hasil:

![Navbar](https://github.com/KhairulWarisinHammami/Article-K2/blob/Bootstrap-fix/bootstrap/NAvbar2.png)

- Cards
  ```html
  <div class="card" style="width: 18rem;">
  <img src="..." class="card-img-top" alt="..." />
  <div class="card-body">
    <h5 class="card-title">Judul Kartu</h5>
    <p class="card-text">Deskripsi singkat.</p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>

![cards](https://github.com/KhairulWarisinHammami/Article-K2/blob/Bootstrap-fix/bootstrap/Cards.png)

- Form

```html
<div class="card" style="width: 18rem;">
  <img src="..." class="card-img-top" alt="..." />
  <div class="card-body">
    <h5 class="card-title">Judul Kartu</h5>
    <p class="card-text">Deskripsi singkat.</p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>
```

Hasil:
![Form](https://github.com/KhairulWarisinHammami/Article-K2/blob/Bootstrap-fix/bootstrap/Form.png)


#### F. Contoh Penerapan: Halaman Sederhana

Berikut contoh lengkap kode dan hasil sebuah halaman profil sederhana:  
```html
<!DOCTYPE html>
<html lang="id">
  <head>
    <meta charset="UTF-8" />
    <meta
      name="viewport"
      content="width=device-width, initial-scale=1.0"
    />
    <title>Profil Saya</title>
    <link
      href="https://cdn.jsdelivr.net/npm/bootstrap@5.4.3/dist/css/bootstrap.min.css"
      rel="stylesheet"
    />
  </head>
  <body>
    <!-- Navbar -->
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
      <div class="container">
        <a class="navbar-brand" href="#">Profil</a>
      </div>
    </nav>

    <!-- Hero Section -->
    <section class="py-5 text-center bg-light">
      <div class="container">
        <h1 class="display-4">Halo, Saya Waris!</h1>
        <p class="lead">
          Mahasiswa Ilmu Komputer yang suka coding dan desain.
        </p>
        <a href="#about" class="btn btn-primary btn-lg">Tentang Saya</a>
      </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-5">
      <div class="container">
        <div class="row align-items-center">
          <div class="col-md-4 text-center">
            <img
              src="https://via.placeholder.com/200"
              class="rounded-circle img-fluid"
              alt="Foto Profil"
            />
          </div>
          <div class="col-md-8">
            <h2>Tentang Saya</h2>
            <p>
              Saya sedang menempuh studi Ilmu Komputer di Universitas Al Azhar.
              Hobi saya basket, musik, dan membangun proyek web menggunakan
              framework modern.
            </p>
            <a href="#contact" class="btn btn-outline-primary"
              >Hubungi Saya</a
            >
          </div>
        </div>
      </div>
    </section>

    <!-- Footer -->
    <footer class="bg-dark text-white text-center py-3">
      &copy; 2025 Waris. All rights reserved.
    </footer>

    <script
      src="https://cdn.jsdelivr.net/npm/bootstrap@5.4.3/dist/js/bootstrap.bundle.min.js"
    ></script>
  </body>
</html>
```

Penjelasan Kode:

##### Markdown

Ini adalah halaman web sederhana bertema "Profil Saya" yang dibuat menggunakan **HTML5** dan **Bootstrap 5.4.3**. Halaman ini memiliki struktur dasar seperti Navbar, Hero Section, About Section, dan Footer. Menggunakan teknologi html5 dan Bootstrap 5.4.3 (CDN)

##### Navbar

```html
<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <div class="container">
    <a class="navbar-brand" href="#">Profil</a>
  </div>
</nav>
```
- Navbar bergaya gelap (bg-dark) dan teks putih (navbar-dark)
- Menggunakan container Bootstrap agar rapi dan responsif

##### Hero Section

```html
<section class="py-5 text-center bg-light">
  <div class="container">
    <h1 class="display-4">Halo, Saya Waris!</h1>
    <p class="lead">Mahasiswa Ilmu Komputer yang suka coding dan desain.</p>
    <a href="#about" class="btn btn-primary btn-lg">Tentang Saya</a>
  </div>
</section>
```

- Tampilan pembuka dengan headline dan CTA
- Menggunakan utilitas Bootstrap (py-5, display-4, btn)

##### About Section

```html
<section id="about" class="py-5">
  <div class="container">
    <div class="row align-items-center">
      <div class="col-md-4 text-center">
        <img src="https://via.placeholder.com/200" class="rounded-circle img-fluid" alt="Foto Profil" />
      </div>
      <div class="col-md-8">
        <h2>Tentang Saya</h2>
        <p>...</p>
        <a href="#contact" class="btn btn-outline-primary">Hubungi Saya</a>
      </div>
    </div>
  </div>
</section>
```

- Terdiri dari dua kolom: foto profil dan deskripsi diri
- Responsif dengan row, col-md-4, dan col-md-8
- Gambar dibulatkan (rounded-circle) dan responsif (img-fluid)

##### Footer

```html
<footer class="bg-dark text-white text-center py-3">
  &copy; 2025 Waris. All rights reserved.
</footer>
```

- Tampilan sederhana di bagian bawah halaman
- Warna latar belakang gelap dan teks putih

##### Hasil Halaman Sederhana Menggunakan Bootstrap

![Hasil Halaman](https://github.com/KhairulWarisinHammami/Article-K2/blob/Bootstrap-fix/bootstrap/Halaman%20Sederhana.png)







  
  

  


 





