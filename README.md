# Praktikum Modul Pemrograman Web 1
Nama : AFLAH ATHALLAH TAMAM KAPUKONG

NIM : 312410280

KELAS : TI.24.A.4

# Langkah-langkah Praktikum
Persiapan membuat dokumen HTML dengan nama file lab4_box.html seperti berikut.
1. Membuat Box Element
Kemudian tambahkan kode untuk membuat box element dengan tag div seperti berikut.
2. CSS Float Property
Selanjutnya tambahkan deklarasi CSS pada head untuk membuat float element, seperti berikut.
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Box Element</title>
    <style>
        div {
            float: left;
            padding: 10px;
        }

        .div1 {
            background: red;
        }

        .div2 {
            background: yellow;
        }

        .div3 {
            background: green;
        }
    </style>
</head>
<body>
    <header>
        <h1>Box Element</h1>
    </header>

    <section>
        <div class="div1">Div 1</div>
        <div class="div2">Div 2</div>
        <div class="div3">Div 3</div>
    </section>
</body>
</html>
```
Hasilnya :

![gambar](https://github.com/Abcdeflahhh/Lab4WEBPW/blob/2be145a739b32f0dd715c807e4b18f6fa61b0443/image/2025-10-16%2016_46_11-Box%20Element%20-%20Prak4PW%20-%20Aflah%20-%20Visual%20Studio%20Code.png41.png)

3. Mengatur Clearfix Element
Clearfix digunakan untuk mengatur element setelah float element. Property clear digunakan untuk mengaturnya.
Tambahkan element div lainnya seteleah div3 seperti berikut.
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Box Element</title>
    <style>
        div {
            float: left;
            padding: 10px;
        }

        .div1 {
            background: red;
        }

        .div2 {
            background: yellow;
        }

        .div3 {
            background: green;
        }

        .div4 {
            background-color: blue;
            clear: left;
            float: none;
        }
    </style>
</head>
<body>
    <header>
        <h1>Box Element</h1>
    </header>

    <section>
        <div class="div1">Div 1</div>
        <div class="div2">Div 2</div>
        <div class="div3">Div 3</div>
        <div class="div4">Div 4</div>
    </section>
</body>
</html>
```

Hasilnya :

![gambar](https://github.com/Abcdeflahhh/Lab4WEBPW/blob/d9ffb6454931a31564ad24b843f1d6eb88c6185d/image/2025-10-16%2016_49_20-index.html%20-%20Prak4PW%20-%20Aflah%20-%20Visual%20Studio%20Code.png42.png)

# Membuat Layout Sederhana
Kita akan membuat layout web sederhana seperti gambar berikut. Buat folder baru dengan nama lab4_layout, kemudian buatlah file baru didalamnya dengan nama
home.html, dan file css dengan nama style.css.
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Layout Sederhana</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div id="container">
    </div>

    <header>
        <h1>Layout Sederhana</h1>
    </header>

    <nav>
        <a href="home.html" class="active">Home</a>
        <a href="artikel.html">Artikel</a>
        <a href="about.html">About</a>
        <a href="kontak.html">Kontak</a>
    </nav>

    <section id="hero"></section>
    <section id="wrapper">
        <section id="main"></section>
        <aside id="sidebar"></aside>
    </section>

    <footer>
        <p>&copy; 2021 - Universitas Pelita Bangsa</p>
    </footer>
</body>
</html>
```

Hasilnya :

![gambar](https://github.com/Abcdeflahhh/Lab4WEBPW/blob/7f6b3211ab5ad19f42b2cf2154a143c7b2fb1b57/image/2025-10-16%2016_50_17-index.html%20-%20Prak4PW%20-%20Aflah%20-%20Visual%20Studio%20Code.png43.png)

Kemudian tambahkan kode CSS untuk membuat layoutnya.
```
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0,300;0,700;1,300&display=swap');

* {
    margin: 0;
    padding: 0;
}

body {
    line-height: 1;
    font-size: 100%;
    font-family: 'Open Sans', sans-serif;
    color: #5a5a5a;
}

#container {
    width: 980px;
    margin: 0 auto;
    box-shadow: 0 0 1em #cccccc;
}

header {
    padding: 20px;
}

header h1 {
    margin: 20px 10px;
    color: #b5b5b5;
}
```

Hasilnya : 

![gambar](https://github.com/Abcdeflahhh/Lab4WEBPW/blob/08b5b9f417adecafe15c24ae11f3293b7640d876/image/2025-10-16%2016_53_19-Layout%20Sederhana%20-%20Prak4PW%20-%20Aflah%20-%20Visual%20Studio%20Code.png44.png)

4. Membuat Navigasi
Kemudian selanjutnya mengatur navigasi.
```
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0,300;0,700;1,300&display=swap');

* {
    margin: 0;
    padding: 0;
}

body {
    line-height: 1;
    font-size: 100%;
    font-family: 'Open Sans', sans-serif;
    color: #5a5a5a;
}

#container {
    width: 980px;
    margin: 0 auto;
    box-shadow: 0 0 1em #cccccc;
}

