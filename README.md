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
  display: flex;
  justify-content: center;
  align-items: center;
}

/* ===== Neon Frame ===== */
.neon-frame {
  width: calc(100vw - 40px);
  min-height: calc(100vh - 40px);
  border: 3px solid red;
  box-shadow:
    0 0 15px red,
    0 0 40px red,
    0 0 80px red;
  animation: glow 2s ease-in-out infinite alternate;
}

@keyframes glow {
  from {
    box-shadow: 0 0 15px red, 0 0 40px black, 0 0 80px red;
  }
  to {
    box-shadow: 0 0 25px red, 0 0 60px black, 0 0 120px red;
  }
}

/* ===== Layout ===== */
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
  font-size: 1rem;
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

.cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 20px;
  max-width: 1000px;
  margin: auto;
}

.card {
  border: 1px solid red;
  padding: 20px;
  box-shadow: 0 0 20px rgba(255,0,0,0.3);
  display: flex;
  flex-direction: column;
  align-items: center;
  transition: transform 0.3s;
  background: #111;
  border-radius: 12px;
}

.card:hover {
  transform: translateY(-5px);
}

.card img {
  width: 100%;
  height: 180px;      
  object-fit: cover;   
  border-radius: 10px;
  margin-bottom: 15px;
}

/* ===== Product Buttons ===== */
.product-btn {
  display: inline-block;
  margin-top: 15px;
  padding: 12px 25px;
  background: red;
  color: white;
  text-decoration: none;
  font-weight: bold;
  border-radius: 8px;
  box-shadow: 0 0 10px red;
  transition: 0.3s;
}

.product-btn:hover {
  background: #ff5555;
  box-shadow: 0 0 20px red;
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

  <!-- Header -->
  <header>
    <img 
      src="https://github.com/user-attachments/assets/24e77390-843e-43cb-a7fd-7bfeeaa2fed6"
      alt="Animated Logo"
      class="center-gif">
  </header>

  <!-- Hero -->
  <div class="hero">
    <h1>Performance Gear</h1>
    <p>Built for Riders & Athletes</p>
    <button>Explore</button>
  </div>

  <!-- Section -->
  <section>
    <h2>Our Products</h2>
    <div class="cards">
      <div class="card">
        <img src="https://github.com/user-attachments/assets/24e77390-843e-43cb-a7fd-7bfeeaa2fed6" alt="High Performance Gear" />
        <h3>High Performance Gear</h3>
        <a href="https://github.com/user-attachments/assets/24e77390-843e-43cb-a7fd-7bfeeaa2fed6" class="product-btn" target="_blank">View Product</a>
      </div>
      <div class="card">
        <img src="https://github.com/user-attachments/assets/6d62477c-299b-4aeb-ba55-9a00a471930f" alt="Athletic Wear" />
        <h3>Athletic Wear</h3>
        <a href="https://github.com/user-attachments/assets/6d62477c-299b-4aeb-ba55-9a00a471930f" class="product-btn" target="_blank">View Product</a>
      </div>
      <div class="card">
        <img src="https://github.com/user-attachments/assets/82290cd4-5806-460d-b310-7569734e6dfd" alt="Rider Protection" />
        <h3>Rider Protection</h3>
        <a href="https://github.com/user-attachments/assets/82290cd4-5806-460d-b310-7569734e6dfd" class="product-btn" target="_blank">View Product</a>
      </div>
    </div>
  </section>

  <!-- Section -->
  <section>
    <h2>Why Choose Us</h2>
    <p>Designed for speed, durability and comfort.</p>
  </section>

  <!-- Footer -->
  <footer>
    © 2026 Performance Gear
  </footer>

</div>

</body>
</html>
