<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portofolio - Rafiqi Althaf Ramadhan</title>
    <link rel="stylesheet" href="style.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</head>
<body>
  <style type="text/css" media="all">/* Gaya Umum & Reset */
:root {
    --bg-color: #1a1a2e;
    --text-color: #e0e0e0;
    --accent-color: #007bff; /* Biru cerah */
    --card-bg: #222535;
    --card-border: #333647;
    --heading-color: #ffffff;
    --font-primary: 'Poppins', sans-serif;
}

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

html {
    scroll-behavior: smooth;
}

body {
    background-color: var(--bg-color);
    color: var(--text-color);
    font-family: var(--font-primary);
    line-height: 1.6;
}

h1, h2, h3 {
    font-weight: 600;
    color: lightblue;
}

a {
    color: var(--accent-color);
    text-decoration: none;
    transition: color 0.3s ease;
}

a:hover {
    color: #4da6ff; /* Warna aksen yang sedikit lebih terang saat hover */
}

.section {
    padding: 80px 5%;
    max-width: 1200px;
    margin: auto;
}

.section-title {
    text-align: center;
    font-size: 2.5rem;
    margin-bottom: 40px;
    position: relative;
    padding-bottom: 10px;
}

.section-title::after {
    content: '';
    position: absolute;
    bottom: 0;
    left: 50%;
    transform: translateX(-50%);
    width: 60px;
    height: 3px;
    background-color: var(--accent-color);
}

/* Navbar */
.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 5%;
    background-color: var(--bg-color);
    position: sticky;
    top: 0;
    z-index: 1000;
}

.logo {
    font-size: 1.8rem;
    font-weight: 700;
    color: var(--accent-color);
}

.nav-links a {
    margin-left: 20px;
    font-size: 1rem;
    font-weight: 600;
    color: var(--text-color);
    transition: color 0.3s ease;
}

.nav-links a:hover {
    color: var(--accent-color);
}

/* Hero Section */
.hero-section {
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 85vh;
    text-align: center;
    padding: 0 5%;
    background-image: linear-gradient(rgba(26, 26, 46, 0.8), rgba(26, 26, 46, 0.8)), url('https://images.unsplash.com/photo-1510519138101-570d1d17d544?q=80&w=2670&auto=format&fit=crop'); /* Contoh gambar background, bisa diganti */
    background-position: center;
    background-size: cover;
}

.hero-content {
    max-width: 800px;
}

.hero-content h1 {
    font-size: 3.5rem;
    margin-bottom: 10px;
    line-height: 1.2;
}

.tagline {
    font-size: 1.5rem;
    font-weight: 400;
    color: #b3b3b3;
    margin-bottom: 20px;
}

.intro-text {
    font-size: 1.1rem;
    margin-bottom: 30px;
}

.hero-actions {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 15px;
}

/* Buttons */
.btn {
    padding: 12px 25px;
    border-radius: 5px;
    font-weight: 600;
    transition: transform 0.3s ease, background-color 0.3s ease;
    display: inline-block;
    text-transform: uppercase;
}

.btn-primary {
    background-color: var(--accent-color);
    color: var(--heading-color);
    border: 2px solid var(--accent-color);
}

.btn-primary:hover {
    background-color: transparent;
    transform: translateY(-3px);
}

.btn-secondary {
    background-color: transparent;
    color: var(--accent-color);
    border: 2px solid var(--accent-color);
}

.btn-secondary:hover {
    background-color: var(--accent-color);
    color: var(--heading-color);
}

.social-icon {
    font-size: 1.8rem;
    color: var(--text-color);
    transition: color 0.3s ease, transform 0.3s ease;
}

.social-icon:hover {
    color: var(--accent-color);
    transform: scale(1.1);
}

/* Skill Section */
.skills-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 30px;
}

.skill-group {
    background-color: var(--card-bg);
    border: 1px solid var(--card-border);
    border-radius: 10px;
    padding: 30px;
    flex: 1;
    min-width: 250px;
    max-width: 350px;
    text-align: center;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.skill-group:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
}

