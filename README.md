
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
            <img src="logo.png" class="logo" width="50" height="50%"> 
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
            <p align="center"> 2 </p>
        </div>
        <div class="book-page" id="page-2">
           
            <p>Aku, North, seorang arsitek dengan ambisi besar, harapan tinggi, dan, jujur saja, temperamen yang meledak-ledak. Hidupku, kalau boleh dirangkum dalam satu kata, adalah “rumit.” Kadang terasa seperti ada skenario takdir yang dirancang khusus untuk menjatuhkanku. <br> <br>

Aku benci berpindah-pindah dari satu kota ke kota lain demi pekerjaanku. Bukan karena aku tidak suka perjalanan—tapi karena jalanan itu sendiri adalah musuhku. Lihat saja, jalan dari kota ke kota harus melewati hutan dengan lintasan penuh batu kasar, berlubang, dan terabaikan. Kayaknya jalanan ini belum pernah disentuh perbaikan sejak zaman dinosaurus punah. Aku bahkan merasa kalau batu-batu itu sengaja menunggu mobilku lewat untuk meledakkan bannya. Aku sudah mengeluarkan uang lebih untuk ban baru, entah sudah berapa kali. Benar-benar menyiksa dompetku. Kalau bisa, aku ingin tinggal di satu kota indah, dengan jalanan mulus, setidaknya untuk setahun saja. Tapi hidupku, seperti biasa, tidak pernah semudah itu. <br> <br>

Besok paginya, aku melangkah masuk ke kantor FCorp, tempat aku bekerja. Hari ini akan ada pembagian tugas baru untuk para arsitek. Sejujurnya, ini adalah salah satu momen yang selalu kunantikan. <i> Apa aku menantikannya karena aku berharap mendapat proyek di kota indah? </i> Tidak, tentu saja tidak. Aku menunggu ini karena... aku bisa duduk berdekatan dengan Ciera, seorang kolega yang entah bagaimana selalu berhasil membuatku kehilangan fokus.<br> <br>

Aku menyukai Ciera. Bukan cinta pada pandangan pertama, tapi, ya... bisa dibilang hampir seperti itu. Aku tidak tahu bagaimana menjelaskan perasaanku—dia terlalu berbeda dariku. Dia tenang, penuh percaya diri, tapi juga sarkastik dan dingin. Semacam teka-teki hidup yang selalu ingin kupecahkan. <br> <br>

Ketika rapat dimulai, seperti biasa, aku berusaha memastikan aku bisa duduk cukup dekat dengannya. Aku hanya ingin mencuri beberapa detik untuk memandang wajahnya, itu saja. Namun, seperti biasa juga, Ciera selalu menyadarinya. <br> <br>

"Kenapa kamu memandangku seperti itu? Kamu aneh tahu," katanya, dengan nada datar dan ekspresi yang nyaris tak berubah. <br> <br>

"Eh, aku cuma... memandang poster di belakangmu," jawabku buru-buru, mencoba terdengar santai.<br> <br>

Dia menoleh ke belakang, ke arah poster yang aku maksud. Sekilas aku pikir dia akan marah atau merasa terganggu, tapi ternyata dia malah tersenyum, meskipun senyum itu lebih seperti menahan tawa. "Seleramu aneh juga," katanya sambil menunjuk poster itu.<br> <br>

Aku menoleh ke arah yang sama, dan langsung ingin menghilang ke bawah meja. Poster itu adalah iklan panggilan untuk para kuli berotot, dengan gambar pria-pria besar yang memamerkan otot mereka di bawah terik matahari. Apa-apaan ini? Malunya bukan main. Aku hanya bisa mengalihkan pandangan kembali ke presentasi di depan ruangan, pura-pura fokus pada omong kosong motivasi dari petinggi perusahaan. <br> <br>

Tapi sebenarnya, tidak ada satu pun kata dari mereka yang masuk ke telingaku. Aku terlalu sibuk memikirkan bagaimana aku bisa memperbaiki kesan di depan Ciera. Hidupku benar-benar penuh dengan momen-momen memalukan seperti ini. <br> <br> </p>
<p align="center"> 2 </p>
        
        </div>
        <div class="book-page" id="page-3">
            
            <p>Rapat akhirnya selesai. Aku bersandar di kursi, hampir tertidur, sampai tiba-tiba salah satu petinggi mendatangiku dengan sebuah amplop tebal. Amplop itu tampak begitu menjanjikan—cukup untuk membuatku langsung tersadar. Aku menatapnya dengan penuh harap. "Apa ini? Bonus? Uang? Atau... uang?" pikirku. Otakku memang sederhana: apa lagi yang bisa diharapkan selain uang? <br> <br>

