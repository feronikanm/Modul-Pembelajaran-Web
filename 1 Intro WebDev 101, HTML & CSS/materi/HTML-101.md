# Hypertext Markup Language (HTML)

HTML berguna untuk menampilkan konten, menghubungkan (link) antar halaman, memberi struktur dan informasi terkait dengan sebuah halaman web. Konten sebuah web tidak hanya terbatas pada teks saja, melainkan konten interaktif lainnya seperti video, audio, gambar dan animasi dapat disisipkan dan ditampilkan pada halaman web.

## Struktur HTML

### A. Tag HTML
```html
<nama_tag></nama_tag>
```

### B. Elemen HTML
Rangkaian dari tag pembuka, konten dan tag penutup disebut dengan elemen HTML.

```html
<h1>Heading</h1>
<p>Paragraf</p>
```

### C. Tag di dalam Elemen Head
Elemen yang ada di dalam head berfungsi sebagai informasi dari dokumen HTML dan tidak akan ditampilkan di layar browser. Beberapa tag yang dapat digunakan di dalam elemn head diantaranya adalah
```html 
<meta>, <title>, <style>, <script>, <link>
```

### D. Tag di dalam Elemen Body
Ada banyak tag yang dapat digunakan untuk menampilkan konten di dalam elemen body.

#### Tag untuk teks 
```html
<h1>, <h2>, <h3>, <h3>, <h4>, <h5>, <p>, dll
```

#### Tag untuk menformat teks
```html
<b>, <i>, <strong>, <em>, <mark>, <del>, dll
```

#### Tag untuk menampilkan gambar
```html
<img>
```

#### Tag untuk membuat tautan
```html
<a>
```

#### Tag untuk membuat tabel
Dengan menggunakan kombinasi tag:
```html
<table>, <thead>, <tbody>, <tr>, <th>, <td>
```

#### Tag untuk membuat list
Dengan menggunakan kombinasi tag:
```html
<ul>, <ol>, <li>, <dl>, <dd>, <dt>
```

#### Tag untuk membuat form input
Dengan menggunakan kombinasi tag:
```html
<form>, <select>, <optgroup>, <option>, <input type="text|checkbox|radio">, <textarea>
```

#### Tag untuk memasukan halaman website lain
```html
<iframe>
```

Seluruh tag HTML lengkapnya bisa dicek di https://www.w3schools.com/tags/. Jangan kaget jika ternyata terdapat banyak tag di HTML. Tidak perlu dihafal karena kita hanya menggunakan seperlunya saja dan penggunaan tag-tag baru memungkinkan akan kita gunakan ketika kita mengerjakan sebuah proyek dan membutuhkan tag-tag baru tersebut.

## Attribut HTML
Atribut memberikan informasi tambahan bagi tag
```html
<namatag nama-atribut="nilai-atribut"></namatag>
```
Contoh:
```html
<a href="login.html">Login</a>
```

Selain tag contoh di atas, sebenarnya ada banyak tag lain yang memerlukan atribut. 

Bila dikelompokkan, ada dua jenis atribut, yakni atribut global dan atribut spesifik. 
- Atribut global adalah atribut yang dapat diterapkan pada tag apapun karena sifatnya yang umum. Contohnya <strong>class, id, lang, title, style, dll</strong>. 
- Atribut spesifik adalah atribut yang hanya berfungsi pada tag-tag tertentu, seperti atribut href yang hanya berlaku pada tag <strong>a</strong> dan <strong>link</strong>, atribut src yang hanya berlaku pada tag <strong>img</strong> dan <strong>script</strong>, dan lain sebagainya.

Selengkapnya mengenai atribut tag HTML bisa ditemukan di https://www.w3schools.com/html/html_attributes.

## Fitur baru di HTML5

### 1. Doctype
DOCTYPE ditulis sebelum tag pembuka html, digunakan untuk memberitahu web browser versi html yang akan ditulis.

HTML5
```html
<!DOCTYPE html>
```

HTML versi lama
```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
```

### 2. Figure
Figure digunakan untuk menentukan konten yang berdiri sendiri, seperti ilustrasi, diagram, foto dll.

```html
<figure>
    <img src="CAT.jpg" alt="Kucing" width="200" height="200">
    <figcaption>
        Gambar kucing dari 9GAG
    </figcaption>
</figure>
```

### 3. "Type" Javascript & Link CSS
Digunakan untuk menghubungkan file HTML dengan Javascript

HTML5
```html
<script src="path/app.js"></script>
```
HTML versi lama
```html
<script src="path/app.js" type="text/javascript"></script>
```

Pada HTML5 tidak perlu ditulis type="text/javascript".

### 4. Atribut Placeholders
Atribut placeholder digunakan untuk memberikan petunjuk atau keterangan pada kolom input
```html
<input type="text" name="search" placeholder="Pencarian">
```

### 5. Atribut Required 
Atribut required digunakna untuk menyatakan bahwa form input tersebut wajib diisi.
```html
Username: <input type="text" name="username" autofocus>
Password: <input type="text" name="password">
```

### 6. Autofocus
Menentukan letak fokus utama pengisian saat website dibuka.
```html
Username: <input type="text" name="username" autofocus>
Password: <input type="text" name="password">
```

### 7. Multimedia Player
Digunakan untuk memasang multimedia player pada halaman website.

Video
```html
<video width="300" height="300" controls muted poster="thumbnail.jpg">
    <source src="video_utama.mp4" type="video/mp4">
    <source src="video alternatif" type="video/ogg">
    Browser anda tidak mendukung format video ini.
</video>
```

Audio
```html
<audio controls loop muted>
    <source src="audio" type="video/ogg">
    Browser anda tidak mendukung format audio ini.
</audio>
```

### 8. 


## Referensi
- Dasar HTML - CodePolitan.com. (n.d.). Retrieved March 3, 2020, from https://www.codepolitan.com/course/lesson/basic-html-dan-css/01-Pengenalan-HTML-dan-CSS/02-dasar-html
- Belajar HTML dari dasar | Sekolah Koding. (n.d.). Retrieved March 3, 2020, from https://sekolahkoding.com/kelas/belajar-html-dari-dasar
- Belajar html5 | Sekolah Koding. (n.d.). Retrieved March 3, 2020, from https://sekolahkoding.com/kelas/belajar-html5
- HTML Reference. (n.d.). Retrieved March 3, 2020, from https://www.w3schools.com/tags/
- HTML Attributes. (n.d.). Retrieved March 3, 2020, from https://www.w3schools.com/html/html_attributes.asp