.skill-group h3 {
    font-size: 1.4rem;
    margin-bottom: 20px;
}

.skill-group ul {
    list-style: none;
    padding: 0;
}

.skill-group li {
    background-color: #333647;
    padding: 8px 15px;
    border-radius: 20px;
    margin: 8px 0;
    display: inline-block;
}

/* Project Section */
.projects-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 30px;
}

.project-card {
    background-color: var(--card-bg);
    border: 1px solid var(--card-border);
    border-radius: 10px;
    overflow: hidden;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.project-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 15px 30px rgba(0, 0, 0, 0.3);
}

.project-img {
    width: 100%;
    height: 200px;
    object-fit: cover;
    display: block;
}

.project-info {
    padding: 20px;
}

.project-info h3 {
    font-size: 1.5rem;
    margin-bottom: 10px;
}

.project-desc {
    font-size: 0.95rem;
    margin-bottom: 15px;
}

.project-tech {
    font-style: italic;
    color: #999;
    margin-bottom: 20px;
}

.project-actions {
    display: flex;
    gap: 10px;
}

/* Contact Section */
.contact-content {
    max-width: 600px;
    margin: auto;
    text-align: center;
}

.contact-email-text {
    font-size: 1.2rem;
    margin-bottom: 20px;
}

.contact-email-link {
    font-weight: bold;
}

.contact-form {
    display: flex;
    flex-direction: column;
    gap: 20px;
    text-align: left;
}

.form-group {
    display: flex;
    flex-direction: column;
}

.form-group label {
    font-weight: 600;
    margin-bottom: 8px;
}

.form-group input,
.form-group textarea {
    padding: 12px;
    border: 1px solid var(--card-border);
    background-color: var(--card-bg);
    color: var(--text-color);
    border-radius: 5px;
    font-family: var(--font-primary);
}

.form-group input:focus,
.form-group textarea:focus {
    outline: none;
    border-color: var(--accent-color);
}

.contact-form .btn-primary {
    align-self: flex-start;
    border-color: var(--accent-color);
}

/* Footer */
.footer {
    text-align: center;
    padding: 30px 5%;
    background-color: #111122;
    border-top: 1px solid #2a2a3e;
}

.footer-social-links {
    margin-top: 15px;
}

.footer-social-links .social-icon {
    margin: 0 10px;
}

/* Responsiveness */
@media (max-width: 768px) {
    .navbar {
        flex-direction: column;
        text-align: center;
    }

    .logo {
        margin-bottom: 15px;
    }

    .nav-links a {
        margin: 0 10px;
    }

    .hero-content h1 {
        font-size: 2.5rem;
    }

    .tagline {
        font-size: 1.2rem;
    }

    .hero-actions {
        flex-direction: column;
        gap: 20px;
    }
    
    .projects-grid {
        grid-template-columns: 1fr;
    }

    .contact-form .btn-primary {
        align-self: center;
    }
}

