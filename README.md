# mely-naily
Luxury Nail Studio - Mely Naily
<!DOCTYPE html>
<html lang="hr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Mely Naily | Luxury Nail Studio</title>

<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;600&family=Montserrat:wght@300;400;500&display=swap" rel="stylesheet">

<style>
:root {
    --rose-light: #fdf2f6;
    --rose-soft: #f8dbe4;
    --rose-accent: #e6a6b6;
    --rose-dark: #c47a8a;
    --text-dark: #2b2b2b;
    --white: #ffffff;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    scroll-behavior: smooth;
}

body {
    font-family: 'Montserrat', sans-serif;
    background: linear-gradient(135deg, #fff, var(--rose-light));
    color: var(--text-dark);
    line-height: 1.7;
}

h1, h2, h3 {
    font-family: 'Cormorant Garamond', serif;
    letter-spacing: 1px;
}

.container {
    width: 90%;
    max-width: 1200px;
    margin: auto;
}

/* NAVBAR */
nav {
    position: fixed;
    width: 100%;
    padding: 20px 0;
    backdrop-filter: blur(10px);
    background: rgba(255,255,255,0.6);
    z-index: 1000;
}

nav .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

nav a {
    text-decoration: none;
    color: var(--text-dark);
    margin-left: 30px;
    font-weight: 400;
    transition: 0.3s;
}

nav a:hover {
    color: var(--rose-dark);
}

/* HERO */
.hero {
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    background: linear-gradient(rgba(255,255,255,0.6), rgba(255,255,255,0.6)),
    url('https://images.unsplash.com/photo-1604654894610-df63bc536371') center/cover no-repeat;
}

.hero h1 {
    font-size: 4rem;
    margin-bottom: 20px;
    animation: fadeIn 1.5s ease forwards;
}

.hero p {
    font-size: 1.2rem;
    margin-bottom: 40px;
    animation: fadeIn 2s ease forwards;
}

.btn {
    padding: 14px 36px;
    border-radius: 50px;
    background: linear-gradient(45deg, var(--rose-accent), var(--rose-dark));
    color: white;
    text-decoration: none;
    font-weight: 500;
    letter-spacing: 1px;
    box-shadow: 0 10px 30px rgba(196,122,138,0.3);
    transition: 0.4s ease;
}

.btn:hover {
    transform: translateY(-3px);
    box-shadow: 0 15px 40px rgba(196,122,138,0.4);
}

/* SECTIONS */
section {
    padding: 120px 0;
}

.section-title {
    text-align: center;
    font-size: 2.5rem;
    margin-bottom: 70px;
}

/* ABOUT */
.about {
    text-align: center;
    max-width: 800px;
    margin: auto;
}

/* SERVICES */
.services {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 40px;
}

.service-card {
    padding: 40px;
    border-radius: 25px;
    background: rgba(255,255,255,0.6);
    backdrop-filter: blur(15px);
    box-shadow: 0 10px 40px rgba(0,0,0,0.05);
    text-align: center;
    transition: 0.4s ease;
}

.service-card:hover {
    transform: translateY(-8px);
}

/* GALLERY */
.gallery {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 20px;
}

.gallery img {
    width: 100%;
    border-radius: 20px;
    transition: 0.5s ease;
}

.gallery img:hover {
    transform: scale(1.05);
}

/* BOOKING */
.booking {
    text-align: center;
    background: linear-gradient(135deg, var(--rose-soft), var(--rose-light));
    padding: 100px 20px;
    border-radius: 40px;
}

/* FOOTER */
footer {
    text-align: center;
    padding: 40px 0;
    background: var(--rose-dark);
    color: white;
    font-size: 0.9rem;
}

/* ANIMATIONS */
@keyframes fadeIn {
    from { opacity: 0; transform: translateY(20px);}
    to { opacity: 1; transform: translateY(0);}
}

@media(max-width:768px){
    .hero h1 {
        font-size: 2.8rem;
    }
}
</style>
</head>
<body>

<nav>
    <div class="container">
        <h3>Mely Naily</h3>
        <div>
            <a href="#about">O nama</a>
            <a href="#services">Usluge</a>
            <a href="#gallery">Galerija</a>
            <a href="#booking">Rezervacija</a>
        </div>
    </div>
</nav>

<section class="hero">
    <div>
        <h1>Mely Naily</h1>
        <p>Luksuzna njega i dizajn noktiju s preciznošću i elegancijom.</p>
        <a href="https://calendly.com/melany-camoo/melynaily" target="_blank" class="btn">Rezerviraj termin</a>
    </div>
</section>

<section id="about">
    <div class="container about">
        <h2 class="section-title">O nama</h2>
        <p>
        U Mely Naily studiju svaki detalj je pažljivo osmišljen kako bi pružio osjećaj luksuza, elegancije i savršene estetike. 
        Svaki set noktiju izrađuje se s preciznošću i strašću prema ljepoti.
        </p>
    </div>
</section>

<section id="services">
    <div class="container">
        <h2 class="section-title">Usluge</h2>
        <div class="services">
            <div class="service-card">Gel nokti</div>
            <div class="service-card">Trajni lak</div>
            <div class="service-card">Nadogradnja noktiju</div>
            <div class="service-card">Korekcija</div>
            <div class="service-card">Nail art dizajn</div>
        </div>
    </div>
</section>

<section id="gallery">
    <div class="container">
        <h2 class="section-title">Galerija radova</h2>
        <div class="gallery">
            <img src="https://images.unsplash.com/photo-1583001809873-a128495da465">
            <img src="https://images.unsplash.com/photo-1616394584738-fc6
