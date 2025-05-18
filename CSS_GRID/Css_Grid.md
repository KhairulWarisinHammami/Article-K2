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





















  














