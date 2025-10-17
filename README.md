DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ardimas Yonifandria Putra - Network & System Specialist</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <meta name="description" content="Ardimas Yonifandria Putra - Alumni SMKN 1 Pacitan TKJ | Mikrotik | Linux Server | Fiber Optics">
    <style>
        :root {
            --bg-primary: #0f0f23;
            --bg-secondary: #1a1a2e;
            --glass-bg: rgba(255, 255, 255, 0.08);
            --glass-border: rgba(255, 255, 255, 0.15);
            --text-primary: #ffffff;
            --text-secondary: #a0a0a0;
            --accent-primary: #00d9ff;
            --accent-secondary: #5a67d8;
            --gradient-primary: linear-gradient(135deg, #0c0c1e 0%, #1a1a2e 50%, #2d3748 100%);
            --gradient-accent: linear-gradient(45deg, #00d9ff, #5a67d8, #48bb78);
            --shadow-neon: 0 0 25px rgba(0, 217, 255, 0.3);
            --shadow-glow: 0 8px 32px rgba(0, 217, 255, 0.1);
        }

        [data-theme="light"] {
            --bg-primary: #f7fafc;
            --bg-secondary: #edf2f7;
            --glass-bg: rgba(255, 255, 255, 0.9);
            --glass-border: rgba(0, 0, 0, 0.08);
            --text-primary: #2d3748;
            --text-secondary: #718096;
            --accent-primary: #3182ce;
            --accent-secondary: #805ad5;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', sans-serif;
            line-height: 1.7;
            color: var(--text-primary);
            background: var(--bg-primary);
            overflow-x: hidden;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        .glass {
            background: var(--glass-bg);
            backdrop-filter: blur(20px);
            border: 1px solid var(--glass-border);
            border-radius: 16px;
            box-shadow: var(--shadow-glow);
        }

        /* Header */
        .header {
            position: fixed;
            top: 0;
            width: 100%;
            background: var(--glass-bg);
            backdrop-filter: blur(20px);
            z-index: 1000;
            padding: 1rem 0;
        }

        .nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .nav-brand {
            font-size: 1.8rem;
            font-weight: 800;
            background: var(--gradient-accent);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .nav-menu {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        .nav-link {
            color: var(--text-primary);
            text-decoration: none;
            font-weight: 500;
            padding: 0.5rem 1rem;
            border-radius: 8px;
            transition: all 0.3s ease;
        }

        .nav-link:hover, .nav-link.active {
            color: var(--accent-primary);
            background: var(--glass-bg);
            box-shadow: var(--shadow-neon);
        }

        .theme-toggle {
            background: var(--glass-bg);
            border: 1px solid var(--glass-border);
            color: var(--text-primary);
            padding: 0.5rem;
            border-radius: 50%;
            cursor: pointer;
        }

        .hamburger {
            display: none;
            flex-direction: column;
            gap: 4px;
            cursor: pointer;
        }

        .hamburger span {
            width: 25px;
            height: 3px;
            background: var(--text-primary);
            transition: 0.3s;
        }

        /* Hero */
        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            background: var(--gradient-primary);
            padding-top: 80px;
        }

        .hero-content {
            text-align: center;
        }

        .hero-title {
            font-size: 3.5rem;
            font-weight: 800;
            background: var(--gradient-accent);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-bottom: 1rem;
        }

        .hero-subtitle {
            font-size: 1.3rem;
            color: var(--text-secondary);
            margin-bottom: 1.5rem;
        }

        .school-badge {
            background: var(--glass-bg);
            padding: 1rem 2rem;
            border-radius: 50px;
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            font-weight: 600;
            margin: 2rem 0;
            box-shadow: var(--shadow-glow);
        }

        .cta-button {
            background: var(--gradient-accent);
            color: white;
            border: none;
            padding: 15px 30px;
            font-size: 1.1rem;
            border-radius: 50px;
            cursor: pointer;
            font-weight: 600;
            transition: all 0.3s ease;
            box-shadow: var(--shadow-neon);
        }

        .cta-button:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 30px rgba(0, 217, 255, 0.4);
        }

        /* Sections */
        section {
            padding: 100px 0;
        }

        .section-title {
            font-size: 2.5rem;
            text-align: center;
            margin-bottom: 3rem;
            font-weight: 700;
            background: var(--gradient-accent);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        /* About */
        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
            align-items: start;
        }

        .about-text {
            background: var(--glass-bg);
            padding: 2rem;
            border-radius: 16px;
        }

        .about-highlight {
            background: linear-gradient(135deg, var(--accent-primary), var(--accent-secondary));
            color: white;
            padding: 1.5rem;
            border-radius: 12px;
            margin: 1.5rem 0;
            font-weight: 600;
        }

        .profile-image {
            width: 300px;
            height: 300px;
            border-radius: 50%;
            background: var(--gradient-accent);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 4rem;
            margin: 0 auto;
            box-shadow: var(--shadow-neon);
        }

        /* Skills - LONG LIST */
        .skills-section {
            background: var(--bg-secondary);
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 2rem;
        }

        .skill-category {
            background: var(--glass-bg);
            padding: 2rem;
            border-radius: 16px;
            border-left: 4px solid var(--accent-primary);
        }

        .skill-category h3 {
            color: var(--accent-primary);
            margin-bottom: 1.5rem;
            font-size: 1.5rem;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .skill-list {
            list-style: none;
        }

        .skill-list li {
            padding: 0.8rem 0;
            padding-left: 2rem;
            position: relative;
            color: var(--text-secondary);
            border-bottom: 1px solid var(--glass-border);
            transition: all 0.3s ease;
        }

        .skill-list li:hover {
            color: var(--text-primary);
            padding-left: 2.5rem;
            background: rgba(0, 217, 255, 0.05);
        }

        .skill-list li::before {
            content: "▸";
            position: absolute;
            left: 0;
            color: var(--accent-primary);
            font-weight: bold;
            font-size: 1.2rem;
        }

        /* Experience */
        .experience-card {
            background: var(--glass-bg);
            padding: 2rem;
            border-radius: 16px;
            margin-bottom: 2rem;
            border-top: 4px solid var(--accent-secondary);
        }

        /* Contact */
        .contact-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 1rem;
            padding: 1.5rem;
            background: var(--glass-bg);
            border-radius: 12px;
            margin-bottom: 1rem;
            transition: all 0.3s ease;
        }

        .contact-item:hover {
            transform: translateX(10px);
            box-shadow: var(--shadow-neon);
        }

        .contact-icon {
            width: 50px;
            height: 50px;
            background: var(--gradient-accent);
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 1.2rem;
        }

        .social-icons {
            display: flex;
            gap: 1rem;
            justify-content: center;
            margin-top: 2rem;
        }

        .social-icon {
            width: 55px;
            height: 55px;
            background: var(--glass-bg);
            border: 2px solid var(--glass-border);
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--text-primary);
            text-decoration: none;
            transition: all 0.3s ease;
        }

        .social-icon:hover {
            background: var(--accent-primary);
            color: white;
            border-color: var(--accent-primary);
            transform: translateY(-3px);
            box-shadow: var(--shadow-neon);
        }

        .form-control {
            width: 100%;
            padding: 1rem;
            background: var(--glass-bg);
            border: 1px solid var(--glass-border);
            border-radius: 8px;
            color: var(--text-primary);
            margin-bottom: 1rem;
        }

        /* Footer */
        .footer {
            background: var(--bg-secondary);
            padding: 2rem 0;
            text-align: center;
            border-top: 1px solid var(--glass-border);
        }

        /* Animations */
        .fade-in {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.6s ease;
        }

        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }

        /* Responsive */
        @media (max-width: 768px) {
            .hamburger { display: flex; }
            .nav-menu {
                display: none;
                position: absolute;
                top: 100%;
                left: 0;
                width: 100%;
                background: var(--glass-bg);
                flex-direction: column;
                padding: 1rem;
            }
            .nav-menu.active { display: flex; }
            .hero-title { font-size: 2.5rem; }
            .about-content, .contact-content { grid-template-columns: 1fr; }
        }
    </style>
</head>
<body>
    <header class="header glass">
        <nav class="nav container">
            <div class="nav-brand">Ardimas YP</div>
            <ul class="nav-menu">
                <li><a href="#home" class="nav-link">Home</a></li>
                <li><a href="#about" class="nav-link">About</a></li>
                <li><a href="#skills" class="nav-link">Skills</a></li>
                <li><a href="#experience" class="nav-link">Experience</a></li>
                <li><a href="#contact" class="nav-link">Contact</a></li>
            </ul>
            <div class="theme-toggle" onclick="toggleTheme()">
                <i class="fas fa-moon"></i>
            </div>
            <div class="hamburger">
                <span></span><span></span><span></span>
            </div>
        </nav>
    </header>

    <section id="home" class="hero">
        <div class="container">
            <div class="hero-content fade-in">
                <h1 class="hero-title">Ardimas Yonifandria Putra</h1>
                <p class="hero-subtitle">Alumni SMKN 1 Pacitan TKJ</p>
                <div class="school-badge glass">
                    <i class="fas fa-graduation-cap"></i>
                    Teknik Komputer dan Jaringan
                </div>
                <button class="cta-button" onclick="scrollToSection('about')">
                    Lihat Skills <i class="fas fa-arrow-down"></i>
                </button>
            </div>
        </div>
    </section>

    <section id="about" class="about">
        <div class="container">
            <h2 class="section-title fade-in">Tentang Saya</h2>
            <div class="about-content">
                <div class="about-text glass fade-in">
                    <p>Alumni <strong>SMKN 1 Pacitan</strong> jurusan <strong>TKJ</strong> dengan fokus pada networking dan system administration.</p>
                    <div class="about-highlight">
                        <i class="fas fa-network-wired"></i>
                        Memiliki ketertarikan khusus di bidang <strong>Fiber Optik</strong> dan teknologi jaringan serat optik
                    </div>
                    <p>Suka mengkonfigurasi server dan networking equipment untuk solusi yang reliable dan efisien.</p>
                </div>
                <div class="profile-image fade-in">
                    <i class="fas fa-user-tie"></i>
                </div>
            </div>
        </div>
    </section>

    <section id="skills" class="skills-section">
        <div class="container">
            <h2 class="section-title fade-in">Keahlian Dasar</h2>
            <div class="skills-grid">
                <div class="skill-category fade-in">
                    <h3><i class="fas fa-router"></i> Konfigurasi Mikrotik</h3>
                    <ul class="skill-list">
                        <li>Basic RouterOS Configuration</li>
                        <li>Interface & Bridge Setup</li>
                        <li>IP Addressing & DHCP Server</li>
                        <li>NAT & Firewall Rules</li>
                        <li>Static & Dynamic Routing</li>
                        <li>Bandwidth Management</li>
                        <li>Hotspot Configuration</li>
                        <li>PPPoE Server/Client</li>
                        <li>Wireless Access Points</li>
                        <li>Troubleshooting Tools</li>
                    </ul>
                </div>

                <div class="skill-category fade-in">
                    <h3><i class="fab fa-linux"></i> Konfigurasi Linux</h3>
                    <ul class="skill-list">
                        <li>OpenSSH Server Configuration</li>
                        <li>User & Permission Management</li>
                        <li>Apache2 Web Server Installation</li>
                        <li>Virtual Host Configuration</li>
                        <li>CasaOS Installation & Management</li>
                        <li>Telnet Server Configuration</li>
                        <li>Mail Server (Postfix/Dovecot)</li>
                        <li>DNS Server (BIND) Setup</li>
                        <li>System Monitoring Tools</li>
                        <li>Log Management & Analysis</li>
                    </ul>
                </div>

                <div class="skill-category fade-in">
                    <h3><i class="fas fa-satellite-dish"></i> Fiber Optik & Networking</h3>
                    <ul class="skill-list">
                        <li>Fiber Optic Cable Testing</li>
                        <li>OTDR Analysis & Interpretation</li>
                        <li>Fiber Splicing Techniques</li>
                        <li>FTTH Network Deployment</li>
                        <li>GPON Technology Basics</li>
                        <li>Fiber Connector Cleaning</li>
                        <li>Power Meter Testing</li>
                        <li>LAN/WAN Infrastructure</li>
                        <li>Network Troubleshooting</li>
                        <li>Switch & Router Configuration</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <section id="experience" class="experience">
        <div class="container">
            <h2 class="section-title fade-in">Pengalaman Kerja</h2>
            <div class="experience-card glass fade-in">
                <h3><i class="fas fa-briefcase"></i> PKL - PT Lentera Digital Nusantara</h3>
                <p><strong>Posisi:</strong> Helper Network Technician</p>
                <p><em>Praktik Kerja Lapangan</em></p>
                <p>Bekerja sebagai helper dalam tim networking, mendukung instalasi, konfigurasi, dan maintenance infrastruktur jaringan perusahaan telekomunikasi.</p>
                <ul class="skill-list" style="margin-top: 1rem;">
                    <li>Assistance konfigurasi networking equipment</li>
                    <li>Testing dan troubleshooting jaringan</li>
                    <li>Dokumentasi teknis proyek</li>
                    <li>Support tim teknis lapangan</li>
                    <li>Monitoring performa jaringan</li>
                </ul>
            </div>
        </div>
    </section>

    <section id="contact" class="contact">
        <div class="container">
            <h2 class="section-title fade-in">Kontak</h2>
            <div class="contact-content">
                <div class="contact-info fade-in">
                    <div class="contact-item glass">
                        <div class="contact-icon">
                            <i class="fas fa-envelope"></i>
                        </div>
                        <div>
                            <h4>Email</h4>
                            <p>anotherardimas@gmail.com</p>
                        </div>
                    </div>
                    <div class="contact-item glass">
                        <div class="contact-icon">
                            <i class="fab fa-instagram"></i>
                        </div>
                        <div>
                            <h4>Instagram</h4>
                            <p>@another_ardimas</p>
                        </div>
                    </div>
                    <div class="contact-item glass">
                        <div class="contact-icon">
                            <i class="fas fa-blog"></i>
                        </div>
                        <div>
                            <h4>Blog</h4>
                            <p>ardimasyoni.blogspot.com</p>
                        </div>
                    </div>
                    <div class="social-icons">
                        <a href="https://instagram.com/another_ardimas" target="_blank" class="social-icon">
                            <i class="fab fa-instagram"></i>
                        </a>
                        <a href="https://ardimasyoni.blogspot.com" target="_blank" class="social-icon">
                            <i class="fas fa-blog"></i>
                        </a>
                        <a href="mailto:anotherardimas@gmail.com" class="social-icon">
                            <i class="fas fa-envelope"></i>
                        </a>
                    </div>
                </div>
                <form class="contact-form glass fade-in">
                    <input type="text" class="form-control" placeholder="Nama Anda" required>
                    <input type="email" class="form-control" placeholder="Email Anda" required>
                    <textarea class="form-control" rows="5" placeholder="Pesan Anda..." required></textarea>
                    <button type="submit" class="cta-button">Kirim Pesan</button>
                </form>
            </div>
        </div>
    </section>

    <footer class="footer">
        <div class="container">
            <p>&copy; 2025 Ardimas Yonifandria Putra. Network & System Specialist.</p>
        </div>
    </footer>

    <script>
        // Theme Toggle
        function toggleTheme() {
            const body = document.body;
            const isDark = body.getAttribute('data-theme') !== 'light';
            body.setAttribute('data-theme', isDark ? 'light' : 'dark');
            localStorage.setItem('theme', isDark ? 'light' : 'dark');
            document.querySelector('.theme-toggle i').className = isDark ? 'fas fa-sun' : 'fas fa-moon';
        }

        // Load theme
        const savedTheme = localStorage.getItem('theme') || 'dark';
        document.body.setAttribute('data-theme', savedTheme);
        document.querySelector('.theme-toggle i').className = savedTheme === 'dark' ? 'fas fa-sun' : 'fas fa-moon';

        // Mobile nav
        document.querySelector('.hamburger').addEventListener('click', () => {
            document.querySelector('.nav-menu').classList.toggle('active');
        });

        // Smooth scroll
        function scrollToSection(id) {
            document.getElementById(id).scrollIntoView({ behavior: 'smooth' });
        }

        document.querySelectorAll('a[href^="#"]').forEach(link => {
            link.addEventListener('click', e => {
                e.preventDefault();
                const target = document.querySelector(link.getAttribute('href'));
                target?.scrollIntoView({ behavior: 'smooth' });
                document.querySelector('.nav-menu')?.classList.remove('active');
            });
        });

        // Fade in
        const observer = new IntersectionObserver(entries => {
            entries.forEach(entry => {
                if (entry.isIntersecting) entry.target.classList.add('visible');
            });
        }, { threshold: 0.1 });

        document.querySelectorAll('.fade-in').forEach(el => observer.observe(el));

        // Form
        document.querySelector('.contact-form').addEventListener('submit', e => {
            e.preventDefault();
            alert('Pesan terkirim! Saya akan balas secepatnya.');
            e.target.reset();
        });
    </script>
</body>
</html>
