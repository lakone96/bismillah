###### selector { property : value;}

- Selector adalah elemen html yang akan dipilih atau diubah style nya(<header>,<main>,dll)
- selector bisa menggunakan elemen html, class, atau id agar lebih spesifik

###### property dan value

- property adalah bagian apa yg akan diubah dan value adalah nilai yg akan dimasukan kedalam property
- berikut contoh property dan value :

- **Ukuran umum**:

  - Nilai panjang: `px`, `rem`, `em`, `%`, `vh`, `vw`

- Gunakan `rem` untuk konsistensi dalam `font-size`, `padding`, `margin`, dll. yang ingin tetap relatif terhadap root. Ini memudahkan untuk mengatur skala secara global.
- Gunakan `em` ketika ingin ukuran relatif terhadap `font-size` elemen itu sendiri, misalnya untuk `margin` atau `padding` yang ingin proporsional dengan teks di dalamnya.
- Gunakan `%` untuk layout yang fluid relatif terhadap parent.
- Gunakan `vh/vw` untuk ukuran yang relatif terhadap viewport, seperti full-screen sections.
- Gunakan `vmin/vmax` untuk elemen yang ingin responsive terhadap ukuran viewport baik secara landscape atau portrait.

Tips:
Biasanya, set root `font-size` ke `62.5% (10px)` untuk memudahkan perhitungan `rem` (`1rem = 10px`) namun tetap accessible (user dapat zoom).
`Namun, lebih aman menggunakan default (16px)` dan menghitung rem accordingly, atau `menggunakan 62.5% dengan hati-hati.`

Contoh setting root:

css
html {
font-size: 62.5%; /_ 10px _/
}

body {
font-size: 1.6rem; /_ 16px _/
}
Dengan begitu, 1rem = 10px, sehingga jika ingin 16px tulis 1.6rem, 24px tulis 2.4rem, dll.
Namun, jika user mengubah font-size di browser, layout akan tetap scaling dengan baik.

#### Font

- font family : <-- mengatur jenis font
- font size : <-- mengatur ukuran font yg disarankan
- font weight : <-- mengatur jenis font (normal, bold, 100-900)
- font-varian : <-- mengubah font menjadi small caps
- font style : <-- mengubah font menjadi cetak miring (normal, italic, oblique)
- line height : <-- mengatur spasi antar baris

# shorthand

- font : (style), (variant), (weight), (size), (height), (family);

#### Font Styling / Text

- color : <-- memberi warna teks
- text-align: <-- mengatur posisi teks kanan kiri tengah
- text-decoration: <-- mengatur dekorasi pada teks

#### Background

- background-color: <-- mengatur warna background
- background-image: url(tempat gambar disimpan) <-- mengatur gambar yg akan digunakan pada background
- background-position: <-- mengatur posisi gambar pada background (top, bottom, left, right, center)
- background-repeat: <-- mengatur jenis pengulangan pada background (repeat, repeat-x, repeat-y, no-repeat)
- background-attachment: <-- Mengatur apakah gambar latar scroll atau fixed (scroll, fixed)
- background-size: <-- Mengatur ukuran gambar latar (auto, cover, contain, nilai spesifik)

# shorthand

- background : (color), url(), (position), (repeat)

#### Gradient

# Syntax Sederhana

- background: linear-gradient(warna awal, ..., warna akhir); <-- mengatur gradient yg akan digunakan pada background

# Syntax Lengkap

- background: linear-gradient((sudut) | (arah), warna awal, ..., warna akhir); <-- mengatur gradient yg akan digunakan pada background
  -- arah (to bottom, to top, to left, to right, to left top, to left bottom, to right top, to right bottom)

#### Pseudo Class

- :hover <-- Style saat kursor berada di atas elemen
- :active <-- Style saat elemen diaktifkan (diklik)
- :focus <-- Style saat elemen mendapat fokus
- ::before <-- Menyisipkan konten sebelum konten elemen
- ::after <-- Menyisipkan konten setelah konten elemen

content:''; <-- Digunakan dengan ::before dan ::after untuk memasukkan konten

#### Layout & Display

display: <- Mengatur bagaimana elemen ditampilkan

