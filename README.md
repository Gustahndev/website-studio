# website-studio
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bella Nails - Manicure & Beleza</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
        }

        header {
            background: linear-gradient(135deg, #d946a6 0%, #ec4899 100%);
            color: white;
            padding: 1rem 0;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        nav {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0 2rem;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: bold;
            letter-spacing: 1px;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        nav a {
            color: white;
            text-decoration: none;
            transition: opacity 0.3s;
        }

        nav a:hover {
            opacity: 0.8;
        }

        .hero {
            background: linear-gradient(135deg, #fdf2f8 0%, #fce7f3 100%);
            padding: 6rem 2rem;
            text-align: center;
        }

        .hero h1 {
            font-size: 3rem;
            color: #be185d;
            margin-bottom: 1rem;
        }

        .hero p {
            font-size: 1.2rem;
            color: #666;
            margin-bottom: 2rem;
        }

        .btn {
            display: inline-block;
            padding: 0.8rem 2rem;
            background: linear-gradient(135deg, #d946a6 0%, #ec4899 100%);
            color: white;
            text-decoration: none;
            border-radius: 50px;
            transition: transform 0.3s, box-shadow 0.3s;
            border: none;
            cursor: pointer;
            font-size: 1rem;
        }

        .btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 20px rgba(217, 70, 166, 0.4);
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
        }

        .section {
            padding: 5rem 0;
        }

        .section h2 {
            font-size: 2.5rem;
            color: #be185d;
            margin-bottom: 3rem;
            text-align: center;
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2rem;
        }

        .service-card {
            background: white;
            padding: 2rem;
            border-radius: 15px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0,0,0,0.08);
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .service-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 30px rgba(217, 70, 166, 0.2);
        }

        .service-icon {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        .service-card h3 {
            color: #d946a6;
            margin-bottom: 1rem;
            font-size: 1.3rem;
        }

        .service-card p {
            color: #666;
            font-size: 0.95rem;
        }

        .service-card .price {
            color: #ec4899;
            font-weight: bold;
            font-size: 1.2rem;
            margin-top: 1rem;
        }

        .testimonials {
            background: linear-gradient(135deg, #fdf2f8 0%, #fce7f3 100%);
        }

        .testimonial-card {
            background: white;
            padding: 2rem;
            border-radius: 10px;
            margin-bottom: 1.5rem;
            border-left: 4px solid #ec4899;
        }

        .stars {
            color: #fbbf24;
            margin-bottom: 0.5rem;
        }

        .testimonial-card p {
            color: #666;
            font-style: italic;
            margin-bottom: 1rem;
        }

        .testimonial-author {
            font-weight: bold;
            color: #d946a6;
        }

        footer {
            background: #1f2937;
            color: white;
            padding: 3rem 2rem;
            text-align: center;
        }

        .contact-section {
            background: white;
        }

        .contact-info {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-bottom: 3rem;
        }

        .info-box {
            text-align: center;
        }

        .info-box h3 {
            color: #d946a6;
            margin-bottom: 0.5rem;
        }

        .info-box p {
            color: #666;
        }

        @media (max-width: 768px) {
            nav ul {
                gap: 1rem;
            }

            .hero h1 {
                font-size: 2rem;
            }

            .section h2 {
                font-size: 1.8rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <div class="logo">✨ Bella Nails</div>
            <ul>
                <li><a href="#servicos">Serviços</a></li>
                <li><a href="#depoimentos">Depoimentos</a></li>
                <li><a href="#contato">Contato</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero">
        <h1>Sua Beleza é Nossa Paixão</h1>
        <p>Unhas impecáveis, acessórios perfeitos e muito mais para você se sentir linda</p>
        <button class="btn" onclick="alert('Agende seu horário! Tel: (11) 98765-4321')">Agende Agora</button>
    </section>

    <section class="section container" id="servicos">
        <h2>Nossos Serviços</h2>
        <div class="services-grid">
            <div class="service-card">
                <div class="service-icon">💅</div>
                <h3>Manicure</h3>
                <p>Unhas bem cuidadas e hidratadas com os melhores esmaltes do mercado</p>
                <div class="price">A partir de R$ 35</div>
            </div>

            <div class="service-card">
                <div class="service-icon">🦶</div>
                <h3>Pedicure</h3>
                <p>Tratamento completo dos pés com esfoliação e hidratação profunda</p>
                <div class="price">A partir de R$ 40</div>
            </div>

            <div class="service-card">
                <div class="service-icon">✨</div>
                <h3>Gel & Esmaltação</h3>
                <p>Unhas de gel de longa duração com cores vibrantes e brilhantes</p>
                <div class="price">A partir de R$ 60</div>
            </div>

            <div class="service-card">
                <div class="service-icon">💎</div>
                <h3>Alongamento</h3>
                <p>Alongamento profissional com fibra de vidro ou acrílico</p>
                <div class="price">A partir de R$ 80</div>
            </div>

            <div class="service-card">
                <div class="service-icon">🎨</div>
                <h3>Nail Art</h3>
                <p>Designs personalizados e criações únicas para suas unhas</p>
                <div class="price">A partir de R$ 50</div>
            </div>

            <div class="service-card">
                <div class="service-icon">💆</div>
                <h3>Massagem Relaxante</h3>
                <p>Massagem nos pés e mãos para relaxamento total</p>
                <div class="price">A partir de R$ 45</div>
            </div>
        </div>
    </section>

    <section class="section testimonials" id="depoimentos">
        <div class="container">
            <h2>O que Dizem Nossas Clientes</h2>
            <div class="testimonial-card">
                <div class="stars">★★★★★</div>
                <p>"Adorei o atendimento! A manicurista foi muito cuidadosa e as unhas ficaram perfeitas. Voltarei com certeza!"</p>
                <div class="testimonial-author">- Marina Silva</div>
            </div>

            <div class="testimonial-card">
                <div class="stars">★★★★★</div>
                <p>"Melhor salão da região! Ambiente limpo, acolhedor e as meninas são super atenciosas. Recomendo!"</p>
                <div class="testimonial-author">- Juliana Costa</div>
            </div>

            <div class="testimonial-card">
                <div class="stars">★★★★★</div>
                <p>"Gel que dura! Ficou maravilhoso e mantém a qualidade por semanas. Muito bom mesmo!"</p>
                <div class="testimonial-author">- Beatriz Santos</div>
            </div>
        </div>
    </section>

    <section class="section contact-section" id="contato">
        <div class="container">
            <h2>Entre em Contato</h2>
            <div class="contact-info">
                <div class="info-box">
                    <h3>📞 Telefone</h3>
                    <p>(11) 98765-4321<br>(11) 3456-7890</p>
                </div>
                <div class="info-box">
                    <h3>📍 Endereço</h3>
                    <p>Rua das Flores, 123<br>São Paulo - SP</p>
                </div>
                <div class="info-box">
                    <h3>🕒 Horário</h3>
                    <p>Seg-Sex: 9h às 19h<br>Sábado: 9h às 18h</p>
                </div>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2025 Bella Nails - Manicure & Beleza. Todos os direitos reservados.</p>
        <p>Siga-nos: Instagram | Facebook | WhatsApp</p>
    </footer>
</body>
</html>
