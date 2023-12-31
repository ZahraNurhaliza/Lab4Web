# Lab4Web

## Langkah-langkah Praktikum
1. Persiapan membuat dokumen HTML dengan nama file lab4_box html seperti berikut.
```html
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
        </header>
</body>
</html>
```
Membuat Box Element
Kemudian tambahkan kode untuk membuat box element dengan tag div seperti berikut.
```html
 <section>
            <div class="div1">Div 1</div>
            <div class="div2">Div 2</div>
            <div class="div3">Div 3</div>
</section>
```
CSS Float Property
Selanjutnya tambahkan deklarasi CSS pada head untuk membuat float element, seperti berikut.
```html
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
```
Selanjutnya buka browser dan refresh kembali.
![image](https://github.com/ZahraNurhaliza/Lab4Web/blob/main/screenshot/ss.1.png)


2. Mengatur Clearfix Element
Clearfix digunakan untuk mengatur element setelah float element. Property clear digunakan untuk mengaturnya.
Tambahkan element div lainnya seteleah div3 seperti berikut.
```html
<div class="div4">Div 4</div>
```
Kemudian atur property clear pada CSS, seperti berikut.
```css
 .div4 {
                background-color: blue;
                clear: left;
                float: none;
            }
```
Selanjutnya buka browser dan refresh kembali.
![image](https://github.com/ZahraNurhaliza/Lab4Web/blob/main/screenshot/ss.2.png)


3. Membuat Layout Sederhana
Buat folder baru dengan nama lab4_layout, kemudian buatlah file baru didalamnya dengan nama home.html, dan file css dengan nama style.css.
```html
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
</body>
</html>
```
Kemudian tulis kode berikut.
```html
</header>
    <nav>
        <a href="home.html" class="active">Home</a>
        <a href="artikel.html">Artikel</a>
        <a href="about.html">About</a>
        <a href="kontak.html">Kontak</a>
    </nav>
    <section id="wrapper">
        <section id="main"></section>
        <aside id="sidebar"></aside>
    </section>
    <footer>
        <p>&copy; 2021 - Universitas Pelita Bangsa</p>
    </footer>
```
Selanjutnya buka browser dan refresh kembali.
![image](https://github.com/ZahraNurhaliza/Lab4Web/blob/main/screenshot/ss.3.png)


Kemudian tambahkan kode CSS untuk membuat layoutnya.
```css
/* import google font */
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap');
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0,300;0,700;1,300&display=swap');
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
Selanjutnya buka browser dan refresh kembali.
![image](https://github.com/ZahraNurhaliza/Lab4Web/blob/main/screenshot/ss.4.png)


4. Membuat Navigasi
Kemudian selanjutnya mengatur navigasi.
```css
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
Selanjutnya buka browser dan refresh kembali.
![image](https://github.com/ZahraNurhaliza/Lab4Web/blob/main/screenshot/ss.5.png)


5. Membuat Hero Panel.
Selanjutnya membuat hero panel. Tambahkan kode HTML dan CSS seperti berikut.
```html
 <section id="hero">
        <h1>Hello World!</h1>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem 
        elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
        vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
        pretium ac.</p>
        <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
    </section>
```
```css
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
Selanjutnya buka browser dan refresh kembali.
![image](https://github.com/ZahraNurhaliza/Lab4Web/blob/main/screenshot/ss.6.png)


6. Mengatur Layout Main dan Sidebar
Selanjutnya mengatur main content dan sidebar, tambahkan CSS float.
```css
/* main content */
#wrapper {
    margin: 0;
    }
#main {
        float: left;
        width: 890px;
        padding: 20px;
}
/* sidebar area */
#sidebar {
        float: right;
        width: 260px;
        padding: 20px;
}
```


7. Membuat Sidebar Widget
Kemudian selanjutnya menambahkan element lain dalam sidebar.
```html
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
Kemudian tambahkan CSS.
```css
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
Selanjutnya buka browser dan refresh kembali.
![image](https://github.com/ZahraNurhaliza/Lab4Web/blob/main/screenshot/ss.7.png)


8. Mengatur Footer
Selanjutnya mengatur tampilan footer. Tambahkan CSS untuk footer.
```css
/* footer */
footer {
    clear:both;
    background-color:#1d1d1d;
    padding:20px;
    color:#eee;
}
```
Selanjutnya buka browser dan refresh kembali.
![image](https://github.com/ZahraNurhaliza/Lab4Web/blob/main/screenshot/ss.8.png)


9. Menambahkan Elemen lainnya pada Main Content
```html
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
Kemudian tambahkan CSS.
```css
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
Selanjutnya buka browser dan refresh kembali.
![image](https://github.com/ZahraNurhaliza/Lab4Web/blob/main/screenshot/ss.9.png)


10. Menambahkan Content Artikel
Selanjutnya membuat content artikel. Tambahkan HTML berikut pada main content.
```html
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
Kemudian tambahkan CSS.
```css
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
Selanjutnya buka browser dan refresh kembali.
![image](https://github.com/ZahraNurhaliza/Lab4Web/blob/main/screenshot/ss.10.png)


## Pertanyaan dan Tugas
1. Tambahkan Layout untuk menu About
=> buat single layout yang berisi deskripsi, portfolio, dll
```html
<!DOCTYPE html>
<html>
<head>
	<title>About Us</title>
    <style>
    body {
        font-family: Courier, Monospace;
        margin: 0;
        padding: 0;
    }
    header {
        background-color: #333;
        color: #fff;
        padding: 20px;
        text-align: center;
    }
    main {
        margin: 80px;
    }
    section {
        margin-bottom: 20px;
    } 
    h2 {
        border-bottom: px solid #ccc;
        padding-bottom: 5px;
    }
    ul {
        list-style-type: none;
        margin: 0;
        padding: 0;
    }
    li {
        margin-bottom: 10px;
    }
    a {
        color: #333;
        text-decoration: none;
    }
</style>
</head>
<body>
	<header>
		<h1>About Us</h1>
	</header>
	<main>
		<section>
			<h2>Deskripsi</h2>
            <img src="c:\Users\Asus\Downloads\d0716228-4481-4333-be72-ef861ce8cb96.jpeg" width="200" alt="Gambar">
			<p>Hi, Perkenalkan nama saya Zahra Nurhaliza, biasa di pangil zahra, saya berusia 19 tahun yang lahir di Jakarta. 
                Saya memiliki mata hitam yang cerah dan rambut berwarna hitam gelap. Saat ini, saya mahasiswa dari Universitas Pelita Bangsa jurusan Teknik Informatika.
                Saya sering menghabiskan waktu untuk mendengarkan musik, menonton drama/film, dan membaca novel di waktu luang. Musik memberi saya inspirasi dan keseimbangan dalam hidup. 
                Selain itu, Salah satu impian saya adalah menjelajahi dunia. Terima kasih telah membaca deskripsi saya, dan saya berharap kita dapat berbagi cerita dan pengalaman bersama di masa depan.</p>
		</section>

		<section>
			<h2>Portfolio</h2>
			<ul>
				<li><a href="#">Favorite person </a></li>
                <img src="c:\Users\Asus\Downloads\jaemin dark.jpeg" width="200" alt="Gambar">
				<li><a href="#">Favorite person </a></li>
                <img src="c:\Users\Asus\Downloads\木星.jpeg" width="200" alt="Gambar">
				<li><a href="#">Favorite person </a></li>
                <img src="c:\Users\Asus\Downloads\🖇 ♯ ww ▸ icon_.jpeg" width="200" alt="Gambar">
			</ul>
		</section>
	</main>
</body>
</html>
```
![image](https://github.com/ZahraNurhaliza/Lab4Web/blob/main/screenshot/ss.11.png)


2. Tambahkan layout untuk menu Contact
=> yang berisi form isian: nama, email, message, dll
```html
<!DOCTYPE html>
<html>
<head>
	<title>Contact Us</title>
	<style>
        body {
	font-family: Courier, Monospace;
	margin: 0;
	padding: 0;
}

header {
	background-color: #333;
	color: #fff;
	padding: 20px;
	text-align: center;
}

main {
	margin: 20px auto;
	max-width: 600px;
}

form label {
	display:block; 
	margin-top:20px; 
	font-size:1.2em; 
	color:#444; 
}

form input[type=text], form input[type=email], form textarea {
	width:100%; 
	padding:10px;  
	border-radius:5px; 
	border:none; 
	margin-top:-5px; 
	line-height:normal; 
	font-size:1.2em; 
}

form input[type=submit] {
	background-color:#333; 
	color:#fff; 
	border:none; 
	padding:10px 20px; 
	border-radius:5px; 
	cursor:pointer; 
	margin-top:-5px; 
	font-size:1.2em; 
}
    </style>
</head>
<body>
	<header>
		<h1>Contact Us</h1>
	</header>

	<main>
        <form action="#" method="post">
            <img src="c:\Users\Asus\Downloads\Notebook Of Contacts free icons designed by Freepik.png" width="100" alt="Gambar">
            <label for="name">Name:</label><br />
            <input type="text" id="name" name="name" required /><br />

            <label for="email">Email:</label><br />
            <input type="email" id="email" name="email" required /><br />

            <label for="message">Message:</label><br />
            <textarea id="message" name="message" required></textarea><br />

            <input type="submit" value="Send Message" />
        </form> 
    </main>
</body> 
</html>
```
![image](https://github.com/ZahraNurhaliza/Lab4Web/blob/main/screenshot/ss.12.png)


## SELESAI