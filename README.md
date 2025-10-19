<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Matheus - Developer Profile</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #fff;
            min-height: 100vh;
            padding: 20px;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            animation: fadeIn 1s ease-in;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        header {
            text-align: center;
            padding: 60px 20px;
            animation: slideDown 1s ease-out;
        }

        @keyframes slideDown {
            from { transform: translateY(-50px); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }

        .profile-img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            border: 5px solid rgba(255, 255, 255, 0.3);
            margin-bottom: 20px;
            animation: pulse 2s infinite;
            background: linear-gradient(135deg, #667eea, #764ba2);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 60px;
            margin-left: auto;
            margin-right: auto;
        }

        @keyframes pulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.05); }
        }

        h1 {
            font-size: 3em;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }

        .subtitle {
            font-size: 1.3em;
            opacity: 0.9;
            margin-bottom: 30px;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 20px;
        }

        .social-btn {
            padding: 12px 25px;
            background: rgba(255, 255, 255, 0.2);
            border: 2px solid rgba(255, 255, 255, 0.3);
            border-radius: 50px;
            color: white;
            text-decoration: none;
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
        }

        .social-btn:hover {
            background: rgba(255, 255, 255, 0.3);
            transform: translateY(-3px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.3);
        }

        .section {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 40px;
            margin-bottom: 30px;
            border: 1px solid rgba(255, 255, 255, 0.2);
            animation: fadeInUp 1s ease-out;
        }

        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }

        h2 {
            font-size: 2em;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 15px;
            margin-top: 20px;
        }

        .skill-card {
            background: rgba(255, 255, 255, 0.15);
            padding: 20px;
            border-radius: 15px;
            text-align: center;
            transition: all 0.3s ease;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }

        .skill-card:hover {
            transform: translateY(-5px);
            background: rgba(255, 255, 255, 0.25);
            box-shadow: 0 10px 30px rgba(0,0,0,0.3);
        }

        .skill-icon {
            font-size: 2.5em;
            margin-bottom: 10px;
        }

        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
            margin-top: 20px;
        }

        .project-card {
            background: rgba(255, 255, 255, 0.15);
            padding: 30px;
            border-radius: 15px;
            transition: all 0.3s ease;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }

        .project-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 40px rgba(0,0,0,0.4);
        }

        .project-card h3 {
            font-size: 1.5em;
            margin-bottom: 15px;
        }

        .stats {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .stat-card {
            background: rgba(255, 255, 255, 0.15);
            padding: 30px;
            border-radius: 15px;
            text-align: center;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }

        .stat-number {
            font-size: 3em;
            font-weight: bold;
            margin-bottom: 10px;
        }

        footer {
            text-align: center;
            padding: 40px;
            margin-top: 40px;
            opacity: 0.8;
        }

        @media (max-width: 768px) {
            h1 { font-size: 2em; }
            .section { padding: 20px; }
            .projects-grid, .skills-grid { grid-template-columns: 1fr; }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div class="profile-img">👨‍💻</div>
            <h1>Matheus</h1>
            <p class="subtitle">Full Stack Developer | Tech Enthusiast | Problem Solver</p>
            <div class="social-links">
                <a href="https://github.com/seu-usuario" class="social-btn">🐙 GitHub</a>
                <a href="https://linkedin.com/in/seu-perfil" class="social-btn">💼 LinkedIn</a>
                <a href="mailto:seu.email@exemplo.com" class="social-btn">📧 Email</a>
            </div>
        </header>

        <div class="section">
            <h2>🚀 Sobre Mim</h2>
            <p style="font-size: 1.1em; line-height: 1.8;">
                Desenvolvedor apaixonado por criar soluções inovadoras e eficientes. 
                Sempre buscando aprender novas tecnologias e compartilhar conhecimento com a comunidade. 
                Focado em escrever código limpo, escalável e que faça a diferença.
            </p>
        </div>

        <div class="section">
            <h2>💻 Tecnologias</h2>
            <div class="skills-grid">
                <div class="skill-card">
                    <div class="skill-icon">🐍</div>
                    <strong>Python</strong>
                </div>
                <div class="skill-card">
                    <div class="skill-icon">⚛️</div>
                    <strong>React</strong>
                </div>
                <div class="skill-card">
                    <div class="skill-icon">🟢</div>
                    <strong>Node.js</strong>
                </div>
                <div class="skill-card">
                    <div class="skill-icon">🎨</div>
                    <strong>CSS/Tailwind</strong>
                </div>
                <div class="skill-card">
                    <div class="skill-icon">🗄️</div>
                    <strong>SQL/NoSQL</strong>
                </div>
                <div class="skill-card">
                    <div class="skill-icon">🐳</div>
                    <strong>Docker</strong>
                </div>
            </div>
        </div>

        <div class="section">
            <h2>📊 GitHub Stats</h2>
            <div class="stats">
                <div class="stat-card">
                    <div class="stat-number">50+</div>
                    <div>Repositórios</div>
                </div>
                <div class="stat-card">
                    <div class="stat-number">1000+</div>
                    <div>Commits</div>
                </div>
                <div class="stat-card">
                    <div class="stat-number">15+</div>
                    <div>Projetos</div>
                </div>
            </div>
        </div>

        <div class="section">
            <h2>🎯 Projetos em Destaque</h2>
            <div class="projects-grid">
                <div class="project-card">
                    <h3>🌐 Projeto Web App</h3>
                    <p>Aplicação full-stack com React e Node.js, incluindo autenticação e dashboard interativo.</p>
                    <p style="margin-top: 15px; opacity: 0.8;">🔧 React • Node.js • MongoDB</p>
                </div>
                <div class="project-card">
                    <h3>🤖 Bot Automatizado</h3>
                    <p>Bot inteligente para automatização de tarefas usando Python e APIs modernas.</p>
                    <p style="margin-top: 15px; opacity: 0.8;">🔧 Python • APIs • Automação</p>
                </div>
                <div class="project-card">
                    <h3>📱 App Mobile</h3>
                    <p>Aplicativo mobile responsivo com interface moderna e funcionalidades avançadas.</p>
                    <p style="margin-top: 15px; opacity: 0.8;">🔧 React Native • Firebase</p>
                </div>
            </div>
        </div>

        <footer>
            <p style="font-size: 1.2em;">💡 "Código é poesia em movimento"</p>
            <p style="margin-top: 10px;">⭐ Feito com 💜 por Matheus</p>
        </footer>
    </div>
</body>
</html>
