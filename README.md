<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Server North</title>
    <link rel="stylesheet" href="styles.css">
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            background-color: #f0f0f0;
            transition: background-color 0.3s, color 0.3s;
        }

        .content {
            background-color: #00b7ff;
            color: #000;
            border: 2px solid #000;
            padding: 20px;
            margin: 20px auto;
            max-width: 800px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            text-align: center;
            transition: background-color 0.3s, color 0.3s;
        }

        .content h1 {
            font-size: 2.5em;
            margin-bottom: 20px;
        }

        .content p {
            font-size: 1.2em;
            margin-bottom: 20px;
        }

        .kategory {
            position: fixed;
            top: 0;
            width: 100%;
            background-color: #333;
            color: white;
            display: flex;
            justify-content: space-around;
            align-items: center;
            padding: 10px 0;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            z-index: 1000;
            transition: background-color 0.3s, color 0.3s;
        }

        .kategory h1 {
            margin: 0;
            font-size: 1.5em;
        }

        .kategory a {
            color: white;
            text-decoration: none;
            padding: 10px 15px;
            transition: background-color 0.3s, transform 0.3s;
        }

        .kategory a:hover {
            background-color: #575757;
            border-radius: 5px;
            transform: scale(1.1);
        }

        .section {
            padding: 100px 20px;
            margin-top: 60px;
            transition: background-color 0.3s, color 0.3s;
        }

        .section:nth-child(odd) {
            background-color: #e9e9e9;
        }

        .section:nth-child(even) {
            background-color: #f7f7f7;
        }

        .section h2 {
            margin-top: 0;
        }

        .file-gallery {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
        }

        .file-item {
            background-color: #fff;
            border: 1px solid #ddd;
            border-radius: 8px;
            padding: 10px;
            text-align: center;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s, box-shadow 0.3s, background-color 0.3s, color 0.3s;
            font-family: Georgia, 'Times New Roman', Times, serif;
        }

        .file-item img {
            width: 200px;
            height: 200px;
            object-fit: cover;
            border-radius: 4px;
            margin-bottom: 10px;
        }

        .file-item p {
            margin: 0;
            color: #333;
        }

        .file-item:hover {
            transform: scale(1.05);
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
        }

        .bottom-nav {
            position: fixed;
            bottom: 0;
            width: 100%;
            background-color: #00bfff;
            box-shadow: 0 -2px 5px rgba(0, 0, 0, 0.1);
            transition: background-color 0.3s;
        }

        .bottom-nav ul {
            list-style-type: none;
            display: flex;
            justify-content: space-around;
            padding: 10px 0;
            margin: 0;
        }

        .bottom-nav li {
            text-align: center;
        }

        .bottom-nav a {
            text-decoration: none;
            color: #333333;
            font-size: 16px;
            display: flex;
            flex-direction: column;
            align-items: center;
            transition: color 0.3s;
        }

        .bottom-nav a img {
            width: 24px;
            height: 24px;
            margin-bottom: 5px;
        }

        .bottom-nav a:hover {
            color: #000;
        }

        .dark-mode {
            background-color: #121212;
            color: #e0e0e0;
        }

        .dark-mode .content {
            background-color: #2e2e2e;
            border-color: #444;
        }

        .dark-mode .kategory {
            background-color: #1f1f1f;
            color: #e0e0e0;
        }

        .dark-mode .section:nth-child(odd) {
            background-color: #1e1e1e;
        }

        .dark-mode .section:nth-child(even) {
            background-color: #2e2e2e;
        }

        .dark-mode .file-item {
            background-color: #2e2e2e;
            border-color: #444;
        }

        .dark-mode .bottom-nav {
            background-color: #1f1f1f;
        }

        .dark-mode-toggle {
            position: fixed;
            top: 10px;
            right: 10px;
            padding: 10px;
            background-color: #333;
            color: #fff;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .dark-mode-toggle:hover {
            background-color: #555;
        }
    </style>
</head>
<body>
    <!-- Kategori Navigasi -->
    <div class="kategory">
        <h1>Kategori</h1>
        <a href="#file-book">File BOOK</a>
        <a href="#antariksa">Antariksa</a>
        <a href="#north-novel">North Novel</a>
        <button class="dark-mode-toggle" onclick="toggleDarkMode()">Toggle Dark Mode</button>
    </div>

    <!-- Konten halaman -->
    <div class="content">
        <h1 style="background-color: rgb(0, 195, 255);color: #ffee00;">North Novel</h1>
        <p>Selamat Datang Di server North Novel <br>
        Kami memiliki berbagai kumpulan buku yang bisa kalian baca. dan pastinya <b>terverifikasi</b></p>
    </div>

    <!-- Konten -->
    <div id="file-book" class="section">
        <h2 style="background-color: chartreuse;color: #000;">File BOOK</h2>
        <p>Ini adalah bagian File BOOK.</p>
        <div class="file-gallery">
            <div class="file-item">
                <a href="path/to/yourfile1.pdf" download>
                    <img src="laut bercerita.jpg" alt="File 1">
                </a>
                <p>Laut Bercerita <br>
                Leila Salikha Chudor</p>
            </div>
            <div class="file-item">
                <a href="Pride and prejudice.pdf" download>
                    <img src="pride and prejudice.jpg" alt="File 2">
                </a>
                <p>Pride and prejudice <br>
                    Jane Austine
                </p>
            </div>
            <div class="file-item">
                <a href="Filosofi Teras (Henry Manampiring).pdf" download>
                    <img src="filosopi teras.jpg" alt="File 2">
                </a>
                <p>Filosofi Teras <br>
                    Henry Manampiring
                </p>
            </div>
        </div>
    </div>

    <div id="antariksa" class="section">
        <h2 style="background-color: #ffda07; color: #0004ff;">Antariksa</h2>
        <p>Ini adalah bagian Antariksa.</p>
    </div>

    <div id="north-novel" class="section">
        <h2 style="background-color: rgb(255, 81, 0);color: #000;">North Novel</h2>
        <p>Ini adalah bagian cerita yang dibuat oleh North.</p>
        <div class="file-item">
            <a href="north.html" download>
                <img src="" alt="North.html">
            </a>
            <p>Getaran misterius
            </p>
            <br> <br> <br>
        </div>
    </div>

    <!-- Navigasi Bawah -->
    <nav class="bottom-nav">
        <ul>
            <li>
                <a href="#home">
                    <img src="home_icon.png" alt="Home">
                    Home
                </a>
            </li>
            <li>
                <a href="#about">
                    <img src="homeikon.png" alt="About">
                    About
                </a>
            </li>
            <li>
                <img src="logo.png" alt="logo" width="70px" height="70%" align="center"><br>
                North Novel <br>
            </li>
            <li>
                <a href="#contact">
                    <img src="contactikon.png" alt="Contact">
                    Contact
                </a>
            </li>
            <li>
                <a href="#account" id="account-link">
                    <img id="account-image" src="ikonpro.png" alt="Account">
                    Account
                </a>
            </li>
        </ul>
    </nav>
    
    <script>
        function toggleDarkMode() {
            document.body.classList.toggle('dark-mode');
        }
    </script>
</body>
</html>
