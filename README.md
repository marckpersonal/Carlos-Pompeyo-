<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Carlos Pompeyo - 18 años. Joven emprendedor especializado en trato al cliente persona a persona. Ayudo negocios a crecer con sistemas digitales y comunicación. HUB CUZAMIL.">
    <title>Carlos Pompeyo | Especialista en Trato al Cliente | HUB CUZAMIL</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary: #ff7a3d;
            --secondary: #0066cc;
            --accent: #ffc107;
            --dark: #1a1a1a;
            --light: #f9f9f9;
            --text: #333;
            --text-light: #666;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Poppins', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
            color: var(--text);
            background: linear-gradient(180deg, #fafafa 0%, #f0f4ff 100%);
            overflow-x: hidden;
        }

        header {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(255, 255, 255, 0.98);
            backdrop-filter: blur(10px);
            z-index: 1000;
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 2px 15px rgba(0, 0, 0, 0.08);
        }

        .logo {
            font-weight: 700;
            font-size: 1.4rem;
            color: var(--primary);
        }

        nav {
            display: flex;
            gap: 2.5rem;
        }

        nav a {
            text-decoration: none;
            color: var(--text);
            font-weight: 500;
            font-size: 0.95rem;
            transition: color 0.3s;
        }

        nav a:hover {
            color: var(--primary);
        }

        .hero {
            margin-top: 90px;
            min-height: calc(100vh - 90px);
            display: grid;
            grid-template-columns: 1fr 1fr;
            align-items: center;
            gap: 4rem;
            padding: 3rem 2rem;
            max-width: 1400px;
            margin-left: auto;
            margin-right: auto;
        }

        .hero-content h1 {
            font-size: 3.2rem;
            line-height: 1.15;
            margin-bottom: 1rem;
            animation: slideInLeft 0.8s ease-out;
        }

        .hero-content .name {
            color: var(--primary);
        }

        .hero-content .subtitle {
            font-size: 1.3rem;
            color: var(--secondary);
            font-weight: 600;
            margin-bottom: 1rem;
        }

        .hero-content p {
            font-size: 1.1rem;
            color: var(--text-light);
            margin-bottom: 2.5rem;
            line-height: 1.7;
            animation: slideInLeft 0.8s ease-out 0.15s both;
        }

        .hero-badge {
            display: inline-block;
            background: #fff3e0;
            color: #e65100;
            padding: 0.6rem 1.2rem;
            border-radius: 50px;
            font-size: 0.9rem;
            font-weight: 600;
            margin-bottom: 1.5rem;
            animation: slideInLeft 0.8s ease-out 0.3s both;
        }

        .cta-group {
            display: flex;
            gap: 1.2rem;
            animation: slideInLeft 0.8s ease-out 0.45s both;
            flex-wrap: wrap;
        }

        .btn {
            padding: 0.95rem 2rem;
            border: none;
            border-radius: 50px;
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s;
            text-decoration: none;
            display: inline-flex;
            align-items: center;
            justify-content: center;
            gap: 0.5rem;
        }

        .btn-primary {
            background: linear-gradient(135deg, var(--primary), #ff6b1a);
            color: white;
            box-shadow: 0 8px 25px rgba(255, 122, 61, 0.25);
        }

        .btn-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 12px 35px rgba(255, 122, 61, 0.35);
        }

        .btn-secondary {
            background: white;
            color: var(--primary);
            border: 2px solid var(--primary);
        }

        .btn-secondary:hover {
            background: var(--primary);
            color: white;
            transform: translateY(-3px);
        }

        .avatar-box {
            width: 100%;
            max-width: 450px;
            aspect-ratio: 1;
            background: linear-gradient(135deg, var(--secondary), var(--primary));
            border-radius: 25px;
            overflow: hidden;
            box-shadow: 0 20px 50px rgba(0, 102, 204, 0.2);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 6rem;
            animation: slideInRight 0.8s ease-out;
        }

        .stats {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 1.2rem;
            margin-top: 3rem;
            animation: slideInLeft 0.8s ease-out 0.6s both;
        }

        .stat {
            background: white;
            padding: 1.8rem;
            border-radius: 16px;
            text-align: center;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.06);
            border-left: 4px solid var(--primary);
        }

        .stat-number {
            font-size: 2.2rem;
            font-weight: 700;
            color: var(--primary);
        }

        .stat-label {
            color: var(--text-light);
            font-size: 0.85rem;
            margin-top: 0.6rem;
            font-weight: 500;
        }

        .about {
            padding: 5.5rem 2rem;
            max-width: 1200px;
            margin: 0 auto;
            background: white;
            border-radius: 25px;
            margin-top: 5rem;
            box-shadow: 0 8px 30px rgba(0, 0, 0, 0.05);
        }

        .about h2 {
            font-size: 2.3rem;
            margin-bottom: 3rem;
            text-align: center;
            font-weight: 700;
        }

        .about-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3.5rem;
            align-items: center;
        }

        .about-text p {
            font-size: 1.05rem;
            line-height: 1.8;
            margin-bottom: 1.5rem;
            color: var(--text-light);
        }

        .about-text strong {
            color: var(--primary);
            font-weight: 600;
        }

        .traits {
            list-style: none;
            margin-top: 2.5rem;
        }

        .traits li {
            padding: 0.9rem 0;
            font-size: 1rem;
            display: flex;
            align-items: center;
            gap: 1rem;
        }

        .traits li::before {
            content: '✓';
            width: 32px;
            height: 32px;
            background: linear-gradient(135deg, var(--primary), #ff6b1a);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-weight: bold;
            flex-shrink: 0;
            font-size: 1.2rem;
        }

        .about-image {
            background: linear-gradient(135deg, var(--accent), var(--primary));
            border-radius: 20px;
            height: 350px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 4rem;
        }

        .services {
            padding: 5.5rem 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .section-title {
            font-size: 2.3rem;
            text-align: center;
            margin-bottom: 3.5rem;
            font-weight: 700;
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2.5rem;
        }

        .service-card {
            background: white;
            padding: 2.2rem;
            border-radius: 18px;
            box-shadow: 0 4px 18px rgba(0, 0, 0, 0.06);
            transition: all 0.3s;
            border-top: 4px solid var(--primary);
        }

        .service-card:hover {
            transform: translateY(-8px);
            box-shadow: 0 12px 30px rgba(0, 0, 0, 0.1);
        }

        .service-icon {
            font-size: 2.8rem;
            margin-bottom: 1rem;
        }

        .service-card h3 {
            font-size: 1.25rem;
            margin-bottom: 0.8rem;
            font-weight: 700;
        }

        .service-card p {
            color: var(--text-light);
            line-height: 1.7;
            font-size: 0.95rem;
        }

        .values {
            padding: 5.5rem 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .values-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2.5rem;
            margin-top: 3rem;
        }

        .value-box {
            padding: 2.5rem;
            background: linear-gradient(135deg, #fff9e6 0%, #fff3e0 100%);
            border-radius: 16px;
            border-left: 5px solid var(--primary);
            text-align: center;
        }

        .value-emoji {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        .value-box h3 {
            font-size: 1.2rem;
            margin-bottom: 0.8rem;
            font-weight: 700;
        }

        .value-box p {
            color: var(--text-light);
            font-size: 0.95rem;
            line-height: 1.6;
        }

        .cta-final {
            padding: 5.5rem 2rem;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            text-align: center;
            margin: 5rem auto;
            border-radius: 25px;
            max-width: 1200px;
        }

        .cta-final h2 {
            font-size: 2.3rem;
            margin-bottom: 1.2rem;
            font-weight: 700;
        }

        .cta-final p {
            font-size: 1.1rem;
            margin-bottom: 2.5rem;
            opacity: 0.95;
            line-height: 1.7;
        }

        .cta-final .cta-group {
            justify-content: center;
        }

        footer {
            background: var(--dark);
            color: white;
            padding: 3.5rem 2rem;
            text-align: center;
        }

        .footer-text {
            margin-bottom: 1.5rem;
        }

        .footer-text strong {
            color: var(--primary);
        }

        .footer-motto {
            font-size: 1.1rem;
            margin-top: 1.5rem;
            font-style: italic;
            opacity: 0.9;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 2rem;
            margin-top: 2.5rem;
        }

        .social-links a {
            color: white;
            text-decoration: none;
            font-weight: 600;
            transition: color 0.3s;
        }

        .social-links a:hover {
            color: var(--primary);
        }

        @keyframes slideInLeft {
            from {
                opacity: 0;
                transform: translateX(-40px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }

        @keyframes slideInRight {
            from {
                opacity: 0;
                transform: translateX(40px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }

        @media (max-width: 768px) {
            header {
                padding: 0.8rem 1rem;
            }

            nav {
                display: none;
            }

            .hero {
                grid-template-columns: 1fr;
                margin-top: 80px;
                padding: 2rem 1rem;
            }

            .hero-content h1 {
                font-size: 2.2rem;
            }

            .about-grid {
                grid-template-columns: 1fr;
                gap: 2.5rem;
            }

            .cta-group {
                flex-direction: column;
            }

            .btn {
                width: 100%;
            }

            .stats {
                grid-template-columns: 1fr;
            }

            .services-grid {
                grid-template-columns: 1fr;
            }

            .values-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">🚀 Carlos Pompeyo</div>
        <nav>
            <a href="#about">Sobre mí</a>
            <a href="#services">Qué hago</a>
            <a href="#values">Mi estilo</a>
            <a href="#contact">Contacto</a>
        </nav>
    </header>

    <section class="hero">
        <div class="hero-content">
            <div class="hero-badge">👨‍💼 Uno de los pioneros del HUB CUZAMIL</div>
            <h1>Hola, soy <span class="name">Carlos</span></h1>
            <div class="subtitle">Especialista en trato al cliente</div>
            <p>Tengo 18 años y acabo de empezar mi viaje en el mundo digital. Mi pasión es <strong>ayudar a otros negocios a crecer</strong> mejorando su comunicación, sistemas y procesos de venta. Persona a persona.</p>

            <div class="cta-group">
                <a href="https://wa.me/529871416354?text=Hola%20Carlos%2C%20vi%20tu%20landing%20y%20me%20gustaría%20hablar%20contigo" class="btn btn-primary" target="_blank">
                    📱 Hablemos por WhatsApp
                </a>
                <a href="mailto:carlospompeyo9@gmail.com" class="btn btn-secondary">
                    ✉️ Envíame un email
                </a>
            </div>

            <div class="stats">
                <div class="stat">
                    <div class="stat-number">18</div>
                    <div class="stat-label">Años - Joven & Energía</div>
                </div>
                <div class="stat">
                    <div class="stat-number">∞</div>
                    <div class="stat-label">Ganas de aprender & crecer</div>
                </div>
            </div>
        </div>

        <div class="avatar-box">📸</div>
    </section>

    <section class="about" id="about">
        <h2>¿Quién soy realmente?</h2>
        <div class="about-grid">
            <div class="about-text">
                <p>Mi nombre es <strong>Carlos Pompeyo</strong>. Tengo 18 años y soy de Cozumel. No soy un experto (todavía), pero soy alguien <strong>genuino, sincero y con muchas ganas de crecer</strong>.</p>
                <p>Hace poco descubrí que me encanta <strong>conectar con personas</strong> y <strong>entender lo que los negocios necesitan</strong>. Por eso me uní al HUB CUZAMIL - para aprender herramientas digitales reales y ayudar a otros a mejorar.</p>
                <p>Lo que me diferencia es que <strong>no soy frío ni automatizado</strong>. Creo que el mejor negocio es aquel donde tú y tu cliente se entienden de verdad. Eso es lo que hago: construyo puentes entre personas.</p>

                <ul class="traits">
                    <li>Amable y honesto en todo</li>
                    <li>Me encanta hacer amigos</li>
                    <li>Divertido cuando agarras confianza</li>
                    <li>Especialista en comunicación real</li>
                    <li>Deportista (beisbol 🥎)</li>
                    <li>Buena onda y poco serio</li>
                </ul>
            </div>
            <div class="about-image">🎯</div>
        </div>
    </section>

    <section class="services" id="services">
        <h2 class="section-title">¿Qué hago exactamente?</h2>
        <div class="services-grid">
            <div class="service-card">
                <div class="service-icon">💬</div>
                <h3>Consultoría 1:1</h3>
                <p>Hablamos de tu negocio, entiendo tus desafíos y te propongo soluciones reales basadas en lo que funciona.</p>
            </div>
            <div class="service-card">
                <div class="service-icon">📱</div>
                <h3>Estrategia Digital</h3>
                <p>Diseñamos juntos cómo llevar tu negocio a plataformas digitales sin perder lo personal que te define.</p>
            </div>
            <div class="service-card">
                <div class="service-icon">📧</div>
                <h3>Comunicación Efectiva</h3>
                <p>Mejoramos cómo te comunicas con clientes. Textos que conviertan, sin ser salesy ni falso.</p>
            </div>
            <div class="service-card">
                <div class="service-icon">🔄</div>
                <h3>Procesos & Sistemas</h3>
                <p>Organizamos tus procesos para que tengas más tiempo y menos estrés. Orden = Ganancias.</p>
            </div>
            <div class="service-card">
                <div class="service-icon">📊</div>
                <h3>Análisis Simple</h3>
                <p>Te muestro métricas reales y fáciles de entender. Números que significan algo para TU negocio.</p>
            </div>
            <div class="service-card">
                <div class="service-icon">👥</div>
                <h3>Mentoría & Apoyo</h3>
                <p>Estoy contigo en el proceso. Preguntas, dudas, bloqueos - respondo porque creo en tu éxito.</p>
            </div>
        </div>
    </section>

    <section class="values" id="values">
        <h2 class="section-title">Mi Estilo de Trabajo</h2>
        <div class="values-grid">
            <div class="value-box">
                <div class="value-emoji">💯</div>
                <h3>Honestidad</h3>
                <p>Te digo la verdad, aunque sea incómoda. Sin promesas falsas. Resultados reales o te lo digo.</p>
            </div>
            <div class="value-box">
                <div class="value-emoji">🤝</div>
                <h3>Persona a Persona</h3>
                <p>Sin egos. Sin jerga complicada. Hablamos como amigos que quieren ayudarse mutuamente.</p>
            </div>
            <div class="value-box">
                <div class="value-emoji">⚡</div>
                <h3>Acción Rápida</h3>
                <p>No me gusta perder tiempo. Planificamos, ejecutamos y medimos. Rápido y bien.</p>
            </div>
            <div class="value-box">
                <div class="value-emoji">📚</div>
                <h3>Siempre Aprendiendo</h3>
                <p>Tengo 18 años. Estoy aprendiendo constantemente. Eso significa que traigo ideas nuevas.</p>
            </div>
            <div class="value-box">
                <div class="value-emoji">😄</div>
                <h3>Buena Onda</h3>
                <p>La vida es para disfrutarla. Trabajamos en serio pero nos divertimos en el camino.</p>
            </div>
            <div class="value-box">
                <div class="value-emoji">🎯</div>
                <h3>Enfocado en Resultados</h3>
                <p>Al final lo que importa es: ¿Creció tu negocio? ¿Vendiste más? Eso es éxito.</p>
            </div>
        </div>
    </section>

    <section class="cta-final" id="contact">
        <h2>¿Hablamos?</h2>
        <p>No tengo una propuesta complicada. Solo quiero conocer tu negocio y ver cómo puedo ayudarte a crecer. Sin presión, sin promesas falsas. Solo persona a persona.</p>
        <div class="cta-group">
            <a href="https://wa.me/529871416354?text=Hola%20Carlos%2C%20quiero%20hablar%20contigo%20sobre%20mi%20negocio" class="btn btn-primary" target="_blank">
                💬 Escribirme por WhatsApp
            </a>
            <a href="mailto:carlospompeyo9@gmail.com" class="btn btn-secondary">
                📧 Enviarme un email
            </a>
        </div>
    </section>

    <footer>
        <div class="footer-text">© 2026 <strong>Carlos Pompeyo</strong> | HUB CUZAMIL - Empoderamiento Social para Cozumel</div>
        <div class="footer-motto">"Deja tu legado vivo y logra tu sueño en vida"</div>
        <div class="social-links">
            <a href="https://wa.me/529871416354" target="_blank">WhatsApp</a>
            <a href="mailto:carlospompeyo9@gmail.com">Email</a>
            <a href="https://cuzamil.io" target="_blank">HUB CUZAMIL</a>
        </div>
    </footer>

    <script>
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({ behavior: 'smooth' });
                }
            });
        });
    </script>
</body>
</html>
