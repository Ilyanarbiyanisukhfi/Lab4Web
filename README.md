# Praktikum 4: CSS Layout (Box Element & Layout Sederhana) - Pemrograman Web
Repository ini dibuat untuk menyelesaikan tugas Praktikum 4 Pemrograman Web.

## Identitas Mahasiswa

| Keterangan      | Data                 |
| --------------- | -------------------- |
| **Nama**        | Ilyan Arbiyani Sukhfi |
| **Kelas**       | I251D                |
| **NIM**         | 312510436            |
| **Mata Kuliah** | Pemrograman Web      |
| **Dosen**       | Agung Nugroho, S.Kom., M.Kom. 

## Struktur Folder Proyek

```
modul-praktikum-4
├── Lab4_Layout/
│   ├── about.html
│   ├── article.html
│   ├── contact.html
│   ├── home.html
│   └── style.css
├── Lab4web/
│   └── Lab4_box.html
└── README.md
```
## Langkah-langkah Praktikum

### 1. Membuat Box Element (`Lab4_box.html`)

Langkah pertama adalah menyiapkan dokumen HTML dasar dengan nama `Lab4_box.html` yang berisi `<header>` dengan judul "Box Element".

<img width="940" height="362" alt="Screenshot 2026-10-15 212402" src="https://github.com/user-attachments/assets/d42f44f7-d3d5-43db-a4df-210fe74114db" />



Kemudian di dalam `<body>` ditambahkan `<section>` yang berisi empat buah `<div>` dengan class `div1` sampai `div4`.

<img width="638" height="147" alt="Screenshot 2026-10-15 212416" src="https://github.com/user-attachments/assets/0b50b07e-9aec-46d8-948a-1aea0aa0d4e4" />

#### CSS Float Property

Pada bagian `<head>` ditambahkan CSS internal untuk membuat float element:

- Semua `div` diberi `float: left` dan `padding: 10px`.
- `.div1` berwarna merah, `.div2` kuning, `.div3` hijau.
- `.div4` berwarna biru dengan `clear: left` dan `float: none` (clearfix) agar tampil di baris baru.

<img width="580" height="477" alt="Screenshot 2026-10-15 212427" src="https://github.com/user-attachments/assets/f6ed04d5-91be-4754-86a9-757feb0ecfd9" />

Hasil di browser: Div1, Div2, dan Div3 tampil sejajar ke samping, sedangkan Div4 berada di bawahnya dengan lebar penuh.

<img width="610" height="329" alt="image" src="https://github.com/user-attachments/assets/5fb3c7e9-e158-4135-9f90-82e02386dc3c" />


---

### 2. Membuat Layout Sederhana (`Lab4_Layout.html`)

Membuat kerangka layout menggunakan semantic element. Dokumen ini menghubungkan file `style.css` dan memiliki `<div id="container">` sebagai pembungkus utama.

<img width="835" height="166" alt="Screenshot 2026-10-15 213033" src="https://github.com/user-attachments/assets/6cb6e599-b317-426b-b541-de024c65926d" />

Di dalam container ditambahkan elemen `<header>`, `<nav>` (Home, Artikel, About, Kontak), `<section id="hero">`, `<section id="wrapper">` (berisi `<section id="main">` dan `<aside id="sidebar">`), serta `<footer>`.

<img width="381" height="178" alt="Screenshot 2026-10-15 213108" src="https://github.com/user-attachments/assets/fb025e9a-122b-45a6-a8b6-4812f7d5ac91" />

<img width="776" height="498" alt="Screenshot 2026-10-15 213306" src="https://github.com/user-attachments/assets/0d9b5c72-8672-4aaa-a700-9f0ab1aeceae" />

Hasil sebelum diberi CSS:

<img width="499" height="227" alt="image" src="https://github.com/user-attachments/assets/e732dd22-b7c0-48b7-abe8-4a1cff3e2c5b" />


---

### 3. Menambahkan CSS Layout (`style.css`)

CSS ditambahkan untuk membuat tampilan dasar layout, meliputi:

- `@import` Google Font **Open Sans** dan **Open Sans Condensed**.
- Reset CSS (`margin: 0; padding: 0`).
- Pengaturan `body` (font-size, font-family, warna teks).
- `#container` dengan lebar `980px`, rata tengah (`margin: 0 auto`), dan `box-shadow`.
- Pengaturan `header` dan `header h1`.

<img width="1515" height="835" alt="Screenshot 2026-10-15 213436" src="https://github.com/user-attachments/assets/ccf05dd0-6841-48ed-bbcf-562e1e1dcf89" />

Hasil di browser:

<img width="959" height="262" alt="image" src="https://github.com/user-attachments/assets/0325dff5-b0eb-49f2-a9b3-1c3a03af7b69" />


---

### 4. Mengatur Navigasi

CSS navigasi dibuat dengan ketentuan:

- `nav` memiliki background biru (`#1f5faa`).
- Link `nav a` ditampilkan `inline-block`, berwarna putih, tebal, tanpa garis bawah.
- `nav a.active` dan `nav a:hover` memiliki background `#2b83ea`.

<img width="510" height="477" alt="Screenshot 2026-10-15 213924" src="https://github.com/user-attachments/assets/88fe57fb-b4f5-4e70-8b2a-f739a34acf39" />

