<table>
  <tr>
    <th colspan="2">DATA MAHASISWA</th>
  </tr>
  <tr>
    <td>Nama</td>
    <td>Wisnu Ikhwansyah Saputra</td>
  </tr>
  <tr>
    <td>NIM</td>
    <td>312210305</td>
  </tr>
  <tr>
    <td>Kelas</td>
    <td>TI.22.A3</td>
  </tr>
</table>

---

<p align="center">PRAKTIKUM 4</p> 

### membuat dokumen html

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

### membuat Box Element

    <section>
        <div class="div1">Div 1</div>
        <div class="div2">Div 2</div>
        <div class="div3">Div 3</div>
    </section>

### menambahkan deklarasi css untuk membuat float element

    <style>
        div {
            float: left;
            padding: 10px;
        }
        .div1 {
            background: red;
        }
        .div2{
            background: yellow;
        }
        .div3{
            background: green;
        }
    </style>

<b>output:</b>

<img width="537" alt="image" src="https://github.com/Wizzs1/Lab4Web/assets/110619093/fce567f7-374f-4155-9dd4-c0f4701cbe59">

### mengatur clearfix element
<bold>menambahkan element div</b>

        <div class="div4">Div 4</div>

<bold>atur properti clear pada css</b>

        .div4{
            background-color: blue;
            clear: left;
            float: none;
        }

<bold>output:</b>
<img width="658" alt="image" src="https://github.com/Wizzs1/Lab4Web/assets/110619093/507ebf58-9e1a-4a3d-8e02-56991c0435d1">

## Membuat Layout Sederhana
### membuat dokumen html

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

### membuat kerangka layout

    <header>
        <h1>Layout Sederhana</h1>
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
    </div>



<img width="461" alt="image" src="https://github.com/Wizzs1/Lab4Web/assets/110619093/62a023ac-779e-4492-b946-eab2f413a7f7">

### menambahkan kode css

    /* import google font */
    @import url('https://fonts.googleapis.com/css2?            family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0,300;0,700;1,300&display=swap');

    /* Reset CSS */
    *{
        margin: 0;
        padding: 0;
    }

    body {
        line-height: 1;
        font-size: 100%;
        font-family:'open Sans', sans-serif ;
        color: #5a5a5a;
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



<img width="550" alt="image" src="https://github.com/Wizzs1/Lab4Web/assets/110619093/4f74fe4a-eb9a-4285-b7e6-a8e03724f401">

### membuat navigasi

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



<img width="530" alt="image" src="https://github.com/Wizzs1/Lab4Web/assets/110619093/f5e090bd-6ee3-40e8-9c0f-4eb8e33abc77">

### membuat hero panel

<b>HTML</b>

    <section id="hero">
        <h1>Hello World!</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. 
            Rem eaque ullam cum aliquam voluptatibus doloremque neque. 
            Iusto perferendis reiciendis minima ab asperiores tempora consequuntur, 
            fugit qui ipsum explicabo nisi deleniti?</p>
            <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
    </section>

<b>CSS</b>

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

    hero p {
        margin-bottom: 20px;
        font-size: 18px;
        line-height: 25px;
    }

<img width="576" alt="image" src="https://github.com/Wizzs1/Lab4Web/assets/110619093/c4f25b9a-aa76-4b89-ae88-baec47e9dd43">

### mengatur layout main dan sidebar
<b>HTML</b>

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
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                Consequuntur, accusamus quas! Quidem eveniet quas dolore fugit repellendus quo ullam, tenetur hic nemo aperiam. 
                Dignissimos debitis aliquam dolor atque sapiente? Fuga?</p>
        </div>
    </aside>

<b>CSS</b>

    /* sidebar area */
    #sidebar {
        float: left;
        width: 640px;
        padding: 20px;
    }

    /* widget */
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

<img width="516" alt="image" src="https://github.com/Wizzs1/Lab4Web/assets/110619093/a85a50df-f82f-4ffe-8cb5-27e21e28cee3">

### menambahkan element lain pada main content
