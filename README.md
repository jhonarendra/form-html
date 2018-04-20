<h1 align="center">Form Input Output dengan JQuery</h1>

<p align="center">Form sederhana ini dapat menampilkan data masukan user langsung pada halaman itu juga dengan menggunakan JQuery. JQuery sendiri adalah framework javascript untuk memudahkan penulisan javascript.</p>

## Pembahasan

Pada file `index.html`, widget input terdapat diantara rangkaian kode
```html
<div id="form">
...
</div>
```
Sedangkan output untuk menampilkan data terdapat pada
```html
<div id="tabel">
...
</div>
```

> Kenapa tidak menggunakan tag `<form>`? Karena data dikirim tidak melalui web server, melainkan hanya menampilkan isian form menggunakan JQuery. Jadi atribut `name=""` juga sebenarnya tidak diperlukan.

Selanjutnya, pada file `script.js` berisi rangkaian kode javascript untuk menampilkan data.

`$("#kirim").click(function(){` berarti apabila elemen dengan id kirim diklik, maka akan dijalankan sebuah fungsi. Berikut penjelasan dari salah satu fungsi.

```javascript
$("#nama").text(
	$("#fnama").val()
);
```
- `"#nama"` merupakan id elemen untuk menampilkan isian form.
- `.text()` adalah fungsi untuk memasukkan data keelemen yang diseleksi.
- `#fnama` merupakan id widget form.
- `.val()` adalah fungsi untuk mengambil value dari form.

Jadi, setelah tombol "Kirim" diklik, semua isian form diambil dan ditampilkan pada elemen yang telah ditentukan.
***
