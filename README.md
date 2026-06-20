# Valentine Day Website

Project ini adalah website sederhana bertema Valentine. Website ini berisi halaman pertanyaan, tombol interaktif, animasi GIF, halaman jawaban, musik latar opsional, dan area foto yang bisa disesuaikan sendiri.

Project ini dibuat sebagai template. Pengguna dapat mengganti teks, GIF, foto, dan musik sesuai kebutuhan.

## Fitur

* Halaman utama dengan pertanyaan Valentine.
* Tombol `Yes` dan `No` yang interaktif.
* Tombol `No` berubah teks setiap kali diklik.
* Tombol `Yes` membesar setelah tombol `No` ditekan.
* Tombol `No` dapat bergerak setelah beberapa kali diklik.
* Halaman `yes.html` sebagai halaman hasil ketika tombol `Yes` dipilih.
* Area foto berjalan pada halaman `yes.html`.
* Musik latar opsional.
* Tampilan sederhana menggunakan HTML, CSS, dan JavaScript.

## Struktur File

```text
valentine-day
├── index.html
├── yes.html
├── style.css
├── script.js
├── yes-script.js
├── Foto
│   ├── Foto1.jpeg
│   ├── Foto2.jpeg
│   ├── Foto3.jpeg
│   └── ...
├── music
│   └── song.mp3
└── README.md
```

Catatan:

Folder `Foto` dan `music` dapat dibuat sendiri jika belum tersedia.

## Cara Menjalankan

Buka file berikut di browser:

```text
index.html
```

Jika project sudah di-deploy menggunakan GitHub Pages, website dapat dibuka melalui link GitHub Pages masing-masing.

## Cara Mengganti Foto

Foto yang tampil pada halaman `yes.html` diatur pada bagian berikut:

```html
<img src="Foto/Foto1.jpeg">
<img src="Foto/Foto2.jpeg">
<img src="Foto/Foto3.jpeg">
```

Agar foto tampil dengan benar, buat folder bernama:

```text
Foto
```

Lalu masukkan foto dengan nama file seperti berikut:

```text
Foto1.jpeg
Foto2.jpeg
Foto3.jpeg
Foto4.jpeg
Foto5.jpeg
Foto6.jpeg
Foto7.jpeg
Foto8.jpeg
Foto9.jpeg
Foto10.jpeg
Foto11.jpeg
Foto12.jpeg
Foto13.jpeg
Foto14.jpeg
Foto15.jpeg
Foto16.jpeg
```

Pastikan penulisan nama folder dan file sama persis, termasuk huruf besar dan kecil.

Contoh yang benar:

```text
Foto/Foto1.jpeg
```

Contoh yang salah:

```text
foto/foto1.jpg
```

Jika nama file berbeda, ubah juga bagian `src` pada file `yes.html`.

Contoh:

```html
<img src="Foto/namafoto.jpeg">
```

## Cara Menambahkan Musik

Repository ini tidak menyertakan file musik bawaan. Pengguna dapat menambahkan musik sendiri jika memiliki hak untuk menggunakan lagu tersebut.

Buat folder:

```text
music
```

Lalu masukkan file musik dengan nama:

```text
song.mp3
```

Strukturnya menjadi:

```text
music/song.mp3
```

Pada file `index.html` dan `yes.html`, musik dipanggil melalui kode berikut:

```html
<audio id="bg-music" loop>
    <source src="music/song.mp3" type="audio/mpeg">
</audio>
```

Jika ingin memakai nama file lain, ubah bagian `src`.

Contoh:

```html
<source src="music/lagu-saya.mp3" type="audio/mpeg">
```

## Catatan Hak Cipta Musik

Project ini tidak menyediakan file musik komersial atau lagu dari artis tertentu. Jika ingin menambahkan musik, gunakan lagu yang memang boleh digunakan, misalnya:

* Musik buatan sendiri.
* Musik bebas royalti.
* Musik dengan lisensi yang mengizinkan penggunaan.
* Musik yang sudah mendapat izin dari pemilik hak cipta.

Hindari mengunggah lagu komersial ke repository public jika tidak memiliki izin penggunaan.

## File yang Bisa Diedit

### `index.html`

Berisi halaman utama, teks pertanyaan, tombol, GIF utama, dan audio.

Bagian teks utama:

```html
<h1>Will you be my Valentine? 💕</h1>
```

Bagian GIF utama:

```html
<img id="cat-gif" src="https://media.tenor.com/K0Op-0SpsvkAAAAj/dudu-cute.gif" alt="cute character">
```

### `script.js`

Berisi logika tombol `Yes` dan `No`.

Bagian pesan tombol `No`:

```javascript
const noMessages = [
    "No",
    "Are you positive? 🤔",
    "Pookie please... 🥺"
]
```

Bagian GIF yang berubah ketika tombol `No` diklik:

```javascript
const gifStages = [
    "https://media.tenor.com/EBV7OT7ACfwAAAAj/u-u-qua-qua-u-quaa.gif"
]
```

### `yes.html`

Berisi halaman hasil setelah tombol `Yes` dipilih.

Bagian foto:

```html
<img src="Foto/Foto1.jpeg">
```

Bagian teks hasil:

```html
<h1 class="yes-title">Knew you would say yes! 🎉</h1>
<p class="yes-message">You just made me the happiest person! 💕</p>
```

### `yes-script.js`

Berisi logika musik dan efek confetti pada halaman `yes.html`.

### `style.css`

Berisi pengaturan tampilan, warna, layout, animasi, tombol, background, dan foto berjalan.

## Catatan

Project ini dibuat untuk latihan dan hiburan. Semua foto dan musik yang digunakan sebaiknya diganti dengan milik sendiri atau aset yang memang memiliki izin untuk digunakan.