header {
    padding: 20px;
}

header h1 {
    margin: 20px 10px;
    color: #b5b5b5;
}

nav {
    display: block;
    background-color: #1f5faa;
}

nav a {
    padding: 15px 30px;
    display: inline-block;
    color: #ffffff;
    font-size: 14px;
    text-decoration: none;
    font-weight: bold;
}

nav a.active,
nav a:hover {
    background-color: #2b83ea;
}
```

Hasilnya :

![gambar](https://github.com/Abcdeflahhh/Lab4WEBPW/blob/9f52a4fcb60f600c1c6606fa9b3bca8c98213bc7/image/2025-10-16%2016_55_30-Layout%20Sederhana%20-%20Prak4PW%20-%20Aflah%20-%20Visual%20Studio%20Code.png45.png)

5. Membuat Hero Panel.
Selanjutnya membuat hero panel. Tambahkan kode HTML dan CSS seperti berikut.
versi html
```
    <section id="hero">
        <h1>Hello World!</h1>
        <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit.
            Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu.
            Proin in leo fringilla, vestibulum mi porta, faucibus felis.
            Integer pharetra est nunc, nec pretium nunc pretium ac.
        </p>
        <a href="home.html">Learn more &raquo;</a>
    </section>

    <footer>
        <p>&copy; 2021 - Universitas Pelita Bangsa</p>
    </footer>
```
versi css

```
#hero {
    background-color: #e4e4e5;
    padding: 20px;
}

#hero h1 {
    margin-bottom: 20px;
    font-size: 35px;
    color: #333;
}

#hero p {
    margin-bottom: 20px;
    font-size: 18px;
    line-height: 25px;
    color: #555;
}
```

Hasilnya :

![gambar](https://github.com/Abcdeflahhh/Lab4WEBPW/blob/98c183ae756fb8ed3fc1db600c54c5d7312304a8/image/2025-10-16%2017_02_31-Layout%20Sederhana%20-%20Prak4PW%20-%20Aflah%20-%20Visual%20Studio%20Code.png46.png)

6. Mengatur Layout Main dan Sidebar
Selanjutnya mengatur main content dan sidebar, tambahkan CSS float.
7. Membuat Sidebar Widget
Kemudian selanjutnya menambahkan element lain dalam sidebar.
untuk html nya
```
<aside class="sidebar">
            <div class="widget">
                <h3 class="widget-title">Widget Header</h3>
                <ul>
                    <li><a href="#">Widget Link</a></li>
                    <li><a href="#">Widget Link</a></li>
                    <li><a href="#">Widget Link</a></li>
                    <li><a href="#">Widget Link</a></li>
                    <li><a href="#">Widget Link</a></li>
                </ul>
            </div>
            <div class="widget">
                <h3 class="widget-title">Widget Text</h3>
                <p>
                    Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. 
                    Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est nunc, 
                    nec pretium nunc pretium ac.
                </p>
            </div>
        </aside>
```
untuk css
```
#wrapper {
    margin: 0;
}

#main {
    float: right;
    width: 640px;
    padding: 20px;
}

#sidebar {
    float: right;
    width: 260px;
    padding: 20px;
}

.widget-box {
    border: 1px solid #eee;
    margin-bottom: 20px;
}

.widget-box .title {
    padding: 10px 16px;
    background-color: #428bca;
    color: #fff;
}

.widget-box ul {
    list-style-type: none;
}

.widget-box li {
    border-bottom: 1px solid #eee;
}

.widget-box li a {
    padding: 10px 16px;
    color: #333;
    display: block;
    text-decoration: none;
}

.widget-box li:hover a {
    background-color: #eee;
}

.widget-box p {
    padding: 15px;
    line-height: 25px;
}

footer {
    clear: both;
    background-color: #d1d1d1;
    padding: 20px;
    color: #eee;
}
```
Hasilnya :

![gambar](https://github.com/Abcdeflahhh/Lab4WEBPW/blob/7f00390caadaacab9a48f38224746b559af4e8a6/image/2025-10-16%2017_21_41-Layout%20Sederhana%20-%20Prak4PW%20-%20Aflah%20-%20Visual%20Studio%20Code.png47.png)

8. Mengatur Footer
Selanjutnya mengatur tampilan footer. Tambahkan CSS untuk footer.
Menambahkan Elemen lainnya pada Main Content

untuk html
```
<article class="entry">
                <h2>First featurette heading.</h2>
                <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="">
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, 
                    iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, 
                    vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc pretium ac.
                </p>
            </article>

            <hr class="divider" />

            <article class="entry">
                <h2>Second featurette heading.</h2>
                <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="" class="right-img">
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, 
                    iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, 
                    vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc pretium ac.
                </p>
            </article>
        </section>
```

untuk css
```
.divider {
  border: 0;
  border-top: 1px solid #eeeeee;
  margin: 40px 0;
}

.entry {
  margin: 15px 0;
}

.entry h2 {
  margin-bottom: 20px;
  color: #333;
}

