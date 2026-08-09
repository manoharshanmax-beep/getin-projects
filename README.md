<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="International Conference on Sustainable Business, Innovation & Global Competitiveness (ICSBIGC–2026)">
    <title>ICSBIGC–2026 | International Conference on Sustainable Business, Innovation & Global Competitiveness</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="styles.css">
    <style>
        <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="International Conference on Sustainable Business, Innovation & Global Competitiveness (ICSBIGC–2026)">
    <title>ICSBIGC–2026 | International Conference on Sustainable Business, Innovation & Global Competitiveness</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="styles.css">
        <style>/* ============================================================
   ICSBIGC-2026 | Optimized Responsive Stylesheet
   Fully adapted for all screen sizes (mobile, tablet, laptop, desktop)
   ============================================================ */

/* ===== RESET & BASE ===== */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

:root {
    --navy: #0b2a4a;
    --navy-dark: #071c33;
    --emerald: #0e9f6e;
    --emerald-dark: #0a7d57;
    --text: #2b3a4a;
    --muted: #5a6b7c;
    --bg: #f4f7fb;
    --white: #ffffff;
    --border: #e3e9f0;
    --shadow: 0 8px 24px rgba(11, 42, 74, 0.10);
    --shadow-lg: 0 12px 32px rgba(11, 42, 74, 0.16);
    --radius: 16px;
}

html {
    scroll-behavior: smooth;
    -webkit-text-size-adjust: 100%;
}

body {
    font-family: 'Inter', Arial, sans-serif;
    color: var(--text);
    background-color: var(--bg);
    line-height: 1.6;
    -webkit-font-smoothing: antialiased;
    overflow-x: hidden;
}

img {
    max-width: 100%;
    height: auto;
    display: block;
}

.container {
    width: 100%;
    max-width: 1700px;
    margin: 0 auto;
    padding: 0 24px;
}

/* ===== NAVBAR ===== */
.navbar {
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
    background-color: #222;
    padding: 10px 20px;
    gap: 10px;
}

.logo,
.logo2 {
    width: 100px;
    height: 100px;
    object-fit: cover;
    border-radius: 50%;
    flex-shrink: 0;
    transition: transform 0.3s ease;
}

.logo:hover,
.logo2:hover {
    transform: scale(1.1);
}

.conference-name {
    flex: 1;
    text-align: center;
    font-size: 22px;
    font-weight: bold;
    color: #fff;
    margin: 0;
    min-width: 160px;
}

.marquee {
    flex-basis: 100%;
    overflow: hidden;
    white-space: nowrap;
    margin-top: 10px;
    border-top: 1px solid rgba(255, 255, 255, 0.15);
    padding-top: 6px;
}

.marquee-content {
    display: inline-block;
    animation: marquee 15s linear infinite;
}

.marquee-content span {
    display: inline-block;
    padding-right: 50px;
    color: #ffd700;
    font-size: 16px;
}

@keyframes marquee {
    0%   { transform: translateX(0); }
    100% { transform: translateX(-50%); }
}

/* ===== HERO ===== */
.hero {
    position: relative;
    background: linear-gradient(135deg, var(--navy-dark) 0%, var(--navy) 60%, var(--emerald) 140%);
    color: var(--white);
    text-align: center;
    padding: 7rem 0 6rem;
    overflow: hidden;
}

.hero-overlay {
    position: absolute;
    inset: 0;
    background-image: radial-gradient(circle at 20% 30%, rgba(14, 159, 110, 0.18), transparent 45%),
                      radial-gradient(circle at 80% 70%, rgba(255, 255, 255, 0.08), transparent 45%);
    pointer-events: none;
}

.hero-content {
    position: relative;
    z-index: 1;
}

.conference-name {
    font-size: 1rem;
    font-weight: 500;
    letter-spacing: 3px;
    text-transform: uppercase;
    color: rgba(255, 255, 255, 0.8);
    margin-bottom: 1rem;
}

.hero-title {
    font-size: 2.6rem;
    font-weight: 800;
    line-height: 1.2;
    margin: 0 auto 0.5rem;
    max-width: 900px;
}

.hero-acronym {
    font-size: 1.3rem;
    font-weight: 600;
    color: var(--emerald);
    letter-spacing: 2px;
    margin-bottom: 1.8rem;
}

.tagline {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 0.2rem 0.6rem;
    font-size: 1.15rem;
    font-weight: 500;
    margin-bottom: 2.2rem;
}

.tagline .dot {
    color: var(--emerald);
    font-weight: 700;
}

