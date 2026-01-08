<!DOCTYPE html>
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
  border: 3px solid cyan;
  box-shadow:
    0 0 15px cyan,
    0 0 40px cyan,
    0 0 80px cyan;
  animation: glow 2s ease-in-out infinite alternate;
}

@keyframes glow {
  from {
    box-shadow: 0 0 15px cyan, 0 0 40px cyan, 0 0 80px cyan;
  }
  to {
    box-shadow: 0 0 25px cyan, 0 0 60px cyan, 0 0 120px cyan;
  }
}

/* ===== Layout ===== */
header {

  padding: 20px;
  text-align: center;
}

header img {
  width: 160px;
  filter: drop-shadow(0 0 20px cyan);
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
  color: cyan;
}

.hero p {
  margin-top: 15px;
  opacity: 0.8;
}

.hero button {
  margin-top: 30px;
  padding: 12px 30px;
  background: transparent;
  border: 2px solid cyan;
  color: cyan;
  cursor: pointer;
  font-size: 1rem;
  box-shadow: 0 0 15px cyan;
}

.hero button:hover {
  background: cyan;
  color: black;
}

/* ===== Sections ===== */
section {
  padding: 80px 20px;
  text-align: center;
}

section h2 {
  color: cyan;
  margin-bottom: 20px;
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
  padding: 30px;
  box-shadow: 0 0 20px rgba(0,255,255,0.3);
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

<div class="neon-frame">
  <img src="![logo gif]" alt="Animated Logo" class="center-gif">
</div>


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
      <div class="card">High Performance Gear</div>
      <div class="card">Athletic Wear</div>
      <div class="card">Rider Protection</div>
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
