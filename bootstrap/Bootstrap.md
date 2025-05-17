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



  
  

  


 





