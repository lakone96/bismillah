### Daftar Tag HTML dan Atributnya

Berikut adalah penjelasan detail tentang tag HTML yang umum digunakan beserta atribut-atributnya.

---

## --> 1. Tag Struktur Dokumen

- **`<!DOCTYPE html>`** Mendefinisikan tipe dokumen sebagai HTML5.
- **`<html>`** Tag root dari dokumen HTML.
- **`<head>`** Berisi metadata tentang dokumen, seperti judul, stylesheet, dan script.
- **`<title>`** Menentukan judul dokumen yang ditampilkan di tab browser.
- **`<meta>`** Menyediakan metadata tentang dokumen HTML.
- Atribut penting: `charset` : Menentukan encoding karakter (contoh: `charset="UTF-8"`)
  `name`: Nama metadata (contoh: `name="viewport"`, `name="description"`)
    `content`: Nilai metadata (contoh: `content="width=device-width, initial-scale=1.0"`)
- **` <body> `** Berisi konten utama dokumen HTML.

---

## --> 2. Tag Heading & Teks

- **`<h1>` hingga `<h6>`**: Heading (judul dan subjudul).
- **`<p>`**: Paragraf.
- **`<br>`**: Line break (baris baru).
- **`<hr>`**: Garis horizontal.
- **`<strong>`**: Teks penting (tebal).
- **`<em>`**: Teks yang ditekankan (miring).
- **`<span>`**: Pengelompokan teks inline (dengan CSS/JS).
  - Atribut: `class`, `id`.
- **`<blockquote>`**: Kutipan panjang.
  - Atribut: `cite` (sumber kutipan).
- **`<q>`**: Kutipan pendek inline.
- **`<code>`**: Menampilkan kode program.
- **`<pre>`**: Teks terformat (spasi dan baris baru dipertahankan).

---

## --> 3. Tag Multimedia
-**` <img> `** Menampilkan gambar.
- Atribut penting:
`src`: URL gambar
`alt`: Teks alternatif untuk aksesibilitas
`width`: Lebar gambar (dalam piksel)
`height`: Tinggi gambar (dalam piksel)
`loading`: Kontrol lazy loading (loading="lazy")
-**` <video> `** Menampilkan video.
- Atribut penting:
`src`: URL video
`controls`: Menampilkan kontrol pemutaran
`autoplay`: Memutar video otomatis
`loop`: Mengulang video
`muted`: Mematikan suara
`poster`: Gambar thumbnail sebelum pemutaran
-**` <audio> `** Menampilkan audio.
- Atribut penting:
`src`: URL audio
`controls`: Menampilkan kontrol pemutaran
`autoplay`: Memutar audio otomatis
`loop`: Mengulang audio

---

## --> 4. Tag Tautan
-**` <a> `** Membuat hyperlink.
- Atribut penting:
`href`: URL tujuan
`target`: Menentukan tempat membuka tautan (`_blank` untuk tab baru)
`rel`: Menentukan hubungan dengan dokumen tertaut (`noopener, noreferrer`)

---

## --> 5. Tag List
-**` <ul> `** Membuat unordered list (list dengan bullet).
-**` <ol> `** Membuat ordered list (list berurutan dengan angka/huruf).
- Atribut penting:
`type`: Jenis penomoran (`1, A, a, I, i`)
`start`: Nilai awal penomoran
-**` <li> `** Item dalam list.

---

## --> 6. Tag Tabel
-**` <table> `** Membuat tabel.
-**` <tr> `** Membuat baris tabel.
-**` <th> `** Membuat sel header tabel.
- Atribut penting:
`colspan`: Jumlah kolom yang dijangkau
`rowspan`: Jumlah baris yang dijangkau
-**` <td> `** Membuat sel data tabel.
Atribut penting:
`colspan`: Jumlah kolom yang dijangkau
`rowspan`: Jumlah baris yang dijangkau

---

## --> 7. Tag Formulir
-**` <form> `** Membuat form untuk input pengguna.
- Atribut penting:
`action`: URL yang akan memproses form
`method`: Metode HTTP (`GET` atau `POST`)
`target`: Di mana menampilkan respons
-**` <input> `** Membuat field input.
- Atribut penting:
`type`: Jenis input (`text, password, email, number, checkbox, radio, tel, url, range, date,week, mounth, time, color`.)
`name`: Nama field
`placeholder`: Teks petunjuk
`required`: Wajib diisi
`value`: Nilai default
-**` <textarea> `** Membuat area teks multi-baris.
- Atribut penting:
`rows`: Jumlah baris
`cols`: Jumlah kolom
`name`: Nama field
-**` <select> `** Membuat dropdown list.
-**` <option> `** Membuat opsi dalam dropdown.
- Atribut penting:
`value`: Nilai opsi
`selected`: Opsi yang terpilih secara default
-**` <button> `** Membuat tombol.
- Atribut penting:
`type`: Jenis tombol (`submit, reset, button`)

---

## --> 8. Tag Semantik HTML5
-**` <header> `** Mewakili header dokumen atau section.
-**` <nav> `** Mewakili bagian navigasi.
-**` <main> `** Mewakili konten utama dokumen.
-**` <aside> `** Mewakili konten samping (sidebar).
-**` <footer> `** Mewakili footer dokumen atau section.
-**` <figure> `** Mengelompokkan konten media dengan keterangannya.
-**` <figcaption> `** Menambahkan keterangan untuk `<figure>`.

---

## --> 9. Tag Lainnya
-**` <div> `** Membuat kontainer generik untuk pengelompokan dan styling.
- Atribut penting:
`class`: Kelas CSS
`id`: Identifier unik
-**` <iframe> `** Menanamkan dokumen HTML lain.
- Atribut penting:
`src`: URL dokumen
`width`: Lebar iframe
`height`: Tinggi iframe
`title`: Judul untuk aksesibilitas

---

## --> 10. Atribut Global
Semua tag HTML mendukung atribut global berikut:
`class`: Menentukan satu atau beberapa kelas CSS
`id`: Identifier unik
`title`: Informasi tambahan (ditampilkan sebagai tooltip)
`data-\*`: Atribut kustom untuk menyimpan data
`hidden`: Menyembunyikan elemen

---

## --> Entitas :

© &#169; &copy; COPYRIGHT SYMBOL
® &#174; &reg; REGISTERED TRADEMARK
€ &#8364; &euro; EURO SIGN
™ &#8482; &trade; TRADEMARK
← &#8592; &larr; LEFTWARDS ARROW
↑ &#8593; &uarr; UPWARDS ARROW
→ &#8594; &rarr; RIGHTWARDS ARROW
↓ &#8595; &darr; DOWNWARDS ARROW
♠ &#9824; &spades; BLACK SPADE SUIT
♣ &#9827; &clubs; BLACK CLUB SUIT
♥ &#9829; &hearts; BLACK HEART SUIT
♦ &#9830; &diams; BLACK DIAMOND SUIT

selengkapnya : [W3shools](https://www.w3schools.com/charsets/ref_html_symbols.asp)