.entry p {
  line-height: 25px;
}

.entry img {
  float: left;
  border-radius: 5px;
  margin-right: 15px;
}
```

Hasilnya : 

![gambar](https://github.com/Abcdeflahhh/Lab4WEBPW/blob/bc7eeb09c71923933fff94d0850ec67f37ed9ac5/image/2025-10-16%2017_23_26-Layout%20Sederhana%20-%20Personal%20-%20Microsoft%E2%80%8B%20Edge.png48.png)

SELESAI.

SOAL & PERTANYAAN

![gambar](https://github.com/Abcdeflahhh/Lab4WEBPW/blob/cb2a65e7f3608ea990aec0b988de425af850400f/image/Screenshot%20from%202025-10-15%2019-22-47.png)

JAWABAN :

1
```
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Layout Sederhana</title>
  <link rel="stylesheet" href="style4.css">
</head>
<body>
  <header>
    <h1>Hubungi Saya</h1>
  </header>

  <nav>
    <a href="#">Home</a>
    <a href="#">Artikel</a>
    <a href="#">About</a>
    <a href="#" class="active">Kontak</a>
  </nav>

  <section id="intro">
    <h2>Ingin Terhubung?</h2>
    <p>Silakan isi formulir berikut untuk mengirimkan pesan, pertanyaan, atau kolaborasi proyek!</p>
  </section>

  <section id="kontak">
    <div class="kontak-container">
      <div class="formulir">
        <h3>Formulir Kontak</h3>
        <form action="#" method="post">
          <label>Nama Lengkap:</label>
          <input type="text" placeholder="Masukkan nama Anda">

          <label>Email:</label>
          <input type="email" placeholder="Masukkan email aktif">

          <label>Pesan:</label>
          <textarea placeholder="Tulis pesan Anda di sini..."></textarea>

          <button type="submit">Kirim Sekarang</button>
        </form>
      </div>

      <div class="informasi">
        <h3>Informasi Kontak</h3>
        <p><strong>Email:</strong> <a href="mailto:info@pelitabangsa.ac.id">info@pelitabangsa.ac.id</a></p>
        <p><strong>Telepon:</strong> (021) 899-8999</p>
        <p><strong>Alamat:</strong> Jl. Inspeksi Kalimalang No.9, Bekasi</p>
      </div>
    </div>
  </section>

  <footer>
    <p>© 2025 - Universitas Pelita Bangsa | Created by AFLAH ATHALLAH TAMAM KAPUKONG</p>
  </footer>
</body>
</html>
```
![gambar](https://github.com/Abcdeflahhh/Lab4WEBPW/blob/76d1cffaeb45476ed144d8c12adde9938450ead5/image/2025-10-16%2017_38_49-Layout%20Sederhana%20-%20Personal%20-%20Microsoft%E2%80%8B%20Edge.png49'.png)

2
```
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Tentang Saya</title>
  <link rel="stylesheet" href="style41.css">
</head>
<body>
  <header>
    <h1>Tentang Saya</h1>
  </header>

  <nav>
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">Artikel</a></li>
      <li><a href="#" class="active">About</a></li>
      <li><a href="#">Kontak</a></li>
    </ul>
  </nav>

  <section class="intro">
    <h2>Kenali Saya Lebih Dekat</h2>
    <p>
      Saya adalah mahasiswa Universitas Pelita Bangsa yang tertarik dengan dunia teknologi, desain web, dan pengembangan digital modern.
    </p>
  </section>

  <section class="main-content">
    <div class="left">
      <img src="images/fotoandre.jpg" alt="Profil">
      <h3>Profil Singkat</h3>
      <p>
        Halo! Saya <strong>AFLAH ATHALLAH TAMAM KAPUKONG</strong>, seorang web developer dan network engineer pemula yang tertarik pada dunia teknologi digital.
Saya gemar menciptakan tampilan website yang responsive dan estetik, sekaligus memahami dasar-dasar jaringan komputer dan keamanan data.
      </p>
    </div>

    <div class="right">
      <h3>Keahlian</h3>
      <ul>
        <li>HTML5 & CSS3</li>
        <li>Responsive Web Design</li>
        <li>Git & Version Control</li>
        <li>Network & Mikrotik</li>
      </ul>

      <h3>Hobi</h3>
      <ul>
        <li>Desain UI/UX</li>
        <li>Fotografi</li>
        <li>Menulis Blog</li>
        <li>Winbox</li>
      </ul>
    </div>
  </section>

  <footer>
    <p>
      © 2025 - Universitas Pelita Bangsa | Dibuat oleh <strong>AFLAH ATHALLAH TAMAM KAPUKONG</strong>
    </p>
  </footer>
</body>
</html>
```
![gambar](https://github.com/Abcdeflahhh/Lab4WEBPW/blob/b04bcd4acf3c0bd73657093223eb505f4c7b1995/image/2025-10-16%2017_53_24-Layout%20Sederhana%20-%20Tentang%20Saya%20-%20Personal%20-%20Microsoft%E2%80%8B%20Edge.png50.png)
