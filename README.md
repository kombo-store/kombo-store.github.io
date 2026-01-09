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

    .neon-frame {
      width: calc(100vw - 40px);
      min-height: calc(100vh - 40px);
      border: 3px solid red;
      box-shadow: 0 0 15px red, 0 0 40px red, 0 0 80px red;
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

    header {
      padding: 20px;
      text-align: center;
    }

    header img {
      width: 160px;
      filter: drop-shadow(0 0 20px red);
    }

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
      box-shadow: 0 0 20px rgba(255, 0, 0, 0.4);
      text-align: center;
    }

    .card-img {
      display: block;
      width: 120px;
      margin: 15px auto 0;
    }

    footer {
      padding: 20px;
      text-align: center;
      opacity: 0.6;
    }
    .card-img {
  display: block;
  width: 120px;
  margin: 15px auto 0;
}

  </style>
</head>

<body>
  <div class="neon-frame">

    <header>
      <img src="rider.png" alt="Logo">
    </header>

    <div class="hero">
      <h1>Performance Gear</h1>
      <p>Built for Riders & Athletes</p>
    </div>

    <section>
      <h2>Our Products</h2>
      <div class="cards">
        <div class="card">High Performance Gear</div>
        <div class="card">Athletic Wear</div>
        <div class="card">
          Rider Protection
          <img src="rider.png" class="card-img">
        </div>
      </div>
    </section>

    <footer>
      © 2026 Performance Gear
    </footer>

  </div>
</body>
</html>
