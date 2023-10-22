# Lab4Web

Nama : Tiara Putri

NIM  : 312210064

Kelas : TI.22.A1

## DAFTAR ISI <br>
| No | Description | Link |
|-----|------|-----|
|1|Instruksi Praktikum|[Click Here](#instruksi-praktikum)|
|2|Langkah-langkah Praktikum|[Click Here](#langkah-langkah-praktikum)|
|3|Pertanyaan dan Tugas|[Click Here](#pertanyaan-dan-tugas)|

## Instruksi Praktikum
1. Persiapkan text editor misalnya VSCode.
2. Buat folder baru dengan nama Lab4Web
3. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya.
4. Lakukan validasi dokumen html dengan mengakses http://validator.w3.org

## Langkah-langkah praktikum
**1. Membuat Box Element**
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Box Element</title>
</head>
<body>
    <header>
        <h1>Box Element</h1>
        <section>
            <div class="div1">Div 1</div>
            <div class="div2">Div 2</div>
            <div class="div3">Div 3</div>
        </section>
        <style>
            div {
            float:left;
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
    </header>
</body>
</html>
```

![Screenshot 2023-10-17 100132](https://github.com/tiaraputriiiiii/Lab4Web/assets/115775237/63eaea3e-3b5d-4163-b370-4cdd2cba419b)

**2. Mengatur Clearfix Element**
> - **Clearfix** digunakan untuk mengatur element setelah float element. Property clear digunakan untuk
mengaturnya.
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Box Element</title>
</head>
<body>
    <header>
        <h1>Box Element</h1>
        <section>
            <div class="div1">Div 1</div>
            <div class="div2">Div 2</div>
            <div class="div3">Div 3</div>
            <div class="div4">Div 4</div>
        </section>
        <style>
            div {
            float:left;
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
    </header>
</body>
</html>
```

![2](https://github.com/tiaraputriiiiii/Lab4Web/assets/115775237/b299c85f-dc94-462b-aaae-9157e807535c)

**3. Membuat Layout Sederhana**
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
```

![1](https://github.com/tiaraputriiiiii/Lab4Web/assets/115775237/fc8adf16-ab3a-4f20-a593-199366b72a80)

> - Kemudian tambahkan kode CSS untuk membuat layoutnya :
```
/* import google font */
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap');
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0 ,300;0,700;1,300&display=swap');

/* Reset CSS */
* {
    margin: 0;
    padding: 0;
}
body {
    line-height:1;
    font-size:100%;
    font-family:'Open Sans', sans-serif;
    color:#5a5a5a;
}
#container {
    width: 980px;
    margin: 0 auto;
    box-shadow: 0 0 1em #cccccc;
}
/* header */
header {
    padding: 20px;
}
header h1 {
    margin: 20px 10px;
    color: #b5b5b5;
}
```

![2](https://github.com/tiaraputriiiiii/Lab4Web/assets/115775237/fa58426f-5459-403f-a4b3-23679d90d530)

**4. Membuat Navigasi**
> - Kemudian selanjutnya mengatur navigasi
```
/* navigasi */
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

![Screenshot 2023-10-17 104551](https://github.com/tiaraputriiiiii/Lab4Web/assets/115775237/b6db8a61-3503-4a4d-b94f-ec571e416a25)

**5. Mmebuat Hero Panel**
> - Membuat hero panel. Tambahkan kode HTML dan CSS seperti berikut.
```
<section id="hero">
    <h1>Hello World!</h1>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
pretium ac.</p>
    <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
</section>
```

```
/* Hero Panel */
#hero {
    background-color: #e4e4e5;
    padding: 50px 20px;
    margin-bottom: 20px;
}
#hero h1 {
      margin-bottom: 20px;
      font-size: 35px;
}
#hero p {
    margin-bottom: 20px;
    font-size: 18px;
    line-height: 25px;
}
```

![4](https://github.com/tiaraputriiiiii/Lab4Web/assets/115775237/5790b10d-d715-414a-9055-db1161a5bed0)

**6. Mengatur Layout Main dan Sidebar**
> - Selanjutnya mengatur main content dan sidebar, tambahkan CSS float
```
/* main content */
#wrapper {
    margin: 0;
}
#main {
  float: left;
  width: 640px;
  padding: 20px;
}
/* sidebar area */
#sidebar {
  float: left;
  width: 260px;
  padding: 20px;
}
```

**7. Membuat Sidebar Widget**
> - Kemudian selanjutnya menambahkan element lain dalam sidebar
```
<aside id="sidebar">
    <div class="widget-box">
        <h3 class="title">Widget Header</h3>
        <ul>
            <li><a href="#">Widget Link</a></li>
            <li><a href="#">Widget Link</a></li>
            <li><a href="#">Widget Link</a></li>
            <li><a href="#">Widget Link</a></li>
            <li><a href="#">Widget Link</a></li>
        </ul>
    </div>
    <div class="widget-box">
        <h3 class="title">Widget Text</h3>
        <p>Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt
arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer
pharetra est nunc, nec pretium nunc pretium ac.</p>
      </div>
</aside>
```
> - Kemudian tambahkan CSS
```
/* widget */
.widget-box {
    border:1px solid #eee;
    margin-bottom:20px;
}
.widget-box .title {
    padding:10px 16px;
    background-color:#428bca;
    color:#fff;
}
.widget-box ul {
    list-style-type:none;
}
.widget-box li {
    border-bottom:1px solid #eee;
}
.widget-box li a {
    padding:10px 16px;
    color:#333;
    display:block;
    text-decoration:none;
}
.widget-box li:hover a {
    background-color:#eee;
}
.widget-box p {
    padding:15px;
    line-height:25px;
}
```

![5](https://github.com/tiaraputriiiiii/Lab4Web/assets/115775237/dc2e474b-345f-434e-a1a8-339c65fa9dbc)

**8. Mengatur Footer**
> - Selanjutnya mengatur tampilan footer. Tambahkan CSS untuk footer
```
/* footer */
footer {
    clear:both;
    background-color:#1d1d1d;
    padding:20px;
    color:#eee;
}
```

![Screenshot 2023-10-17 130616](https://github.com/tiaraputriiiiii/Lab4Web/assets/115775237/45860205-7398-4719-a538-d7c4b55088a9)

**9. Menambahkan Elemen lainnya pada Main Content**
```
<section id="main">
    <div class="row">
        <div class="box">
            <img src="https://dummyimage.com/120/db7d25/fff.png" alt=""
class="image-circle">
            <h3>Heading</h3>
            <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
euismod.</p>
            <a href="#" class="btn btn-default">View detail</a>
      </div>
      <div class="box">
          <img src="https://dummyimage.com/120/3e73e6/fff.png" alt=""
class="image-circle">
          <h3>Heading</h3>
          <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
euismod.</p>
    <a href="#" class="btn btn-default">View detail</a>
      </div>
      <div class="box">
          <img src="https://dummyimage.com/120/71e6d4/fff.png" alt=""
class="image-circle">
            <h3>Heading</h3>
            <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
euismod.</p>
            <a href="#" class="btn btn-default">View detail</a>
        </div>
    </div>
</section>
```
> - Kemudian tambahkan CSS :
```
/* box */
.box {
    display:block;
    float:left;
    width:33.333333%;
    box-sizing:border-box;
    -moz-box-sizing:border-box;
    -webkit-box-sizing:border-box;
    padding:0 10px;
text-align:center;
}
.box h3 {
    margin: 15px 0;
}
.box p {
    line-height: 20px;
    font-size: 14px;
    margin-bottom: 15px;
}
box img {
    border: 0;
    vertical-align: middle;
}
.image-circle {
    border-radius: 50%;
}
.row {
    margin: 0 -10px;
    box-sizing: border-box;
    -moz-box-sizing: border-box;
    -webkit-box-sizing: border-box;
}
.row:after, .row:before,
.entry:after, .entry:before {
    content:'';
    display:table;
}
.row:after,
.entry:after {
    clear:both;
}
```

![6](https://github.com/tiaraputriiiiii/Lab4Web/assets/115775237/64001197-e170-4886-8c19-247b103454f1)

**10. Menambahkan Content Artikel**
> - Selanjutnya membuat content artikel. Tambahkan HTML berikut pada main content
```
<hr class="divider" />
<article class="entry">
    <h2>First featurette heading.</h2>
    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="">
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
pretium ac.</p>
</article>
<hr class="divider" />
<article class="entry">
    <h2>First featurette heading.</h2>
    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt=""
class="right-img">
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
pretium ac.</p>
</article>
```

> - Kemudian tambahkan CSS
```
.divider {
    border:0;
    border-top:1px solid #eeeeee;
    margin:40px 0;
}
/* entry */
.entry {
    margin: 15px 0;
}
.entry h2 {
    margin-bottom: 20px;
}
.entry p {
    line-height: 25px;
}
.entry img {
    float: left;
    border-radius: 5px;
    margin-right: 15px;
}
.entry .right-img {
    float: right;
}
```

![7](https://github.com/tiaraputriiiiii/Lab4Web/assets/115775237/ab5496d1-500b-4c9d-ba2a-35808bd29794)

**11. Lakukan validasi dokumen HTML dengan mengakses http://validator.w3.org/**

![validasi jigsaw](https://github.com/tiaraputriiiiii/Lab4Web/assets/115775237/9e1d1da1-d569-49ba-a896-62ff50fa0370)

## Pertanyaan dan Tugas
1. Tambahkan Layout untuk menu `About` => buat single layout yang berisi deskripsi, portfolio, dll
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Layout Sederhana</title>
    <link rel="stylesheet" href="style_about.css">
</head>
<body>
    <div id="container">
        <header>
            <h1>About Me</h1>
        </header>
        <nav>
            <a href="home.html">Home</a>
            <a href="artikel.html">Artikel</a>
            <a href="about.html" class="active">About</a>
            <a href="kontak.html">Kontak</a>
        </nav>
        <section id="about" class="about">
            <h2>About</h2>
            <div class="row">
                <div class="about-img">
                    <img src="c:\Users\HP\AppData\Local\Packages\5319275A.WhatsAppDesktop_cv1g1gvanyjgm\TempState\D89C0C700FC0F0824A075D9027473CBF\WhatsApp Image 2023-09-06 at 14.54.11_0691b94f.jpg" alt="tentangdipca">
                </div>
                <div class="content">
                    <h3>Hello!!</h3>
                    <p>perkenalkan nama saya Tiara Putri saya adalah anak pertama dari dua bersaudara, saudara kandung saya bernama Muhammad Zidan Ramadhan. saat ini usia saya 19 tahun dan saya sedang menempuh s1 di jurusan Teknik Informatika di Universitas Pelita Bnngsa. saya mamiliki 3 teman di kelas yang selalu mensupport perkuliahan saya diantaranya adalah Syifa, Fathia, dan Aas.</p>
                </div>
            </div>
            <h4>Portofolio</h4>
            <p>Saya suka sekali mneggambar, membuat desain dan semua yang bersangkutan dengan kesenia. saya juga suka musik, saat saya duduk di bangku SMA saya pernah menjadi anggota paduan suara yang diadakan oleh pemda Kabupaten Bekasi.</p>
        </section>
        </body>
        </html>
```

![layout about](https://github.com/tiaraputriiiiii/Lab4Web/assets/115775237/1b0c993a-e95d-43e7-a9ce-6c5308abe3e3)

2. Tambahkan layout untuk menu `Contact` => yang berisi form isian: nama, email, message, dll
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Layout Sederhana</title>
    <link rel="stylesheet" href="style_kontak.css">
</head>
<body>
    <div id="container">
        <header>
            <h1>Layout sederhana</h1>
        </header>
        <nav>
            <a href="home.html">Home</a>
            <a href="artikel.html">Artikel</a>
            <a href="about.html">About</a>
            <a href="kontak.html" class="active">Kontak</a>
        </nav>
        <section id="contact" class="contact">
            <h2>contact</h2>
            <div class="container">
                <form>
                    <label for="name">Nama:</label>
                    <input type="text" id="name" name="name" required>
                    
                    <label for="email">Email:</label>
                    <input type="email" id="email" name="email" required>
                    
                    <label for="message">Pesan:</label>
                    <textarea id="message" name="message" rows="4" required></textarea>
                    
                    <input type="submit" value="Kirim Pesan">
                </form>
            </div>
                    </section>
                </body>
                </html>
```

![contact](https://github.com/tiaraputriiiiii/Lab4Web/assets/115775237/7e9ab4e7-5e7d-4dc3-b778-059935fdb294)

## Selesai, Terima kasih
