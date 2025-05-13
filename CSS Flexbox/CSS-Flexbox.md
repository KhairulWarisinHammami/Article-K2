  ### CSS Flexbox
  CSS Flexbox, atau lengkapnya Flexible Box Layout, adalah salah satu teknik layout di CSS yang dirancang untuk menyusun elemen-elemen dalam satu baris atau satu kolom dengan cara yang fleksibel, mudah diatur, dan responsif terhadap ukuran layar atau perangkat.
  
  ### Pengantar
  Dalam pengembangan web modern, tata letak (layout) yang fleksibel dan responsif merupakan kebutuhan kebutuhan utama. CSS Flexbox atau Flexible Box Layout adalah salah satu fitur powerful dari CSS3 yang dirancang khusus untuk menyederhanakan proses pembuatan layout satu dimensi, baik dalam arah horizontal (baris) maupun vertikal (kolom). Dengan Flexbox, pengembang dapat mengatur posisi, ukuran, dan spasi antar elemen dengan lebih mudah tanpa harus bergantung pada teknik lama seperti float atau positioning yang rumit. Artikel ini akan membahas konsep dasar Flexbox, properti-properti penting yang digunakan, serta contoh penggunaannya dalam membangun layout web yang efisien dan responsif.

  ### Konsep Dasar Flexbox
  CSS Flexbox dirancang untuk mengatur elemen dalam satu dimensi: **baris (row)** atau **kolom (column)**. Konsep dasarnya adalah mengubah perilaku default elemen dalam HTML agar lebih fleksibel dan mudah diatur secara tata letak.

Berikut beberapa konsep inti dalam Flexbox:

### 1. Flex Container
Flex container adalah elemen induk yang diatur dengan `display: flex` atau `display: inline-flex`. Semua elemen anak dari container ini secara otomatis menjadi **flex items**.

```css
.container {
  display: flex;
}
```

### 2. Flex Items
Flex items adalah elemen anak langsung dari flex container. Item ini akan merespons aturan tata letak yang diterapkan oleh container.

```html
<div class="container">
  <div class="item">Item 1</div>
  <div class="item">Item 2</div>
</div>
```

### 3. Main Axis vs Cross Axis
* **Main Axis** adalah arah utama aliran item (default-nya horizontal: kiri ke kanan).
* **Cross Axis** adalah arah tegak lurus dari main axis (default-nya vertikal: atas ke bawah).

Kita bisa mengubah main axis menggunakan properti `flex-direction`.

```css
.container {
  flex-direction: row; /* atau column, row-reverse, column-reverse */
}
```

### 4. Spasi dan Perataan
Flexbox menyediakan properti seperti `justify-content`, `align-items`, dan `align-content` untuk mengatur:
* Posisi item pada main axis (horizontal).
* Posisi item pada cross axis (vertikal).
* Distribusi spasi di antara item-item.

### 5. Fleksibilitas Ukuran
Flexbox memungkinkan item untuk **tumbuh (grow)**, **menyusut (shrink)**, atau memiliki ukuran dasar tertentu melalui properti seperti `flex`, `flex-grow`, `flex-shrink`, dan `flex-basis`.

Konsep-konsep ini menjadi pondasi dalam memahami dan menggunakan Flexbox secara efektif. Dengan penguasaan dasar ini, kamu akan lebih mudah membangun layout yang adaptif dan bersih tanpa banyak trik CSS tambahan.
