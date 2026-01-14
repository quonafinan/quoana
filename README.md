<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<title>QUONA | Investimentos com IA</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;800&display=swap" rel="stylesheet">

<style>
:root {
    --primary: #00e0ff;
    --secondary: #0066ff;
    --dark: #0a0f1f;
    --card: rgba(18, 24, 41, 0.85);
    --text: #f1f5f9;
    --muted: #9ca3af;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Inter', sans-serif;
    background: radial-gradient(circle at top, #0f1b3d, #050814);
    color: var(--text);
}

/* HEADER */
header {
    position: relative;
    padding: 120px 20px;
    text-align: center;
    background:
        linear-gradient(rgba(5,8,20,0.85), rgba(5,8,20,0.95)),
        url("https://images.unsplash.com/photo-1642790553016-73f99f92e1bb") center/cover no-repeat;
}

header h1 {
    font-size: 56px;
    font-weight: 800;
    letter-spacing: 2px;
    background: linear-gradient(90deg, var(--primary), var(--secondary));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
}

header p {
    margin-top: 20px;
    font-size: 22px;
    max-width: 760px;
    margin-inline: auto;
    color: var(--muted);
}

/* NAV */
nav {
    background: rgba(15,21,40,0.95);
    backdrop-filter: blur(10px);
    display: flex;
    justify-content: center;
    gap: 30px;
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
    padding: 90px 20px;
}

section h2 {
    text-align: center;
    font-size: 38px;
    margin-bottom: 60px;
    background: linear-gradient(90deg, var(--primary), var(--secondary));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
}

/* GRID */
.grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 35px;
}

/* CARD */
.card {
    background: var(--card);
    border-radius: 20px;
    overflow: hidden;
    transition: 0.4s;
    backdrop-filter: blur(15px);
    border: 1px solid rgba(255,255,255,0.05);
}

.card:hover {
    transform: translateY(-10px) scale(1.02);
    box-shadow: 0 30px 60px rgba(0,0,0,0.6);
}

/* CARD IMAGE */
.card .thumb {
    height: 160px;
    background-size: cover;
    background-position: center;
    position: relative;
}

.card .thumb::after {
    content: "";
    position: absolute;
    inset: 0;
    background: linear-gradient(to top, rgba(10,15,31,0.9), transparent);
}

/* CARD CONTENT */
.card-content {
    padding: 25px;
}

.card h3 {
    margin-bottom: 12px;
    font-size: 20px;
}

.card p {
    color: var(--muted);
    font-size: 15px;
    margin-bottom: 15px;
}

.card iframe {
    width: 100%;
    height: 200px;
    border-radius: 14px;
    border: none;
}

/* FOOTER */
footer {
    background: #0b1025;
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
    width: 62px;
    height: 62px;
    background-color: #25d366;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #fff;
    font-size: 30px;
    text-decoration: none;
    box-shadow: 0 0 30px rgba(0,0,0,0.5);
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
    <p>Investimentos inteligentes na bolsa de valores com Inteligência Artificial de última geração</p>
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
    <div class="thumb" style="background-image:url('https://images.unsplash.com/photo-1551288049-bebda4e38f71')"></div>
    <div class="card-content">
        <h3>Primeiros Passos</h3>
        <p>Aprenda a começar e ativar a IA da QUONA.</p>
        <iframe src="https://www.youtube.com/embed/VIDEO_ID"></iframe>
    </div>
</div>

<div class="card">
    <div class="thumb" style="background-image:url('https://images.unsplash.com/photo-1620712943543-bcc4688e7485')"></div>
    <div class="card-content">
        <h3>Configuração da IA</h3>
        <p>Automatize seus investimentos com segurança.</p>
        <iframe src="https://www.youtube.com/embed/VIDEO_ID"></iframe>
    </div>
</div>

</div>
</section>

<footer>
© 2026 QUONA • Plataforma de Investimentos com IA
</footer>

<a class="whatsapp" href="https://wa.me/5599999999999" target="_blank">💬</a>

</body>
</html>
