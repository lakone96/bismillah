# Daftar Property CSS yang Umum Digunakan

Property CSS yang paling umum digunakan beserta nilai-nilainya, dengan fokus pada property yang relevan untuk mempelajari Tailwind CSS:

## 1. Layout & Positioning

### `display`
Mengatur bagaimana elemen ditampilkan.
- **Nilai umum**:
  - `block` (Tailwind: `block`)
  - `inline` (Tailwind: `inline`)
  - `inline-block` (Tailwind: `inline-block`)
  - `flex` (Tailwind: `flex`)
  - `grid` (Tailwind: `grid`)
  - `none` (menyembunyikan elemen, Tailwind: `hidden`)

### `position`
Mengatur metode positioning elemen.
- **Nilai umum**:
  - `static` (Tailwind: `static`)
  - `relative` (Tailwind: `relative`)
  - `absolute` (Tailwind: `absolute`)
  - `fixed` (Tailwind: `fixed`)
  - `sticky` (Tailwind: `sticky`)

### `top`, `right`, `bottom`, `left`
Mengatur posisi elemen yang dipositioning.
- **Nilai umum**:
  - Nilai panjang: `px`, `rem`, `em`, `%`, dll. (Tailwind: `top-4`, `left-1/2`)
  - `auto` (Tailwind: `top-auto`)

### `float`
Mengatur bagaimana elemen mengambang.
- **Nilai umum**:
  - `left` (Tailwind: `float-left`)
  - `right` (Tailwind: `float-right`)
  - `none` (Tailwind: `float-none`)

### `clear`
Mengatur sisi mana yang tidak boleh ada elemen floating.
- **Nilai umum**:
  - `left` (Tailwind: `clear-left`)
  - `right` (Tailwind: `clear-right`)
  - `both` (Tailwind: `clear-both`)
  - `none` (Tailwind: `clear-none`)

## 2. Box Model

### `width` dan `height`
Mengatur lebar dan tinggi elemen.
- **Nilai umum**:
  - Nilai panjang: `px`, `rem`, `em`, `%`, `vh`, `vw` (Tailwind: `w-4`, `h-8`, `w-1/2`)
  - `auto` (Tailwind: `w-auto`)
  - `max-content`, `min-content`, `fit-content`

### `margin`
Mengatur jarak luar elemen.
- **Nilai umum**:
  - Nilai panjang: `px`, `rem`, `em`, `%` (Tailwind: `m-4`, `mx-2`, `my-3`)
  - `auto` (Tailwind: `mx-auto`)

### `padding`
Mengatur jarak dalam elemen.
- **Nilai umum**:
  - Nilai panjang: `px`, `rem`, `em`, `%` (Tailwind: `p-4`, `px-2`, `py-3`)

### `border`
Mengatur border elemen.
- **Nilai umum**:
  - `border-width` (Tailwind: `border`, `border-2`)
  - `border-style` (Tailwind: `border-solid`, `border-dashed`)
  - `border-color` (Tailwind: `border-red-500`)

### `border-radius`
Mengatur sudut lengkung border.
- **Nilai umum**:
  - Nilai panjang: `px`, `rem`, `em`, `%` (Tailwind: `rounded`, `rounded-lg`, `rounded-full`)

### `box-sizing`
Mengatur bagaimana lebar dan tinggi dihitung.
- **Nilai umum**:
  - `content-box` (default)
  - `border-box` (Tailwind: tidak langsung, tetapi penting untuk layout)

## 3. Flexbox

### `flex-direction`
Mengatur arah item flex.
- **Nilai umum**:
  - `row` (Tailwind: `flex-row`)
  - `row-reverse` (Tailwind: `flex-row-reverse`)
  - `column` (Tailwind: `flex-column`)
  - `column-reverse` (Tailwind: `flex-column-reverse`)

### `justify-content`
Mengatur penjajaran item flex pada sumbu utama.
- **Nilai umum**:
  - `flex-start` (Tailwind: `justify-start`)
  - `flex-end` (Tailwind: `justify-end`)
  - `center` (Tailwind: `justify-center`)
  - `space-between` (Tailwind: `justify-between`)
  - `space-around` (Tailwind: `justify-around`)
  - `space-evenly` (Tailwind: `justify-evenly`)