Dengan rasa penasaran dan sedikit terlalu banyak imajinasi, aku membuka amplop itu. Namun, begitu aku melihat isinya, harapanku runtuh seperti gedung tanpa fondasi yang benar. Dokumen tugas. Ya, tugas baru. Aku terdiam, mencoba mencerna kekecewaanku. "Kenapa sih hidup selalu begini?" gerutuku dalam hati.  <br> <br>

Tapi tunggu. Tugas kali ini ada yang berbeda. Nama lokasinya: Lembah Emas. Aku membaca lagi untuk memastikan. Lembah Emas? Apa itu berarti ada emas di mana-mana? Kalau benar, bukankah aku bisa kaya? Pikiran itu langsung membakar semangatku. "Ini mungkin kesempatan terbaikku untuk mengubah nasib!" pikirku sambil buru-buru mengemasi barang-barangku. <br> <br>

Peralatan kerja adalah hal yang paling aku jaga. Jam tangan, topi arsitek, dan jas andalan yang pernah menolongku dari banyak kejadian buruk. Ah, terlalu banyak cerita tentang itu, jadi aku malas menjelaskannya sekarang. Fokusku adalah Lembah Emas. Aku hanya perlu bersiap-siap dan berangkat.  <br> <br>

Namun, sebelum aku benar-benar bisa berlari keluar kantor, Ciera tiba-tiba muncul di hadapanku. Langkahnya tergesa-gesa, dan wajahnya terlihat seperti ada hal penting yang ingin disampaikan. Jantungku langsung berdegup lebih cepat. Sesuatu yang penting! Apa ini saatnya? Apakah dia akan bilang dia menyukaiku?  <br> <br>

"North, aku ingin mengatakan sesuatu," katanya, serius. <br> <br>

Ini dia! Aku menunggu dengan seluruh ekspektasi terbaik yang pernah kumiliki. Rasanya seluruh dunia berhenti sejenak, hanya menyisakan aku dan Ciera di ruangan itu. <br> <br>

"Kalau kamu mau badan yang bagus, mending coba masuk ke grup olahraga milik ayahku. Dia pelatih terbaik, mantan tentara. Aku yakin dia bisa membantumu," katanya, tanpa jeda.  <br> <br>

Dang. Rasanya seperti ditampar papan proyek. Ekspetasiku hancur berkeping-keping. Aku terdiam, setengah kaku seperti batu bata baru dicetak. "Baiklah, aku mungkin akan mempertimbangkannya. Aku punya banyak kegiatan lain, jadi mungkin aku bisa di hari libur," jawabku akhirnya, mencoba tetap terdengar cool.  <br> <br>

Ciera hanya mengangguk ringan, lalu pergi begitu saja tanpa banyak basa-basi. Biasa. Begitulah dia. Kadang aku bertanya-tanya kenapa aku bisa tertarik pada seseorang yang selalu menghancurkan ekspektasiku berkali-kali. <br> <br>

Setelah kejadian itu, aku kembali fokus pada tugas ke Lembah Emas. Aku memeriksa daftar barang bawaan dan memastikan semua siap. Ini akan menjadi perjalanan panjang, dan aku harus benar-benar mempersiapkan diri. Aku berjalan ke mobil dengan penuh semangat, tapi… dimana kunciku? Aku mengaduk-aduk kantong celana, tas, dan bahkan jas favoritku, tapi kunci itu tidak ada di mana-mana. "Astaga, kenapa lagi hidupku begini?"  <br> <br> </p>
      <p align="center"> 3 </p>
      
        </div>
        <div class="book-page" id="page-4">
           
            <p>Kereta akhirnya berhenti di stasiun Lembah Emas. Aku melangkah keluar dengan koper besar di tangan, sedikit terengah karena beban beratnya. Semua ini gara-gara aku lupa di mana menaruh kunci mobilku. Untungnya, mobil itu kutinggalkan di parkiran yang katanya aman. Kata Satpam sih begitu. Tapi, ya... aku tidak pernah benar-benar yakin. <br> <br>

Udara di kota ini terasa berbeda. Ada aroma khas yang tidak bisa kujelaskan, semacam bau logam yang samar, bercampur dengan aroma bunga-bunga dari taman kota yang terlihat dari kejauhan. Ini adalah kota impianku—tempat di mana kekayaan dan kesuksesan seperti menetes dari setiap sudutnya. Orang-orang selalu bilang kalau mata uang LB, mata uang lokal kota ini, punya nilai yang lebih tinggi dibandingkan kota mana pun. Tapi sekarang, aku tidak merasa seperti orang sukses. Aku hanya merasa seperti orang asing dengan koper berat dan dompet tipis.<br> <br>

