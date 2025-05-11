### Git dan GitHub  

![Gambar Git dan GItHub](https://github.com/KhairulWarisinHammami/Article-K2/blob/Gitaa/Git%20dan%20GitHub/Git%20dan%20GitHub.jpg)  

#### Pengertian

**1. Git**  
   Git merupakan sebuah sistem kontrol versi (Version Control System, VCS) yang digunakan untuk mencatat setiap perubahan pada kode atau program secara efisien. Fungsi utama pada Git yaitu melacak perubahan pada file proyek, sebagai sarana pengembang kerja bersama atau kolaborasi tanpa konflik dan menyimpan riwayat perubahan kode sehingga bisa kembali ke versi sebelumnya jika terjadi kesalahan.

**2. GitHub**  
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
**1. Konfigurasi Awal Git**  
  | Perintah | Fungsi | 
  |:---|:---|  
  | git config --global user.name "nama" | Mengatur nama pengguna |  
  | git config --global user.email "email@example.com" | Mengatur email pengguna |  
  | git config --list | Menampilkan konfigurasi Git yang sedang aktif |  

**2. membuat dan Mengelola Repository**  
  | Perintah | Fungsi |  
  |:---|:---|  
  | git init | Membuat repository Git baru di folder lokal |  
  | git clone [url] | Menyalin repository dari remote ke lokal |  
 
**3. Perubahan dan Penyimpanan**  
  | Perintah | Fungsi |  
  |:---|:---|  
  | git status | Menampilkan sataus perubahan file |  
  | git add [file] | Menambahkan file ke staging area |  
  | git add | Menambahkan semua perubahan ke staging |  
  | git comit -m "pesan" | Menyimpan perubahan ke repository lokal |  
  | git diff | Menampilkan perbedaan sebelum di-*commit* |  

**4. Remote Repository**  
  | Perintah | Fungsi |  
  |:---|:---|  
  | git remote add origin [url] | Menambahkan remote repository |  
  | git push -u origin master | Mengirim commit ke remote branch utama |  
  | git pull | Menngambil update terbaru dari remote repository |  
  | git fetch | Mengambil update dari remote, tanpa marge otomatis |  

 **5. Branching dan Marging**  
  | Perintah | Fungsi |  
  |:---|:---|  
  | git branch | Melihat semua branch |  
  | git branch [nama] | Membuat branch baru |  
  | git checkout [nama] | Berpindah ke branch tertentu |  
  | git marge [nama] | Menggabungkan branch ke branch aktif |  
  | git branch -d [nama] | Menghapus branch lokal |  

 **6. Riwayat dan Refisi**  
  | Perintah | Fungsi |  
  |:---|:---|  
  | git log | Melihat riwayat commit |  
  | git log --online | Log singkat satu baris per commit |  
  | git checkout [commit_id] | Berpindah ke commit tertentu |  
  | git revert [commit_id] | Membatalkan commit tertentu dengan membuat commit baru |  
  | git reset --hard [commit_id] | Mengembalikan ke commit tertentu (berbahaya: menghapus perubahan) |  

 **7. Pembersihan dan Penanganan Sementara**  
  | Perintah | Fungsi |  
  |:---|:---|  
  | git stash | Menyimpan perubahan sementara |  
  | git stash pop | Mengembalikan perubahan yang di-stash |  
  | git rm [file] | Menghapus file dari repo dan file system |  
 
 
