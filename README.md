<!-- Boxed title section -->
<div style="border: 3px solid orange; padding: 12px; border-radius: 10px; background-color: #1e1e1e; color: Black; font-size: 1.2em; font-weight: bold;">
  Proyek Artikel - Kelompok 1
</div>

---

Repositori ini berisi hasil kerja kolaboratif dalam menyusun sebuah artikel dengan menggunakan GitHub.
Artikel yang dibuat membahas empat topik utama, yaitu:

1. Dasar-dasar Git dan GitHub  
2. CSS Flexbox dan penggunaannya  
3. CSS Grid dan penggunaannya  
4. Bootstrap serta implementasinya

---

### Anggota:

- *Khairul Warisin Hammami* (admin, integrator & Bootstrap)  
- *Inggita Delsa Aviva* (Git dan GitHub)  
- *Ahmad Arfin* (CSS Flexbox)  
- *Julkarnaen* (CSS Grid)

---

Setiap kontributor bekerja melalui fitur branch dan pull request, lalu digabungkan oleh admin melalui proses review.
Melalui proyek ini, kami tidak hanya memperdalam pemahaman teknis, tetapi juga melatih kerja sama tim dalam pengembangan berbasis Git.

---

### Git dan GitHub  

![Gambar Git dan GItHub](https://github.com/KhairulWarisinHammami/Article-K2/blob/Gitaa/Git%20dan%20GitHub/Git%20dan%20GitHub.jpg)  

#### Pengertian

**A. Git**  
   Git merupakan sebuah sistem kontrol versi (Version Control System, VCS) yang digunakan untuk mencatat setiap perubahan pada kode atau program secara efisien. Fungsi utama pada Git yaitu melacak perubahan pada file proyek, sebagai sarana pengembang kerja bersama atau kolaborasi tanpa konflik dan menyimpan riwayat perubahan kode sehingga bisa kembali ke versi sebelumnya jika terjadi kesalahan.

**B. GitHub**  
   GitHub adalah layanan hosting berbasis cloud untuk repositori Git, yang diibaratkan seperti media sosial untuk kode, dan memungkinkan kolaborasi pengembang secara online. Fungsi utama pada GitHub yaitu menyimpan dan membagikan kode secara online, kolabirasi antar-pengembang menggunakan fitur seperti *pull requests* dan *issues*


#### Perbedaan Git dan GitHub

 Git merupakan sebuah sistem kontrol versi yang digunakan untuk melacak dan mengelola perubahan dalam suatu file proyek, terutama dalam pengembang perangkat lunak. Dengan menggunakan Git, pengembang dapat bekerja secara lokal dalam komputer, mencatat riwayat perubahan kode, membuat cabang (*branch*) untuk fitur baru, dan menyatukanya kembali ke versi utama tanpa kehilangan data. Git sangat membantu dalam kolaborasi karena memungkinkan banyak orang bekerja pada bagian yang berbeda tetapi dalam proyek yang sama.  

 Sedangkan GitHub, dalah layanan hosting berbasis cloud yang menyediakan tempat penyimpanan repositori git secara online. GItHub mempermudah kolaborasi antar-pengembang dengan meyediakan fitur seperti *pull request*, *issues*, dan *code review*. Dengan GitHub, pengembang dapat membagikan kode mereka ke publik atau tim, berkontribusi pada proyek open-source, dan mengintegrasikan berbagai layanan otomatis seperti CI/CD.

 Git dapat digunakan tanpa GitHub, akan tetati GitHub tidak bisa bekerja tanpa Git karena Git adalah teknologi dasar yang digunakan untuk mengelola versi kode.  

Atau jika disimpulkan:  
| Aspek | Git | GitHub |
|:---|:---|:---|
| Jenis | Aplikasi atau sistem kontrol versi (VCS) | Layanan hosting berbasis cloud |  
| Fungsi utama | Melacak dan mengelola perubahan kode secara lokal | Menyimpan dan membagikan repositori Git secara online |  
| Tempat bekerja | Lokal (di komputer) | Online (di wesite GitHub.com) |    
| Kegunaan | Digunakan untuk mengatur versi kode | Digunakan untuk kolaborasi, review, dan distribusi kode |  
| Koneksi internet | Tidak selalu diperlukan | Diperlukan untuk mengakses, meyimpan, atau berbagi kode |  
| Antarmuka | Command Line Interface (CLI) | Web interface + CLI support |  
| Kolabirasi tim | Terbatas tanpa layanan tambahan | Mendukung pull request, issue tracking, kode reviev, dsb |  


#### Dasar-dasar Git  

 Berikut adalah dasar-dasar Git yang mencakup perintah umum dan fungsinya:  
**A. Konfigurasi Awal Git**  
  | Perintah | Fungsi | 
  |:---|:---|  
  | git config --global user.name "nama" | Mengatur nama pengguna |  
  | git config --global user.email "email@example.com" | Mengatur email pengguna |  
  | git config --list | Menampilkan konfigurasi Git yang sedang aktif |  

**B. membuat dan Mengelola Repository**  
  | Perintah | Fungsi |  
  |:---|:---|  
  | git init | Membuat repository Git baru di folder lokal |  
  | git clone [url] | Menyalin repository dari remote ke lokal |  
 
**C. Perubahan dan Penyimpanan**  
  | Perintah | Fungsi |  
  |:---|:---|  
  | git status | Menampilkan sataus perubahan file |  
  | git add [file] | Menambahkan file ke staging area |  
  | git add | Menambahkan semua perubahan ke staging |  
  | git comit -m "pesan" | Menyimpan perubahan ke repository lokal |  
  | git diff | Menampilkan perbedaan sebelum di-*commit* |  

**D. Remote Repository**  
  | Perintah | Fungsi |  
  |:---|:---|  
  | git remote add origin [url] | Menambahkan remote repository |  
  | git push -u origin master | Mengirim commit ke remote branch utama |  
  | git pull | Menngambil update terbaru dari remote repository |  
  | git fetch | Mengambil update dari remote, tanpa marge otomatis |  

 **E. Branching dan Marging**  
  | Perintah | Fungsi |  
  |:---|:---|  
  | git branch | Melihat semua branch |  
  | git branch [nama] | Membuat branch baru |  
  | git checkout [nama] | Berpindah ke branch tertentu |  
  | git marge [nama] | Menggabungkan branch ke branch aktif |  
  | git branch -d [nama] | Menghapus branch lokal |  

 **F. Riwayat dan Refisi**  
  | Perintah | Fungsi |  
  |:---|:---|  
  | git log | Melihat riwayat commit |  
  | git log --online | Log singkat satu baris per commit |  
  | git checkout [commit_id] | Berpindah ke commit tertentu |  
  | git revert [commit_id] | Membatalkan commit tertentu dengan membuat commit baru |  
  | git reset --hard [commit_id] | Mengembalikan ke commit tertentu (berbahaya: menghapus perubahan) |  

 **G. Pembersihan dan Penanganan Sementara**  
  | Perintah | Fungsi |  
  |:---|:---|  
  | git stash | Menyimpan perubahan sementara |  
  | git stash pop | Mengembalikan perubahan yang di-stash |  
  | git rm [file] | Menghapus file dari repo dan file system |  


#### Dasar-dasar GitHub
 Berikut adalah dasar-dasar GitHub dan bagaimana cara mengimplementasikannya:  
 **1. Buat Akun**  
 - Buka situs GitHub di github.com, lalu buat akun baru dengan menekan tombol "Sign up"
 - Isi informasi yang dibutuhkan seperti email, kata sandi, dan username, lalu tekan tombol "Continue"
 - Verfikasi email dengan menyelesaikan captca, lalu tekan "Submit> Create Account"
 - sukkan kode verifikasi yang telah dikirimkan melalui email
 - Tekan "Skip this for now" jika ingin melewati proses personalisasi akun, selanjutnya sistem akan menunjukkan dashboard GitHub

   ![Signup](https://github.com/KhairulWarisinHammami/Article-K2/blob/Gitaa/Git%20dan%20GitHub/Images/signup.png)

**2. Membuat Repository**
- Buka akun GitHub dan masuk ke Situs GitHub
- Klik tombol "New" atau "Create Repository" di sudut kanan ats halaman
- Masukkan "Nama Repository" dan "Deskripsi" (opsional)
- Pilih apakah repository akan bersifat "Publik" atau "Privat"
- Centang pada "Add a README file" jika ingin menambahkan file README
- Tekan "Create repository" untuk menyelesaikan proses

  ![Create Repo](https://github.com/KhairulWarisinHammami/Article-K2/blob/Gitaa/Git%20dan%20GitHub/Images/Create%20Repo.png)

**3. Upload Proyek Pertama Kali ke GitHub Via Git**  
  Berikut adalah bagian langkah-langkah awal:  
  a. Pastikan Git sudah terinstal: buka terminal atau CMD, lalu ketik: "git --version", jika sudah terinstal akan muncul versi Git
  b. Buat Repository di GitHub:
  
  - untuk membuat repository lakukan seperti pada langkah-langkah sebelumnya (ke-2. Membuat Repository)
  - Jangan centang "Initialize this repository with a README"  

 Kemudian berikut adalah langkah-langkah inti dalam mengupload proyek:  
Misalnya kamu telah memiliki folder lokal: "projek-saya/"  
a. Masuk ke folder proyek  
   - cd path/ke/projek-saya  
b. Inisialisasi Git  
   - git init  
c. Tambahkan semua file ke staging area  
   - git add  
d. Commit perubahan  
   - git commit -m "commit pertama"
     ![git commit](https://github.com/KhairulWarisinHammami/Article-K2/blob/Gitaa/Git%20dan%20GitHub/Images/Git.png)  
e. Tambahkan remote repository dari GitHub (Ganti <username> dan <repo> sesuai dengan akun GitHub)  
   - git remote add origin https://github.com/<username>/<repo>.git
     ![remote origin](https://github.com/KhairulWarisinHammami/Article-K2/blob/Gitaa/Git%20dan%20GitHub/Images/Remote%20add%20git.png)  
f. Push ke GitHub  
   - git branch -M main  
   - git push -u origin main
     ![push](https://github.com/KhairulWarisinHammami/Article-K2/blob/Gitaa/Git%20dan%20GitHub/Images/image.png)

**4. Konsep Fork, Pull Request dan Collaboration**  
a. Fork  
   Fork (atau forking) adalah proses menyalin sebuah proyek atau repositori milik orang lain, termasuk seluruh riwayat perubahannya, ke dalam akun GitHub pribadi. Tujuan dari tindakan ini adalah untuk memungkinkan pengguna melakukan modifikasi atau pengembangan sesuai keinginan tanpa memberikan dampak langsung terhadap repositori asli.   

b. Pull Request  
   Pull request digunakan untuk memberi tahu pemilik repository asli bahwa Anda memiliki perubahan atau penambahan kode yang diusulkan untuk digabungkan ke dalam proyek mereka. Melalui pull request, kontributor dapat berpartisipasi dalam pengembangan proyek orang lain dengan mengajukan modifikasi yang telah mereka buat. Selain itu, pull request juga menjadi sarana untuk meminta tinjauan (code review), berdiskusi tentang implementasi, serta menyempurnakan kode bersama tim atau komunitas pengembang sebelum perubahan tersebut diintegrasikan ke dalam basis kode utama.  

c. Collaboration  
   Kolaborasi berarti bekerja bersama orang lain dalam satu proyek. Dalam GitHub, dilakukan dengan memberi akses kepada pengguna lain untuk mengedit, push, atau mengelola repository Anda secara langsung.  
   
#### Berikut adalah langkah-langkah untuk mengimplementasikan fork, pull request, dan kolaborasi:  
a. Fork Repository  
   Fork repository dilakukan jika anda bekerja dengan salinan proyek orang lain. Langkah-langkah:  
   - Akses Repository Asli:  
      Kunjungi halaman repository yang ingin Anda kontribusikan di GitHub.  
   - Fork Repository:  
      Klik tombol Fork yang ada di pojok kanan atas halaman repository. GitHub akan menyalin repository tersebut ke akun GitHub Anda, sehingga Anda memiliki versi independen dari proyek tersebut.
       
![Fork](https://github.com/KhairulWarisinHammami/Article-K2/blob/Gitaa/Git%20dan%20GitHub/Images/FORKING.png)  

b. Pull Request  
   Setelah Anda melakukan perubahan pada repository hasil fork, Anda akan membuat pull request untuk meminta agar perubahan tersebut digabungkan ke repository asli. Langkah-langkah:
   - Buat Branch Baru:
     Sebelum mulai mengubah kode, buatlah branch baru di repo lokal Anda untuk mengerjakan perubahan, misalnya: **git checkout -b fitur-baru**  
   - Lakukan Perubahan:
     Edit file yang ingin Anda ubah, lalu commit perubahan tersebut: **git add .** **git commit -m "Menambahkan fitur baru"**
   - Push Perubahan ke Repository Fork:
     Setelah perubahan selesai, kirim (push) ke repository fork Anda di GitHub: **git push origin fitur-baru**
   - Buat Pull Request:
     1). Kembali ke GitHub dan buka repository fork Anda
     2). Klik tombol Compare & Pull Request yang muncul setelah Anda melakukan push
     3). Pilih repository asli sebagai tujuan pull request dan beri deskripsi mengenai perubahan yang Anda lakukan
     4). Klik Create Pull Request untuk mengajukan perubahan tersebut

     ![Pull request](https://github.com/KhairulWarisinHammami/Article-K2/blob/Gitaa/Git%20dan%20GitHub/Images/Pull2.png)
     

c. Collaboration

![collaboration](https://github.com/KhairulWarisinHammami/Article-K2/blob/Gitaa/Git%20dan%20GitHub/Images/Collaborators.png)

   Kolaborasi memungkinkan banyak pengembang bekerja bersama pada satu proyek, baik melalui pull request ataupun kerja langsung pada branch utama. Langkah-langkah:  
   - Meninjau Pull Request:  
     Setelah Anda mengajukan pull request, pemilik repository atau kontributor lain akan meninjau perubahan Anda. Mereka bisa memberi komentar, memberikan masukan, atau meminta revisi.  
   - Diskusi dan Revisi:  
     Jika ada masukan atau perbaikan yang perlu dilakukan, lakukan perubahan di branch yang sama, commit, dan push lagi ke repository fork Anda. GitHub akan secara otomatis memperbarui pull request dengan perubahan baru tersebut.
   - Merge Pull Request:  
     Setelah pull request Anda diterima dan disetujui, pemilik repository atau kolaborator lain akan menggabungkan perubahan Anda ke repository utama menggunakan fitur Merge di GitHub. Perubahan Anda akan terintegrasi ke dalam basis kode proyek utama.
   - Kolaborasi Langsung:  
     Jika Anda memiliki akses sebagai collaborator di repository, Anda dapat melakukan perubahan langsung di branch utama atau branch lain tanpa melalui fork. Namun, proses yang lebih umum adalah menggunakan pull request untuk menjaga keamanan dan integritas kode.  

**5. Contoh Workflow Kolaboratif:** 
- Fork dan clone repository.
- Buat branch baru untuk fitur atau perbaikan.
- Lakukan perubahan, commit, dan push ke repository fork Anda.
- Buat pull request ke repository asli.
- Review dan diskusi perubahan melalui komentar pada pull request.
- Setelah disetujui, pemilik repository akan melakukan merge.

---

  ### CSS Flexbox
  CSS Flexbox, atau lengkapnya Flexible Box Layout, adalah salah satu teknik layout di CSS yang dirancang untuk menyusun elemen-elemen dalam satu baris atau satu kolom dengan cara yang fleksibel, mudah diatur, dan responsif terhadap ukuran layar atau perangkat.
  
  ### Pengantar
  Dalam pengembangan web modern, tata letak (layout) yang fleksibel dan responsif merupakan kebutuhan kebutuhan utama. CSS Flexbox atau Flexible Box Layout adalah salah satu fitur powerful dari CSS3 yang dirancang khusus untuk menyederhanakan proses pembuatan layout satu dimensi, baik dalam arah horizontal (baris) maupun vertikal (kolom). Dengan Flexbox, pengembang dapat mengatur posisi, ukuran, dan spasi antar elemen dengan lebih mudah tanpa harus bergantung pada teknik lama seperti float atau positioning yang rumit. Artikel ini akan membahas konsep dasar Flexbox, properti-properti penting yang digunakan, serta contoh penggunaannya dalam membangun layout web yang efisien dan responsif.

  ### Konsep Dasar Flexbox
  CSS Flexbox dirancang untuk mengatur elemen dalam satu dimensi: **baris (row)** atau **kolom (column)**. Konsep dasarnya adalah mengubah perilaku default elemen dalam HTML agar lebih fleksibel dan mudah diatur secara tata letak.

Berikut beberapa konsep inti dalam Flexbox:

#### 1. Flex Container
Flex container adalah elemen induk yang diatur dengan `display: flex` atau `display: inline-flex`. Semua elemen anak dari container ini secara otomatis menjadi **flex items**.

```css
.container {
  display: flex;
}
```

#### 2. Flex Items
Flex items adalah elemen anak langsung dari flex container. Item ini akan merespons aturan tata letak yang diterapkan oleh container.

```html
<div class="container">
  <div class="item">Item 1</div>
  <div class="item">Item 2</div>
</div>
```

#### 3. Main Axis vs Cross Axis
* **Main Axis** adalah arah utama aliran item (default-nya horizontal: kiri ke kanan).
* **Cross Axis** adalah arah tegak lurus dari main axis (default-nya vertikal: atas ke bawah).

Kita bisa mengubah main axis menggunakan properti `flex-direction`.

```css
.container {
  flex-direction: row; /* atau column, row-reverse, column-reverse */
}
```

#### 4. Spasi dan Perataan
Flexbox menyediakan properti seperti `justify-content`, `align-items`, dan `align-content` untuk mengatur:
* Posisi item pada main axis (horizontal).
* Posisi item pada cross axis (vertikal).
* Distribusi spasi di antara item-item.

#### 5. Fleksibilitas Ukuran
Flexbox memungkinkan item untuk **tumbuh (grow)**, **menyusut (shrink)**, atau memiliki ukuran dasar tertentu melalui properti seperti `flex`, `flex-grow`, `flex-shrink`, dan `flex-basis`.

Konsep-konsep ini menjadi pondasi dalam memahami dan menggunakan Flexbox secara efektif. Dengan penguasaan dasar ini, kamu akan lebih mudah membangun layout yang adaptif dan bersih tanpa banyak trik CSS tambahan.

 ### Penggunaan CSS Flexbox
#### Contoh Kasus : Tiga Kotak Sejajar dan Responsif
Kita ingin membuat 3 kotak sejajar (horizontal) yang:
* Sama lebar
* Otomatis turun ke bawah jika layar mengecil (misalnya di HP)

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Contoh Flexbox</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <div class="container">
    <div class="item">Kotak 1</div>
    <div class="item">Kotak 2</div>
    <div class="item">Kotak 3</div>
  </div>

</body>
</html>
```

```css
/* Flex Container */
.container {
  display: flex;              /* Aktifkan Flexbox */
  justify-content: space-between; /* Jarak merata antar item */
  flex-wrap: wrap;            /* Supaya bisa pindah baris jika layar kecil */
  gap: 20px;                  /* Jarak antar kotak */
  padding: 20px;
  background-color: #f4f4f4;
}

/* Flex Items */
.item {
  background-color: #4CAF50;
  color: white;
  flex: 1 1 30%;              /* Grow, shrink, dan ukuran awal 30% */
  padding: 40px;
  text-align: center;
  border-radius: 8px;
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
}
```

#### Penjelasan penggunaan CSS Flexbox
```display: flex;```
Properti ini digunakan pada elemen induk (dalam hal ini .container) untuk mengaktifkan Flexbox. Setelah Flexbox diaktifkan, semua elemen anak di dalamnya (dalam contoh ini, .item) akan otomatis diatur dalam satu baris secara horizontal (default). Flexbox memberikan kontrol penuh terhadap cara penempatan dan ukuran setiap item di dalam container.

```flex-wrap: wrap;```
Secara default, semua item Flexbox akan tetap berada di satu baris meskipun sudah tidak cukup ruang. Dengan menambahkan flex-wrap: wrap, kita mengizinkan item untuk pindah ke baris baru jika ruang horizontal tidak cukup. Ini sangat penting untuk membuat tampilan responsif, agar tetap terlihat rapi di berbagai ukuran layar.

```justify-content: space-between;```
Properti ini digunakan untuk mengatur penempatan item sepanjang sumbu utama (main axis), yaitu secara horizontal (kiri ke kanan) secara default. Nilai space-between akan menyebarkan item secara merata, menempatkan item pertama di paling kiri dan terakhir di paling kanan, dengan jarak yang sama di antara item-item yang ada. Ini membuat tampilan lebih simetris dan seimbang.

```gap: 20px;```
Menentukan jarak tetap antara setiap item flex. Ini lebih praktis dan bersih dibanding menggunakan margin pada masing-masing item, karena gap hanya berlaku antar elemen dan tidak memengaruhi jarak luar container.

```flex: 1 1 30%;```
Ini adalah shorthand untuk tiga properti sekaligus:
* flex-grow: 1 → Item boleh mengembang jika ada ruang kosong.
* flex-shrink: 1 → Item boleh mengecil jika ruang tidak cukup.
* flex-basis: 30% → Ukuran dasar item adalah 30% dari lebar container.
Jadi, setiap kotak akan mencoba mengambil sekitar 30% dari lebar container, tapi juga bisa membesar atau mengecil tergantung ruang yang tersedia. Ini yang membuat tampilan menjadi fleksibel.

Properti tampilan lainnya (padding, background-color, border-radius, text-align, dll.)
Properti ini digunakan untuk memberi gaya visual, seperti warna, teks rata tengah, jarak dalam kotak, sudut membulat, dan bayangan. Tujuannya untuk membuat tampilannya lebih menarik dan enak dilihat.

#### Tampilan flexbox ketika berkerja di layar berbeda
* Di layar lebar (seperti laptop atau desktop):
Ketiga kotak akan tampil berdampingan secara horizontal, dengan jarak merata di antara mereka.

![desktop](https://github.com/KhairulWarisinHammami/Article-K2/blob/ec12b0305934d4f1424bd492ef76897beb2cabc0/CSS%20Flexbox/desktop.jpeg)

* Di layar kecil (seperti smartphone atau tablet):
Kotak-kotak tersebut akan secara otomatis turun ke baris baru, tampil satu per satu secara vertikal agar tetap mudah dibaca dan responsif terhadap ukuran layar.

![hp](https://github.com/KhairulWarisinHammami/Article-K2/blob/ec12b0305934d4f1424bd492ef76897beb2cabc0/CSS%20Flexbox/hp.jpeg)

---

### Css Grid   
adalah sistem layout dua dimensi di CSS yang digunakan untuk mengatur elemen dalam baris dan kolom. Berbeda dengan Flexbox yang lebih cocok untuk layout satu dimensi (horizontal atau vertikal),
CSS Grid memungkinkan kamu mengatur layout dalam dua dimensi secara bersamaan (horizontal dan vertikal).

##  Dasar Penggunaan CSS Grid  
- Untuk menggunakan CSS Grid, kamu harus menetapkan elemen sebagai grid container dengan properti:  
css  

display: grid; 

-Contoh dasar:  
html

<div class="container">
  <div>Item 1</div>
  <div>Item 2</div>
  <div>Item 3</div>
</div>  
css  

.container {
  display: grid;
  grid-template-columns: 100px 100px 100px;
}
-Hasilnya: 3 kolom, masing-masing selebar 100px.  
## Properti Penting di CSS Grid  
| Properti                   | Fungsi                              |
| -------------------------- | ----------------------------------- |
| `display: grid;`           | Mengaktifkan grid layout.           |
| `grid-template-columns`    | Menentukan jumlah dan lebar kolom.  |
| `grid-template-rows`       | Menentukan jumlah dan tinggi baris. |
| `gap` atau `grid-gap`      | Mengatur jarak antar elemen grid.   |
| `grid-column` / `grid-row` | Mengatur posisi item dalam grid.    |
| `grid-area`                | Mengatur area grid khusus.          |  
## Contoh Lebih Lanjut
css  

.container {
  display: grid;  
  grid-template-columns: 1fr 2fr;
  grid-template-rows: auto auto;
  gap: 10px;
}  

## Penjelasan:  
- 1fr dan 2fr berarti kolom pertama mendapatkan 1 bagian dan kolom kedua mendapatkan 2 bagian dari ruang yang tersedia.  
- gap: 10px; memberi jarak antar elemen grid sebesar 10px.  

## Kenapa CSS Grid Berguna?  
- Memudahkan membuat layout kompleks (seperti galeri, dashboard, dll).
- Lebih fleksibel untuk desain responsif.  
- Bisa mencampur ukuran absolut (px), relatif (%), dan unit fr.   

### Modul Tata Letak Grid CSS 
**Pengertian**  
CSS Grid Layout adalah modul CSS yang digunakan untuk membuat layout dua dimensi (baris dan kolom) secara mudah dan fleksibel. Modul ini memungkinkan developer mengatur posisi elemen dalam sebuah wadah (container) tanpa harus menggunakan float atau positioning manual.  

## Struktur Dasar Grid
Untuk menggunakan Grid CSS, kita harus menentukan elemen induk (container) dan elemen anak (item):  
css  
.container {
  display: grid;
}  

Semua elemen di dalam .container akan menjadi grid item.

## Membuat Kolom dan Baris  
Gunakan properti:  
- grid-template-columns untuk mendefinisikan kolom.
-  grid-template-rows untuk mendefinisikan baris.
css  
  .container {
  display: grid;
  grid-template-columns: 200px 1fr 1fr;
  grid-template-rows: 100px auto;
}  
Artinya:  
- iga kolom: 200px, sisanya terbagi rata (1fr dan 1fr).
- grid-template-rows untuk mendefinisikan baris.
 csss  
.container {
  display: grid;
  grid-template-columns: 200px 1fr 1fr;
  grid-template-rows: 100px auto;
}   

Artinya:  
- Tiga kolom: 200px, sisanya terbagi rata (1fr dan 1fr).    
- Dua baris: 100px dan tinggi otomatis.  

## Satuan Umum yang Digunakan  
- px: satuan tetap.   
- fr: fraction unit (bagian dari ruang yang tersedia).  
- %: persentase dari wadah.  
- auto: menyesuaikan isi.  

## Gap atau Jarak Antar Grid  
Untuk mengatur jarak antar baris dan kolom:  
css   
.container {
  display: grid;
  gap: 10px;           /* jarak semua sisi */
  row-gap: 15px;       /* khusus baris */
  column-gap: 20px;    /* khusus kolom */
}   

## Penempatan Grid Item Secara Spesifik  
Gunakan:  
- grid-column   
- grid-row   
Contoh:  
css
.item1 {
  grid-column: 1 / 3; /* item melebar dari kolom 1 ke 2 */
  grid-row: 1 / 2;    /* item berada di baris 1 */
}   

## Grid Area    
Kita bisa menamai bagian-bagian layout:   
css     
.container {
  display: grid;
  grid-template-areas:
    "header header"
    "sidebar main"
    "footer footer";
  grid-template-columns: 200px 1fr;
}  

.header  { grid-area: header; }  
.sidebar { grid-area: sidebar; }  
.main    { grid-area: main; }  
.footer  { grid-area: footer; }     

## Posisi dan Perataan Item  
Perataan horizontal dan vertikal:  
- justify-items: rata horizontal isi grid.  
- align-items: rata vertikal isi grid.  
- justify-self, align-self: berlaku per-item.  
  
css   
.container {
  align-items: center;
  justify-items: start;
}   

## Grid Responsif dengan repeat() dan media query   
css  
.container {
  display: grid;
  grid-template-columns: repeat(3, 1fr); /* 3 kolom seimbang */
}

@media (max-width: 600px) {
  .container {
    grid-template-columns: 1fr; /* 1 kolom di layar kecil */
  }
}    

## Contoh Sederhana HTML + CSS Grid   
html    
<style> 
  .container {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 10px;
  }  
  .item {
    background: lightblue;
    padding: 20px;
    text-align: center;
  }  
  
</style>  
<div class="container">
  <div class="item">1</div>
  <div class="item">2</div>
  <div class="item">3</div>
  <div class="item">4</div>
</div>  

## Kelebihan CSS Grid   
- Bisa mengatur layout kompleks dengan mudah.   
- Mendukung dua dimensi (baris dan kolom).    
- Responsif untuk berbagai ukuran layar.    
- Lebih bersih dibanding float atau position.  


### Kolom, Baris dan Celah Grid CSS    
1. ## Kolom (grid-template-columns)  
 Properti ini mengatur jumlah kolom dan ukuran setiap kolom dalam grid.   
Ukuran bisa berupa:  
- Piksel (px): lebar tetap.  
- Fraksi (fr): membagi ruang sisa secara proporsional.   
- Persen (%), auto, dan lain-lain.  
Contoh:  
css   
grid-template-columns: 150px 1fr 2fr;  

Penjelasan:  

| Kolom | Ukuran | Deskripsi                               |
| ----- | ------ | --------------------------------------- |
| 1     | 150px  | Lebar tetap 150 piksel                  |
| 2     | 1fr    | Ambil 1 bagian dari sisa ruang yang ada |
| 3     | 2fr    | Ambil 2 bagian dari sisa ruang yang ada |    

Jadi, jika total ruang kosong 300px, kolom kedua akan 100px dan kolom ketiga 200px.   

2. ## (grid-template-rows)  
Mengatur jumlah baris dan tinggi setiap baris.   
Bisa menggunakan:  
- auto → tinggi otomatis sesuai isi.  
- ukuran tetap (misal 100px).  

Contoh:    
css   
grid-template-rows: auto 100px;  

Penjelasan:  

| Baris | Ukuran | Deskripsi                      |
| ----- | ------ | ------------------------------ |
| 1     | auto   | Tinggi menyesuaikan isi konten |
| 2     | 100px  | Tinggi tetap 100 piksel        |   

3. ## Celah / Jarak (gap)  
- Mengatur jarak antar kolom dan baris agar grid tidak menempel.  
-  mengatur jarak antar baris dan kolom sekaligus.  

Bisa juga pakai:  

- row-gap untuk jarak antar baris saja.  
- column-gap untuk jarak antar kolom saja.  
Contoh:  
css  
gap: 20px;

atau terpisah:  
ccs  
row-gap: 10px;
column-gap: 30px;

4. ## Contoh Lengkap dengan Penjelasan HTML  
html  
<div class="grid-container">
  <div class="item">A</div>
  <div class="item">B</div>
  <div class="item">C</div>
  <div class="item">D</div>
  <div class="item">E</div>
  <div class="item">F</div>
</div>  

# CSS  
css  
.grid-container {
  display: grid;

  /* 3 kolom: 150px, 1fr, 2fr */
  grid-template-columns: 150px 1fr 2fr;

  /* 2 baris: auto tinggi dan 100px */
  grid-template-rows: auto 100px;

  /* jarak antar kolom dan baris 20px */
  gap: 20px;

  background-color: #f0f0f0;
  padding: 15px;
  border: 2px solid #ccc;
}  

.item {
  background-color: #007acc;
  color: white;
  font-size: 18px;
  text-align: center;
  padding: 20px;
  border-radius: 8px;
}  

5. ## Visualisasi Hasil Grid  
+----------------+----------------+--------------------+
|       A        |       B        |         C          | ← Baris 1 (auto tinggi)
+----------------+----------------+--------------------+
|       D        |       E        |         F          | ← Baris 2 (100px tinggi)  
+----------------+----------------+--------------------+

Kolom:  
- Kolom 1: Lebar tetap 150px  
- Kolom 2: Ambil 1 bagian fraksi dari ruang tersisa  
- Kolom 3: Ambil 2 bagian fraksi dari ruang tersisa  

Gap (celah) antar kolom dan baris: 20px   

6. ## Ringkasan Cara Kerja  
- Browser membuat grid berdasarkan kolom dan baris yang kita definisikan.  
- Setiap elemen .item ditempatkan ke dalam sel grid secara otomatis.  
- Jarak antar elemen dibuat oleh properti gap.  
- Ukuran kolom dan baris fleksibel mengikuti aturan yang sudah dibuat.  


### Wadah Grid CSS    
1. Pengertian Grid Container  
**Grid Container** adalah elemen HTML yang dijadikan sebagai "wadah" dari tata letak grid menggunakan properti CSS display: grid.  
Semua aturan grid seperti pembentukan kolom, baris, dan penempatan item berlaku hanya di dalam elemen ini.  

Semua elemen anak langsung dari grid container akan menjadi grid item.  

 2. ## Cara Membuat Grid Container  
Untuk membuat grid container, cukup menambahkan properti display: grid pada elemen HTML.  
Contoh dasar:    
css    
.container {
  display: grid;
}  

HTML:  
css  
<div class="container">
  <div class="item">Item 1</div>
  <div class="item">Item 2</div>
</div>

3. ## Properti-Penting Grid Container  
Berikut beberapa properti yang sering digunakan dalam grid container:    

| Properti                | Fungsi                                            |
| ----------------------- | ------------------------------------------------- |
| `grid-template-columns` | Menentukan jumlah dan ukuran kolom.               |
| `grid-template-rows`    | Menentukan jumlah dan ukuran tinggi baris.        |
| `gap`                   | Menentukan jarak antar baris dan kolom.           |
| `row-gap`               | Mengatur jarak khusus antar baris saja.           |
| `column-gap`            | Mengatur jarak khusus antar kolom saja.           |
| `grid-template-areas`   | Menyusun layout berdasarkan area-area bernama.    |
| `justify-items`         | Posisi horizontal isi tiap sel grid.              |
| `align-items`           | Posisi vertikal isi tiap sel grid.                |
| `place-items`           | Kombinasi dari `justify-items` dan `align-items`. |   


4. Contoh Lengkap Grid Container   
HTML:   
html  
<div class="container">
  <div class="item">A</div>
  <div class="item">B</div>
  <div class="item">C</div>
  <div class="item">D</div>
</div>  

CSS:      
css    
.container {
  display: grid;

  /* Buat 2 kolom dengan ukuran 1fr dan 2fr */
  grid-template-columns: 1fr 2fr;

  /* Buat 2 baris, tinggi 100px dan auto */
  grid-template-rows: 100px auto;

  /* Jarak antar kolom dan baris */
  gap: 15px;

  /* Posisi isi dalam sel */
  justify-items: center;
  align-items: center;

  /* Tampilan tambahan */
  padding: 20px;
  background-color: #f9f9f9;
  border: 2px solid #ccc;
}  

.item {
  background-color: #2196F3;
  color: white;
  font-size: 18px;
  text-align: center;
  padding: 20px;
  border-radius: 8px;
}  

5. ## Visualisasi Hasil Grid
   
+------------+--------------------+
|     A      |         B          | ← Baris 1 (100px)
+------------+--------------------+
|     C      |         D          | ← Baris 2 (tinggi auto)    
+------------+--------------------+

Kolom   
- Kolom 1: 1fr (1 bagian)    
- Kolom 2: 2fr (2 bagian)   

Gap (jarak antara baris dan kolom): 15px  

6. ## Contoh Grid Container dengan Area Bernama  
css     
.container {
  display: grid;
  grid-template-columns: 1fr 3fr;
  grid-template-rows: auto 1fr auto;
  grid-template-areas:
    "header header"
    "sidebar main"
    "footer footer";
  gap: 10px;
}  

.header { grid-area: header; }
.sidebar { grid-area: sidebar; }
.main { grid-area: main; }
.footer { grid-area: footer; }  

html   
<div class="container">
  <div class="header">Header</div>
  <div class="sidebar">Sidebar</div>
  <div class="main">Main Content</div>
  <div class="footer">Footer</div>
</div>

7. ## Ringkasan Cara Kerja Grid Container   
- Grid Container dibuat dengan display: grid.   
- Di dalamnya, kita tentukan  
> Jumlah dan ukuran kolom (grid-template-columns)  
> Jumlah dan tinggi baris (grid-template-rows)  
> Celah antar sel (gap)  
- Elemen anak di dalam container otomatis jadi grid item.  
- Bisa menambahkan area bernama (grid-template-areas) untuk tata letak yang mudah dibaca.  

8. ## Tips Tambahan
> Grid container sangat cocok untuk membuat layout halaman seperti:  
- Header - Sidebar - Main - Footer  
- Galeri Gambar  
- Tata letak dashboard   
> Bisa digabung dengan media queries untuk membuat layout responsif di berbagai ukuran layar.  

### CSS Grid Item  
1. **Apa itu Item Kotak CSS?**

Item Kotak biasanya mengacu pada elemen-elemen anak dalam layout grid atau flexbox yang diperlakukan sebagai "kotak" dalam tata letak.
Dalam konteks CSS Grid, setiap anak langsung dari container grid disebut grid item (item kotak).

3. **Container Grid vs Item Kotak**
- Grid Container: elemen induk yang di-set display: grid;
- Grid Item (Item Kotak): elemen anak langsung di dalam container grid

3. **Properti Penting untuk Item Kotak di CSS Grid**
   
| Properti            | Keterangan                                                                                                       | Contoh                                                |
| ------------------- | ---------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------- |
| `grid-column-start` | Menentukan garis kolom awal tempat item dimulai                                                                  | `grid-column-start: 1;`                               |
| `grid-column-end`   | Menentukan garis kolom akhir tempat item berhenti                                                                | `grid-column-end: 3;`                                 |
| `grid-column`       | Shortcut untuk `grid-column-start / grid-column-end`                                                             | `grid-column: 1 / 3;`                                 |
| `grid-row-start`    | Menentukan garis baris awal tempat item dimulai                                                                  | `grid-row-start: 2;`                                  |
| `grid-row-end`      | Menentukan garis baris akhir tempat item berhenti                                                                | `grid-row-end: 4;`                                    |
| `grid-row`          | Shortcut untuk `grid-row-start / grid-row-end`                                                                   | `grid-row: 2 / 4;`                                    |
| `grid-area`         | Bisa mengatur area grid dengan nama area atau dengan shorthand `row-start / column-start / row-end / column-end` | `grid-area: 1 / 1 / 3 / 4;` atau `grid-area: myArea;` |
| `justify-self`      | Mengatur posisi item secara horizontal di dalam grid cell (start, center, end, stretch)                          | `justify-self: center;`                               |
| `align-self`        | Mengatur posisi item secara vertikal di dalam grid cell (start, center, end, stretch)                            | `align-self: end;`                                    |
| `place-self`        | Shortcut untuk `align-self` dan `justify-self`                                                                   | `place-self: center end;`                             | ]       

4. **Contoh Lengkap Item Kotak CSS Grid**    
html

<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Contoh Item Kotak CSS Grid</title>
  <style>
    .grid-container {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      grid-template-rows: 100px 100px;
      gap: 10px;
      padding: 20px;
      background-color: #eee;
    }
    /* Item Kotak Umum */
    .grid-item {
      background-color: #4CAF50;
      color: white;
      font-size: 20px;
      display: flex;
      justify-content: center;
      align-items: center;
      border-radius: 8px;
    }
    /* Item1 mulai dari kolom 1 sampai 3 */
    .item1 {
      grid-column: 1 / 3;
      grid-row: 1 / 2;
      background-color: #2196F3;
    }
    /* Item2 mulai dari kolom 3 sampai 5 dan baris 1 */
    .item2 {
      grid-column: 3 / 5;
      grid-row: 1 / 2;
      background-color: #FF5722;
    }
    /* Item3 menempati baris ke-2 dan semua kolom */
    .item3 {
      grid-column: 1 / 5;
      grid-row: 2 / 3;
      background-color: #9C27B0;
    }
  </style>
</head>
<body>

  <h2>Contoh Item Kotak CSS Grid</h2>

  <div class="grid-container">
    <div class="grid-item item1">Item 1</div>
    <div class="grid-item item2">Item 2</div>
    <div class="grid-item item3">Item 3</div>
  </div>

</body>
</html>

5. **Penjelasan Contoh**
.grid-container punya 4 kolom dan 2 baris, masing-masing 100px tinggi.

.item1 mengisi dari kolom 1 sampai sebelum kolom 3 (kolom 1 dan 2), baris 1.

.item2 mengisi kolom 3 sampai sebelum kolom 5 (kolom 3 dan 4), baris 1.

.item3 mengisi seluruh baris ke-2 (semua 4 kolom).

Setiap item diberi warna dan text agar terlihat jelas.  

6. **Properti Tambahan Berguna untuk Item Kotak**
- justify-self dan align-self untuk mengatur posisi isi item.
- 
- order (di flexbox) untuk mengatur urutan item (tidak berlaku di grid).

- place-self shortcut menggabungkan justify-self & align-self.

- grid-area untuk memberi nama dan mengelompokkan area.

**Kesimpulan**
- Item Kotak CSS dalam Grid adalah elemen yang kamu tempatkan di dalam grid container dan bisa diatur posisinya dengan properti seperti grid-column, grid-row, dan grid-area.

- Kamu bisa mengatur ukuran, posisi, dan tata letak item dengan properti-properti tersebut.

- Grid sangat powerful untuk layout modern yang kompleks.


---

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


---




  
  

  


 



























  

