.hero-meta {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 1rem;
}

.badge {
    background: rgba(255, 255, 255, 0.12);
    border: 1px solid rgba(255, 255, 255, 0.25);
    padding: 0.6rem 1.4rem;
    border-radius: 50px;
    font-size: 0.95rem;
    font-weight: 500;
    backdrop-filter: blur(4px);
}

/* ===== BUTTONS ===== */
.btn-register {
    display: inline-block;
    background: var(--emerald);
    color: var(--white);
    font-weight: 700;
    font-size: 1.05rem;
    text-decoration: none;
    padding: 0.9rem 2.4rem;
    border-radius: 50px;
    box-shadow: 0 8px 20px rgba(14, 159, 110, 0.35);
    transition: transform 0.2s ease, box-shadow 0.2s ease, background 0.2s ease;
    cursor: pointer;
    border: none;
}

.btn-register:hover {
    background: var(--emerald-dark);
    transform: translateY(-2px) scale(1.02);
    box-shadow: 0 12px 26px rgba(14, 159, 110, 0.45);
}

/* ===== SECTIONS & CARDS ===== */
.section {
    padding: 3.5rem 0;
}

.section + .section {
    padding-top: 0;
}

.card {
    background: var(--white);
    border-radius: var(--radius);
    box-shadow: var(--shadow);
    padding: 2.2rem 2.4rem;
    border-top: 4px solid var(--emerald);
}

.card-header {
    margin-bottom: 1.4rem;
}

.card-header h2 {
    font-size: 1.6rem;
    font-weight: 700;
    color: var(--navy);
}

.underline {
    width: 56px;
    height: 4px;
    background: var(--emerald);
    border-radius: 4px;
    margin-top: 0.5rem;
}

/* ===== ABOUT ===== */
.about-grid {
    display: grid;
    grid-template-columns: 1.2fr 1fr;
    gap: 2rem;
    align-items: start;
}

.about-text p {
    margin-bottom: 1rem;
    color: var(--muted);
}

.about-text strong,
.organisers strong {
    color: var(--navy);
}

.organisers {
    background: var(--bg);
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 1.6rem;
}

.organisers h3 {
    color: var(--emerald-dark);
    font-size: 0.85rem;
    letter-spacing: 1.5px;
    text-transform: uppercase;
    margin-bottom: 0.7rem;
}

.org-name {
    font-size: 1.15rem;
    font-weight: 700;
    color: var(--navy);
    margin-bottom: 0.4rem;
}

.org-college,
.org-city {
    color: var(--muted);
}

.accreditation {
    display: inline-block;
    margin-top: 1rem;
    background: linear-gradient(135deg, var(--emerald), var(--emerald-dark));
    color: var(--white);
    font-weight: 600;
    font-size: 0.85rem;
    padding: 0.4rem 1rem;
    border-radius: 50px;
}

/* ===== CHIEF GUESTS ===== */
.chief {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 1.6rem;
    padding: 20px;
    max-width: 1700px;
    margin: 20px auto;
}

