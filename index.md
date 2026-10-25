
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>CodeWithPrasoon</title>
<style>
* { box-sizing: border-box; }

body {
    margin: 0;
    font-family: Arial, sans-serif;
    color: #222;
}
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 20px;
    padding: 20px 8%;
    background: #142d60;
    color: white;
}
nav { display: flex; flex-wrap: wrap; gap: 20px; }
nav a { color: white; text-decoration: none; }

.hero {
    display: grid;
    grid-template-columns: 1fr 1fr;
    align-items: center;
    gap: 30px;
    padding: 60px 8%;
    background: #eaf3ff;
}
.hero h1 { font-size: clamp(2rem, 4vw, 3rem); }
.hero p { font-size: 1.1rem; line-height: 1.6; }
.hero img {
    width: 100%;
    max-width: 450px;
    height: auto;
}
.btn {
    display: inline-block;
    background: orange;
    color: black;
    padding: 12px 25px;
    border-radius: 6px;
    text-decoration: none;
}
.features { padding: 50px 8%; text-align: center; }
.cards {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 20px;
}
.card {
    background: #f1f1f1;
    padding: 25px;
    border-radius: 10px;
    min-width: 0;
    overflow-wrap: anywhere;
}
footer {
    background: #142d60;
    color: white;
    text-align: center;
    padding: 20px;
}

/* Tablet */
@media (max-width: 900px) {
    header { flex-wrap: wrap; }
    .hero { gap: 20px; padding: 40px 6%; }
    .cards { grid-template-columns: repeat(2, minmax(0, 1fr)); }
}

/* Mobile */
@media (max-width: 600px) {
    header { flex-direction: column; text-align: center; }
    nav { justify-content: center; }
    .hero { grid-template-columns: 1fr; text-align: center; }
    .hero img { margin: auto; }
    .cards { grid-template-columns: 1fr; }
    .features { padding: 30px 6%; }
}
</style>
</head>
<body>

<header>
    <h2>CodeWithPrasoon</h2>
    <nav>
        <a href="#home">Home</a>
        <a href="#features">Features</a>
        <a href="#contact">Contact</a>
    </nav>
</header>

<main>
    <section class="hero" id="home">
        <div>
            <h1>Learn Web Development</h1>
            <p>Master HTML, CSS and JavaScript
            to build modern responsive websites.</p>
            <a href="#features" class="btn">Get Started</a>
        </div>
        <img src="images/coding.jpg" alt="Web development illustration">
    </section>

    <section class="features" id="features">
        <h2>Our Features</h2>
        <div class="cards">
            <article class="card">
                <h3>HTML</h3>
                <p>Learn website structure.</p>
            </article>
            <article class="card">
                <h3>CSS</h3>
                <p>Create beautiful designs.</p>
            </article>
            <article class="card">
                <h3>JavaScript</h3>
                <p>Build interactive websites.</p>
            </article>
        </div>
    </section>
</main>

<footer id="contact">
    <p>Contact: anandprasoon6@gmail.com</p>
    <p>&copy; 2026 Prasoon Anand</p>
</footer>

</body>
</html>