### `align-items`
Mengatur penjajaran item flex pada sumbu silang.
- **Nilai umum**:
  - `stretch` (Tailwind: `items-stretch`)
  - `flex-start` (Tailwind: `items-start`)
  - `flex-end` (Tailwind: `items-end`)
  - `center` (Tailwind: `items-center`)
  - `baseline` (Tailwind: `items-baseline`)

### `flex-wrap`
Mengatur apakah item flex dipaksa dalam satu baris atau dapat dibungkus.
- **Nilai umum**:
  - `nowrap` (Tailwind: `flex-nowrap`)
  - `wrap` (Tailwind: `flex-wrap`)
  - `wrap-reverse` (Tailwind: `flex-wrap-reverse`)

### `flex`
Mengatur bagaimana item flex tumbuh atau menyusut.
- **Nilai umum**:
  - `flex-grow` `flex-shrink` `flex-basis` (Tailwind: `flex-1`, `flex-auto`, `flex-none`)

## 4. Grid

### `grid-template-columns` dan `grid-template-rows`
Mendefinisikan kolom dan baris grid.
- **Nilai umum**:
  - `repeat()`, `minmax()`, `auto`, `fr` units (Tailwind: `grid-cols-3`, `grid-rows-2`)

### `gap`
Mengatur jarak antara grid items.
- **Nilai umum**:
  - Nilai panjang: `px`, `rem` (Tailwind: `gap-4`, `gap-x-2`, `gap-y-3`)

### `grid-column` dan `grid-row`
Mengatur penempatan item pada grid.
- **Nilai umum**:
  - Line numbers, span (Tailwind: `col-span-2`, `row-span-3`)

## 5. Typography

### `font-family`
Mengatur jenis font.
- **Nilai umum**:
  - Nama font: `Arial`, `Helvetica`, `sans-serif` (Tailwind: `font-sans`, `font-serif`)

### `font-size`
Mengatur ukuran font.
- **Nilai umum**:
  - `px`, `rem`, `em` (Tailwind: `text-xs`, `text-sm`, `text-base`, `text-lg`)

### `font-weight`
Mengatur ketebalan font.
- **Nilai umum**:
  - `normal`, `bold`, `100`-`900` (Tailwind: `font-normal`, `font-medium`, `font-bold`)

### `text-align`
Mengatur perataan teks.
- **Nilai umum**:
  - `left` (Tailwind: `text-left`)
  - `center` (Tailwind: `text-center`)
  - `right` (Tailwind: `text-right`)
  - `justify` (Tailwind: `text-justify`)

### `line-height`
Mengatur tinggi baris.
- **Nilai umum**:
  - Unitless numbers, `px`, `rem` (Tailwind: `leading-none`, `leading-normal`, `leading-relaxed`)

### `letter-spacing`
Mengatur jarak antar huruf.
- **Nilai umum**:
  - `px`, `em` (Tailwind: `tracking-tight`, `tracking-normal`, `tracking-wide`)

### `text-transform`
Mengatur transformasi teks.
- **Nilai umum**:
  - `none` (Tailwind: `normal-case`)
  - `uppercase` (Tailwind: `uppercase`)
  - `lowercase` (Tailwind: `lowercase`)
  - `capitalize` (Tailwind: `capitalize`)

### `text-decoration`
Mengatur dekorasi teks.
- **Nilai umum**:
  - `none` (Tailwind: `no-underline`)
  - `underline` (Tailwind: `underline`)
  - `line-through` (Tailwind: `line-through`)

## 6. Colors & Backgrounds

### `color`
Mengatur warna teks.
- **Nilai umum**:
  - HEX: `#ff0000`
  - RGB: `rgb(255, 0, 0)`
  - RGBA: `rgba(255, 0, 0, 0.5)`
  - HSL: `hsl(0, 100%, 50%)`
  - Nama warna: `red` (Tailwind: `text-red-500`, `text-blue-700`)

### `background-color`
Mengatur warna latar belakang.
- **Nilai umum**:
  - Sama seperti `color` (Tailwind: `bg-red-500`, `bg-blue-700`)

