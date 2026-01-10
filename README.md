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

/* ===== BODY BACKGROUND ===== */
body {
  min-height: 100vh;
  background: #000;
  color: #fff;
  font-family: Arial, sans-serif;
  position: relative;
  overflow-x: hidden;
}

/* ===== RED BLUR ===== */
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

/* ===== GRAY SMOKE ===== */
body::after {
  content: "";
  position: fixed;
  width: 700px;
  height: 700px;
  background: radial-gradient(
    circle,
    rgba(200,200,200,0.35) 0%,
    rgba(120,120,120,0.18) 40%,
    rgba(0,0,0,0) 70%
  );
  filter: blur(180px);
  opacity: 0.45;
  bottom: -200px;
  right: -200px;
  z-index: -2;
}

/* ===== Neon Frame ===== */
.neon-frame {
  position: relative;
  max-width: 1200px;
  min-height: 100vh;
  margin: 20px auto;
  border: 3px solid red;
  box-shadow: 0 0 15px red, 0 0 40px red;
  background-color: rgba(0,0,0,0.78);
  border-radius: 12px;
}

/* ===== Header ===== */
header {
  padding: 16px 0;
  text-align: center;
}

header img {
  width: 140px;
  filter: drop-shadow(0 0 15px red);
}

/* ===== Hero ===== */
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
}

.hero button:hover {
  background: red;
  color: black;
}

/* ===== Sections ===== */
section {
  padding: 60px 20px;
  text-align: center;
}

section h2 {
  color: red;
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
  border: 1px solid red;
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
  background: red;
  color: white;
  text-decoration: none;
  border-radius: 8px;
}

.product-btn:hover {
  background: #ff5555;
}

/* ===== Instagram Icon ثابت ===== */
.instagram-icon {
  position: fixed;
  bottom: 20px;
  left: 20px;
  width: 52px;
  height: 52px;
  background: black;
  border: 2px solid red;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  box-shadow: 0 0 12px red;
  z-index: 1000;
}

.instagram-icon svg {
  width: 22px;
  height: 22px;
  fill: white;
}

.instagram-icon:hover {
  background: red;
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
}

/* ===== Lightbox ===== */
#lightbox {
  display: none;
  position: fixed;
  z-index: 2000;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0,0,0,0.9);
  justify-content: center;
  align-items: center;
}

#lightbox img {
  max-width: 80%;
  max-height: 80%;
  border: 3px solid red;
  border-radius: 10px;
}

#lightbox .close-btn {
  position: absolute;
  top: 20px;
  right: 20px;
  color: white;
  font-size: 28px;
  cursor: pointer;
}
</style>
</head>

<body>

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
      <h3>High Performance Gear</h3>
      <a href="#" class="product-btn">View Product</a>
    </div>
    <div class="card" data-images='[
      "https://github.com/user-attachments/assets/6d62477c-299b-4aeb-ba55-9a00a471930f",
      "https://github.com/user-attachments/assets/82290cd4-5806-460d-b310-7569734e6dfd"
    ]'>
      <img src="https://github.com/user-attachments/assets/6d62477c-299b-4aeb-ba55-9a00a471930f">
      <h3>Athletic Wear</h3>
      <a href="#" class="product-btn">View Product</a>
    </div>
    <div class="card" data-images='[
      "https://github.com/user-attachments/assets/82290cd4-5806-460d-b310-7569734e6dfd",
      "https://github.com/user-attachments/assets/6d62477c-299b-4aeb-ba55-9a00a471930f"
    ]'>
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

<!-- ===== Lightbox ===== -->
<div id="lightbox">
  <span class="close-btn">&times;</span>
  <img src="" alt="Product Image">
</div>

<script>
const lightbox = document.getElementById('lightbox');
const lightboxImg = lightbox.querySelector('img');
const closeBtn = lightbox.querySelector('.close-btn');
let currentImages = [];
let currentIndex = 0;

document.querySelectorAll('.product-btn').forEach(btn => {
  btn.addEventListener('click', e => {
    e.preventDefault();
    const card = btn.closest('.card');
    currentImages = JSON.parse(card.dataset.images);
    currentIndex = 0;
    lightboxImg.src = currentImages[currentIndex];
    lightbox.style.display = 'flex';
  });
});

lightbox.addEventListener('click', e => {
  if(e.target !== lightboxImg && e.target !== closeBtn){
    // Next image on background click
    currentIndex = (currentIndex + 1) % currentImages.length;
    lightboxImg.src = currentImages[currentIndex];
  }
});

closeBtn.addEventListener('click', () => {
  lightbox.style.display = 'none';
});
</script>

</div>

</body>
</html>
