
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Novel North</title>
    <style>
        /* Navbar Styles */
        .navbar {
            display: flex;
            align-items: center;
            justify-content: space-between;
            background-color: #333;
            color: #fff;
            padding: 10px 20px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .navbar .logo {
            font-size: 24px;
            font-weight: bold;
            color: #fff;
            text-decoration: none;
        }

        .nav-buttons {
            display: flex;
            gap: 15px;
        }

        .nav-buttons button {
            background-color: #555;
            border: none;
            border-radius: 5px;
            padding: 10px 15px;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .nav-buttons button:hover {
            background-color: #777;
        }

        .nav-buttons button a {
            text-decoration: none;
            color: #fff;
            font-size: 14px;
        }

        .nav-buttons button a:hover {
            color: #ffd700;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .navbar {
                flex-wrap: wrap;
                justify-content: center;
                text-align: center;
            }

            .nav-buttons {
                flex-wrap: wrap;
                justify-content: center;
                gap: 10px;
            }
        }

        /* Global Styles */
        body {
            font-family: 'Georgia', serif;
            background-color: #f9f9f9;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        header {
            width: 100%;
            background-color: #333;
            color: #fff;
            padding: 15px 0;
            text-align: center;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
        }

        header h1 {
            margin: 0;
            font-size: 24px;
        }

        #book-container {
            width: 70%;
            max-width: 800px;
            margin: 20px auto;
            background-color: #fff;
            border: 2px solid #ddd;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            position: relative;
        }

        .book-page {
            padding: 20px;
            display: none;
        }

        .book-page h2 {
            margin-top: 0;
            color: #555;
            text-align: center;
        }

        .book-page p {
            text-align: justify;
            line-height: 1.8;
            color: #333;
        }

        .controls {
            display: flex;
            justify-content: space-between;
            background-color: #f4f4f4;
            padding: 10px;
            position: sticky;
            bottom: 0;
            border-top: 1px solid #ddd;
        }

        .controls button {
            padding: 10px 20px;
            background-color: #333;
            color: #fff;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
            transition: background-color 0.3s;
        }

        .controls button:hover {
            background-color: #555;
        }

        #scroll-top {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background-color: #333;
            color: #fff;
            border: none;
            border-radius: 50%;
            width: 50px;
            height: 50px;
            cursor: pointer;
            font-size: 24px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
            display: none;
            justify-content: center;
            align-items: center;
        }

        #scroll-top:hover {
            background-color: #555;
        }

        #book-container:active {
            transform: scale(1.05);
        }

         /* Floating Zoom Buttons */
         .zoom-controls {
            position: fixed;
            bottom: 20px;
            right: 20px;
            display: flex;
            flex-direction: column;
            gap: 10px;
            z-index: 1000;
        }

        .zoom-controls button {
            background-color: #333;
            color: #fff;
            border: none;
            border-radius: 50%;
            width: 40px;
            height: 40px;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            font-size: 20px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s, background-color 0.3s;
        }

        .zoom-controls button:hover {
            background-color: #555;
            transform: scale(1.1);
        }

        #warning {
            display: none;
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background-color: rgba(0, 0, 0, 0.8);
            color: #fff;
            padding: 20px;
            border-radius: 10px;
            text-align: center;
            z-index: 9999;
            font-family: Arial, sans-serif;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.3);
        }

    </style>
</head>

