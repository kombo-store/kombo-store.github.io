<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Performance Gear for Riders & Athletes</title>

<style>
* { box-sizing: border-box; margin: 0; padding: 0; }

/* ===== BODY ===== */
body {
  min-height: 100vh;
  background: #000;
  color: #fff;
  font-family: Arial, sans-serif;
  overflow-x: hidden;
}

/* ===== BACKGROUND EFFECTS ===== */
body::before {
  content: "";
  position: fixed;
  width: 520px;
  height: 520px;
  background: red;
  filter: blur(230px);
  opacity: 0.35;
  top: -160px;
  left: -160px;
  z-index: -2;
}

body::after {
  content: "";
  position: fixed;
  width: 700px;
  height: 700px;
  background: radial-gradient(circle, rgba(200,200,200,0.35), rgba(0,0,0,0));
  filter: blur(180px);
  opacity: 0.45;
  bottom: -200px;
  right: -200px;
  z-index: -2;
}

/* ===== TOP NAV ===== */
.top-nav {
  position: fixed;
  top: 0;
  width: 100%;
  height: 64px;
  background: rgba(0,0,0,0.9);
  backdrop-filter: blur(12px);
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 40px;
  z-index: 9000;
  border-bottom: 1px solid rgba(255,0,0,0.3);
  box-shadow: 0 0 15px rgba(255,0,0,0.25);
}

.top-nav img {
  height: 34px;
  filter: drop-shadow(0 0 12px red);
}

.nav-links {
  display: flex;
  gap: 28px;
}

.nav-links a {
  color: #fff;
  text-decoration: none;
  font-size: 14px;
  letter-spacing: 1px;
  position: relative;
  transition: 0.3s;
}

.nav-links a::after {
  content: "";
  position: absolute;
  bottom: -8px;
  left: 0;
  width: 0;
  height: 2px;
  background: red;
  transition: 0.3s;
}

.nav-links a:hover {
  color: red;
}

.nav-links a:hover::after {
  width: 100%;
}

/* ===== FRAME ===== */
.neon-frame {
  max-width: 1200px;
  min-height: 100vh;
  margin: 0 auto;
  padding-top: 100px;
  border: 3px solid red;
  box-shadow: 0 0 15px red, 0 0 40px red;
  background: rgba(0,0,0,0.78);
  border-radius: 12px;
  position: relative;
  z-index: 1;
}

/* ===== HEADER ===== */
header {
  padding: 18px;
  text-align: center;
}

header img {
  width: 140px;
  filter: drop-shadow(0 0 15px red);
}

/* ===== HERO ===== */
.hero {
  padding: 60px 20px;
  text-align: center;
}

.hero h1 {
  font-size: 2.6rem;
  color: red;
}

.hero p {
  margin-top: 10px;
  opacity: 0.85;
}

.hero button {
  margin-top: 22px;
  padding: 10px 26px;
  border: 2px solid red;
  background: transparent;
  color: red;
  cursor: pointer;
  transition: 0.3s;
}

.hero button:hover {
  background: red;
  color: black;
}

/* ===== SECTIONS ===== */
section {
  padding: 60px 20px;
  text-align: center;
}

section h2 {
  color: red;
  margin-bottom: 30px;
}

/* ===== CARDS ===== */
.cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 20px;
  max-width: 1000px;
  margin: auto;
}

.card {
  background: #111;
  border: 1px solid red;
  padding: 18px;
  border-radius: 12px;
  transition: 0.3s;
}

.card:hover {
  transform: translateY(-6px);
  box-shadow: 0 0 15px red;
}

.card img {
  width: 100%;
  height: 190px;
  object-fit: cover;
  border-radius: 10px;
  margin-bottom: 12px;
}

/* ===== BUTTON ===== */
.product-btn {
  display: inline-block;
  padding: 10px 22px;
  background: red;
  color: white;
  text-decoration: none;
  border-radius: 8px;
  transition: 0.3s;
}

.product-btn:hover {
  background: #ff5555;
  transform: scale(1.05);
}

