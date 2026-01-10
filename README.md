<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Performance Gear for Riders & Athletes</title>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

/* ===== BODY (STATIC CINEMATIC BACKGROUND) ===== */
body {
  min-height: 100vh;
  background:
    radial-gradient(circle at top left, rgba(120, 0, 0, 0.45), transparent 55%),
    radial-gradient(circle at bottom right, rgba(120, 120, 120, 0.25), transparent 60%),
    #000;
  color: #fff;
  font-family: Arial, sans-serif;
}

/* ===== Neon Frame ===== */
.neon-frame {
  position: relative;
  max-width: 1200px;
  min-height: 100vh;
  margin: 20px auto;
  border: 3px solid #8b0000;
  box-shadow: 0 0 15px #8b0000, 0 0 40px #4d0000;
  background-color: rgba(0,0,0,0.75);
  border-radius: 12px;
}

/* ===== Header ===== */
header {
  padding: 16px 0;
  text-align: center;
}

header img {
  width: 140px;
  filter: drop-shadow(0 0 15px #8b0000);
}

/* ===== Hero ===== */
.hero {
  padding: 60px 20px;
  text-align: center;
}

.hero h1 {
  font-size: 2.6rem;
  color: #b30000;
}

.hero p {
  margin-top: 10px;
  opacity: 0.85;
}

.hero button {
  margin-top: 22px;
  padding: 10px 26px;
  border: 2px solid #8b0000;
  background: transparent;
  color: #b30000;
  cursor: pointer;
}

.hero button:hover {
  background: #8b0000;
  color: black;
}

/* ===== Sections ===== */
section {
  padding: 60px 20px;
  text-align: center;
}

section h2 {
  color: #b30000;
  margin-bottom: 30px;
}

/* ===== Cards ===== */
.cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 20px;
  max-width: 1000px;
  margin: auto;
}

.card {
  background: #111;
  border: 1px solid #8b0000;
  padding: 18px;
  border-radius: 12px;
}

.card img {
  width: 100%;
  height: 190px;
  object-fit: cover;
  border-radius: 10px;
  margin-bottom: 12px;
}

.card h3 {
  margin-bottom: 12px;
}

/* ===== Product Button ===== */
.product-btn {
  display: inline-block;
  padding: 10px 22px;
  background: #8b0000;
  color: white;
  text-decoration: none;
  border-radius: 8px;
}

.product-btn:hover {
  background: #b30000;
}

/* ===== Instagram Icon ===== */
.instagram-icon {
  position: fixed;
  bottom: 20px;
  left: 20px;
  width: 52px;
  height: 52px;
  background: rgba(0,0,0,0.4);
  border: 2px solid #8b0000;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  box-shadow: 0 0 12px #8b0000;
  backdrop-filter: blur(6px);
  transition: all 0.3s ease;
  animation: fadeIn 1.5s ease forwards;
  opacity: 0;
  z-index: 10;
}

.instagram-icon svg {
  width: 22px;
  height: 22px;
  fill: white;
}

.instagram-icon:hover {
  background: #8b0000;
  transform: scale(1.15);
  box-shadow: 0 0 20px #b30000, 0 0 40px #8b0000;
}

/* ===== Fade-in Animation ===== */
@keyframes fadeIn {
  to { opacity: 1; }
}

/* ===== Footer ===== */
footer {
  padding: 18px;
  text-align: center;
  opacity: 0.6;
}

/* ===== Responsive ===== */
@media (max-width: 768px) {
  .hero {
    padding: 40px 20px;
  }
  .card img {
    height: 160px;
  }
  .instagram-icon {
    width: 46px;
    height: 46px;
  }
}
</style>
</head>

<body>

<div class="neon-frame">

<header>
  <img src="https://github.com/user-attachments/assets/24e77390-843e-43cb-a7fd-7bfeeaa2fed6" alt="Logo">
</header>

<div class="hero">
  <h1>Performance Gear</h1>
  <p>Built for Riders & Athletes</p>
  <button>Explore</button>
</div>

<section>
  <h2>Our Products</h2>
  <div class="cards">
    <div class="card">
      <img src="https://github.com/user-attachments/assets/6d62477c-299b-4aeb-ba55-9a00a471930f">
      <h3>High Performance Gear</h3>
      <a href="#" class="product-btn">View Product</a>
    </div>
    <div class="card">
      <img src="https://github.com/user-attachments/assets/6d62477c-299b-4aeb-ba55-9a00a471930f">
      <h3>Athletic Wear</h3>
      <a href="#" class="product-btn">View Product</a>
    </div>
    <div class="card">
      <img src="https://github.com/user-attachments/assets/82290cd4-5806-460d-b310-7569734e6dfd">
      <h3>Rider Protection</h3>
      <a href="#" class="product-btn">View Product</a>
    </div>

  </div>
</section>

<section>
  <h2>Why Choose Us</h2>
  <p>Designed for speed, durability and comfort.</p>
</section>

<footer>
  © 2026 Performance Gear
</footer>

<!-- Instagram -->
<a href="https://www.instagram.com/_kombo1/" class="instagram-icon" target="_blank" aria-label="@_kombo1">
  <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
    <path d="M7 2C4.243 2 2 4.243 2 7v10c0 2.757 2.243 5 5 5h10c2.757 0 5-2.243 5-5V7c0-2.757-2.243-5-5-5H7zm10 2c1.654 0 3 1.346 3 3v10c0 1.654-1.346 3-3 3H7c-1.654 0-3-1.346-3-3V7c0-1.654 1.346-3 3-3h10zm-5 3a5 5 0 100 10 5 5 0 000-10zm0 2a3 3 0 110 6 3 3 0 010-6zm4.5-.75a1.25 1.25 0 11-2.5 0 1.25 1.25 0 012.5 0z"/>
  </svg>
</a>

</div>
</body>
</html>