.guest {
    background: var(--white);
    border: 5px solid var(--bg);
    border-radius: 20px;
    padding: 1.5rem;
    text-align: center;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease, box-shadow 0.3s ease, background 0.3s ease, color 0.3s ease;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.guest:hover {
    background-color: var(--emerald);
    color: #ffffff;
    transform: scale(1.03);
    box-shadow: 0 0 20px rgba(0, 255, 255, 0.4);
}

.guest:hover p,
.guest:hover h3 {
    color: #ffffff;
}

.guest h3 {
    font-size: 20px;
    font-weight: bold;
    margin: 10px 0;
    color: #333;
    text-transform: uppercase;
}

.guest p {
    font-size: 14px;
    line-height: 1.5;
    color: #555;
    margin: 8px 0;
}

.guest-image {
    width: 200px;
    height: 200px;
    object-fit: cover;
    border-radius: 50%;
    margin-bottom: 15px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}

.guest-button a button {
    background: linear-gradient(135deg, #4caf50, #2e7d32);
    color: #fff;
    font-size: 14px;
    font-weight: bold;
    padding: 10px 20px;
    border: none;
    border-radius: 25px;
    cursor: pointer;
    transition: all 0.3s ease;
    position: relative;
    overflow: hidden;
}

.guest-button a button:hover {
    background: linear-gradient(135deg, #66bb6a, #388e3c);
    transform: scale(1.05);
    box-shadow: 0 6px 14px rgba(0, 0, 0, 0.3);
}

.guest-button a button::after {
    content: "";
    position: absolute;
    background: rgba(255, 255, 255, 0.4);
    border-radius: 50%;
    width: 100px;
    height: 100px;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%) scale(0);
    opacity: 0;
    transition: transform 0.5s ease, opacity 0.8s ease;
}

.guest-button a button:hover::after {
    transform: translate(-50%, -50%) scale(2);
    opacity: 1;
}

/* ===== FEE TABLE ===== */
.fee-table-wrap {
    overflow-x: auto;
}

.fee-table {
    width: 100%;
    border-collapse: collapse;
    max-width: 620px;
}

.fee-table thead th {
    background: var(--navy);
    color: var(--white);
    text-align: left;
    padding: 0.9rem 1.4rem;
    font-weight: 600;
    font-size: 0.95rem;
}

.fee-table thead th:last-child {
    text-align: center;
}

.fee-table tbody td {
    padding: 0.9rem 1.4rem;
    border-bottom: 1px solid var(--border);
}

.fee-table tbody td:last-child {
    text-align: center;
    font-weight: 700;
    color: var(--emerald-dark);
}

.fee-table tbody tr:nth-child(even) {
    background: var(--bg);
}

.fee-table tbody tr:last-child td {
    border-bottom: none;
}

.note {
    margin-top: 1.2rem;
    font-size: 0.9rem;
    color: var(--muted);
    font-style: italic;
}

/* ===== TIMELINE ===== */
.timeline {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 1.4rem;
}

.timeline-item {
    background: var(--bg);
    border: 1px solid var(--border);
    border-left: 4px solid var(--emerald);
    border-radius: 12px;
    padding: 1.3rem 1.4rem;
}

.tl-date {
    display: block;
    font-size: 1.3rem;
    font-weight: 800;
    color: var(--emerald-dark);
    margin-bottom: 0.3rem;
}

.tl-label {
    font-weight: 500;
    color: var(--navy);
}

/* ===== CTA ===== */
.cta-section {
    padding-top: 0.5rem;
}

.cta-card {
    background: linear-gradient(135deg, var(--navy-dark), var(--navy));
    color: var(--white);
    text-align: center;
    border-radius: var(--radius);
    box-shadow: var(--shadow-lg);
    padding: 3rem 2rem;
}

.cta-card h2 {
    font-size: 1.7rem;
    margin-bottom: 0.6rem;
}

.cta-card p {
    color: rgba(255, 255, 255, 0.85);
    margin-bottom: 1.8rem;
    max-width: 520px;
    margin-left: auto;
    margin-right: auto;
}

/* ===== CONTACT ===== */
.contact-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 1.4rem;
}

.contact-item {
    text-align: center;
    background: var(--bg);
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 1.6rem 1rem;
}

.contact-item h4 {
    color: var(--navy);
    margin-bottom: 0.4rem;
}

.contact-icon {
    font-size: 1.8rem;
    display: block;
    margin-bottom: 0.5rem;
}

.contact-value {
    font-weight: 600;
    color: var(--navy);
    word-break: break-word;
}

/* ===== FOOTER ===== */
.footer {
    background: var(--navy-dark);
    color: rgba(255, 255, 255, 0.75);
    text-align: center;
    padding: 3rem 0 2rem;
    margin-top: 2rem;
}

.footer-org {
    font-weight: 600;
    color: var(--white);
    margin-bottom: 0.8rem;
}

.footer-invite {
    margin-bottom: 1.2rem;
}

.footer-invite strong,
.footer-copy {
    color: var(--emerald);
    font-weight: 600;
}

.footer-copy {
    font-size: 0.85rem;
    margin-top: 1.2rem;
    color: rgba(255, 255, 255, 0.55);
}

/* ============================================================
   RESPONSIVE BREAKPOINTS
   ============================================================ */

/* Tablets & small laptops (768px and below) */
@media (max-width: 768px) {
    .navbar {
        flex-direction: column;
        align-items: center;
        text-align: center;
    }

    .logo,
    .logo2 {
        width: 70px;
        height: 70px;
        margin: 5px 0;
    }

    .conference-name {
        font-size: 18px;
        margin: 10px 0;
    }

    .marquee-content span {
        font-size: 14px;
    }

    .hero {
        padding: 5rem 0 4rem;
    }

    .hero-title {
        font-size: 1.9rem;
    }

    .hero-acronym {
        font-size: 1.1rem;
    }

    .tagline {
        font-size: 1rem;
    }

    .about-grid {
        grid-template-columns: 1fr;
        gap: 1.5rem;
    }

    .card {
        padding: 1.8rem 1.4rem;
    }

    .cta-card h2 {
        font-size: 1.4rem;
    }

    .chief {
        grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
        padding: 12px;
    }
}

/* Mobile portrait (480px and below) */
@media (max-width: 480px) {
    .container {
        padding: 0 16px;
    }

    .hero {
        padding: 4rem 0 3rem;
    }

    .hero-title {
        font-size: 1.6rem;
    }

    .hero-acronym {
        font-size: 1rem;
    }

    .badge {
        padding: 0.5rem 1rem;
        font-size: 0.85rem;
    }

    .logo,
    .logo2 {
        width: 60px;
        height: 60px;
    }

    .conference-name {
        font-size: 16px;
    }

    .card {
        padding: 1.5rem 1.1rem;
    }

    .card-header h2 {
        font-size: 1.3rem;
    }

    .cta-card {
        padding: 2rem 1.2rem;
    }

    .cta-card h2 {
        font-size: 1.3rem;
    }

    .btn-register {
        padding: 0.8rem 1.8rem;
        font-size: 0.95rem;
    }

    .guest-image {
        width: 150px;
        height: 150px;
    }

    .guest h3 {
        font-size: 17px;
    }

    .guest p {
        font-size: 13px;
    }

    .fee-table thead th,
    .fee-table tbody td {
        padding: 0.7rem 1rem;
    }
}

/* Very large desktop screens (1600px and above) */
@media (min-width: 1600px) {
    .hero-title {
        font-size: 3rem;
    }

    .container,
    .chief {
        max-width: 1800px;
    }
}

/* ===== REDUCED MOTION (accessibility) ===== */
@media (prefers-reduced-motion: reduce) {
    * {
        animation-duration: 0.001ms !important;
        animation-iteration-count: 1 !important;
        transition-duration: 0.001ms !important;
        scroll-behavior: auto !important;
    }
}
</style>
</head>
<body>
  
       
  
  <div class="navbar">
  <img src="SRNM LOGO.jpeg" alt="Logo" class="logo">
  <p class="conference-name">Sri S. Ramasamy Naidu Memorial College,sattur</p>
  <img src="srnm.png" alt="Logo" class="logo2">

  <div class="marquee">
    <div class="marquee-content">
        
      <span>அன்பு, அறிவு, தொண்டு - Love, Knowledge, Service</span>
      <span>அன்பு, அறிவு, தொண்டு - Love, Knowledge, Service</span>
    </div>
  </div>
</div>



              
            
     

     
    </ul>
    
    </div>    
</div>


    <!-- HERO SECTION -->
    <header class="hero" id="home">
        <div class="hero-overlay"></div>
        <div class="container hero-content">
            
            <p class="conference-name">International Conference on</p>
            <h1 class="hero-title">Sustainable Business, Innovation &amp; Global Competitiveness</h1>
            <p class="hero-acronym">(ICSBIGC–2026)</p>
            <div class="tagline">
                <span>Present</span>
                <span class="dot">•</span>
                <span>Publish</span>
                <span class="dot">•</span>
                <span>Connect</span>
                <span class="dot">•</span>
                <span>Grow</span>
            </div>
            <div class="hero-meta">
                <span class="badge">📅 25 August 2026</span>
                <span class="badge">🌐 Hybrid Mode</span>
                 <div class="container">
            
                <h2>Ready to be a part of ICSBIGC–2026?</h2><br> <br>
            
                <a href="https://forms.gle/SjU58Aezp9YNaehK8" target="_blank" rel="noopener" class="btn-register">Register Now</a>
            
            </div>
        </div>
    </header>

    <!-- ORGANISER / ABOUT -->
    <section class="section" id="about">
        <div class="container">
            <div class="card">
                <div class="card-header">
                    <h2>About ICSBIGC–2026</h2>
                    <div class="underline"></div>
                </div>
                <div class="about-grid">
                    <div class="about-text">
                        <p>
The International Conference on Sustainable Business, Innovation & Global Competitiveness (ICSBIGC–2026) is a platform for academicians, researchers, industry experts, policymakers, entrepreneurs, and students to share knowledge, present research, and discuss new ideas in business.
The conference focuses on sustainable business, innovation, technology, and global competitiveness. It aims to promote quality research, innovation, collaboration, and sustainable development.
<br>
<b>Publication</b><br>
Selected research papers will be considered for publication in peer-reviewed journals and conference proceedings.
All accepted papers will be published in the conference proceedings with ISBN. Selected high-quality papers may also be published in peer-reviewed journals with ISSN, subject to the review process.</p>
<p><b>About the Department</b><br>The Department of Commerce (Computer Application), established in 1997–1998, is
dedicated to delivering quality commerce education integrated with contemporary
computer applications. With a student strength of over 300, the department fosters
academic excellence through an industry-oriented curriculum, experienced faculty,
technology-enabled learning, and outcome-based education. Regular seminars,
workshops, guest lectures, industrial visits, and skill enhancement programmes provide
students with practical exposure and professional competencies, preparing them for
successful careers, higher education, and entrepreneurial pursuits in the evolving global
business environment.</p>
                    </div>
                    <div class="organisers">
                        <h3>Organiser</h3>
                        <p class="org-name">Department of Commerce (CA)</p>
                        <p class="org-college">Sri S. Ramasamy Naidu Memorial College,</p>
                        <p class="org-city">Sattur, Tamil Nadu, India</p>
                        <div class="accreditation">NAAC A++ Accredited</div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CHIEF GUESTS -->

    <div class="chief">
        <div class="guest">
            <img src="Screenshot 2026-08-09 113142.png" alt="Chief Guest" class="guest-image">
            <h3>Dr M.I.M. RIYATH</h3>


            <p>Senior Lecturer, Department of Accountancy & Finance, Faculty of Management & Commerce, South Eastern University of Sri Lanka, University Park, Oluvil, Sri Lanka.</p>
             <div class="guest-button">
                <a href="https://scholar.google.com/citations?hl=en&user=KsAwhLIAAAAJ"><button>Google Scholar</button> </a>
              </div>
        </div>
         <div class="guest">
             <img src="Screenshot 2026-08-09 113154.png" alt="Chief Guest" class="guest-image">
            <h3>Dr V.MUTHUKUMAR.</h3>
            <p >

Assistant Professor Department of Commerce, Madras Christian College, Tambaram, Chennai, Tamil Nadu, India.</p>
 <div class="guest-button">
                <a href="https://scholar.google.com/citations?hl=en&user=KsAwhLIAAAAJ"><button>Google Scholar</button> </a>
              </div>
         </div>
          <div class="guest">
             <img src="Screenshot 2026-08-09 113203.png" alt="Chief Guest" class="guest-image">
            <h3>Mr M.FARWIS</h3>
            <p >Chief Guest</p>

Assistant Professor


            <p >PG & Research Department of Commerce, Pasumpon Muthuramalinga Thevar College, Melaneelithanallur, Sankarankovil, Tamil Nadu,</p>
             <div class="guest-button">
                <a href="https://scholar.google.com/citations?hl=en&user=KsAwhLIAAAAJ"><button>Google Scholar</button> </a>
              </div>
          </div>

           <div class="guest">
             <img src="Screenshot 2026-08-09 113212.png" alt="Chief Guest" class="guest-image">
            
              <h3>Dr S.JEYAKUMAR</h3>
             

Assistant Professor


            <p >PG & Research Department of Commerce, Pasumpon Muthuramalinga Thevar College, Melaneelithanallur, Sankarankovil, Tamil Nadu,</p>
             <div class="guest-button">
                <a href="https://scholar.google.com/citations?hl=en&user=KsAwhLIAAAAJ"><button>Google Scholar</button> </a>
              </div>
          </div>
           </div>
           
    </div>

    <!-- PUBLICATION NOTE -->
    <section class="section" id="publication">
        <div class="container">
            <div class="card">
                <div class="card-header">
                    <h2>Publication Note</h2>
                    <div class="underline"></div>
                </div>
                <p>Selected high‑quality research papers will be published in an ISSN‑registered journal (soft copy) with a nominal publication fee of approximately ₹500..</p>
            </div>
        </div>
    </section>

    <!-- REGISTRATION FEE -->
    <section class="section" id="registration">
        <div class="container">
            <div class="card">
                <div class="card-header">
                    <h2>Registration Fee</h2>
                    <div class="underline"></div>
                </div>
                <div class="fee-table-wrap">
                    <table class="fee-table">
                        <thead>
                            <tr>
                                <th>Category</th>
                                <th>Fee (INR)</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                                <td>UG / PG Students</td>
                                <td>₹150</td>
                            </tr>
                            <tr>
                                <td>Research Scholars</td>
                                <td>₹200</td>
                            </tr>
                            <tr>
                                <td>Academicians</td>
                                <td>₹300</td>
                            </tr>
                            <tr>
                                <td>Industry Experts</td>
                                <td>₹400</td>
                            </tr>
                        </tbody>
                    </table>
                </div>
                <p class="note">Registration includes conference kit, participation certificate and conference materials.</p>
            </div>
        </div>
    </section>

    <!-- IMPORTANT DATES -->
    <section class="section" id="dates">
        <div class="container">
            <div class="card">
                <div class="card-header">
                    <h2>Important Dates</h2>
                    <div class="underline"></div>
                </div>
                <div class="timeline">
                    <div class="timeline-item">
                        <span class="tl-date">14 Aug</span>
                        <span class="tl-label">Abstract Submission</span>
                    </div>
                    <div class="timeline-item">
                        <span class="tl-date">21 Aug</span>
                        <span class="tl-label">Full Paper Submission</span>
                    </div>
                    <div class="timeline-item">
                        <span class="tl-date">23 Aug</span>
                        <span class="tl-label">Registration Deadline(Participation only)</span>
                    </div>
                    <div class="timeline-item">
                        <span class="tl-date">25 Aug</span>
                        <span class="tl-label">Conference Date</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- REGISTER CTA -->
    <section class="section cta-section" id="register">
        <div class="container">
            <div class="cta-card">
                <h2>Ready to be a part of ICSBIGC–2026?</h2>
                <p>Register now to present your research and connect with a global community.</p>
                <a href="https://forms.gle/SjU58Aezp9YNaehK8" target="_blank" rel="noopener" class="btn-register">Register Now</a>
            </div>
        </div>
    </section>

    <!-- CONTACT -->
    <section class="section" id="contact">
        <div class="container">
            <div class="card">
                <div class="card-header">
                    <h2>Conference Queries</h2>
                    <div class="underline"></div>
                </div>
                <div class="contact-grid">
                    <div class="contact-item"><br>
                        <span class="contact-icon">📧</span>
                        <p class="contact-value">srnmcconference2026@gmail.com</p>
                    </div>
                    <div class="contact-item"><br>
                        <span class="contact-icon">📞</span>
                        <h4>Dr V.Sundarraj <br>(Convener) </h4>
                        <p class="contact-value">+91 9790397452</p>
                    </div>
                    <div class="contact-item"><br>
                        <span class="contact-icon">📞</span>
                        <h4>Dr M.Maharaja<br> (Organising Secretary) </h4>
                        <p class="contact-value">+91 9952270359</p>
                    </div>
                     <div class="contact-item">
                        <p><b>For Enquiry in Hindi<b></p>
                        <span class="contact-icon">📞</span>
                        <h4>Mr B.Manohar<br>(Student Coordinator)</h4>
                        <p class="contact-value">+91 9626750414</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
   

    <!-- FOOTER -->
    <footer class="footer">
        <div class="container footer-inner">
             <p class="footer-org">Department of Commerce (CA)</p>
            <p class="footer-org">Sri S. Ramasamy Naidu Memorial College,<br>Sattur, Tamil Nadu, India</p>
            <p class="footer-invite">We cordially invite you to join us at <strong>ICSBIGC–2026</strong>.</p>
            <p class="footer-copy">© 2026 Department of Commerce (CA) · SRNM College · All Rights Reserved</p>
        </div>
    </footer>

</body>
</html>


    </style>
</head>
<body>
  
       
  
  <div class="navbar">
  <img src="SRNM LOGO.jpeg" alt="Logo" class="logo">
  <p class="conference-name">Sri S. Ramasamy Naidu Memorial College,sattur</p>
  <img src="srnm.png" alt="Logo" class="logo2">

  <div class="marquee">
    <div class="marquee-content">
        
      <span>அன்பு, அறிவு, தொண்டு - Love, Knowledge, Service</span>
      <span>அன்பு, அறிவு, தொண்டு - Love, Knowledge, Service</span>
    </div>
  </div>
</div>



              
            
     

     
    </ul>
    
    </div>    
</div>


    <!-- HERO SECTION -->
    <header class="hero" id="home">
        <div class="hero-overlay"></div>
        <div class="container hero-content">
            
            <p class="conference-name">International Conference on</p>
            <h1 class="hero-title">Sustainable Business, Innovation &amp; Global Competitiveness</h1>
            <p class="hero-acronym">(ICSBIGC–2026)</p>
            <div class="tagline">
                <span>Present</span>
                <span class="dot">•</span>
                <span>Publish</span>
                <span class="dot">•</span>
                <span>Connect</span>
                <span class="dot">•</span>
                <span>Grow</span>
            </div>
            <div class="hero-meta">
                <span class="badge">📅 25 August 2026</span>
                <span class="badge">🌐 Hybrid Mode</span>
                 <div class="container">
            
                <h2>Ready to be a part of ICSBIGC–2026?</h2><br> <br>
            
                <a href="https://forms.gle/SjU58Aezp9YNaehK8" target="_blank" rel="noopener" class="btn-register">Register Now</a>
            
            </div>
        </div>
    </header>

    <!-- ORGANISER / ABOUT -->
    <section class="section" id="about">
        <div class="container">
            <div class="card">
                <div class="card-header">
                    <h2>About ICSBIGC–2026</h2>
                    <div class="underline"></div>
                </div>
                <div class="about-grid">
                    <div class="about-text">
                        <p>
The International Conference on Sustainable Business, Innovation & Global Competitiveness (ICSBIGC–2026) is a platform for academicians, researchers, industry experts, policymakers, entrepreneurs, and students to share knowledge, present research, and discuss new ideas in business.
The conference focuses on sustainable business, innovation, technology, and global competitiveness. It aims to promote quality research, innovation, collaboration, and sustainable development.
<br>
<b>Publication</b><br>
Selected research papers will be considered for publication in peer-reviewed journals and conference proceedings.
All accepted papers will be published in the conference proceedings with ISBN. Selected high-quality papers may also be published in peer-reviewed journals with ISSN, subject to the review process.</p>
<p><b>About the Department</b><br>The Department of Commerce (Computer Application), established in 1997–1998, is
dedicated to delivering quality commerce education integrated with contemporary
computer applications. With a student strength of over 300, the department fosters
academic excellence through an industry-oriented curriculum, experienced faculty,
technology-enabled learning, and outcome-based education. Regular seminars,
workshops, guest lectures, industrial visits, and skill enhancement programmes provide
students with practical exposure and professional competencies, preparing them for
successful careers, higher education, and entrepreneurial pursuits in the evolving global
business environment.</p>
                    </div>
                    <div class="organisers">
                        <h3>Organiser</h3>
                        <p class="org-name">Department of Commerce (CA)</p>
                        <p class="org-college">Sri S. Ramasamy Naidu Memorial College,</p>
                        <p class="org-city">Sattur, Tamil Nadu, India</p>
                        <div class="accreditation">NAAC A++ Accredited</div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CHIEF GUESTS -->

    <div class="chief">
        <div class="guest">
            <img src="Screenshot 2026-08-09 113142.png" alt="Chief Guest" class="guest-image">
            <h3>Dr M.I.M. RIYATH</h3>


            <p>Senior Lecturer, Department of Accountancy & Finance, Faculty of Management & Commerce, South Eastern University of Sri Lanka, University Park, Oluvil, Sri Lanka.</p>
             <div class="guest-button">
                <a href="https://scholar.google.com/citations?hl=en&user=KsAwhLIAAAAJ"><button>Google Scholar</button> </a>
              </div>
        </div>
         <div class="guest">
             <img src="Screenshot 2026-08-09 113154.png" alt="Chief Guest" class="guest-image">
            <h3>Dr V.MUTHUKUMAR.</h3>
            <p >

Assistant Professor Department of Commerce, Madras Christian College, Tambaram, Chennai, Tamil Nadu, India.</p>
 <div class="guest-button">
                <a href="https://scholar.google.com/citations?hl=en&user=KsAwhLIAAAAJ"><button>Google Scholar</button> </a>
              </div>
         </div>
          <div class="guest">
             <img src="Screenshot 2026-08-09 113203.png" alt="Chief Guest" class="guest-image">
            <h3>Mr M.FARWIS</h3>
            <p >Chief Guest</p>

Assistant Professor


            <p >PG & Research Department of Commerce, Pasumpon Muthuramalinga Thevar College, Melaneelithanallur, Sankarankovil, Tamil Nadu,</p>
             <div class="guest-button">
                <a href="https://scholar.google.com/citations?hl=en&user=KsAwhLIAAAAJ"><button>Google Scholar</button> </a>
              </div>
          </div>

           <div class="guest">
             <img src="Screenshot 2026-08-09 113212.png" alt="Chief Guest" class="guest-image">
            
              <h3>Dr S.JEYAKUMAR</h3>
             

Assistant Professor


            <p >PG & Research Department of Commerce, Pasumpon Muthuramalinga Thevar College, Melaneelithanallur, Sankarankovil, Tamil Nadu,</p>
             <div class="guest-button">
                <a href="https://scholar.google.com/citations?hl=en&user=KsAwhLIAAAAJ"><button>Google Scholar</button> </a>
              </div>
          </div>
           </div>
           
    </div>

    <!-- PUBLICATION NOTE -->
    <section class="section" id="publication">
        <div class="container">
            <div class="card">
                <div class="card-header">
                    <h2>Publication Note</h2>
                    <div class="underline"></div>
                </div>
                <p>Selected high‑quality research papers will be published in an ISSN‑registered journal (soft copy) with a nominal publication fee of approximately ₹500..</p>
            </div>
        </div>
    </section>

    <!-- REGISTRATION FEE -->
    <section class="section" id="registration">
        <div class="container">
            <div class="card">
                <div class="card-header">
                    <h2>Registration Fee</h2>
                    <div class="underline"></div>
                </div>
                <div class="fee-table-wrap">
                    <table class="fee-table">
                        <thead>
                            <tr>
                                <th>Category</th>
                                <th>Fee (INR)</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                                <td>UG / PG Students</td>
                                <td>₹150</td>
                            </tr>
                            <tr>
                                <td>Research Scholars</td>
                                <td>₹200</td>
                            </tr>
                            <tr>
                                <td>Academicians</td>
                                <td>₹300</td>
                            </tr>
                            <tr>
                                <td>Industry Experts</td>
                                <td>₹400</td>
                            </tr>
                        </tbody>
                    </table>
                </div>
                <p class="note">Registration includes conference kit, participation certificate and conference materials.</p>
            </div>
        </div>
    </section>

    <!-- IMPORTANT DATES -->
    <section class="section" id="dates">
        <div class="container">
            <div class="card">
                <div class="card-header">
                    <h2>Important Dates</h2>
                    <div class="underline"></div>
                </div>
                <div class="timeline">
                    <div class="timeline-item">
                        <span class="tl-date">14 Aug</span>
                        <span class="tl-label">Abstract Submission</span>
                    </div>
                    <div class="timeline-item">
                        <span class="tl-date">21 Aug</span>
                        <span class="tl-label">Full Paper Submission</span>
                    </div>
                    <div class="timeline-item">
                        <span class="tl-date">23 Aug</span>
                        <span class="tl-label">Registration Deadline(Participation only)</span>
                    </div>
                    <div class="timeline-item">
                        <span class="tl-date">25 Aug</span>
                        <span class="tl-label">Conference Date</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- REGISTER CTA -->
    <section class="section cta-section" id="register">
        <div class="container">
            <div class="cta-card">
                <h2>Ready to be a part of ICSBIGC–2026?</h2>
                <p>Register now to present your research and connect with a global community.</p>
                <a href="https://forms.gle/SjU58Aezp9YNaehK8" target="_blank" rel="noopener" class="btn-register">Register Now</a>
            </div>
        </div>
    </section>

    <!-- CONTACT -->
    <section class="section" id="contact">
        <div class="container">
            <div class="card">
                <div class="card-header">
                    <h2>Conference Queries</h2>
                    <div class="underline"></div>
                </div>
                <div class="contact-grid">
                    <div class="contact-item"><br>
                        <span class="contact-icon">📧</span>
                        <p class="contact-value">srnmcconference2026@gmail.com</p>
                    </div>
                    <div class="contact-item"><br>
                        <span class="contact-icon">📞</span>
                        <h4>Dr V.Sundarraj <br>(Convener) </h4>
                        <p class="contact-value">+91 9790397452</p>
                    </div>
                    <div class="contact-item"><br>
                        <span class="contact-icon">📞</span>
                        <h4>Dr M.Maharaja<br> (Organising Secretary) </h4>
                        <p class="contact-value">+91 9952270359</p>
                    </div>
                     <div class="contact-item">
                        <p><b>For Enquiry in Hindi<b></p>
                        <span class="contact-icon">📞</span>
                        <h4>Mr B.Manohar<br>(Student Coordinator)</h4>
                        <p class="contact-value">+91 9626750414</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
   

    <!-- FOOTER -->
    <footer class="footer">
        <div class="container footer-inner">
             <p class="footer-org">Department of Commerce (CA)</p>
            <p class="footer-org">Sri S. Ramasamy Naidu Memorial College,<br>Sattur, Tamil Nadu, India</p>
            <p class="footer-invite">We cordially invite you to join us at <strong>ICSBIGC–2026</strong>.</p>
            <p class="footer-copy">© 2026 Department of Commerce (CA) · SRNM College · All Rights Reserved</p>
        </div>
    </footer>

</body>
</html>

