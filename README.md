<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Kombo Store</title>

  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;700;800&display=swap" rel="stylesheet">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Poppins', sans-serif;
      background: radial-gradient(circle at top, #141414, #000);
      color: #fff;
    }

    /* HEADER */
    .header {
      position: fixed;
      top: 0;
      width: 100%;
      padding: 20px 60px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      backdrop-filter: blur(12px);
      z-index: 1000;
    }

    .logo {
      font-size: 28px;
      font-weight: 800;
      letter-spacing: 2px;
    }

    .header nav {
      display: flex;
    }

    .header nav a {
      margin: 0 15px;
      text-decoration: none;
      color: #fff;
      position: relative;
    }

    .header nav a::after {
      content: '';
      position: absolute;
      bottom: -5px;
      left: 0;
      width: 0;
      height: 2px;
      background: #ff1e1e;
      transition: .3s;
    }

    .header nav a:hover::after {
      width: 100%;
    }

    /* CART */
    .cart {
      position: relative;
      font-size: 24px;
      cursor: pointer;
    }

    #cart-count {
      position: absolute;
      top: -8px;
      right: -12px;
      background: #ff1e1e;
      color: #fff;
      font-size: 14px;
      padding: 2px 7px;
      border-radius: 50%;
      font-weight: bold;
    }

    /* Hamburger */
    .hamburger {
      display: none;
      flex-direction: column;
      cursor: pointer;
      gap: 5px;
    }

    .hamburger span {
      width: 25px;
      height: 3px;
      background: #fff;
      transition: 0.3s;
    }

    /* HERO */
    .hero {
      height: 100vh;
      background: url("hero.jpg") center/cover no-repeat;
      position: relative;
      display: flex;
      align-items: center;
      padding-left: 60px;
    }

    .overlay {
      position: absolute;
      inset: 0;
      background: rgba(0,0,0,.65);
    }

    .hero-content {
      position: relative;
      max-width: 600px;
    }

    .hero h1 {
      font-size: 70px;
      letter-spacing: 4px;
      margin-bottom: 20px;
    }

    .hero p {
      color: #ccc;
      margin-bottom: 30px;
    }

    .main-btn {
      background: #ff1e1e;
      padding: 15px 45px;
      border: none;
      font-weight: bold;
      color: #fff;
      cursor: pointer;
      transition: .3s;
    }

    .main-btn:hover {
      background: #c70000;
      transform: translateY(-3px);
    }

    /* PRODUCTS */
    .products {
      padding: 120px 60px;
      background: #000;
    }

    .products h2 {
      font-size: 40px;
      margin-bottom: 60px;
      letter-spacing: 3px;
    }

    .products-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 40px;
    }

    .product-card {
      background: #111;
      overflow: hidden;
      transition: .4s;
      position: relative;
    }

    .product-card img {
      width: 100%;
      height: 420px;
      object-fit: cover;
      transition: .4s;
    }

    .product-card:hover img {
      transform: scale(1.1);
    }

    .product-info {
      padding: 20px;
    }

    .product-info h3 {
      margin-bottom: 10px;
    }

    .product-info span {
      color: #ff1e1e;
      font-weight: bold;
    }

    .product-info button {
      margin-top: 15px;
      width: 100%;
      padding: 12px;
      background: transparent;
      border: 1px solid #ff1e1e;
      color: #fff;
      cursor: pointer;
      transition: .3s;
    }

    .product-info button:hover {
      background: #ff1e1e;
    }

    /* RESPONSIVE */
    @media (max-width: 768px) {

      .header nav {
        position: fixed;
        top: 0;
        right: -100%;
        width: 200px;
        height: 100%;
        background: #111;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        transition: 0.3s;
        gap: 30px;
        z-index: 999;
      }

      .header nav.active {
        right: 0;
      }

      .hamburger {
        display: flex;
      }

      .products-grid {
        grid-template-columns: 1fr;
        gap: 20px;
      }

      .hero {
        padding-left: 30px;
        text-align: center;
        justify-content: center;
      }

      .hero h1 {
        font-size: 48px;
      }

      .hero p {
        font-size: 18px;
      }
    }
  </style>
</head>
<body>
  <!-- HEADER -->
  <header class="header">
    <div class="logo">KOMBO</div>
    <nav>
      <a href="#">Shop</a>
      <a href="#">Collections</a>
      <a href="#">About</a>
      <a href="#">Contact</a>
    </nav>
    <div class="cart">
      🛒 <span id="cart-count">0</span>
    </div>
    <div class="hamburger" id="hamburger">
      <span></span>
      <span></span>
      <span></span>
    </div>
  </header>

  <!-- HERO -->
  <section class="hero">
    <div class="overlay"></div>
    <div class="hero-content">
      <h1>WEAR THE POWER</h1>
      <p>Streetwear built for dominance</p>
      <button class="main-btn">SHOP NOW</button>
    </div>
  </section>

  <!-- PRODUCTS -->
  <section class="products">
    <h2>KOMBO DROPS</h2>
    <div class="products-grid">
      <div class="product-card">
        <img src="hoodie1.jpg" alt="Hoodie">
        <div class="product-info">
          <h3>Black Shadow Hoodie</h3>
          <span>950 EGP</span>
          <button class="add-to-cart">Add to Cart</button>
        </div>
      </div>
      <div class="product-card">
        <img src="jacket1.jpg" alt="Jacket">
        <div class="product-info">
          <h3>Red Strike Jacket</h3>
          <span>1450 EGP</span>
          <button class="add-to-cart">Add to Cart</button>
        </div>
      </div>
      <div class="product-card">
        <img src="tshirt1.jpg" alt="Tshirt">
        <div class="product-info">
          <h3>Kombo Core Tee</h3>
          <span>450 EGP</span>
          <button class="add-to-cart">Add to Cart</button>
        </div>
      </div>
    </div>
  </section>

  <!-- JS -->
  <script>
    // Add to Cart
    let cartCount = 0;
    const cartCountEl = document.getElementById('cart-count');
    const addButtons = document.querySelectorAll('.add-to-cart');

    addButtons.forEach(btn => {
      btn.addEventListener('click', () => {
        cartCount++;
        cartCountEl.textContent = cartCount;
        btn.textContent = "Added";
        btn.disabled = true;
        btn.style.background = "#555";
      });
    });

    // Hamburger Menu
    const hamburger = document.getElementById('hamburger');
    const nav = document.querySelector('.header nav');

    hamburger.addEventListener('click', () => {
      nav.classList.toggle('active');
      hamburger.classList.toggle('open');
    });
  </script>

</body>
</html>