- block <-- Elemen ditampilkan sebagai blok (mengambil lebar penuh)
- inline <-- Elemen ditampilkan sebaris dengan elemen lain tinggi dan lebar tidak bisa diatur
- inline-block <-- Elemen ditampilkan sebaris dengan elemen lain tinggi dan lebar bisa diatur
- flex <-- Menggunakan model layout flexbox
- grid <-- Menggunakan model layout grid
- none <-- Menyembunyikan elemen

overflow: <-- Mengatur konten yang overflow (visible, hidden, scroll, auto)

#### Spacing & Sizing

margin: (top), (right), (bottom), (left)
margin: (top-bottom), (left-right) <-- Mengatur jarak di luar elemen (shorthand)
margin-top: <-- Mengatur jarak atas elemen
margin-right: <-- Mengatur jarak kanan elemen
margin-bottom: <-- Mengatur jarak bawah elemen
margin-left: <-- Mengatur jarak kiri elemen

padding: (top), (right), (bottom), (left)
padding: (top-bottom), (left-right) <-- Mengatur jarak di dalam elemen (shorthand)
padding-top: - Mengatur jarak dalam bagian atas elemen
padding-right: - Mengatur jarak dalam bagian kanan elemen
padding-bottom: - Mengatur jarak dalam bagian bawah elemen
padding-left: - Mengatur jarak dalam bagian kiri elemen

#### Borders & Outline

border: (width, style, color) <-- Shorthand untuk mengatur border
border-width: <-- Mengatur ketebalan border
border-style: <-- Mengatur gaya border (solid, dashed, dotted, double, none)
border-color: <- Mengatur warna border
border-radius: <-- Mengatur radius sudut border
border-top-left-radius: <-- Mengatur radius sudut kiri atas
outline: <-- Garis di luar border (tidak mempengaruhi layout)

box-sizing: border-box <-- agar ukuran elemen tidak terpengaruh margin dan padding

#### CSS Reset

