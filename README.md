<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SMK Negeri 7 Batam - INOVATIF DAN BERBUDAYA</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            background-color: #000;
            color: #fff;
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header */
        header {
            background-color: #000;
            padding: 1rem 0;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 2px 10px rgba(255, 215, 0, 0.3);
        }

        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 15px;
        }

        .logo-image {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            object-fit: cover;
            border: 2px solid #FFD700;
        }

        .logo-circle {
            width: 50px;
            height: 50px;
            background-color: #FFD700;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 24px;
            font-weight: bold;
            color: #000;
        }

        .school-name {
            font-size: 1.5rem;
            font-weight: bold;
            color: #FFD700;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 30px;
        }

        nav a {
            color: #fff;
            text-decoration: none;
            padding: 10px 15px;
            border-radius: 5px;
            transition: all 0.3s;
        }

        nav a:hover {
            background-color: #FFD700;
            color: #000;
        }

        /* Mobile Menu */
        .mobile-menu {
            display: none;
            background-color: #FFD700;
            color: #000;
            border: none;
            padding: 10px;
            border-radius: 5px;
            cursor: pointer;
        }

        @media (max-width: 768px) {
            nav ul {
                display: none;
            }
            .mobile-menu {
                display: block;
            }
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #000 0%, #333 50%, #000 100%);
            padding: 100px 0;
            text-align: center;
        }

        .hero h1 {
            font-size: 3rem;
            color: #FFD700;
            margin-bottom: 20px;
        }

        .hero h2 {
            font-size: 4rem;
            font-weight: bold;
            margin-bottom: 30px;
        }

        .hero p {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto 50px;
            color: #ccc;
        }

        .hero-logo {
            width: 120px;
            height: 120px;
            background: linear-gradient(135deg, #FFD700, #FFC107);
            border-radius: 50%;
            margin: 0 auto;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 0 10px 30px rgba(255, 215, 0, 0.3);
        }

        .hero-logo-inner {
            width: 90px;
            height: 90px;
            background-color: #000;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 3rem;
            font-weight: bold;
            color: #FFD700;
        }

        .hero-logo img {
            width: 90px;
            height: 90px;
            border-radius: 50%;
            object-fit: cover;
        }

        /* Statistics Section */
        .stats {
            background-color: #FFD700;
            padding: 80px 0;
        }

        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
        }

        .stat-card {
            background-color: #000;
            padding: 40px 20px;
            border-radius: 10px;
            text-align: center;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
        }

        .stat-icon {
            font-size: 3rem;
            margin-bottom: 20px;
        }

        .stat-number {
            font-size: 3rem;
            font-weight: bold;
            color: #FFD700;
            margin-bottom: 10px;
        }

        .stat-label {
            color: #fff;
            font-weight: bold;
            font-size: 0.9rem;
        }

        /* Principal Section */
        .principal {
            background-color: #000;
            padding: 80px 0;
            text-align: center;
        }

        .principal h2 {
            font-size: 2.5rem;
            color: #FFD700;
            margin-bottom: 10px;
        }

        .principal h3 {
            font-size: 1.5rem;
            margin-bottom: 50px;
        }

        .principal-card {
            background-color: #333;
            border: 2px solid #FFD700;
            border-radius: 15px;
            padding: 40px;
            max-width: 800px;
            margin: 0 auto;
        }

        .principal-avatar {
            width: 120px;
            height: 120px;
            background-color: #FFD700;
            border-radius: 50%;
            margin: 0 auto 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            overflow: hidden;
            border: 3px solid #FFD700;
        }

        .principal-avatar img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            border-radius: 50%;
        }

        .principal-title {
            color: #FFD700;
            font-size: 1.3rem;
            margin-bottom: 20px;
        }

        .principal-message {
            color: #ccc;
            font-size: 1.1rem;
            line-height: 1.8;
        }

        /* School Identity Section */
        .identity {
            background-color: #333;
            padding: 80px 0;
        }

        .identity h2 {
            text-align: center;
            font-size: 2.5rem;
            color: #FFD700;
            margin-bottom: 50px;
        }

        .tabs {
            max-width: 800px;
            margin: 0 auto;
        }

        .tab-buttons {
            display: flex;
            background-color: #000;
            border: 2px solid #FFD700;
            border-radius: 10px 10px 0 0;
        }

        .tab-button {
            flex: 1;
            padding: 15px;
            background: none;
            border: none;
            color: #fff;
            cursor: pointer;
            transition: all 0.3s;
        }

        .tab-button.active {
            background-color: #FFD700;
            color: #000;
        }

        .tab-content {
            background-color: #000;
            border: 2px solid #FFD700;
            border-top: none;
            border-radius: 0 0 10px 10px;
            padding: 30px;
        }

        .tab-pane {
            display: none;
        }

        .tab-pane.active {
            display: block;
        }

        .info-item {
            display: flex;
            justify-content: space-between;
            padding: 10px 0;
            border-bottom: 1px solid #444;
        }

        .info-label {
            color: #ccc;
            font-weight: bold;
        }

        .info-value {
            color: #fff;
        }

        /* Values Section */
        .values {
            background: linear-gradient(135deg, #FFD700, #FFC107);
            padding: 80px 0;
        }

        .values-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
            gap: 30px;
        }

        .value-card {
            background-color: #000;
            padding: 60px 40px;
            border-radius: 15px;
            text-align: center;
        }

        .value-title {
            font-size: 3rem;
            font-weight: bold;
            color: #FFD700;
            margin-bottom: 20px;
        }

        .value-subtitle {
            font-size: 1.2rem;
            color: #fff;
        }

        /* Programs Section */
        .programs {
            background-color: #333;
            padding: 80px 0;
        }

        .programs h2 {
            text-align: center;
            font-size: 2.5rem;
            color: #FFD700;
            margin-bottom: 20px;
        }

        .programs h3 {
            text-align: center;
            font-size: 1.5rem;
            margin-bottom: 50px;
        }

        .program-card {
            background-color: #000;
            border: 2px solid #FFD700;
            border-radius: 15px;
            padding: 40px;
            max-width: 800px;
            margin: 0 auto;
        }

        .program-title {
            color: #FFD700;
            font-size: 1.5rem;
            text-align: center;
            margin-bottom: 20px;
        }

        .program-subtitle {
            color: #fff;
            font-size: 1.2rem;
            text-align: center;
            margin-bottom: 30px;
        }

        .program-list {
            list-style: none;
        }

        .program-list li {
            display: flex;
            align-items: center;
            margin-bottom: 15px;
            color: #ccc;
        }

        .program-list li::before {
            content: "●";
            color: #FFD700;
            font-size: 1.5rem;
            margin-right: 15px;
        }

        /* News Section */
        .news {
            background-color: #000;
            padding: 80px 0;
            text-align: center;
        }

        .news h2 {
            font-size: 2.5rem;
            color: #FFD700;
            margin-bottom: 20px;
        }

        .news h3 {
            font-size: 1.5rem;
            margin-bottom: 30px;
        }

        .news-button {
            background-color: #FFD700;
            color: #000;
            border: none;
            padding: 15px 30px;
            border-radius: 5px;
            font-size: 1.1rem;
            font-weight: bold;
            cursor: pointer;
            transition: all 0.3s;
        }

        .news-button:hover {
            background-color: #FFC107;
            transform: translateY(-2px);
        }

        /* CTA Section */
        .cta {
            background-color: #FFD700;
            color: #000;
            padding: 60px 0;
            text-align: center;
        }

        .cta h2 {
            font-size: 2rem;
            margin-bottom: 10px;
        }

        .cta h3 {
            font-size: 2.5rem;
            font-weight: bold;
        }

        /* Footer */
        footer {
            background-color: #000;
            padding: 60px 0 20px;
        }

        .footer-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-bottom: 40px;
        }

        .footer-section h4 {
            color: #FFD700;
            font-size: 1.2rem;
            margin-bottom: 20px;
        }

        .footer-section ul {
            list-style: none;
        }

        .footer-section li {
            margin-bottom: 10px;
        }

        .footer-section a {
            color: #ccc;
            text-decoration: none;
            transition: color 0.3s;
        }

        .footer-section a:hover {
            color: #FFD700;
        }

        .social-links {
            display: flex;
            gap: 15px;
        }

        .social-link {
            width: 40px;
            height: 40px;
            background-color: #333;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #fff;
            text-decoration: none;
            transition: all 0.3s;
        }

        .social-link:hover {
            background-color: #FFD700;
            color: #000;
        }

        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid #333;
            color: #666;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2rem;
            }
            
            .hero h2 {
                font-size: 2.5rem;
            }
            
            .hero p {
                font-size: 1rem;
            }
            
            .tab-buttons {
                flex-direction: column;
            }
            
            .values-grid {
                grid-template-columns: 1fr;
            }
            
            .value-card {
                padding: 40px 20px;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <div class="header-content">
                <div class="logo">
                    <!-- School Logo -->
                    <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRxl7z_QFJUAFkMIqtdf7SfCwnBebHB8aC4WQ&s" 
                         alt="Logo SMK Negeri 7 Batam" class="logo-image">
                    <div class="school-name">SMK NEGERI 7 BATAM</div>
                </div>
                <nav>
                    <ul>
                        <li><a href="#home">Home</a></li>
                        <li><a href="#profil">Profil</a></li>
                        <li><a href="#program">Program</a></li>
                        <li><a href="#keahlian">Konsentrasi Keahlian</a></li>
                        <li><a href="#gtk">GTK dan Siswa</a></li>
                        <li><a href="#sarpras">SarPras</a></li>
                        <li><a href="#kegiatan">Kegiatan</a></li>
                        <li><a href="#galeri">Galeri</a></li>
                        <li><a href="#berita">Berita</a></li>
                        <li><a href="#blog">Blog</a></li>
                        <li><a href="#kontak">Kontak</a></li>
                        <li><a href="#login">Login</a></li>
                    </ul>
                </nav>
                <button class="mobile-menu">☰</button>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container">
            <h1>SELAMAT DATANG di</h1>
            <h2>SMK NEGERI 7 BATAM</h2>
            <p>
                SMK Negeri 7 Batam Mewujudkan Peserta Didik yang Beriman, Bertaqwa kepada<br>
                <strong style="color: #FFD700;">TUHAN YANG MAHA ESA</strong> dan Berakhlak Mulia, Terampil, Unggul, dan Berdaya Saing<br>
                <strong style="color: #FFD700;">Global di Era Teknologi Digital.</strong>
            </p>
            <div class="hero-logo">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRxl7z_QFJUAFkMIqtdf7SfCwnBebHB8aC4WQ&s" 
                     alt="Logo SMK Negeri 7 Batam">
            </div>
        </div>
    </section>

    <!-- Statistics Section -->
    <section class="stats">
        <div class="container">
            <div class="stats-grid">
                <div class="stat-card">
                    <div class="stat-icon">👨‍🏫</div>
                    <div class="stat-number">85</div>
                    <div class="stat-label">GURU DAN TENAGA KEPENDIDIKAN</div>
                </div>
                <div class="stat-card">
                    <div class="stat-icon">🏫</div>
                    <div class="stat-number">36</div>
                    <div class="stat-label">ROMBEL</div>
                </div>
                <div class="stat-card">
                    <div class="stat-icon">📚</div>
                    <div class="stat-number">5</div>
                    <div class="stat-label">KONSENTRASI KEAHLIAN</div>
                </div>
                <div class="stat-card">
                    <div class="stat-icon">👨‍🎓</div>
                    <div class="stat-number">1200</div>
                    <div class="stat-label">PESERTA DIDIK</div>
                </div>
            </div>
        </div>
    </section>

    <!-- School Identity Section -->
    <section class="identity">
        <div class="container">
            <h2>IDENTITAS SEKOLAH</h2>
            <div class="tabs">
                <div class="tab-buttons">
                    <button class="tab-button active" onclick="showTab('identitas')">Identitas Sekolah</button>
                    <button class="tab-button" onclick="showTab('kontak')">Kontak</button>
                    <button class="tab-button" onclick="showTab('ketersediaan')">Ketersediaan</button>
                </div>
                <div class="tab-content">
                    <div id="identitas" class="tab-pane active">
                        <div class="info-item">
                            <span class="info-label">Akreditasi:</span>
                            <span class="info-value">A</span>
                        </div>
                        <div class="info-item">
                            <span class="info-label">Kurikulum:</span>
                            <span class="info-value">Kurikulum Merdeka</span>
                        </div>
                        <div class="info-item">
                            <span class="info-label">NPSN:</span>
                            <span class="info-value">69774885</span>
                        </div>
                        <div class="info-item">
                            <span class="info-label">Status:</span>
                            <span class="info-value">Negeri</span>
                        </div>
                        <div class="info-item">
                            <span class="info-label">Bentuk Pendidikan:</span>
                            <span class="info-value">SMK</span>
                        </div>
                        <div class="info-item">
                            <span class="info-label">Status Kepemilikan:</span>
                            <span class="info-value">Pemerintah Daerah</span>
                        </div>
                        <div class="info-item">
                            <span class="info-label">SK Pendirian Sekolah:</span>
                            <span class="info-value">KPTS.367/HK/IX/2014</span>
                        </div>
                        <div class="info-item">
                            <span class="info-label">Tanggal SK Pendirian:</span>
                            <span class="info-value">2014-09-05</span>
                        </div>
                        <div class="info-item">
                            <span class="info-label">SK Izin Operasional:</span>
                            <span class="info-value">KPTS.367/HK/IX/2014</span>
                        </div>
                        <div class="info-item">
                            <span class="info-label">Tanggal SK Izin Operasional:</span>
                            <span class="info-value">2015-10-23</span>
                        </div>
                    </div>
                    <div id="kontak" class="tab-pane">
                        <div class="info-item">
                            <span class="info-label">Email:</span>
                            <span class="info-value"><a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="384b5553565d5f5d4a510f5a594c5955785f55595154165b5755">[email&#160;protected]</a></span>
                        </div>
                        <div class="info-item">
                            <span class="info-label">Alamat:</span>
                            <span class="info-value">Perumahan Sekawan Pemko, Kelurahan Belian, Kec. Batam Kota</span>
                        </div>
                        <div class="info-item">
                            <span class="info-label">Kota:</span>
                            <span class="info-value">Batam, Prov. Kepulauan Riau</span>
                        </div>
                        <div class="info-item">
                            <span class="info-label">Kode Pos:</span>
                            <span class="info-value">29463</span>
                        </div>
                    </div>
                    <div id="ketersediaan" class="tab-pane">
                        <div class="info-item">
                            <span class="info-label">Laboratorium Komputer:</span>
                            <span class="info-value" style="color: #4CAF50;">Tersedia</span>
                        </div>
                        <div class="info-item">
                            <span class="info-label">Laboratorium Bahasa:</span>
                            <span class="info-value" style="color: #4CAF50;">Tersedia</span>
                        </div>
                        <div class="info-item">
                            <span class="info-label">Perpustakaan:</span>
                            <span class="info-value" style="color: #4CAF50;">Tersedia</span>
                        </div>
                        <div class="info-item">
                            <span class="info-label">Ruang Praktik:</span>
                            <span class="info-value" style="color: #4CAF50;">Tersedia</span>
                        </div>
                        <div class="info-item">
                            <span class="info-label">Aula:</span>
                            <span class="info-value" style="color: #4CAF50;">Tersedia</span>
                        </div>
                        <div class="info-item">
                            <span class="info-label">Lapangan Olahraga:</span>
                            <span class="info-value" style="color: #4CAF50;">Tersedia</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Values Section -->
    <section class="values">
        <div class="container">
            <div class="values-grid">
                <div class="value-card">
                    <div class="value-title">INOVATIF</div>
                    <div class="value-subtitle">Pioneering Solutions and Innovations</div>
                </div>
                <div class="value-card">
                    <div class="value-title">BERBUDAYA</div>
                    <div class="value-subtitle">Diverse Ethnicities and Religions</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Programs Section -->
    <section class="programs" id="keahlian">
        <div class="container">
            <h2>KONSENTRASI KEAHLIAN</h2>
            <h3>Konsentrasi Unggulan<br>SMK Negeri 7 Batam</h3>
            <div class="program-card">
                <div class="program-title">Rencana Aksi Program SMK Pusat Keunggulan</div>
                <div class="program-subtitle">SMK Negeri 7 Batam, SMK Pusat Keunggulan</div>
                <ul class="program-list">
                    <li>Mengembangkan kerjasama dengan DUDIKA</li>
                    <li>Memiliki kelas industri untuk semua konsentrasi keahlian</li>
                    <li>Memiliki Lembaga Sertifikasi Profesi</li>
                </ul>
            </div>
        </div>
    </section>

    <!-- News Section -->
    <section class="news" id="berita">
        <div class="container">
            <h2>SMK NEGERI 7 BATAM</h2>
            <h3>Berita Terbaru</h3>
            <button class="news-button">Selengkapnya</button>
        </div>
    </section>

    <!-- CTA Section -->
    <section class="cta">
        <div class="container">
            <h2>Ayo Bergabung di</h2>
            <h3>SMK Negeri 7 Batam</h3>
        </div>
    </section>

    <!-- Footer -->
    <footer id="kontak">
        <div class="container">
            <div class="footer-grid">
                <div class="footer-section">
                    <h4>Ikuti Kami</h4>
                    <div class="social-links">
                        <a href="#" class="social-link">📘</a>
                        <a href="#" class="social-link">📷</a>
                    </div>
                </div>
                <div class="footer-section">
                    <h4>Navigasi</h4>
                    <ul>
                        <li><a href="#home">Home</a></li>
                        <li><a href="#kontak">Kontak</a></li>
                    </ul>
                </div>
                <div class="footer-section">
                    <h4>Tautan Penting</h4>
                    <ul>
                        <li><a href="#">Disdik Kota Batam</a></li>
                        <li><a href="#">Disdik Provinsi Kepri</a></li>
                        <li><a href="#">Dapodik SMK Negeri 7 Batam</a></li>
                        <li><a href="#">Peta Lokasi SMK Negeri 7 Batam</a></li>
                    </ul>
                </div>
                <div class="footer-section">
                    <h4>Tentang Kami</h4>
                    <p style="color: #ccc; font-size: 0.9rem; line-height: 1.6;">
                        Perumahan Sekawan Pemko,<br>
                        Kelurahan Belian, Kec. Batam Kota,<br>
                        Kota Batam, Prov. Kepulauan Riau<br>
                        Kode Pos : 29463<br><br>
                        <strong style="color: #FFD700;"><a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="07746a6c69626062756e30656673666a47606a666e6b2964686a">[email&#160;protected]</a></strong>
                    </p>
                </div>
            </div>
            <div class="copyright">
                <p>@2024 Hak Cipta, SMK NEGERI 7 BATAM</p>
            </div>
        </div>
    </footer>

    <script data-cfasync="false" src="/cdn-cgi/scripts/5c5dd728/cloudflare-static/email-decode.min.js"></script><script>
        function showTab(tabName) {
            // Hide all tab panes
            const panes = document.querySelectorAll('.tab-pane');
            panes.forEach(pane => pane.classList.remove('active'));
            
            // Remove active class from all buttons
            const buttons = document.querySelectorAll('.tab-button');
            buttons.forEach(button => button.classList.remove('active'));
            
            // Show selected tab pane
            document.getElementById(tabName).classList.add('active');
            
            // Add active class to clicked button
            event.target.classList.add('active');
        }

        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Counter animation for statistics
        function animateCounters() {
            const counters = document.querySelectorAll('.stat-number');
            const targets = [85, 36, 8, 1200];
            
            counters.forEach((counter, index) => {
                const target = targets[index];
                const duration = 2000;
                const steps = 60;
                const increment = target / steps;
                let current = 0;
                
                const timer = setInterval(() => {
                    current += increment;
                    if (current >= target;
                    counter.textContent = Math.floor(current);
                }, duration / steps);
            });
        }

        // Trigger counter animation when stats section is visible
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    animateCounters();
                    observer.unobserve(entry.target);
                }
            });
        });

        observer.observe(document.querySelector('.stats'));
    </script>
</body>
</html>