Saat melangkah keluar dari halte, mataku tertuju pada seorang pria yang sedang membagikan brosur. Tapi tunggu, dia bukan pembagi brosur biasa. Penampilannya... terlalu mewah. Jasnya hitam rapi dengan dasi merah anggur yang mengilap. Bahkan sepatunya tampak lebih mahal dari koperku. Dia seperti orang kaya yang nyasar menjadi pemasar jalanan.<br> <br>

Aku mendekatinya dengan rasa penasaran. Pria itu menoleh, dan senyumnya segera merekah, seperti dia sudah menungguku sejak tadi. Yang kuingat jelas darinya adalah aroma khas cengkih yang tajam.<br> <br>

"Halo, Tuan," sapanya ramah. Suaranya lembut tapi ada sesuatu yang membuatnya terasa menusuk. "Apa Anda baru di sini? Saya punya penawaran bagus untuk Anda. Sebuah peta lengkap Kota Lembah Emas. Jika Anda tersesat, peta ini akan menjadi penyelamat Anda." <br> <br>

Aku menatapnya lekat-lekat, mencoba menganalisisnya. Ada sesuatu yang aneh dari cara dia berbicara, seperti dia tahu sesuatu tentangku. "Berapa harga brosur itu?" tanyaku, mencoba terdengar santai. <br> <br>

"Hanya 10 LB. Itu setara dengan <b> Rp100.000 </b>. Penawaran yang sangat murah untuk pendatang baru seperti Anda," katanya sambil tersenyum lebih lebar.<br> <br>

100.000? Aku hampir tersedak udara. Itu uang terakhirku. Uang makan sebulan saja tidak pernah sebesar itu. Aku membuka dompet, memastikan lagi kalau aku tidak salah. Ya, isinya cuma 100.000 pas. Sial, hari ini benar-benar tidak berpihak padaku.<br> <br>

Aku menatap pria itu lagi, lalu ke brosur di tangannya. Rasa ragu dan frustrasi berperang di kepalaku. "Baiklah," gumamku akhirnya, menarik napas panjang sebelum mengeluarkan uang itu. Tanganku gemetar saat menyerahkannya.<br> <br>

"Wah, Tuan, Anda benar-benar murah hati... dan naif," katanya sambil tersenyum, kali ini lebih tajam. Aku masih memegang ujung uangnya, ragu-ragu melepaskannya.<br> <br>

"Apa tidak ada diskon? 20% saja?" tanyaku, mencoba negosiasi terakhir dengan suara kecil.<br> <br>

"Maaf, tidak ada diskon. Anda sudah memutuskan membelinya, jadi uang tidak bisa dikembalikan," jawabnya dengan nada tegas tapi tetap sopan. <br> <br>

Dengan berat hati, aku akhirnya merelakan uang terakhirku. Pria itu menggenggam uangku dengan ringan, lalu memasukkannya ke kantong celana hitamnya dengan anggun. Dia merapikan dasinya, menatapku lagi dengan tatapan yang sulit diartikan. <br> <br>

"Terima kasih sudah berbisnis dengan saya, Tuan. Tapi, izinkan saya memberi Anda peringatan," katanya, suaranya tiba-tiba lebih pelan namun tajam. "Kota ini bukanlah tempat untuk orang senaif Anda. Di sini, baik orang jahat maupun orang baik bisa menghabisi Anda. Saya harap Anda siap." <br> <br>

Sebelum aku sempat merespons, dia melangkah pergi dengan tenang, tanpa pamit. Bau cengkihnya masih tertinggal di udara.<br> <br>

Aku berdiri di sana, memegang brosur yang baru saja menghabiskan seluruh uangku. Kata-katanya terus terngiang di kepalaku. "Orang baik pun bisa menghabisi Anda." <i> Apa maksudnya? Kenapa dia berbicara seolah-olah dia tahu sesuatu tentangku? </i> <br> <br>

Tapi aku memutuskan untuk mengabaikan semua itu. Aku terlalu lelah dan lapar untuk memikirkan hal-hal aneh. Yang penting sekarang adalah mencari makan... walaupun aku bahkan tidak tahu bagaimana melakukannya tanpa uang.</p> <br> <br>
<p align="center"> 4 </p>
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