<img width="752" height="240" alt="image" src="https://github.com/user-attachments/assets/fc16e22a-90f6-4866-b155-4190e529a3b0" />


---

### 5. Membuat Hero Panel

Menambahkan kode HTML pada `<section id="hero">` berisi judul, paragraf, dan tombol "Learn more", lalu diberi style: background abu-abu (`#e4e4e5`), padding, serta pengaturan ukuran font `h1` dan `p`.

<img width="1002" height="172" alt="Screenshot 2026-10-15 214046" src="https://github.com/user-attachments/assets/9f25352e-6692-465a-b06c-fe2abaed32da" />

<img width="732" height="416" alt="Screenshot 2026-10-15 214105" src="https://github.com/user-attachments/assets/0f77aa07-87d2-4a8c-94e0-fdec7e81bc0f" />

<img width="440" height="254" alt="image" src="https://github.com/user-attachments/assets/584c4f57-aa78-450f-897b-c47056ad9927" />


---

### 6. Menambahkan CSS Float untuk Main Content dan Sidebar

- `#main` dan `#sidebar` menggunakan `float: left`.
- Lebar `#main` = `640px`, lebar `#sidebar` = `260px`, keduanya dengan `padding: 20px`.
- Sidebar berisi dua `widget-box` (daftar link dan teks) yang diberi style border, title berwarna biru (`#428bca`), list tanpa bullet, dan efek hover.

<img width="472" height="415" alt="Screenshot 2026-10-15 214325" src="https://github.com/user-attachments/assets/5c383462-7168-4183-a72d-08509962a501" />

<img width="1005" height="452" alt="Screenshot 2026-10-15 214351" src="https://github.com/user-attachments/assets/10e99933-6180-4baf-996c-d5aef530d667" />

<img width="595" height="852" alt="Screenshot 2026-10-15 214419" src="https://github.com/user-attachments/assets/bc00003b-d7d7-45f6-84a1-43549338106d" />

<img width="361" height="413" alt="image" src="https://github.com/user-attachments/assets/86ef685a-47ed-43b1-b265-9b225c4bf1d4" />


---

### 7. Mengubah Tampilan Footer

Footer diberi style background gelap dengan teks putih agar terlihat berbeda dari konten utama.

<img width="671" height="73" alt="Screenshot 2026-10-15 214628" src="https://github.com/user-attachments/assets/5f39b232-f4aa-4aa5-9802-eb1084c03556" />

<img width="535" height="165" alt="Screenshot 2026-10-15 214613" src="https://github.com/user-attachments/assets/2add179c-5076-40eb-97a9-1e4523803683" />

<img width="1240" height="73" alt="Screenshot 2026-10-15 214805" src="https://github.com/user-attachments/assets/756b4190-391d-4e63-b38e-9914fa7d90d7" />

---

### 8. Menambahkan Elemen Lain pada Main Content

Menambahkan `div.row` yang berisi tiga `div.box`. Masing-masing box memiliki gambar, heading, paragraf, dan tombol "View detail". CSS yang digunakan:

- `.box` dengan `float: left`, `width: 33.333333%`, `box-sizing: border-box`, dan `text-align: center`.
- `.image-circle` dengan `border-radius: 50%` agar gambar berbentuk lingkaran.
- `.row` dengan margin negatif dan clearfix (`:before` dan `:after` dengan `display: table` dan `clear: both`).

<img width="1087" height="477" alt="Screenshot 2026-10-15 214928" src="https://github.com/user-attachments/assets/a569ee42-a909-4b37-9b04-543d66255c1a" />

<img width="657" height="641" alt="Screenshot 2026-10-15 214950" src="https://github.com/user-attachments/assets/2bf2390e-6a14-4b28-a234-d8f7ac3af5f4" />

<img width="711" height="506" alt="Screenshot 2026-10-15 215002" src="https://github.com/user-attachments/assets/854360ff-f74b-4da4-8587-aa82a88f95fd" />


<img width="322" height="272" alt="image" src="https://github.com/user-attachments/assets/26d56f2f-edb4-4cf1-b944-71b15aea41a8" />


---

### 9. Membuat Content Artikel

Menambahkan dua `<article class="entry">` yang dipisah dengan `<hr class="divider">`. Artikel pertama memiliki gambar di kiri, sedangkan artikel kedua memakai class `right-img` sehingga gambar berada di kanan.

CSS `.entry`:
- `margin: 15px 0`, `h2` dengan `margin-bottom: 20px`, dan `p` dengan `line-height: 25px`.
- `.entry img` menggunakan `float: left`, `border-radius: 5px`, dan `margin-right: 15px`.
- `.entry .right-img` menggunakan `float: right` dengan margin kiri `15px`.

<img width="1116" height="425" alt="Screenshot 2026-10-15 215540" src="https://github.com/user-attachments/assets/06ed77f1-b677-4601-8e69-1db50f8a4e43" />

<img width="765" height="691" alt="Screenshot 2026-10-15 215554" src="https://github.com/user-attachments/assets/1898e1b4-5cd7-4636-81c1-c2f13d3aa52b" />

<img width="469" height="316" alt="image" src="https://github.com/user-attachments/assets/cce429ae-882d-4f25-9c75-d7394e306fa7" />

ada pun hasil screenshot dari tugas untuk menampilkan about dan contact
