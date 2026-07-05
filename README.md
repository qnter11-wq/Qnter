<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Instalacje Elektryczne i Automatyka</title>
    <style>
        /* Reset i podstawowe style */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        :root {
            --bg-dark: #1a1a24;
            --bg-light: #f4f6f9;
            --accent: #ffb703; /* Elektryzujący żółty/pomarańczowy */
            --text-dark: #2b2d42;
            --text-light: #ffffff;
            --card-bg: #ffffff;
        }

        body {
            background-color: var(--bg-light);
            color: var(--text-dark);
            line-height: 1.6;
        }

        /* Nagłówek i Nawigacja */
        header {
            background-color: var(--bg-dark);
            color: var(--text-light);
            padding: 1rem 2rem;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0,0,0,0.3);
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: var(--text-light);
        }

        .logo span {
            color: var(--accent);
        }

        .nav-links a {
            color: var(--text-light);
            text-decoration: none;
            margin-left: 1.5rem;
            font-weight: 500;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: var(--accent);
        }

        /* Sekcja główna (Hero) */
        .hero {
            background: linear-gradient(rgba(26, 26, 36, 0.85), rgba(26, 26, 36, 0.95)), url('https://images.unsplash.com/photo-1621905251189-08b45d6a269e?auto=format&fit=crop&w=1200&q=80') no-repeat center center/cover;
            color: var(--text-light);
            padding: 5rem 2rem;
            text-align: center;
        }

        .hero-content {
            max-width: 800px;
            margin: 0 auto;
        }

        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }

        .hero h1 span {
            color: var(--accent);
        }

        .hero p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
            opacity: 0.9;
        }

        .btn {
            display: inline-block;
            background-color: var(--accent);
            color: var(--bg-dark);
            padding: 0.8rem 2rem;
            text-decoration: none;
            font-weight: bold;
            border-radius: 4px;
            transition: transform 0.2s, background-color 0.3s;
        }

        .btn:hover {
            transform: translateY(-2px);
            background-color: #e5a100;
        }

        /* Usługi */
        .services {
            max-width: 1200px;
            margin: 4rem auto;
            padding: 0 2rem;
        }

        .section-title {
            text-align: center;
            margin-bottom: 3rem;
            font-size: 2rem;
            position: relative;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 60px;
            height: 4px;
            background-color: var(--accent);
            margin: 0.5rem auto 0;
            border-radius: 2px;
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }

        .service-card {
            background-color: var(--card-bg);
            padding: 2.5rem 2rem;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            text-align: center;
            transition: transform 0.3s, box-shadow 0.3s;
            border-top: 4px solid transparent;
        }

        .service-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px rgba(0,0,0,0.1);
            border-top: 4px solid var(--accent);
        }

        .service-icon {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }

        .service-card h3 {
            margin-bottom: 1rem;
            font-size: 1.3rem;
        }

        /* Kontakt */
        .contact {
            background-color: var(--bg-dark);
            color: var(--text-light);
            padding: 4rem 2rem;
            text-align: center;
        }

        .contact-container {
            max-width: 600px;
            margin: 0 auto;
        }

        .contact-info {
            margin-top: 2rem;
            display: grid;
            gap: 1.5rem;
        }

        .contact-item {
            background: rgba(255,255,255,0.05);
            padding: 1.5rem;
            border-radius: 6px;
        }

        .contact-item h4 {
            color: var(--accent);
            margin-bottom: 0.3rem;
            text-transform: uppercase;
            font-size: 0.9rem;
            letter-spacing: 1px;
        }

        .contact-item p, .contact-item a {
            font-size: 1.4rem;
            color: var(--text-light);
            text-decoration: none;
            font-weight: bold;
        }

        /* Stopka */
        footer {
            background-color: #111118;
            color: rgba(255,255,255,0.5);
            text-align: center;
            padding: 1.5rem;
            font-size: 0.9rem;
        }

        /* Responsywność */
        @media (max-width: 768px) {
            .nav-container {
                flex-direction: column;
                gap: 1rem;
            }
            .nav-links a {
                margin: 0 0.7rem;
            }
            .hero h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>

    <!-- Nawigacja -->
    <header>
        <div class="nav-container">
            <div class="logo">E-Lima Elektryka/Automatyka<span></span></div>
            <nav class="nav-links">
                <a href="#uslugi">Usługi</a>
                <a href="#kontakt">Kontakt</a>
            </nav>
        </div>
    </header>

    <!-- Sekcja Główna -->
    <section class="hero">
        <div class="hero-content">
            <h1>Profesjonalne Instalacje Elektryczne i Automatyka</h1>
            <p>Bezpieczeństwo, nowoczesność i niezawodność dla Twojego domu i firmy. Kompleksowe wykonawstwo na najwyższym poziomie.</p>
            <a href="#kontakt" class="btn">Zadzwoń lub napisz</a>
        </div>
    </section>

    <!-- Sekcja Usług -->
    <section class="services" id="uslugi">
        <h2 class="section-title">Co oferujemy?</h2>
        <div class="services-grid">
            
            <div class="service-card">
                <div class="service-icon">⚡</div>
                <h3>Instalacje Elektryczne</h3>
                <p>Projektowanie, montaż oraz modernizacja instalacji nisko i silnoprądowych. Pomiary i serwis.</p>
            </div>

            <div class="service-card">
                <div class="service-icon">🤖</div>
                <h3>Automatyka</h3>
                <p>Inteligentne systemy sterowania budynkiem, optymalizacja pracy urządzeń i systemów przemysłowych.</p>
            </div>

            <div class="service-card">
                <div class="service-icon">🚧</div>
                <h3>Napędy Bram</h3>
                <p>Dobór, montaż i programowanie automatyki do bram wjazdowych oraz garażowych wiodących marek.</p>
            </div>

            <div class="service-card">
                <div class="service-icon">👁️</div>
                <h3>Monitoring (CCTV)</h3>
                <p>Nowoczesne systemy kamer z podglądem na żywo w telefonie. Zabezpieczenie posesji i firm.</p>
            </div>

            <div class="service-card">
                <div class="service-icon">🚨</div>
                <h3>Systemy Alarmowe</h3>
                <p>Instalacja certyfikowanych systemów SSWiN. Profesjonalna ochrona przed włamaniem i pożarem.</p>
            </div>

        </div>
    </section>

    <!-- Sekcja Kontakt -->
    <section class="contact" id="kontakt">
        <div class="contact-container">
            <h2 class="section-title">Zapraszamy do kontaktu</h2>
            <p>Potrzebujesz wyceny lub masz pytania? Skontaktuj się ze mną telefonicznie lub mailowo.</p>
            
            <div class="contact-info">
                <div class="contact-item">
                    <h4>Telefon</h4>
                    <a href="tel:+48501508422">+48 501 508 422</a>
                </div>

                <div class="contact-item">
                    <h4>Telefon</h4>
                    <a href="tel:+48655744407">+48 665 744 407</a>
                </div>

                <div class="contact-item">
                    <h4>E-mail</h4>
                    <a href="marek.konik.lima@gmail.com">marek.konik.lima@gmail.com</a>
                </div>

                <div class="contact-item">
                    <h4>Obszar działania</h4>
                    <p>Wielkopolska</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Stopka -->
    <footer>
        <p>&copy; 2026 E-Lima. Wszelkie prawa zastrzeżone.</p>
    </footer>

</body>
</html>

