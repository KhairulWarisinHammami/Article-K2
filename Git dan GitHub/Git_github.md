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
