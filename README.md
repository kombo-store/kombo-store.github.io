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

/* ===== BODY ===== */
body {
  min-height: 100vh;
  background: #000;
  color: #fff;
  font-family: Arial, sans-serif;
  position: relative;
  overflow-x: hidden;
}

/* ===== DARK RED BLUR (CINEMATIC CORE) ===== */
body::before {
  content: "";
  position: fixed;
  width: 650px;
  height: 650px;
  background: #7a0000; /* أحمر غامق */
  filter: blur(260px);
  opacity: 0.45;
  top: -200px;
  left: -200px;
  z-index: -3;
}

/* ===== HEAVY GRAY SMOKE ===== */
body::after {
  content: "";
  position: fixed;
  width: 900px;
  height: 900px;
  background: radial-gradient(
    circle,
    rgba(200,200,200,0.45) 0%,
    rgba(120,120,120,0.25) 35%,
    rgba(40,40,40,0.15) 55%,
    rgba(0,0,0,0) 75%
  );
  filter: blur(220px);
  opacity: 0.55;
  bottom: -300px;
  right: -300px;
  z-index: -3;
}

/* ===== EXTRA SMOKE LAYER ===== */
.smoke-layer {
  position: fixed;
  inset: 0;
  background: radial-gradient(
    ellipse at top,
    rgba(160,160,160,0.18),
    rgba(0,0,0,0.9)
  );
  filter: blur(120px);
  z-index: -2;
}

/* ===== CINEMATIC VIGNETTE ===== */
.vignette {
  position: fixed;
  inset: 0;
  background: radial-gradient(
    ellipse at center,
    rgba(0,0,0,0) 40%,
    rgba(0,0,0,0.75) 100%
  );
  z-index: -1;
}

/* ===== Neon Frame ===== */
.neon-frame {
  position: relative;
  max-width: 1200px;
  min-height: 100vh;
  margin: 20px auto;
  border: 3px solid #8b0000;
  box-shadow: 0 0 20px #8b0000, 0 0 60px #4d0000;
  background-color: rgba(0,0,0,0.82);
  border-radius: 12px;
}

/* ===== Header ===== */
header {
  padding: 16px 0;
  text-align: center;
}

header img {
  width: 140px;
  filter: drop-shadow(0 0 20px #8b0000);
}

/* ===== Hero ===== */
.hero {
  padding: 70px 20px;
  text-align: center;
}

.hero h1 {
  font-size: 2.8rem;
  color: #b30000;
  letter-spacing: 1px;
}

.hero p {
  margin-top: 12px;
  opacity: 0.85;
}

.hero button {
  margin-top: 26px;
  padding: 12px 30px;
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
  padding: 70px 20px;
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
  gap: 22px;
  max-width: 1000px;
  margin: auto;
}

.card {
  background: rgba(15,15,15,0.95);
  border: 1px solid #8b0000;
  padding: 18px;
  border-radius: 12px;
  box-shadow: 0 0 15px rgba(139,0,0,0.5);
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
  position: absolute;
  bottom: 20px;
  left: 20px;
  width: 52px;
  height: 52px;
  background: black;
  border: 2px solid #8b0000;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  box-shadow: 0 0 18px #8b0000;
}

.instagram-icon svg {
  width: 22px;
  height: 22px;
  fill: white;
}

.instagram-icon:hover {
  background: #8b0000;
}

/* ===== Footer ===== */
footer {
  padding: 20px;
  text-align: center;
  opacity: 0.55;
}

/* ===== Responsive ===== */
@media (max-width: 768px) {
  .hero {
    padding: 50px 20px;
  }
  .card img {
    height: 160px;
  }
}
</style>
</head>

<body>

<div class="smoke-layer"></div>
<div class="vignette"></div>

<div class="neon-frame">

<header>
  <img src="https://github.com/user-attachments/assets/24e77390-843e-43cb-a7fd-7bfeeaa2fed6">
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

<footer>
  © 2026 Performance Gear
</footer>

<!-- Instagram -->
<a href="https://www.instagram.com/_kombo1/"
   class="instagram-icon"
   target="_blank">
  <svg xmlns="http://www.w3.org/2000/svg" width="26" height="26" fill="white" viewBox="0 0 24 24">
    <path d="M7 2C4.243 2 2 4.243 2 7v10c0 2.757 2.243 5 5 5h10c2.757 0 5-2.243 5-5V7c0-2.757-2.243-5-5-5H7zm10 2c1.654 0 3 1.346 3 3v10c0 1.654-1.346 3-3 3H7c-1.654 0-3-1.346-3-3V7c0-1.654 1.346-3 3-3h10zm-5 3a5 5 0 100 10 5 5 0 000-10zm0 2a3 3 0 110 6 3 3 0 010-6zm4.5-.75a1.25 1.25 0 11-2.5 0 1.25 1.25 0 012.5 0z"/>
  </svg>
</a>

</div>

</body>
</html>
