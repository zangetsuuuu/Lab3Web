Nama : Rafif Isdarufa Athallah

NIM : 312210299

Kelas : TI.22.A3

---

## Pratikum

### Membuat List dalam HTML

- Buat dokumen HTML seperti berikut:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>
        <h1>Membuat List</h1>
    </header>
</body>
</html>
```

---

#### Membuat Ordered List

- Tambahkan tag `<section>` dengan atribut `id`.
- Untuk membuat *ordered list*, gunakan tag `<ol>`.
- Simpan perubahan dan lihat hasilnya.

```html
    <section id="order-list">
        <h2>Ordered List</h2>
        <ol>
            <li>Pemograman Web</li>
            <li>Sistem Informasi</li>
            <li>Basis Data 2</li>
        </ol>
    </section>
```

![List 1](./images/List%20(1).jpeg)

---

#### Membuat Unoredered List

- Tambahkan tag `<section>` dengan atribut `id`.
- Untuk membuat *unordered list*, gunakan tag `<ul>`.
- Berikan atribut `type="square"` pada tag `<ul>` untuk membuatnya menjadi kotak.
- Simpan perubahan dan lihat hasilnya.

```html
    <section id="unorder-list">
        <h2>Unordered List</h2>
        <ul type="square">
            <li>Jaringan Komputer</li>
            <li>Struktur Data</li>
            <li>Algoritma & Pemograman</li>
        </ul>
    </section>
```

![List 2](./images/List%20(2).jpeg)

---

#### Membuat Description List

- Tambahkan tag `<section>` dengan atribut `id`.
- Untuk membuat *description list*, gunakan tag `<dl>`.
- Tag `<dt>` digunakan untuk menandai item dalam list, sedangkan tag `<dd>` digunakan untuk memberikan definisi atau penjelasan dari item tersebut.
- Simpan perubahan dan lihat hasilnya.

```html
    <section id="desc-list">
        <h2>Description List</h2>
        <dl>
            <dt>Fakultas Teknik</dt>
            <dd>Teknik Industri</dd>
            <dd>Teknik Informatika</dd>
            <dd>Teknik Lingkungan</dd>
            <br>
            <dt>Fakultas Ekonomi dan Bisnis</dt>
            <dd>Akutansi</dd>
            <dd>Manajemen</dd>
            <dd>Bisnis Digital</dd>
        </dl>
    </section>
```

![List 3](./images/List%20(3).jpeg)

---

### Membuat Tabel dalam HTML

- Buat dokumen HTML seperti berikut:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>
        <h1>Membuat Tabel</h1>
    </header>
</body>
</html>
```

---

#### Membuat tabel sederhana

- Tag `<table>` digunakan untuk membuat sebuah tabel.
- Tag `<thead>` digunakan untuk menandai bagian kepala dari tabel. Tag ini berisi baris judul atau nama kolom.
- Tag `<tr>` digunakan untuk menandai baris dalam tabel.
- Tag `<th>` digunakan untuk menandai sel header dalam tabel. Tag ini berisi judul atau nama kolom.
- Tag `<tbody>` digunakan untuk menandai bagian isi dari tabel.
- Tag `<td>` digunakan untuk menandai sel dalam tabel. Biasanya, tag ini berisi data yang ditampilkan dalam tabel.
- Simpan perubahan dan lihat hasilnya.

```html
    <table border="1">
        <thead>
            <tr>
                <th>No.</th>
                <th>Fakultas</th>
                <th>Program Studi</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>1.</td>
                <td>Teknik</td>
                <td>Teknik Informatika</td>
            </tr>
            <tr>
                <td>2.</td>
                <td>Teknik</td>
                <td>Teknik Industri</td>
            </tr>
            <tr>
                <td>3.</td>
                <td>Teknik</td>
                <td>Teknik Lingkungan</td>
            </tr>
        </tbody>
    </table>
```

![Tabel 1](./images/Tabel%20(1).jpeg)

---

#### Mengatur Margin dan Padding

- Untuk mengatur _margin_ dan _padding_ pada cel data, tambahkan atribut `cellpadding` dan 
`cellspacing` pada tag `<table>`.
- Simpan perubahan dan lihat hasilnya.

```html
    <table border="1" cellpadding="4" cellspacing="0">
```

![Tabel 2](./images/Tabel%20(2).jpeg)

