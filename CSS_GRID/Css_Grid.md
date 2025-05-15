### Css Grid   
adalah sistem layout dua dimensi di CSS yang digunakan untuk mengatur elemen dalam baris dan kolom. Berbeda dengan Flexbox yang lebih cocok untuk layout satu dimensi (horizontal atau vertikal),
CSS Grid memungkinkan kamu mengatur layout dalam dua dimensi secara bersamaan (horizontal dan vertikal).

##  Dasar Penggunaan CSS Grid  
-Untuk menggunakan CSS Grid, kamu harus menetapkan elemen sebagai grid container dengan properti:  
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
-1fr dan 2fr berarti kolom pertama mendapatkan 1 bagian dan kolom kedua mendapatkan 2 bagian dari ruang yang tersedia.  
-gap: 10px; memberi jarak antar elemen grid sebesar 10px.  

## Kenapa CSS Grid Berguna?  
-Memudahkan membuat layout kompleks (seperti galeri, dashboard, dll).
-Lebih fleksibel untuk desain responsif.  
-Bisa mencampur ukuran absolut (px), relatif (%), dan unit fr.