/* ===== INSTAGRAM ===== */
.instagram-icon {
  position: fixed;
  bottom: 24px;
  left: 24px;
  width: 54px;
  height: 54px;
  background: black;
  border: 2px solid red;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  box-shadow: 0 0 15px red;
  z-index: 9500;
  transition: 0.3s;
}

.instagram-icon:hover {
  background: red;
  transform: scale(1.08);
}

.instagram-icon svg {
  width: 22px;
  height: 22px;
  fill: white;
}

/* ===== LIGHTBOX ===== */
#lightbox {
  position: fixed;
  inset: 0;
  background: rgba(0,0,0,0.95);
  display: none;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  z-index: 9800;
}

#lightbox img {
  max-width: 80%;
  max-height: 80%;
  border: 3px solid red;
  border-radius: 12px;
}

#lightbox-controls button {
  margin: 10px;
  padding: 6px 14px;
  background: black;
  color: red;
  border: 2px solid red;
  border-radius: 6px;
  cursor: pointer;
}
</style>
</head>

<body>

<!-- TOP NAV -->
<div class="top-nav">
  <img src="https://github.com/user-attachments/assets/24e77390-843e-43cb-a7fd-7bfeeaa2fed6">
  <div class="nav-links">
    <a href="#">Products</a>
    <a href="#">Media</a>
    <a href="#">Athletes</a>
    <a href="#">About</a>
    <a href="#">Support</a>
  </div>
</div>

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
    <div class="card" data-images='[
      "https://github.com/user-attachments/assets/6d62477c-299b-4aeb-ba55-9a00a471930f",
      "https://github.com/user-attachments/assets/82290cd4-5806-460d-b310-7569734e6dfd"
    ]'>
      <img src="https://github.com/user-attachments/assets/6d62477c-299b-4aeb-ba55-9a00a471930f">
      <h3>Athletic Wear</h3>
      <a href="#" class="product-btn">View Product</a>
    </div>
    <div class="card" data-images='[
      "https://github.com/user-attachments/assets/ef44d2a3-a222-4fb3-ae27-e79fc5e8dffc"
    ]'>
      <img src="https://github.com/user-attachments/assets/ef44d2a3-a222-4fb3-ae27-e79fc5e8dffc">
      <h3>Hoodie</h3>
      <a href="#" class="product-btn">View Product</a>
    </div>

  </div>
</section>

<footer style="text-align:center;opacity:.6;padding:18px">
  © 2026 Performance Gear
</footer>

</div>

<!-- INSTAGRAM -->
<a href="https://www.instagram.com/_kombo1/" class="instagram-icon" target="_blank">
  <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
    <path d="M7 2C4.243 2 2 4.243 2 7v10c0 2.757 2.243 5 5 5h10c2.757 0 5-2.243 5-5V7c0-2.757-2.243-5-5-5H7zm10 2c1.654 0 3 1.346 3 3v10c0 1.654-1.346 3-3 3H7c-1.654 0-3-1.346-3-3V7c0-1.654 1.346-3 3-3h10z"/>
  </svg>
</a>

<!-- LIGHTBOX -->
<div id="lightbox">
  <img src="">
  <div id="lightbox-controls">
    <button id="prev">Prev</button>
    <button id="next">Next</button>
    <button id="close">Close</button>
  </div>
</div>

<script>
const lightbox = document.getElementById('lightbox');
const lightboxImg = lightbox.querySelector('img');
const cards = document.querySelectorAll('.card');
let imgs = [], index = 0;

cards.forEach(card => {
  card.querySelector('.product-btn').onclick = e => {
    e.preventDefault();
    imgs = JSON.parse(card.dataset.images);
    index = 0;
    lightboxImg.src = imgs[index];
    lightbox.style.display = 'flex';
  };
});

prev.onclick = () => {
  index = (index - 1 + imgs.length) % imgs.length;
  lightboxImg.src = imgs[index];
};

next.onclick = () => {
  index = (index + 1) % imgs.length;
  lightboxImg.src = imgs[index];
};

close.onclick = () => lightbox.style.display = 'none';
</script>

</body>
</html>