---

#### Menggabungkan Sel Data

- Untuk menggabungkan sel data, gunakan atribut `rowspan` dan `colspan`
- Atribut `rowspan` untuk menggabungkan baris (secara vertikal) dan `colspan` untuk menggabungkan kolom (secara horizontal).
- Simpan perubahan dan lihat hasilnya.

```html
    <table border="1" cellpadding="6" cellspacing="0">
        <thead>
            <tr>
                <th>No.</th>
                <th>Fakultas</th>
                <th>Program Studi</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>1.</td>
                <td rowspan="3">Teknik</td>
                <td>Teknik Informatika</td>
            </tr>
            <tr>
                <td>2.</td>
                <td>Teknik Industri</td>
            </tr>
            <tr>
                <td>3.</td>
                <td>Teknik Lingkungan</td>
            </tr>
        </tbody>
    </table>
```

![Tabel 3](./images/Tabel%20(3).jpeg)

---

### Membuat Form dalam HTML

- Buat dokumen HTML seperti berikut:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>
        <h1>Membuat Form</h1>
    </header>
</body>
</html>
```

---

#### Membuat Form Sederhana

- Tag `<form>` digunakan untuk membuat form pada halaman web. Form ini dapat berisi elemen-elemen seperti `<input>`, `<textarea>`, dan `<button>`.
- Tag `<fieldset>` digunakan untuk mengelompokkan beberapa elemen form menjadi satu kelompok. Tag ini digunakan untuk membuat form yang kompleks.
- Tag `<legend>` digunakan untuk menambahkan judul atau deskripsi pada elemen `<fieldset>`.
- Tag `<label>` digunakan untuk menandai elemen form dan memberikan deskripsi atau label pada elemen tersebut.
- Tag `<input>` digunakan untuk membuat elemen form yang memungkinkan pengguna memasukkan data seperti teks, angka, atau pilihan.
- Tag `<textarea>` digunakan untuk membuat elemen form yang memungkinkan pengguna memasukkan teks dalam jumlah yang lebih besar.
- Simpan perubahan dan lihat hasilnya.

```html
    <form action="proses.php" method="post">
        <fieldset>
            <legend>Data Pelanggan</legend>
            <p>
                <label for="nama">Nama</label>
                <input type="text" id="nama" name="nama">
            </p>
            <p>
                <label for="alamat">Alamat</label>
                <textarea name="alamat" id="alamat" cols="20" rows="3"></textarea>
            </p>
            <p>
                <label>Jenis Kelamin :</label>
                <input type="radio" id="jk_l" name="kelamin" value="L">
                <label for="jk_1">Laki-laki</label>
                <input type="radio" id="jk_p" name="kelamin" value="P">
                <label for="jk_p">Perempuan</label>
            </p>
            <p>
                <input type="submit" value="Login">
            </p>
        </fieldset>
    </form>
```

![Form 1](./images/Form%20(1).jpeg)

---

#### Menambahkan Style pada Form

- Tambahkan _style_ berikut, agar form terlihat lebih menarik.
- Simpan perubahan dan lihat hasilnya.

```html
    <style>
        body {
            font-family: "Onest", sans-serif;
            background-color: #f2f2f2;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        h1 {
            margin: 20px;
        }

        form {
            background-color: white;
            border-radius: 5px;
            padding: 24px;
            margin: 20px;
            width: 50%;
        }

        legend {
            font-size: 24px;
            font-weight: bold;
        }

        label {
            display: inline-block;
            margin-bottom: 4px;
        }

        input[type="text"], textarea {
            width: 95.75%;
            padding: 12px;
            margin-bottom: 16px;
            margin-right: 20px;
            border: 1px solid rgb(151, 151, 151);
        }

        input[type="submit"] {
            background-color: #4CAF50; /* Green */
            color: white;
            display: inline-block;
            width: 100%;
            padding: 10px 20px;
            margin-top: 12px;
            text-transform: uppercase;
            font-weight: 600;
            letter-spacing: 4px;
            text-align: center;
            text-decoration: none;
            font-size: 16px;
            border: none;
            cursor: pointer;
        }
    </style>
```

![Form 2](./images/Form%20(2).jpeg)

---

### Pertanyaan

- Buatlah form yang menampilkan _dropdown_ menu dan _listbox_ dengan _multiple selection_.