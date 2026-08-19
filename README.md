<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sacred Haven | Sanctuary of Peace</title>
    <!-- Classic Serif & Elegant Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@400;600;700&family=Sorts+Mill+Goudy:ital@0;1&display=swap" rel="stylesheet">
    
    <style>
        /* CSS RESET & VARIABLES */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --gold-primary: #d4af37;
            --gold-light: #f3e5ab;
            --navy-deep: #0b1325;
            --navy-light: #18233c;
            --cream-bg: #fdfbf7;
            --text-dark: #2c2825;
            --text-muted: #665f57;
            --border-gold: rgba(212, 175, 55, 0.4);
        }

        body {
            font-family: 'Sorts Mill Goudy', serif;
            background-color: var(--cream-bg);
            color: var(--text-dark);
            line-height: 1.8;
            overflow-x: hidden;
        }

        h1, h2, h3, h4, .sacred-font {
            font-family: 'Cinzel', serif;
            letter-spacing: 1px;
        }

        /* HEADER & NAVIGATION */
        header {
            background-color: var(--navy-deep);
            color: var(--gold-light);
            border-bottom: 3px solid var(--gold-primary);
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
        }

        nav {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1.2rem 2rem;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 12px;
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--gold-primary);
            text-transform: uppercase;
        }

        .logo-emblem {
            font-size: 2rem;
            line-height: 1;
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        .nav-links a {
            color: var(--gold-light);
            text-decoration: none;
            font-family: 'Cinzel', serif;
            font-size: 0.95rem;
            text-transform: uppercase;
            transition: color 0.3s ease;
        }

        .nav-links a:hover {
            color: var(--gold-primary);
        }

        /* HERO SECTION */
        .hero {
            background: linear-gradient(rgba(11, 19, 37, 0.75), rgba(11, 19, 37, 0.85)),
                        url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="100" height="100" viewBox="0 0 100 100"><path d="M50 0 L100 50 L50 100 L0 50 Z" fill="none" stroke="rgba(212, 175, 55, 0.05)" stroke-width="1"/></svg>');
            background-color: var(--navy-deep);
            color: var(--cream-bg);
            text-align: center;
            padding: 6rem 2rem;
            position: relative;
        }

        .hero-content {
            max-width: 800px;
            margin: 0 auto;
        }

        .hero-symbol {
            font-size: 3rem;
            color: var(--gold-primary);
            margin-bottom: 1rem;
        }

        .hero h1 {
            font-size: 2.8rem;
            color: var(--gold-primary);
            margin-bottom: 1rem;
            text-shadow: 0 2px 4px rgba(0,0,0,0.5);
        }

        .hero p {
            font-size: 1.25rem;
            margin-bottom: 2rem;
            font-style: italic;
        }

        /* SACRED BORDER FRAME */
        .ornate-border {
            border: 2px solid var(--gold-primary);
            outline: 1px solid var(--gold-primary);
            outline-offset: 5px;
            padding: 2.5rem;
            margin: 2rem 0;
            background: rgba(255, 255, 255, 0.02);
            position: relative;
        }

        /* DAILY VERSE / QUOTE BOX */
        .daily-quote-section {
            max-width: 900px;
            margin: -3rem auto 4rem;
            position: relative;
            z-index: 10;
            padding: 0 1.5rem;
        }

        .quote-card {
            background: var(--cream-bg);
            border: 1px solid var(--border-gold);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            padding: 2.5rem;
            text-align: center;
            border-radius: 4px;
        }

        .quote-card h3 {
            color: var(--navy-deep);
            font-size: 1.1rem;
            text-transform: uppercase;
            margin-bottom: 1rem;
            letter-spacing: 2px;
        }

        .quote-text {
            font-size: 1.3rem;
            font-style: italic;
            color: var(--text-dark);
            margin-bottom: 1rem;
            min-height: 80px;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .quote-source {
            font-family: 'Cinzel', serif;
            font-weight: 600;
            color: var(--gold-primary);
        }

        .btn-gold {
            background-color: var(--gold-primary);
            color: var(--navy-deep);
            border: none;
            padding: 0.75rem 1.8rem;
            font-family: 'Cinzel', serif;
            font-weight: 700;
            text-transform: uppercase;
            cursor: pointer;
            transition: all 0.3s ease;
            margin-top: 1rem;
        }

        .btn-gold:hover {
            background-color: var(--gold-light);
            box-shadow: 0 0 15px rgba(212, 175, 55, 0.4);
        }

        /* MAIN CONTENT & SERVICES */
        .main-content {
            max-width: 1100px;
            margin: 0 auto;
            padding: 2rem 1.5rem;
        }

        .section-title {
            text-align: center;
            margin-bottom: 3rem;
        }

        .section-title h2 {
            font-size: 2.2rem;
            color: var(--navy-deep);
        }

        .divider {
            height: 2px;
            width: 120px;
            background: linear-gradient(to right, transparent, var(--gold-primary), transparent);
            margin: 0.75rem auto;
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-bottom: 4rem;
        }

        .service-card {
            background-color: #ffffff;
            border: 1px solid #e8e2d5;
            padding: 2rem;
            text-align: center;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .service-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px rgba(0,0,0,0.08);
            border-color: var(--gold-primary);
        }

        .service-icon {
            font-size: 2.5rem;
            color: var(--gold-primary);
            margin-bottom: 1rem;
        }

        .service-card h3 {
            color: var(--navy-deep);
            margin-bottom: 0.75rem;
        }

        /* PRAYER REQUEST SECTION */
        .prayer-section {
            background-color: var(--navy-light);
            color: var(--cream-bg);
            padding: 4rem 2rem;
            margin-top: 4rem;
        }

        .prayer-container {
            max-width: 650px;
            margin: 0 auto;
        }

        .prayer-section h2 {
            color: var(--gold-primary);
            text-align: center;
        }

        .prayer-form {
            display: flex;
            flex-direction: column;
            gap: 1.2rem;
            margin-top: 2rem;
        }

        .form-group input, 
        .form-group textarea {
            width: 100%;
            padding: 1rem;
            background: rgba(255, 255, 255, 0.05);
            border: 1px solid var(--border-gold);
            color: #ffffff;
            font-family: 'Sorts Mill Goudy', serif;
            font-size: 1rem;
        }

        .form-group input::placeholder, 
        .form-group textarea::placeholder {
            color: #a0aab8;
        }

        .form-group input:focus, 
        .form-group textarea:focus {
            outline: none;
            border-color: var(--gold-primary);
            background: rgba(255, 255, 255, 0.1);
        }

        /* FOOTER */
        footer {
            background-color: var(--navy-deep);
            color: var(--gold-light);
            text-align: center;
            padding: 3rem 1rem 1.5rem;
            border-top: 1px solid var(--border-gold);
        }

        .footer-symbol {
            font-size: 2rem;
            color: var(--gold-primary);
            margin-bottom: 1rem;
        }

        .footer-links {
            margin: 1.5rem 0;
        }

        .footer-links a {
            color: var(--gold-light);
            margin: 0 1rem;
            text-decoration: none;
            font-size: 0.9rem;
        }

        .copyright {
            font-size: 0.85rem;
            color: #7a8a9e;
            margin-top: 1.5rem;
        }

        /* RESPONSIVE DESIGN */
        @media (max-width: 768px) {
            .nav-links { display: none; } /* Simplified for single page snippet */
            .hero h1 { font-size: 2rem; }
            .hero p { font-size: 1rem; }
            .ornate-border { padding: 1.5rem; }
        }
    </style>
</head>
<body>

    <!-- NAVIGATION -->
    <header>
        <nav>
            <div class="logo">
                <span class="logo-emblem">✙</span>
                <span>Sacred Haven</span>
            </div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#teachings">Teachings</a></li>
                <li><a href="#sanctuary">Sanctuary</a></li>
                <li><a href="#intentions">Intentions</a></li>
            </ul>
        </nav>
    </header>

    <!-- HERO SECTION -->
    <section class="hero" id="home">
        <div class="hero-content">
            <div class="ornate-border">
                <div class="hero-symbol">✦</div>
                <h1>Welcome to the Sanctuary</h1>
                <p>"Where stillness meets the divine, and peace resides within the heart."</p>
                <a href="#intentions" style="text-decoration: none;">
                    <button class="btn-gold">Submit an Intention</button>
                </a>
            </div>
        </div>
    </section>

    <!-- DAILY SCRIPTURE / QUOTE WIDGET (JAVASCRIPT POWERED) -->
    <section class="daily-quote-section">
        <div class="quote-card">
            <h3>— Daily Reflection —</h3>
            <div class="quote-text" id="quoteText">
                "Loading sacred wisdom..."
            </div>
            <div class="quote-source" id="quoteSource"></div>
            <button class="btn-gold" style="padding: 0.4rem 1rem; font-size: 0.8rem;" onclick="cycleQuote()">New Reflection</button>
        </div>
    </section>

    <!-- MAIN SERVICES / PILLARS -->
    <main class="main-content" id="teachings">
        <div class="section-title">
            <h2>Pillars of Faith & Peace</h2>
            <div class="divider"></div>
        </div>

        <div class="services-grid">
            <div class="service-card">
                <div class="service-icon">📖</div>
                <h3>Sacred Words</h3>
                <p>Explore ancient wisdom and teachings designed to guide your daily journey and bring quiet reflection to your soul.</p>
            </div>

            <div class="service-card">
                <div class="service-icon">🕊️</div>
                <h3>Inner Peace</h3>
                <p>Join our guided meditation gatherings focused on stillness, reflection, and deepening your connection to the divine.</p>
            </div>

            <div class="service-card">
                <div class="service-icon">🤝</div>
                <h3>Fellowship</h3>
                <p>Connect with a compassionate community bound together by love, charity, and mutual spiritual support.</p>
            </div>
        </div>
    </main>

    <!-- PRAYER / INTENTION FORM SECTION -->
    <section class="prayer-section" id="intentions">
        <div class="prayer-container">
            <h2>Offer a Prayer or Intention</h2>
            <div class="divider"></div>
            <p style="text-align: center; margin-top: 1rem; color: var(--gold-light);">
                Leave your prayer requests or sacred intentions below. Our community keeps all requests in quiet reflection.
            </p>

            <form class="prayer-form" id="prayerForm">
                <div class="form-group">
                    <input type="text" id="nameInput" placeholder="Your Name (Optional)" />
                </div>
                <div class="form-group">
                    <textarea id="prayerInput" rows="4" placeholder="Write your prayer or reflection here..." required></textarea>
                </div>
                <button type="submit" class="btn-gold" style="width: 100%;">Send Intention</button>
            </form>
            <div id="formResponse" style="text-align: center; margin-top: 1rem; color: var(--gold-primary); font-style: italic;"></div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer>
        <div class="footer-symbol">☥</div>
        <p class="sacred-font">Sacred Haven Sanctuary</p>
        <div class="footer-links">
            <a href="#home">Home</a> | 
            <a href="#teachings">Teachings</a> | 
            <a href="#intentions">Prayers</a>
        </div>
        <p class="copyright">&copy; 2026 Sacred Haven. All rights reserved. Walk in light.</p>
    </footer>

    <!-- JAVASCRIPT -->
    <script>
        // Sacred Reflections Data
        const sacredWisdom = [
            {
                text: "The light shines in the darkness, and the darkness has not overcome it.",
                source: "— John 1:5"
            },
            {
                text: "Peace comes from within. Do not seek it without.",
                source: "— Buddha"
            },
            {
                text: "Be still, and know that stillness carries the answers you seek.",
                source: "— Psalm 46:10"
            },
            {
                text: "Love is patient, love is kind. It does not envy, it does not boast.",
                source: "— 1 Corinthians 13:4"
            },
            {
                text: "When you do things from your soul, you feel a river moving in you, a joy.",
                source: "— Rumi"
            }
        ];

        let currentIndex = 0;

        // Function to update the reflection box
        function displayQuote(index) {
            const quoteTextEl = document.getElementById('quoteText');
            const quoteSourceEl = document.getElementById('quoteSource');
            
            // Subtle fade effect
            quoteTextEl.style.opacity = 0;
            quoteSourceEl.style.opacity = 0;

            setTimeout(() => {
                quoteTextEl.textContent = `"${sacredWisdom[index].text}"`;
                quoteSourceEl.textContent = sacredWisdom[index].source;
                quoteTextEl.style.transition = 'opacity 0.5s ease';
                quoteSourceEl.style.transition = 'opacity 0.5s ease';
                quoteTextEl.style.opacity = 1;
                quoteSourceEl.style.opacity = 1;
            }, 200);
        }

        // Cycle through wisdom array manually
        function cycleQuote() {
            currentIndex = (currentIndex + 1) % sacredWisdom.length;
            displayQuote(currentIndex);
        }

        // Initialize default quote on load
        window.addEventListener('DOMContentLoaded', () => {
            displayQuote(0);
        });

        // Handle Intention Form Submission
        document.getElementById('prayerForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            const name = document.getElementById('nameInput').value.trim() || 'Anonymous traveler';
            const responseEl = document.getElementById('formResponse');

            responseEl.textContent = `Blessings, ${name}. Your intention has been received with grace.`;
            
            // Reset form fields
            this.reset();

            // Clear response message after 5 seconds
            setTimeout(() => {
                responseEl.textContent = '';
            }, 5000);
        });
    </script>
</body>
</html>
