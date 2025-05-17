### Bootstrap
Bootstrap adalah framework front-end paling populer di dunia yang membantu developer membangun situs web dan aplikasi yang intuitif, responsif, dan estetis dengan cepat. Dikembangkan pertama kali oleh para engineer dari Twitter pada tahun 2011, Bootstrap kini berada di versi 5.x dengan komunitas yang sangat aktif dan ekosistem yang kaya.

#### Pengantar

Pada dasarnya, Bootstrap menyederhanakan proses pembuatan antarmuka (UI) web dengan menyediakan komponen HTML, CSS, dan JavaScript siap pakai. Alih-alih menulis CSS dari nol untuk tombol, form, navbar, dan layout, Anda cukup mengimpor pustaka Bootstrap dan memanfaatkan kelas-kelas utilitas serta komponen yang telah dirancang secara konsisten. Hal ini memungkinkan tim developer fokus pada logika dan konten, tanpa harus khawatir tentang detail styling dan responsivitas.

Lebih jauh lagi, Bootstrap dibangun di atas sistem grid fleksibel yang memudahkan penataan elemen pada berbagai ukuran layar, mulai dari ponsel hingga desktop besar. Dengan demikian, Anda dapat menciptakan desain yang adaptif dan user-friendly tanpa harus menulis banyak media query secara manual. Selain itu, dokumentasi Bootstrap sangat komprehensif, lengkap dengan contoh kode dan animasi interaktif, sehingga baik pemula maupun developer berpengalaman dapat dengan mudah memahami dan menerapkan konsep-konsepnya.

#### Instalasi Bootstrap

Panduan ini menjelaskan cara menginstal dan menggunakan **Bootstrap**, framework CSS populer untuk membuat antarmuka web yang responsif dan modern.

#### 📦 Cara Instalasi

##### 1. Menggunakan CDN (Cara Termudah)

Jika Anda tidak ingin mengunduh file apa pun, Anda bisa menggunakan Bootstrap langsung dari CDN.

Tambahkan baris berikut di bagian `<head>` dan sebelum tag penutup `</body>` pada file HTML Anda:

```html
<!-- CSS Bootstrap -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">

<!-- JS Bootstrap (opsional, jika menggunakan komponen seperti modal, dropdown, dsb.) -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>


