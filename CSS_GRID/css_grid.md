### CSS Grid   
 yang memungkinkan kita membuat desain web yang rapi dan fleksibel menggunakan sistem baris dan kolom. CSS Grid sangat powerful untuk membuat layout 2 dimensi, artinya kamu bisa mengatur posisi elemen secara horizontal (baris) dan vertikal (kolom) sekaligus.   
### Cara Menggunakan CSS Grid   
  Untuk menggunakan CSS Grid, kamu perlu menentukan elemen kontainer dan anak-anaknya:   
   
##  Menjadikan elemen sebagai Grid Container   
.container {
  display: grid;
}   
  
##  Menentukan jumlah kolom dan baris   
.container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr; /* 3 kolom dengan lebar yang sama */
  grid-template-rows: auto auto; /* 2 baris otomatis */
}   
  
##  Contoh HTML + CSS:  
<div class="container">
  <div class="item">1</div>
  <div class="item">2</div>
  <div class="item">3</div>
  <div class="item">4</div>
</div>  

 .container {
  display: grid;
  grid-template-columns: repeat(2, 1fr); /* 2 kolom */
  gap: 10px; /* jarak antar elemen */
}

.item {
  background-color: lightblue;
  padding: 20px;
  text-align: center;
}   
###  Istilah Penting dalam CSS Grid  

| Istilah                          | Penjelasan                                                     
| -------------------------------- | -------------------------------------------------------------- |
| `grid-template-columns`          | Menentukan jumlah dan ukuran kolom                             |
| `grid-template-rows`             | Menentukan jumlah dan ukuran baris                             |
| `gap` / `row-gap` / `column-gap` | Jarak antar kolom/baris                                        |
| `grid-column` / `grid-row`       | Menentukan posisi dan rentang elemen                           |
| `fr`                             | Satuan fleksibel (fraction / pecahan dari ruang yang tersedia) |   

###  Kapan Menggunakan CSS Grid?
Ketika kamu ingin membuat layout kompleks yang melibatkan baris dan kolom

Saat kamu butuh kontrol penuh terhadap penempatan elemen

Untuk membangun grid responsif tanpa banyak media query








