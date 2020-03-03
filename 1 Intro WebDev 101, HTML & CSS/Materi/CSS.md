# Cascading Style Sheets (CSS)
CSS singkatan dari Cascading Style Sheeet, yaitu dokumen yang berisi definisi style untuk sebuah dokumen HTML atau untuk mengatur tampilan dari dokumen HTML, meliputi layout dokumen, pewarnaan dan tampilan font dan teks dan lain sebagainya.

## Struktur Penulisan CSS
```css
selector { 
    property:value
}

selector { 
    property:value; 
    property:value 
}
```
- <strong>Selector</strong> adalah bagian CSS yang berfungsi untuk memilih elemen yang akan dikenai style.
- <strong>Property</strong> adalah jenis style yang akan diterapkan pada elemen.
- <strong>Value</strong> adalah nilai dari property yang digunakan.

Property dan value CSS ditulis di dalam kurung kurawal. Bila property CSS yang digunakan lebih dari satu, maka pisahkan dengan semicolon.

Contoh:

```html
<style>
h1 {
    font-size: 40px; 
    color: orange; 
}
</style>

<h1>Heading</h1>
```

## Teknik Memasang CSS
Terdapat 3 cara dalam memasang CSS pada dokumen HTML, yakni:

### A. Inline Style
Menulis CSS di dalam tag HTML, pada atribut 'style'.
```html
<h1 style="font-size:40px; color:orange;">
    Heading
</h1>
```

### B. Internal Style Sheet
Menulis kode CSS di dalam file dokumen HTML, tapi dimasukan ke dalam tag 'style'.
```html
<style>
h1 {
    font-size: 40px; 
    color: orange; 
}
</style>

<h1>Heading</h1>
```

### C. External Style Sheet
Menulis CSS di file terpisah dari dokumen HTML.

File style.css:
```css
h1 {
    font-size: 40px;
    color: orange;
}
```

File index.html:
```html
<!-- Menghubungkan ke file CSS -->
<link href="style.css" rel="stylesheet">

<h1>Heading</h1>
```

## CSS Properties
Property digunakan untuk memilih jenis style apa yang akan diterapkan pada tag, class, atau id yang telah dipilih pada selector, dan pada satu selector bisa berisi beberapa property. Pada CSS terdapat banyak sekali property yang dapat digunakan untuk menghias webisite.

Jenis property CSS diantaranya adalah

- Background
- Border
- Border
- Layouting
- Font & Text, dll.
- List & Marker
- Animation & Transition

Setidaknya ada total 350+ properties CSS

<img src="../Images/are_you_kidding_me.jpeg">

Kita tidak perlu menghafal semuanya, cukup pahami apa fungsi dari property yang akan digunakan. Referensi property CSS lebih lengkap bisa dilihat di https://www.w3schools.com/cssref/

## Selector
Pada CSS terdapat selector yang digunakan untuk memilih elemen HTML yang akan dikenai style. Pemilihan elemen menggunakan nama tag, nilai atribut, atau pola tertentu.

Contoh penulisan selector:
```css
h1 { 
    color:red 
}
```
Cara bacanya: "*Pilih elemen h1 pada document, lalu set property colornya menjadi red*"

Terdapat 2 macam tag selector, yakni *<strong>single selector</strong>* dan *<strong>multiple selector</strong>*. Single selector seperti contoh di atas sedangkan multiple selector tampak seperti di bawah ini:

```css
h1, h2, h3, p {
    font-family: "arial", sans-sarif;
    color: #666;
}
```

### Selector dengan id dan class
Kita juga dapat menggunakan id & class sebagai selector class. Bedanya adalah jika id hanya boleh dipanggil satu kali saja, class bisa dipanggil berkali kali pada satu halaman. Selector class ditulis dengan awalan titik atau dot “.”. Sedangkan selector id ditulis dengan awalan pagar “#”.

Contoh:
```html
<style>
    #higlight {
        background-color: yellow
    }
    
    .red {
        color:red
    }
</style>

<p class="red">Ini selector class 1</p> <br>
<p class="red">Ini selector class 2</p> <br>
<p id="higlight">Ini selector id</p> <br>
```

## Referensi
- CSS dan Style HTML Dasar - CodePolitan.com. (n.d.). Retrieved March 3, 2020, from https://www.codepolitan.com/course/lesson/basic-html-dan-css/01-Pengenalan-HTML-dan-CSS/03-css-dan-style-html-dasar