kunjungi web berikut lalu copy semua kode di dalam blok
[meyerweb](https://meyerweb.com/eric/tools/css/reset/)

#### Float

float: <-- Mengatur elemen mengambang (left, right, none)
.cf:before,
.cf:after {
content: " "; /_ 1 _/
display: table; /_ 2 _/
}

.cf:after {
clear: both;
}

#### Position

position: <-- Mengatur metode positioning elemen

- static <- Posisi normal (default)
- relative <-- Posisi relatif terhadap posisi normalnya
- absolute <-- Posisi relatif terhadap elemen parent terdekat yang dipositioned
- fixed <-- Posisi relatif terhadap viewport (tetap di tempat saat discroll)
- sticky <-- Hybrid antara relative dan fixed (biasanya pada header)

top, right, bottom, left <- Mengatur offset untuk elemen yang dipositioned

z-index - Mengatur tumpukan elemen (stacking order)

#### Opacity

opacity: (0 = transparan, 1 = opaque) <-- Mengatur transparansi elemen

#### Box Shadow & Text Shadow

box-shadow: (x-offset), (y-offset), (blur), (color) <-- Menambahkan efek bayangan pada elemen
box-shadow: (inset), (x-offset), (y-offset), (blur), (spread), (color) <-- Menambahkan efek bayangan pada elemen

- (spread) <-- ukuran bayangan
- (inset) <-- bayangan masuk ke dalam

text-shadow: (x-offset), (y-offset), (blur), (color) <-- Menambahkan efek bayangan pada teks

##########################################################################################################

### Flexbox Properties

flex-direction <- Mengatur arah item flex

- row <- Secara horizontal (default)
- column <- Secara vertikal
- row-reverse - Secara horizontal terbalik
- column-reverse <- Secara vertikal terbalik

justify-content <- Mengatur perataan item sepanjang sumbu utama

- flex-start <- Item berkumpul di awal container
- flex-end <- Item berkumpul di akhir container
- center <- Item berkumpul di tengah container
- space-between <- Item tersebar merata (item pertama di awal, terakhir di akhir)
- space-around <- Item tersebar merata dengan ruang setengahnya di ujung
- space-evenly <- Item tersebar merata dengan ruang sama di ujung

align-items <- Mengatur perataan item sepanjang sumbu silang

- stretch <- Item meregang untuk mengisi container (default)
- flex-start <- Item berkumpul di awal sumbu silang
- flex-end <- Item berkumpul di akhir sumbu silang
- center <- Item berkumpul di tengah sumbu silang
- baseline <- Item sejajar sesuai baseline mereka

flex-wrap <- Mengatur apakah item flex dipaksa dalam satu baris atau dapat dibungkus

- nowrap <- Semua item flex dalam satu baris (default)
- wrap <- Item flex akan membungkus ke beberapa baris
- wrap-reverse <- Item flex akan membungkus ke beberapa baris secara terbalik

Grid Properties
grid-template-columns - Mendefinisikan kolom dan ukurannya dalam grid
grid-template-rows - Mendefinisikan baris dan ukurannya dalam grid
grid-column-gap - Mengatur jarak antara kolom grid
grid-row-gap - Mengatur jarak antara baris grid
grid-gap - Shorthand untuk mengatur row-gap dan column-gap
grid-template-areas - Mendefinisikan area grid dengan nama
grid-area - Menetapkan elemen ke area grid tertentu

width - Mengatur lebar elemen

height - Mengatur tinggi elemen
min-width - Mengatur lebar minimum elemen
max-width - Mengatur lebar maksimum elemen
min-height - Mengatur tinggi minimum elemen
max-height - Mengatur tinggi maksimum elemen

Typography
font-family - Mengatur jenis font teks

font-size - Mengatur ukuran font teks

font-weight - Mengatur ketebalan font (normal, bold, 100-900)

font-style - Mengatur gaya font (normal, italic, oblique)

line-height - Mengatur tinggi baris teks

text-align - Mengatur perataan teks (left, right, center, justify)

text-decoration - Mengatur dekorasi teks (underline, overline, line-through, none)

text-transform - Mengatur kapitalisasi teks (uppercase, lowercase, capitalize)

letter-spacing - Mengatur spasi antar huruf

word-spacing - Mengatur spasi antar kata

Colors & Backgrounds
color - Mengatur warna teks

background-color - Mengatur warna latar belakang elemen

background-image - Mengatur gambar latar belakang elemen

background-repeat - Mengatur pengulangan gambar latar (repeat, repeat-x, repeat-y, no-repeat)

background-position - Mengatur posisi gambar latar (top, bottom, left, right, center)

background-size - Mengatur ukuran gambar latar (auto, cover, contain, nilai spesifik)

background-attachment - Mengatur apakah gambar latar scroll atau fixed (scroll, fixed)

Effects

visibility - Mengatur visibilitas elemen (visible, hidden, collapse)

Transforms & Transitions
transform - Mengaplikasikan transformasi 2D atau 3D

translate() - Memindahkan elemen

rotate() - Memutar elemen

scale() - Mengubah ukuran elemen

skew() - Miringkan elemen sepanjang sumbu X dan Y

transition - Shorthand untuk mengatur transisi

transition-property - Menentukan properti yang akan ditransisikan

transition-duration - Menentukan durasi transisi

transition-timing-function - Menentukan kurva kecepatan transisi

transition-delay - Menentukan penundaan sebelum transisi dimulai

Animation
animation - Shorthand untuk mengatur animasi

animation-name - Menentukan nama @keyframes animasi

animation-duration - Menentukan durasi animasi

animation-timing-function - Menentukan kurva kecepatan animasi

animation-delay - Menentukan penundaan sebelum animasi dimulai

animation-iteration-count - Menentukan berapa kali animasi diulang

animation-direction - Menentukan apakah animasi diputar mundur

animation-fill-mode - Menentukan style yang diterapkan saat animasi tidak dimainkan

Other Properties
cursor - Mengatur jenis kursor saat di atas elemen

overflow - Mengatur konten yang overflow (visible, hidden, scroll, auto)

z-index - Mengatur tumpukan elemen (stacking order)

box-sizing - Mengatur bagaimana lebar dan tinggi dihitung

list-style - Mengatur style untuk list items
