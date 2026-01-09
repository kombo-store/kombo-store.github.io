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

body {
  background: #000;
  color: #fff;
  font-family: Arial, sans-serif;
}

/* ===== Frame ===== */
.neon-frame {
  position: relative;
  max-width: 1200px;
  margin: 20px auto;
  border: 3px solid red;
  box-shadow: 0 0 15px red, 0 0 40px red;
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

/* ===== Products ===== */
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

/* ===== Button ===== */
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

/* ===== Instagram Icon ===== */
.instagram-icon {
  position: absolute;
  bottom: 16px;
  left: 16px;
  width: 52px;
  height: 52px;
  background: black;
  border: 2px solid red;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  box-shadow: 0 0 12px red;
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
      <a href="https://github.com/user-attachments/assets/6d62477c-299b-4aeb-ba55-9a00a471930f"
         class="product-btn" target="_blank">View Product</a>
    </div>
    <div class="card">
      <img src="https://github.com/user-attachments/assets/6d62477c-299b-4aeb-ba55-9a00a471930f">
      <h3>Athletic Wear</h3>
      <a href="https://github.com/user-attachments/assets/6d62477c-299b-4aeb-ba55-9a00a471930f"
         class="product-btn" target="_blank">View Product</a>
    </div>
    <div class="card">
      <img src="https://github.com/user-attachments/assets/82290cd4-5806-460d-b310-7569734e6dfd">
      <h3>Rider Protection</h3>
      <a href="https://github.com/user-attachments/assets/82290cd4-5806-460d-b310-7569734e6dfd"
         class="product-btn" target="_blank">View Product</a>
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
<a href="https://www.instagram.com/_kombo1/"
   class="instagram-icon"
   target="_blank"
   aria-label="Instagram">
  <svg viewBox="0 0 448 512">
    <path d="M224.1 141c-63.6 0-114.9 51.3-114.9 114.9s51.3 114.9 114.9 114.9S339 319.5 339 255.9 287.7 141 224.1 141zm0 189.6c-41.3 0-74.7-33.4-74.7-74.7s33.4-74.7 74.7-74.7 74.7 33.4 74.7 74.7-33.4 74.7-74.7 74.7zm146.4-194.3c0 14.9-12 26.9-26.9 26.9s-26.9-12-26.9-26.9 12-26.9 26.9-26.9 26.9 12 26.9 26.9zM398.8 80.5c-1.7-35.3-9.9-66.6-36.2-92.9C336.4-18.7 305.1-26.9 269.8-28.6c-35.5-1.7-56.1-1.7-91.6 0C142.9-26.9 111.6-18.7 85.3 7.6 59 33.9 50.8 65.2 49.1 100.5c-1.7 35.5-1.7 56.1 0 91.6 1.7 35.3 9.9 66.6 36.2 92.9 26.3 26.3 57.6 34.5 92.9 36.2 35.5 1.7 56.1 1.7 91.6 0 35.3-1.7 66.6-9.9 92.9-36.2 26.3-26.3 34.5-57.6 36.2-92.9 1.7-35.5 1.7-56.1 0-91.6z"/>
  </svg>
</a>

</div>

</body>
</html>