h1 {
  color: lightblue;
}
    
  </style>

    <header class="navbar">
        <div class="logo">RAR</div>
        <nav class="nav-links">
            <a href="#about">Tentang Saya</a>
            <a href="#skills">Skill</a>
            <a href="#projects">Proyek</a>
            <a href="#contact">Kontak</a>
        </nav>
    </header>

    <main>
        <section class="hero-section">
            <div class="hero-content">
                <h1>Rafiqi Althaf Ramadhan</h1>
                <p class="tagline">Calon Web Developer </p>
                <p class="intro-text">Seorang Pelajar Jurusan PPLG di SMK Negeri 1 Ciomas</p>
                <div class="hero-actions">
                    <a href="#projects" class="btn btn-primary">Lihat Proyek Saya</a>
                    <a href="https://www.facebook.com/share/16AoNmWN21/" target="_blank" class="social-icon" aria-label="Facebook"><i class="fab fa-facebook"></i></a>
                    <a href="https://www.instagram.com/ukpdll?igsh=MXhoeGIyc3dqcXQ1bg==" target="_blank" aria-label="Instagram"><i class="fab fa-instagram"></i></a>
                </div>
            </div>
        </section>

        <section id="about" class="section">
            <h2 class="section-title">Tentang Saya</h2>
            <div class="about-content">
                <p> Saya adalah seorang pelajar di SMK Negeri 1 Ciomas. Saat ini saya duduk di bangku kelas X PPLG 1. Saya mempunyai minat dan ketertarikan di dunia teknologi. Saya ingin terus mengasah kemampuan di bidang ini untuk menjadi Web Developer Profesional
                </p>
            </div>
        </section>

        <section id="skills" class="section">
            <h2 class="section-title">Skill</h2>
            <div class="skills-container">
                <div class="skill-group">
                    <h3><i class="fas fa-code"></i> Bahasa Pemrograman</h3>
                    <ul>
                        <li>HTML</li>
                        <li>CSS</li>
                        <li>Java Script</li>
                        <li>...</li>
                    </ul>
                </div>
                <div class="skill-group">
                    <h3><i class="fas fa-cubes"></i> Framework/Library</h3>
                    <ul>
                        <li>React.js</li>
                        <li>Laravel</li>
                        <li>Node.js</li>
                        <li>...</li>
                    </ul>
                </div>
                <div class="skill-group">
                    <h3><i class="fas fa-tools"></i> Tools</h3>
                    <ul>
                        <li>Git</li>
                        <li>Docker</li>
                        <li>Figma</li>
                        <li>...</li>
                    </ul>
                </div>
            </div>
        </section>

        <section id="projects" class="section">
            <h2 class="section-title">Proyek</h2>
            <div class="projects-grid">
                <div class="project-card">
                  


                <div class="project-card">
                
                    <div class="project-info">
                        <h3>Form Peminjaman iPhone</h3>
                        <p class="project-desc">Aplikasi web untuk mengelola daftar dan riwayat peminjaman iPhone.</p>
                        <p class="project-tech"><strong>HTML:</strong>CSS</p>
                        <div class="project-actions">
                            <a href="#" class="btn btn-secondary">Live Demo</a>
                            <a href="#" class="btn btn-secondary">Lihat Kode</a>
                        </div>
                    </div>
                </div>
                
                <div class="project-card">
                  
                    <div class="project-info">
                        <h3>Coming Soon</h3>
                        
  
                        <div class="project-actions">
                            <a href="#" class="btn btn-secondary">Live Demo</a>
                            <a href="#" class="btn btn-secondary">Lihat Kode</a>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section id="contact" class="section">
            <h2 class="section-title">Kontak</h2>
            <div class="contact-content">
                <p class="contact-email-text">Hubungi saya melalui email di: <a href="mailto:rafiqialthaf8@gmail.com" class="contact-email-link">rafiqialthaf8@gmail.com</a></p>
                <form class="contact-form">
                    <div class="form-group">
                        <label for="name">Nama</label>
                        <input type="text" id="name" name="name" required>
                    </div>
                    <div class="form-group">
                        <label for="email">Email</label>
                        <input type="email" id="email" name="email" required>
                    </div>
                    <div class="form-group">
                        <label for="message">Pesan</label>
                        <textarea id="message" name="message" rows="5" required></textarea>
                    </div>
                    <button type="submit" class="btn btn-primary">Kirim Pesan</button>
                </form>
            </div>
        </section>
    </main>

    <footer class="footer">
        <p>&copy; 2025 Rafiqi Althaf Ramadhan.</p>
        <div class="footer-social-links">
            <a href="https://github.com/yourusername" target="_blank" class="social-icon" aria-label="GitHub"><i class="fab fa-github"></i></a>
            <a href="https://linkedin.com/in/yourusername" target="_blank" class="social-icon" aria-label="LinkedIn"><i class="fab fa-linkedin"></i></a>
        </div>
    </footer>
    
</body>
</html>
