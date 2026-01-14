<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<title>QUONA | Investimentos Inteligentes com IA</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">

<style>
:root {
    --primary: #0a84ff;
    --dark: #0b1220;
    --dark2: #0f172a;
    --card: #111827;
    --text: #e5e7eb;
    --muted: #9ca3af;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Inter', sans-serif;
    background: var(--dark);
    color: var(--text);
}

/* HERO */
.hero {
    background: linear-gradient(rgba(10,20,40,0.85), rgba(10,20,40,0.85)),
    url("https://images.unsplash.com/photo-1559526324-593bc073d938") center/cover no-repeat;
    padding: 140px 20px;
    text-align: center;
}

.hero h1 {
    font-size: 56px;
    font-weight: 700;
}

.hero p {
    margin-top: 20px;
    font-size: 20px;
    max-width: 800px;
    margin-inline: auto;
    color: var(--muted);
}

.hero button {
    margin-top: 40px;
    padding: 15px 35px;
    font-size: 16px;
    font-weight: 600;
    border: none;
    border-radius: 8px;
    background: var(--primary);
    color: white;
    cursor: pointer;
}

.hero button:hover {
    opacity: 0.9;
}

/* NAV */
nav {
    background: rgba(15,23,42,0.9);
    backdrop-filter: blur(8px);
    position: sticky;
    top: 0;
    z-index: 100;
    display: flex;
    justify-content: center;
    gap: 30px;
    padding: 18px;
}

nav a {
    color: var(--text);
    text-decoration: none;
    font-weight: 600;
}

nav a:hover {
    color: var(--primary);
}

/* SECTION */
section {
    max-width: 1200px;
    margin: auto;
    padding: 100px 20px;
}

section h2 {
    font-size: 38px;
    margin-bottom: 15px;
}

section .desc {
    color: var(--muted);
    max-width: 700px;
    margin-bottom: 60px;
}

/* GRID */
.grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 40px;
}

/* CARD */
.card {
    background: var(--card);
    border-radius: 18px;
    overflow: hidden;
    box-shadow: 0 20px 50px rgba(0,0,0,0.5);
}

.card img {
    width: 100%;
    height: 200px;
    object-fit: cover;
}

.card .content {
    padding: 25px;
}

.card h3 {
    margin-bottom: 12px;
}

.card p {
    color: var(--muted);
    font-size: 15px;
}

.card iframe {
    width: 100%;
    height: 200px;
    border: none;
}

/* FOOTER */
footer {
    background: var(--dark2);
    padding: 40px;
    text-align: center;
    color: var(--muted);
    font-size: 14px;
}

/* WHATSAPP */
.whatsapp {
    position: fixed;
    bottom: 25px;
    right: 25px;
    width: 60px;
    height: 60px;
    background: #25d366;
    color: white;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 28px;
    text-decoration: none;
    z-index: 999;
}
</style>
</head>

<body>

<!-- HERO -->
<div class="hero">
    <h1>QUONA</h1>
    <p>
        Tecnologia de ponta em investimentos automatizados na bolsa de valores
        com Inteligência Artificial avançada.
    </p>
    <button onclick="window.location.href='#investimentos'">
        Conhecer Plataforma
    </button>
</div>

<!-- NAV -->
<nav>
    <a href="#tutoriais">Tutoriais</a>
    <a href="#investimentos">Investimentos</a>
    <a href="#aprendizado">Aprendizado</a>
    <a href="#duvidas">Dúvidas</a>
    <a href="#sacar">Como Sacar</a>
</nav>

<!-- TUTORIAIS -->
<section id="tutoriais">
    <h2>Tutoriais</h2>
    <p class="desc">Guias completos para operar com segurança na plataforma QUONA.</p>

    <div class="grid">
        <div class="card">
            <img src="https://images.unsplash.com/photo-1556155092-8707de31f9c4">
            <div class="content">
                <iframe src="https://www.youtube.com/embed/VIDEO_ID"></iframe>
                <h3>Primeiros Passos</h3>
                <p>Criação de conta e ativação da IA.</p>
            </div>
        </div>

        <div class="card">
            <img src="https://images.unsplash.com/photo-1551836022-d5d88e9218df">
            <div class="content">
                <iframe src="https://www.youtube.com/embed/VIDEO_ID"></iframe>
                <h3>Configurações Avançadas</h3>
                <p>Gerenciamento de risco e automações.</p>
            </div>
        </div>
    </div>
</section>

<!-- INVESTIMENTOS -->
<section id="investimentos">
    <h2>Investimentos</h2>
    <p class="desc">Nossa IA opera com base em dados, análise técnica e controle de risco.</p>

    <div class="grid">
        <div class="card">
            <img src="https://images.unsplash.com/photo-1642790106117-e829e14a795f">
            <div class="content">
                <iframe src="https://www.youtube.com/embed/VIDEO_ID"></iframe>
                <h3>Estratégias Inteligentes</h3>
                <p>Operações automatizadas e decisões baseadas em dados.</p>
            </div>
        </div>

        <div class="card">
            <img src="https://images.unsplash.com/photo-1559526324-4b87b5e36e44">
            <div class="content">
                <iframe src="https://www.youtube.com/embed/VIDEO_ID"></iframe>
                <h3>Proteção de Capital</h3>
                <p>Gestão profissional de risco.</p>
            </div>
        </div>
    </div>
</section>

<!-- APRENDIZADO -->
<section id="aprendizado">
    <h2>Aprendizado</h2>
    <p class="desc">Conteúdo educacional para investidores de todos os níveis.</p>

    <div class="grid">
        <div class="card">
            <img src="https://images.unsplash.com/photo-1526628953301-3e589a6a8b74">
            <div class="content">
                <iframe src="https://www.youtube.com/embed/VIDEO_ID"></iframe>
                <h3>Mercado Financeiro</h3>
                <p>Fundamentos e conceitos essenciais.</p>
            </div>
        </div>
    </div>
</section>

<!-- DÚVIDAS -->
<section id="duvidas">
    <h2>Dúvidas Frequentes</h2>
    <p class="desc">Transparência e segurança em primeiro lugar.</p>

    <div class="grid">
        <div class="card">
            <img src="https://images.unsplash.com/photo-1581092160562-40aa08e78837">
            <div class="content">
                <iframe src="https://www.youtube.com/embed/VIDEO_ID"></iframe>
                <h3>Segurança e Saques</h3>
                <p>Como protegemos seus dados e fundos.</p>
            </div>
        </div>
    </div>
</section>

<!-- SACAR -->
<section id="sacar">
    <h2>Como Sacar</h2>
    <p class="desc">Processo simples, transparente e rápido.</p>

    <div class="grid">
        <div class="card">
            <img src="https://images.unsplash.com/photo-1565372195458-9de0b320ef04">
            <div class="content">
                <iframe src="https://www.youtube.com/embed/VIDEO_ID"></iframe>
                <h3>Solicitar Saque</h3>
                <p>Passo a passo para retirada dos lucros.</p>
            </div>
        </div>
    </div>
</section>

<footer>
    © 2026 QUONA • Tecnologia Financeira • Investimentos com Inteligência Artificial
</footer>

<a class="whatsapp" href="https://wa.me/5599999999999" target="_blank">💬</a>

</body>
</html>
