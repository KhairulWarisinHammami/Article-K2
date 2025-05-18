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

![desktop](https://github.com/KhairulWarisinHammami/Article-K2/blob/ec12b0305934d4f1424bd492ef76897beb2cabc0/CSS%20Flexbox/desktop.jpeg]

* Di layar kecil (seperti smartphone atau tablet):
Kotak-kotak tersebut akan secara otomatis turun ke baris baru, tampil satu per satu secara vertikal agar tetap mudah dibaca dan responsif terhadap ukuran layar.

![hp](https://github.com/KhairulWarisinHammami/Article-K2/blob/ec12b0305934d4f1424bd492ef76897beb2cabc0/CSS%20Flexbox/hp.jpeg]