<body>
    <header>
        <div class="navbar">
            <img src="logo.png" class="logo" width="50" height="50%"> North 
            <div class="nav-buttons">
                <button><a href="file:///C:/Users/tisna/OneDrive/Desktop/Website%20lab/Firdaus%20Server(1).html">Home</a></button>
                <button><a href="file:///C:/Users/LENOVO/Desktop/belajar%20code/New%20folder/contact.html">Contact</a></button>
                <button><a href="file:///C:/Users/LENOVO/Desktop/belajar%20code/New%20folder/login.html">Login Yuk</a></button>
                <button><a href="file:///C:/Users/LENOVO/Desktop/belajar%20code/New%20folder/pembelajaran.html">3 Tema Pembelajaran</a></button>
                <button><a href="file:///C:/Users/tisna/OneDrive/Desktop/Website%20lab/link%20belajar.html" style="color: red;">Pembelajaran</a></button>
                
            </div>
        </div>
    </header>

    <div id="book-container">
        <div class="book-page" id="page-1">
            <h2>Bab 1 - Kota Lembah Emas</h2>
            <p><i>Malam tiba di Kota Lembah Emas. Langit dipenuhi bintang-bintang, sementara gedung-gedung besar berdiri megah menghiasi pemandangan. Namun, ada sesuatu yang terasa ganjil. Setiap bangunan—dari rumah kecil hingga gedung pencakar langit—dilengkapi dengan pengait besar di atapnya. Tidak ada yang tahu pasti tujuan benda itu, dan penduduk kota jarang membicarakannya, seolah-olah itu hanyalah bagian biasa dari kehidupan sehari-hari. <br>

                <br>Kota Lembah Emas dikenal sebagai pusat kemakmuran. Dengan tambang emas besar di lembah dan hutan luas di kaki gunung, kota ini memegang kekayaan alam yang melimpah. Mata uangnya, LB, lebih mahal dan kuat dibandingkan kota mana pun, menjadi simbol kejayaan yang membuat daerah ini disegani. Namun, di balik kemewahan dan gemerlapnya, ada misteri yang membuat penduduk selalu waspada: getaran misterius yang datang tanpa peringatan.<br>
                <br>Guncangan itu terjadi hampir setiap siang hari. Tidak peduli seberapa kokoh bangunannya, setiap minggu ada saja gedung yang runtuh atau retak. Rumor terus beredar—mulai dari penjelasan logis seperti aktivitas lempeng bumi atau dampak tambang yang terlalu dalam, hingga desas-desus yang jauh lebih gelap. Sebagian orang percaya bahwa getaran itu adalah peringatan dari makhluk kuno yang tinggal jauh di dalam perut bumi, penjaga kekayaan alam Lembah Emas.<br>
                <br>Aku sendiri tidak percaya semua itu. Hingga kini, belum ada informasi resmi yang dapat menjelaskan penyebab getaran ini. Ilmuwan tidak pernah datang untuk menyelidiki, atau mungkin mereka sengaja tidak diundang. Tidak ada penelitian, tidak ada jawaban. Anehnya, meskipun misteri ini belum terpecahkan, kota ini tidak pernah kehilangan penduduk. Orang-orang tetap berdatangan, tergoda oleh janji kekayaan yang mengalahkan rasa takut<br>
                <br>Namun, semakin lama aku tinggal di sini, semakin aku merasa ada sesuatu yang disembunyikan. Pengait-pengait di atap, gedung-gedung yang dibangun ulang berulang kali, dan sikap penduduk yang tampaknya menghindari topik ini. Kota ini seperti diam-diam menyimpan rahasia besar.<br>
                <br>Hingga suatu hari, aku melihat sesuatu yang mengubah semuanya.<br></i>
            </p> 
            <p> North Arlington <br>
                29.9.2009<br>
            </p>
        </div>
        <div class="book-page" id="page-2">
            <h2>Bab 2 - Misteri yang Belum Terpecahkan</h2>
            <p>Guncangan terjadi hampir setiap minggu. Rumor tentang makhluk kuno di perut bumi menjadi perbincangan...</p>
        </div>
        <div class="book-page" id="page-3">
            <h2>Bab 3 - Penemuan Baru</h2>
            <p>Aku menemukan sesuatu yang mengubah segalanya. Pengait di atap, bangunan yang terus direnovasi...</p>
        </div>
        <div class="book-page" id="page-4">
            <h2>Bab 4 - Akhir dari Misteri</h2>
            <p>Pada akhirnya, aku mengetahui kebenarannya. Kota ini menyimpan rahasia besar yang tidak pernah
                terungkap...</p>
        </div>

        <div class="controls">
            <button id="prev">⬅️ Sebelumnya</button>
            <button id="next">Berikutnya ➡️</button>
        </div>
    </div>
    <div class="zoom-controls">
        <button id="zoom-in">➕</button>
        <button id="zoom-out">➖</button>
    </div>

    <button id="scroll-top">⬆️</button>

    <script>
        const pages = document.querySelectorAll('.book-page');
        const prevButton = document.getElementById('prev');
        const nextButton = document.getElementById('next');
        const scrollTopButton = document.getElementById('scroll-top');
        let currentPage = 0;

        // Show the initial page
        function showPage(index) {
            pages.forEach((page, i) => {
                page.style.display = i === index ? 'block' : 'none';
            });
        }

        // Update button states
        function updateButtons() {
            prevButton.disabled = currentPage === 0;
            nextButton.disabled = currentPage === pages.length - 1;
        }

        // Scroll to top when the button is clicked
        scrollTopButton.addEventListener('click', () => {
            window.scrollTo({ top: 0, behavior: 'smooth' });
        });

        // Show scroll-top button when scrolled
        window.addEventListener('scroll', () => {
            scrollTopButton.style.display = window.scrollY > 100 ? 'flex' : 'none';
        });

        // Event listeners for navigation
        prevButton.addEventListener('click', () => {
            if (currentPage > 0) {
                currentPage--;
                showPage(currentPage);
                updateButtons();
            }
        });

        nextButton.addEventListener('click', () => {
            if (currentPage < pages.length - 1) {
                currentPage++;
                showPage(currentPage);
                updateButtons();
            }
        });

        // Initialize the book
        showPage(currentPage);
        updateButtons();

        const zoomInButton = document.getElementById('zoom-in');
        const zoomOutButton = document.getElementById('zoom-out');
        let zoomLevel = 1;

        // Event Listener for Zoom In
        zoomInButton.addEventListener('click', () => {
            zoomLevel += 0.1;
            document.body.style.transform = `scale(${zoomLevel})`;
            document.body.style.transformOrigin = 'center';
        });

        // Event Listener for Zoom Out
        zoomOutButton.addEventListener('click', () => {
            zoomLevel = Math.max(0.5, zoomLevel - 0.1); // Minimum zoom level of 0.5
            document.body.style.transform = `scale(${zoomLevel})`;
            document.body.style.transformOrigin = 'center';
        });

        // Mencegah Klik Kanan
        document.addEventListener('contextmenu', (event) => {
            event.preventDefault(); // Mencegah menu klik kanan
            showWarning(); // Menampilkan peringatan
        });

        // Mencegah Shortcut Copy (Ctrl+C) dan Highlight
        document.addEventListener('keydown', (event) => {
            if ((event.ctrlKey && event.key === 'c') || (event.ctrlKey && event.key === 'x')) {
                event.preventDefault(); // Mencegah shortcut copy atau cut
                showWarning();
            }
        });

        // Menampilkan Peringatan
        function showWarning() {
            const warning = document.getElementById('warning');
            warning.style.display = 'block';
            setTimeout(() => {
                warning.style.display = 'none';
            }, 2000); // Sembunyikan peringatan setelah 2 detik
        }

    </script>
</body>

</html>
