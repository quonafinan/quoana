
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<title>QUONA | Investimentos com IA</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">

<style>
:root {
    --primary: #00c6ff;
    --secondary: #0072ff;
    --dark: #0b0f19;
    --card: #121829;
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
    background-color: var(--dark);
    color: var(--text);
}

/* HEADER */
header {
    background: linear-gradient(135deg, var(--secondary), var(--primary));
    padding: 80px 20px;
    text-align: center;
}

header h1 {
    font-size: 48px;
    font-weight: 700;
}

header p {
    margin-top: 15px;
    font-size: 20px;
    max-width: 700px;
    margin-inline: auto;
}

/* NAV */
nav {
    background-color: #0f1528;
    display: flex;
    justify-content: center;
    gap: 25px;
    padding: 18px;
    position: sticky;
    top: 0;
    z-index: 100;
}

nav a {
    color: var(--text);
    text-decoration: none;
    font-weight: 600;
    transition: 0.3s;
}

nav a:hover {
    color: var(--primary);
}

/* SECTION */
section {
    max-width: 1200px;
    margin: auto;
    padding: 80px 20px;
}

section h2 {
    text-align: center;
    font-size: 34px;
    margin-bottom: 50px;
    color: var(--primary);
}

/* GRID */
.grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 30px;
}

/* CARD */
.card {
    background-color: var(--card);
    padding: 25px;
    border-radius: 16px;
    transition: 0.3s;
    box-shadow: 0 0 0 rgba(0,0,0,0);
}

.card:hover {
    transform: translateY(-6px);
    box-shadow: 0 15px 40px rgba(0,0,0,0.4);
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
    border-radius: 12px;
    border: none;
    margin-bottom: 15px;
}

/* FOOTER */
footer {
    background-color: #0f1528;
    padding: 30px;
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
    background-color: #25d366;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #fff;
    font-size: 28px;
    text-decoration: none;
    box-shadow: 0 0 20px rgba(0,0,0,0.4);
    z-index: 999;
}

.whatsapp:hover {
    background-color: #1ebe5d;
}
</style>
</head>

<body>

<header>
    <h1>QUONA</h1>
    <p>Plataforma inteligente de investimentos na bolsa de valores com Inteligência Artificial</p>
</header>

<nav>
    <a href="#tutoriais">Tutoriais</a>
    <a href="#investimentos">Investimentos</a>
    <a href="#duvidas">Dúvidas</a>
    <a href="#aprendizado">Aprendizado</a>
    <a href="#sacar">Como Sacar</a>
</nav>

<section id="tutoriais">
    <h2>Tutoriais</h2>
    <div class="grid">
        <div class="card">
            <iframe src="https://www.youtube.com/embed/VIDEO_ID"></iframe>
            <h3>Primeiros passos</h3>
            <p>Conheça a plataforma QUONA e como ativar a IA.</p>
        </div>
        <div class="card">
            <iframe src="https://www.youtube.com/embed/VIDEO_ID"></iframe>
            <h3>Configuração da IA</h3>
            <p>Automatize seus investimentos com segurança.</p>
        </div>
    </div>
</section>

<section id="investimentos">
    <h2>Investimentos</h2>
    <div class="grid">
        <div class="card">
            <iframe src="https://www.youtube.com/embed/VIDEO_ID"></iframe>
            <h3>Estratégias Inteligentes</h3>
            <p>Como a IA analisa o mercado financeiro.</p>
        </div>
        <div class="card">
            <iframe src="https://www.youtube.com/embed/VIDEO_ID"></iframe>
            <h3>Gestão de Risco</h3>
            <p>Proteção de capital e controle automatizado.</p>
        </div>
    </div>
</section>

<section id="duvidas">
    <h2>Dúvidas Frequentes</h2>
    <div class="grid">
        <div class="card">
            <iframe src="https://www.youtube.com/embed/VIDEO_ID"></iframe>
            <h3>Segurança</h3>
            <p>Como seus dados e investimentos são protegidos.</p>
        </div>
    </div>
</section>

<section id="aprendizado">
    <h2>Aprendizado</h2>
    <div class="grid">
        <div class="card">
            <iframe src="https://www.youtube.com/embed/VIDEO_ID"></iframe>
            <h3>Mercado Financeiro</h3>
            <p>Aprenda os fundamentos da bolsa.</p>
        </div>
        <div class="card">
            <iframe src="https://www.youtube.com/embed/VIDEO_ID"></iframe>
            <h3>IA na Prática</h3>
            <p>Como algoritmos operam em tempo real.</p>
        </div>
    </div>
</section>

<section id="sacar">
    <h2>Como Sacar</h2>
    <div class="grid">
        <div class="card">
            <iframe src="https://www.youtube.com/embed/VIDEO_ID"></iframe>
            <h3>Solicitação de Saque</h3>
            <p>Passo a passo para retirar seus lucros.</p>
        </div>
    </div>
</section>

<footer>
    © 2026 QUONA • Plataforma de Investimentos com IA
</footer>

<a class="whatsapp" href="https://wa.me/5599999999999" target="_blank">💬</a>

</body>
</html>