### `background-image`
Mengatur gambar latar belakang.
- **Nilai umum**:
  - `url('image.jpg')` (Tailwind: `bg-[url('/img/image.jpg')]`)
  - Gradien: `linear-gradient()`, `radial-gradient()` (Tailwind: `bg-gradient-to-r`)

### `background-size`
Mengatur ukuran gambar latar belakang.
- **Nilai umum**:
  - `cover` (Tailwind: `bg-cover`)
  - `contain` (Tailwind: `bg-contain`)
  - Nilai panjang: `px`, `%`

### `background-position`
Mengatur posisi gambar latar belakang.
- **Nilai umum**:
  - `center`, `top`, `bottom`, `left`, `right` (Tailwind: `bg-center`, `bg-top`)

### `background-repeat`
Mengatur pengulangan gambar latar belakang.
- **Nilai umum**:
  - `repeat` (Tailwind: `bg-repeat`)
  - `no-repeat` (Tailwind: `bg-no-repeat`)
  - `repeat-x`, `repeat-y` (Tailwind: `bg-repeat-x`, `bg-repeat-y`)

## 7. Effects & Transitions

### `opacity`
Mengatur transparansi elemen.
- **Nilai umum**:
  - `0` hingga `1` (Tailwind: `opacity-0`, `opacity-50`, `opacity-100`)

### `box-shadow`
Mengatur bayangan elemen.
- **Nilai umum**:
  - Nilai bayangan: `offset-x offset-y blur-radius spread-radius color` (Tailwind: `shadow`, `shadow-md`, `shadow-lg`)

### `transform`
Menerapkan transformasi 2D atau 3D.
- **Nilai umum**:
  - `translate()`, `rotate()`, `scale()`, `skew()` (Tailwind: `translate-x-4`, `rotate-45`, `scale-110`)

### `transition`
Mengatur transisi antara states.
- **Nilai umum**:
  - Property, duration, timing-function, delay (Tailwind: `transition`, `duration-300`, `ease-in-out`)

## 8. Miscellaneous

### `cursor`
Mengatur jenis kursor.
- **Nilai umum**:
  - `auto`, `default`, `pointer`, `text`, `move` (Tailwind: `cursor-pointer`, `cursor-text`)

### `overflow`
Mengatur bagaimana konten yang overflow ditangani.
- **Nilai umum**:
  - `visible` (Tailwind: `overflow-visible`)
  - `hidden` (Tailwind: `overflow-hidden`)
  - `scroll` (Tailwind: `overflow-scroll`)
  - `auto` (Tailwind: `overflow-auto`)

### `z-index`
Mengatur tumpukan elemen.
- **Nilai umum**:
  - Bilangan bulat: `0`, `10`, `50`, `100` (Tailwind: `z-0`, `z-10`, `z-50`)

### `visibility`
Mengatur visibilitas elemen.
- **Nilai umum**:
  - `visible` (Tailwind: `visible`)
  - `hidden` (Tailwind: `invisible`)

## Konsep Penting untuk Tailwind CSS

Tailwind CSS menggunakan pendekatan utility-first, di mana setiap class mewakili satu property CSS. Beberapa konsep penting:

1. **Responsive Design**: Tailwind menggunakan breakpoints (sm, md, lg, xl, 2xl)
   - Contoh: `md:text-center`, `lg:p-8`

2. **State Variants**: Tailwind mendukung state seperti hover, focus, active
   - Contoh: `hover:bg-blue-700`, `focus:outline-none`

3. **Spacing Scale**: Tailwind menggunakan skala spacing yang konsisten
   - 0, 0.5, 1, 1.5, 2, 2.5, 3, 3.5, 4, ... (dalam rem)

4. **Color Palette**: Tailwind memiliki palette warna yang konsisten
   - 50, 100, 200, ..., 900 untuk setiap warna

5. **Dark Mode**: Tailwind mendukung dark mode
   - Contoh: `dark:bg-gray-800`, `dark:text-white`

Dengan memahami property CSS dan nilai-nilainya, Kamu akan lebih mudah memahami dan menggunakan Tailwind CSS, karena pada dasarnya Tailwind adalah kumpulan class yang mewakili property CSS tersebut.