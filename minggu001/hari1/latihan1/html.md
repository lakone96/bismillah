Berikut adalah daftar tag HTML yang umum digunakan beserta atribut pentingnya (tidak termasuk tag yang usang/deprecated):

### 1. Tag Struktur Dokumen

- **`<!DOCTYPE html>`**: Mendefinisikan tipe dokumen sebagai HTML5.
- **`<html>`**: Elemen root dokumen.
  - Atribut: `lang` (bahasa dokumen, contoh: `lang="id"`).
- **`<head>`**: Berisi metadata dokumen.
- **`<title>`**: Judul halaman (ditampilkan di tab browser).
- **`<meta>`**: Metadata tambahan.
  - Atribut: `charset` (encoding, contoh: `charset="UTF-8"`), `name="viewport"` (untuk responsive design), `content`.
- **`<body>`**: Konten utama halaman.

---

### 2. Tag Konten Teks

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

### 3. Tag Multimedia

- **`<img>`**: Gambar.
  - Atribut: `src` (sumber gambar), `alt` (teks alternatif), `width`, `height`, `loading="lazy"`.
- **`<video>`**: Video.
  - Atribut: `src`, `controls`, `autoplay`, `loop`, `muted`, `poster` (thumbnail).
- **`<audio>`**: Audio.
  - Atribut: `src`, `controls`, `autoplay`, `loop`.
- **`<source>`**: Sumber alternatif media (dalam `<video>`/`<audio>`).
  - Atribut: `src`, `type` (contoh: `type="video/mp4"`).

---

### 4. Tag Tautan

- **`<a>`**: Tautan/hyperlink.
  - Atribut: `href` (URL), `target` (contoh: `target="_blank"` untuk buka tab baru), `rel` (contoh: `rel="noopener"`).

---

### 5. Tag List

- **`<ul>`**: Unordered list (list dengan bullet).
- **`<ol>`**: Ordered list (list berangka).
  - Atribut: `type` (jenis penomoran), `start` (mulai dari angka tertentu).
- **`<li>`**: Item list.

---

### 6. Tag Tabel

- **`<table>`**: Tabel.
- **`<thead>`**: Header tabel.
- **`<tbody>`**: Body tabel.
- **`<tfoot>`**: Footer tabel.
- **`<tr>`**: Baris tabel.
- **`<th>`**: Sel header tabel.
  - Atribut: `colspan`, `rowspan`.
- **`<td>`**: Sel data tabel.
  - Atribut: `colspan`, `rowspan`.

---

### 7. Tag Formulir

- **`<form>`**: Formulir input.
  - Atribut: `action` (URL pengolahan data), `method` (`GET`/`POST`), `target`.
- **`<input>`**: Field input.
  - Atribut: `type` (text, email, password, number, checkbox, radio, date, file, dll.), `name`, `placeholder`, `required`, `value`.
- **`<textarea>`**: Input teks multi-baris.
  - Atribut: `rows`, `cols`, `name`, `placeholder`.
- **`<select>`**: Dropdown list.
- **`<option>`**: Opsi dalam `<select>`.
  - Atribut: `value`, `selected`.
- **`<label>`**: Label untuk input.
  - Atribut: `for` (id input terkait).
- **`<button>`**: Tombol.
  - Atribut: `type` (submit, reset, button).

---

### 8. Tag Semantik HTML5

- **`<header>`**: Header halaman atau section.
- **`<nav>`**: Navigasi.
- **`<main>`**: Konten utama.
- **`<article>`**: Konten independen (artikel, blog post).
- **`<section>`**: Bagian dalam dokumen.
- **`<aside>`**: Konten samping (sidebar).
- **`<footer>`**: Footer halaman atau section.
- **`<figure>`**: Konten mandiri (gambar, diagram).
- **`<figcaption>`**: Keterangan untuk `<figure>`.

---

### 9. Tag Lainnya

- **`<div>`**: Kontainer generik untuk grouping.
  - Atribut: `class`, `id`.
- **`<iframe>`**: Embed konten dari sumber lain.
  - Atribut: `src`, `width`, `height`, `title`.
- **`<progress>`**: Progress bar.
  - Atribut: `value`, `max`.
- **`<time>`**: Menandai waktu/tanggal.
  - Atribut: `datetime` (format mesin).

---

### Catatan:

- **Atribut Global**: Semua tag di atas mendukung atribut global seperti `class`, `id`, `style`, `title`, `data-*`, `hidden`, `lang`, `tabindex`, dll.
- **Atribut Event**: Seperti `onclick`, `onmouseover`, dll. (biasanya ditambahkan via JavaScript).
- **HTML5 Focus**: Tag semantik seperti `<article>`, `<section>`, dll. lebih disarankan untuk menggantikan `<div>` yang generik.

Pastikan untuk selalu memvalidasi HTML menggunakan tools seperti [W3C Validator](https://validator.w3.org/) untuk memastikan kesesuaian dengan standar terkini.
