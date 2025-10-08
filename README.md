<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfólio - Júlia Bomfonti de Oliveira</title>
    <style>
        
        body {
            margin: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #f4f4f9;
            color: #333;
            line-height: 1.6;
        }

        .container {
            width: 90%;
            max-width: 1100px;
            margin: 0 auto;
        }

        
        header {
            background-color: #4a4e69;
            color: white;
            padding: 20px 0;
        }

        header .container {
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
        }

        @media (min-width: 768px) {
            header .container {
                flex-direction: row;
                justify-content: space-between;
                text-align: left;
            }
        }

        nav ul {
            list-style: none;
            padding: 0;
            margin: 10px 0 0;
            display: flex;
            gap: 20px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            transition: color 0.3s ease;
        }

        nav ul li a:hover {
            color: #ffcc70;
        }

        .hero {
            background-color: #9a8c98;
            color: white;
            text-align: center;
            padding: 80px 20px;
        }

        .hero h2 {
            font-size: 2em;
            margin-bottom: 10px;
        }

        .hero p {
            font-size: 1.2em;
        }

       
        section {
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 2px 6px rgba(0,0,0,0.1);
            margin: 40px auto;
            padding: 30px 20px;
        }

        h2 {
            color: #22223b;
            border-bottom: 2px solid #9a8c98;
            padding-bottom: 10px;
        }

        
        #sobre p {
            text-align: justify;
        }

       
        .grid-projetos {
            display: grid;
            grid-template-columns: 1fr;
            gap: 20px;
            margin-top: 20px;
        }

        @media (min-width: 700px) {
            .grid-projetos {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        .projeto {
            background-color: #f8f8fc;
            padding: 20px;
            border-radius: 10px;
            border-left: 5px solid #9a8c98;
            transition: transform 0.2s ease;
        }

        .projeto:hover {
            transform: translateY(-5px);
        }

        .projeto h3 {
            margin-top: 0;
            color: #4a4e69;
        }

      
        .contato form {
            display: flex;
            flex-direction: column;
            gap: 15px;
            margin-top: 15px;
        }

        @media (min-width: 700px) {
            .contato form {
                flex-direction: row;
                flex-wrap: wrap;
            }

            .contato input[type="text"],
            .contato input[type="email"] {
                flex: 1 1 45%;
            }

            .contato textarea {
                flex: 1 1 100%;
            }
        }

        .contato input, .contato textarea {
            padding: 10px;
            border-radius: 5px;
            border: 1px solid #ccc;
            font-size: 1em;
        }

        .contato button {
            background-color: #4a4e69;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s;
            align-self: flex-start;
        }

        .contato button:hover {
            background-color: #22223b;
        }

        
        footer {
            background-color: #4a4e69;
            color: white;
            text-align: center;
            padding: 20px;
            font-size: 0.9em;
        }

        footer a {
            color: #ffcc70;
            text-decoration: none;
            margin: 0 8px;
        }

        footer a:hover {
            text-decoration: underline;
        }

    </style>
</head>
<body>

    
    <header>
        <div class="container">
            <h1>Júlia Bomfonti de Oliveira</h1>
            <nav>
                <ul>
                    <li><a href="#sobre">Sobre</a></li>
                    <li><a href="#projetos">Projetos</a></li>
                    <li><a href="#contato">Contato</a></li>
                </ul>
            </nav>
        </div>
    </header>

    
    <section class="hero">
        <div class="container">
            <h2>Estudante de Análise e Desenvolvimento de Sistemas</h2>
            <p>Interessada em tecnologia, design e inovação.</p>
        </div>
    </section>

   
    <section id="sobre" class="container">
        <h2>Sobre Mim</h2>
        <p>Gosto de aprender coisas novas e aplicar meus conhecimentos em projetos práticos. Tenho interesse em programação, design digital e soluções criativas que possam ajudar no dia a dia.</p>
        <p>Minhas principais habilidades incluem: lógica de programação, HTML, trabalho em equipe e vontade de aprender sempre.</p>
    </section>

    
    <section id="projetos" class="container">
        <h2>Projetos</h2>
        <div class="grid-projetos">
            <div class="projeto">
                <h3>Site Pessoal</h3>
                <p>Criação de uma página simples em HTML para apresentar meu perfil profissional e projetos pessoais.</p>
            </div>
            <div class="projeto">
                <h3>Trabalho em Grupo</h3>
                <p>Participação em projeto acadêmico focado em sustentabilidade e tecnologia, aplicando conceitos de design e programação.</p>
            </div>
        </div>
    </section>

   
    <section id="contato" class="container contato">
        <h2>Contato</h2>
        <p>Email: <a href="mailto:julia.bomfonti2004@gmail.com">julia.bomfonti2004@gmail.com</a></p>
        <form>
            <input type="text" placeholder="Seu nome" required>
            <input type="email" placeholder="Seu e-mail" required>
            <textarea rows="4" placeholder="Sua mensagem" required></textarea>
            <button type="submit">Enviar</button>
        </form>
    </section>

   
    <footer>
        <p>&copy; 2025 Júlia Bomfonti de Oliveira. Todos os direitos reservados.</p>
        <p>Me siga no 
            <a href="https://www.instagram.com/juliabomf/">Instagram</a> | 
            <a href="https://www.linkedin.com/in/j%C3%BAlia-bomfonti-de-oliveira-bbb83b309/">LinkedIn</a> | 
            <a href="https://github.com/jbomfonti">GitHub</a>
        </p>
    </footer>

</body>
</html>
