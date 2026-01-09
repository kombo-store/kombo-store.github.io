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
  min-height: 100vh;
}

/* ===== Neon Frame ===== */
.neon-frame {
  width: calc(100vw - 40px);
  min-height: calc(100vh - 40px);
  margin: 20px;
  border: 3px solid red;
  box-shadow: 0 0 20px red, 0 0 60px red;
}

/* ===== Header ===== */
header {
  padding: 20px;
  text-align: center;
}

header img {
  width: 160px;
  filter: drop-shadow(0 0 20px red);
}

/* ===== Hero ===== */
.hero {
  height: 70vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.hero h1 {
  font-size: 3rem;
  color: red;
}

.hero p {
  margin-top: 15px;
  opacity: 0.8;
}

.hero button {
  margin-top: 30px;
  padding: 12px 30px;
  background: transparent;
  border: 2px solid red;
  color: red;
  cursor: pointer;
  box-shadow: 0 0 15px red;
}

.hero button:hover {
  background: red;
  color: black;
}

/* ===== Sections ===== */
section {
  padding: 80px 20px;
  text-align: center;
}

section h2 {
  color: red;
  margin-bottom: 40px;
}

/* ===== Cards ===== */
.cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 25px;
  max-width: 1000px;
  margin: auto;
}

.card {
  background: #111;
  border: 1px solid red;
  padding: 20px;
  border-radius: 12px;
  box-shadow: 0 0 20px rgba(255,0,0,0.3);
}

.card img {
  width: 100%;
  height: 200px;
  object-fit: cover;
  border-radius: 10px;
  margin-bottom: 15px;
}

.card h3 {
  margin-bottom: 15px;
}

/* ===== Buttons ===== */
.product-btn {
  display: inline-block;
  padding: 12px 25px;
  background: red;
  color: white;
  text-decoration: none;
  font-weight: bold;
  border-radius: 8px;
  box-shadow: 0 0 10px red;
}

.product-btn:hover {
  background: #ff5555;
}

/* ===== Instagram ===== */
.instagram-link {
  position: fixed;
  bottom: 20px;
  left: 20px;
  color: white;
  text-decoration: none;
  font-weight: bold;
  border: 2px solid red;
  padding: 10px 18px;
  border-radius: 10px;
  box-shadow: 0 0 15px red;
}

.instagram-link:hover {
  background: red;
  color: black;
}

/* ===== Footer ===== */
footer {
  padding: 20px;
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

</div>

<!-- Instagram -->
<a href="https://www.instagram.com/_kombo1/" 
   class="instagram-link" target="_blank">
Instagram
</a>

</body>
</html>
