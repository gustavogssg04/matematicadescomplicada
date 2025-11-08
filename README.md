<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aulas Particulares - Professor Particular</title>
    <style>
        /* Estilos gerais */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial', sans-serif;
        }
        
        body {
            line-height: 1.6;
            color: #333;
            background-color: #f9f9f9;
        }
        
        .container {
            width: 90%;
            max-width: 1100px;
            margin: 0 auto;
            padding: 20px;
        }
        
        section {
            padding: 60px 0;
        }
        
        h1, h2, h3 {
            margin-bottom: 20px;
            color: #2c3e50;
        }
        
        p {
            margin-bottom: 15px;
        }
        
        .btn {
            display: inline-block;
            background: #3498db;
            color: white;
            padding: 12px 25px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            text-decoration: none;
            font-size: 16px;
            margin-top: 10px;
            transition: background 0.3s;
        }
        
        .btn:hover {
            background: #2980b9;
        }
        
        /* Header */
        header {
            background: white;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 100;
        }
        
        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 0;
        }
        
        .logo {
            font-size: 24px;
            font-weight: bold;
            color: #3498db;
            text-decoration: none;
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 20px;
        }
        
        nav ul li a {
            text-decoration: none;
            color: #333;
            font-weight: 500;
            transition: color 0.3s;
        }
        
        nav ul li a:hover {
            color: #3498db;
        }
        
        /* Hero */
        .hero {
            background: linear-gradient(135deg, #3498db, #2c3e50);
            color: white;
            text-align: center;
            padding: 150px 0 100px;
            margin-top: 70px;
        }
        
        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 20px;
            color: white;
        }
        
        .hero p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 30px;
        }
        
        /* Sobre */
        .about-content {
            display: flex;
            align-items: center;
            gap: 40px;
        }
        
        .about-text {
            flex: 1;
        }
        
        .about-image {
            flex: 1;
            text-align: center;
        }
        
        .about-image img {
            max-width: 100%;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        /* Matérias */
        .subjects {
            background: #f1f1f1;
        }
        
        .subjects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }
        
        .subject-card {
            background: white;
            padding: 25px;
            border-radius: 8px;
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
            text-align: center;
            transition: transform 0.3s;
        }
        
        .subject-card:hover {
            transform: translateY(-5px);
        }
        
        .subject-icon {
            font-size: 40px;
            margin-bottom: 15px;
        }
        
        /* Contato */
        .contact-form {
            max-width: 600px;
            margin: 0 auto;
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 5px;
            font-weight: 500;
        }
        
        .form-control {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 16px;
        }
        
        textarea.form-control {
            min-height: 150px;
            resize: vertical;
        }
        
        /* Footer */
        footer {
            background: #2c3e50;
            color: white;
            text-align: center;
            padding: 30px 0;
        }
        
        .social-links {
            margin: 20px 0;
        }
        
        .social-links a {
            display: inline-block;
            color: white;
            margin: 0 10px;
            font-size: 20px;
            text-decoration: none;
        }
        
        /* Responsividade */
        @media (max-width: 768px) {
            .header-container {
                flex-direction: column;
                text-align: center;
            }
            
            nav ul {
                margin-top: 15px;
            }
            
            .about-content {
                flex-direction: column;
            }
            
            .hero h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container header-container">
            <a href="#" class="logo">Aulas Particulares</a>
            <nav>
                <ul>
                    <li><a href="#sobre">Sobre</a></li>
                    <li><a href="#materias">Matérias</a></li>
                    <li><a href="#contato">Contato</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <h1>Aulas Particulares de Qualidade</h1>
            <p>Reforço escolar, preparação para vestibulares e acompanhamento personalizado para todas as idades.</p>
            <a href="#contato" class="btn">Agende uma Aula Experimental</a>
        </div>
    </section>

    <!-- Sobre -->
    <section id="sobre">
        <div class="container">
            <h2>Sobre o Professor</h2>
            <div class="about-content">
                <div class="about-text">
                    <p>Olá! Sou professor com mais de 10 anos de experiência em aulas particulares. Minha metodologia é focada nas necessidades específicas de cada aluno, criando um plano de estudos personalizado.</p>
                    <p>Formado em Matemática pela USP e com especialização em Educação, já ajudei centenas de estudantes a alcançarem seus objetivos acadêmicos.</p>
                    <p>Ofereço aulas presenciais na região de São Paulo e aulas online para todo o Brasil.</p>
                    <a href="#contato" class="btn">Entre em Contato</a>
                </div>
                <div class="about-image">
                    <!-- Substitua pela sua foto -->
                    <img src="https://images.unsplash.com/photo-1568602471122-7832951cc4c5?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=80" alt="Professor">
                </div>
            </div>
        </div>
    </section>

    <!-- Matérias -->
    <section id="materias" class="subjects">
        <div class="container">
            <h2>Matérias que Ensino</h2>
            <div class="subjects-grid">
                <div class="subject-card">
                    <div class="subject-icon">🧮</div>
                    <h3>Matemática</h3>
                    <p>Do básico ao avançado, incluindo álgebra, geometria e cálculo.</p>
                </div>
                <div class="subject-card">
                    <div class="subject-icon">🧪</div>
                    <h3>Física e Química</h3>
                    <p>Conceitos fundamentais e resolução de problemas.</p>
                </div>
                <div class="subject-card">
                    <div class="subject-icon">🔤</div>
                    <h3>Português</h3>
                    <p>Gramática, redação e interpretação de texto.</p>
                </div>
                <div class="subject-card">
                    <div class="subject-icon">🌎</div>
                    <h3>História e Geografia</h3>
                    <p>Conteúdo contextualizado e preparação para vestibulares.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contato -->
    <section id="contato">
        <div class="container">
            <h2>Entre em Contato</h2>
            <div class="contact-form">
                <form id="formContato">
                    <div class="form-group">
                        <label for="nome">Nome</label>
                        <input type="text" id="nome" class="form-control" required>
                    </div>
                    <div class="form-group">
                        <label for="email">Email</label>
                        <input type="email" id="email" class="form-control" required>
                    </div>
                    <div class="form-group">
                        <label for="telefone">Telefone/WhatsApp</label>
                        <input type="tel" id="telefone" class="form-control">
                    </div>
                    <div class="form-group">
                        <label for="mensagem">Mensagem</label>
                        <textarea id="mensagem" class="form-control" required></textarea>
                    </div>
                    <button type="submit" class="btn">Enviar Mensagem</button>
                </form>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p>Aulas Particulares - Professor Particular</p>
            <div class="social-links">
                <a href="#">📘</a>
                <a href="#">📷</a>
                <a href="#">📱</a>
            </div>
            <p>Email: professor@aulasparticulares.com | Tel: (11) 99999-9999</p>
            <p>&copy; 2023 - Todos os direitos reservados</p>
        </div>
    </footer>

    <script>
        // Formulário de contato
        document.getElementById('formContato').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Mensagem enviada com sucesso! Entrarei em contato em breve.');
            this.reset();
        });
        
        // Smooth scroll para links internos
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                const targetId = this.getAttribute('href');
                if(targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if(targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                }
            });
        });
    </script>
</body>
</html>
