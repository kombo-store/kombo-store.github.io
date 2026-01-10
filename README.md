<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Performance Gear for Riders & Athletes</title>

<style>
* { box-sizing: border-box; margin:0; padding:0; font-family: Arial,sans-serif; }

/* ===== BODY ===== */
body {
  min-height:100vh;
  background: #000;
  color:#fff;
}

/* ===== Neon Frame ===== */
.neon-frame {
  position: relative;
  max-width: 1200px;
  min-height: 100vh;
  margin:20px auto;
  border:3px solid #8b0000;
  box-shadow:0 0 15px #8b0000, 0 0 40px #4d0000;
  background-color: rgba(0,0,0,0.75);
  border-radius:12px;
  padding-bottom:80px;
}

/* ===== Header ===== */
header { padding:16px 0; text-align:center; }
header img { width:140px; filter: drop-shadow(0 0 15px #8b0000); }

/* ===== Hero ===== */
.hero { padding:60px 20px; text-align:center; }
.hero h1 { font-size:2.6rem; color:#b30000; }
.hero p { margin-top:10px; opacity:0.85; }
.hero button { margin-top:22px; padding:10px 26px; border:2px solid #8b0000; background:transparent; color:#b30000; cursor:pointer; }
.hero button:hover { background:#8b0000; color:black; }

/* ===== Sections ===== */
section { padding:60px 20px; text-align:center; }
section h2 { color:#b30000; margin-bottom:30px; }

/* ===== Cards ===== */
.cards { display:grid; grid-template-columns:repeat(auto-fit,minmax(260px,1fr)); gap:20px; max-width:1000px; margin:auto; }
.card { background:#111; border:1px solid #8b0000; padding:18px; border-radius:12px; text-align:center; }
.card img { width:100%; height:190px; object-fit:cover; border-radius:10px; margin-bottom:12px; }
.card h3 { margin-bottom:12px; }
.product-btn { display:inline-block; padding:10px 22px; background:#8b0000; color:white; text-decoration:none; border-radius:8px; cursor:pointer; }
.product-btn:hover { background:#b30000; }

/* ===== Lightbox / Modal ===== */
#lightboxModal {
  display:none;
  position:fixed;
  top:0; left:0;
  width:100%;
  height:100%;
  background: rgba(0,0,0,0.9);
  z-index:1000;
  align-items:center;
  justify-content:center;
}

#lightboxModal img {
  max-width:90%;
  max-height:80%;
  border-radius:12px;
}

#lightboxModal .close, #lightboxModal .prev, #lightboxModal .next {
  position:absolute;
  color:#fff;
  font-size:2rem;
  cursor:pointer;
  user-select:none;
  padding:8px 12px;
  background: rgba(0,0,0,0.5);
  border-radius:6px;
  transition:0.3s;
}

#lightboxModal .close:hover, #lightboxModal .prev:hover, #lightboxModal .next:hover { background: #8b0000; }

#lightboxModal .close { top:20px; right:20px; }
#lightboxModal .prev { top:50%; left:20px; transform:translateY(-50%); }
#lightboxModal .next { top:50%; right:20px; transform:translateY(-50%); }

/* ===== Responsive ===== */
@media(max-width:768px){
  .hero { padding:40px 20px; }
  .card img { height:160px; }
  #lightboxModal .close, #lightboxModal .prev, #lightboxModal .next { font-size:1.5rem; padding:6px 10px; }
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
    <div class="card" data-images='["https://github.com/user-attachments/assets/6d62477c-299b-4aeb-ba55-9a00a471930f","https://github.com/user-attachments/assets/82290cd4-5806-460d-b310-7569734e6dfd"]'>
      <img src="https://github.com/user-attachments/assets/6d62477c-299b-4aeb-ba55-9a00a471930f" alt="High Performance Gear">
      <h3>High Performance Gear</h3>
      <a class="product-btn">View Product</a>
    </div>
    <div class="card" data-images='["https://github.com/user-attachments/assets/6d62477c-299b-4aeb-ba55-9a00a471930f","https://github.com/user-attachments/assets/82290cd4-5806-460d-b310-7569734e6dfd"]'>
      <img src="https://github.com/user-attachments/assets/6d62477c-299b-4aeb-ba55-9a00a471930f" alt="Athletic Wear">
      <h3>Athletic Wear</h3>
      <a class="product-btn">View Product</a>
    </div>
    <div class="card" data-images='["https://github.com/user-attachments/assets/82290cd4-5806-460d-b310-7569734e6dfd","https://github.com/user-attachments/assets/6d62477c-299b-4aeb-ba55-9a00a471930f"]'>
      <img src="https://github.com/user-attachments/assets/82290cd4-5806-460d-b310-7569734e6dfd" alt="Rider Protection">
      <h3>Rider Protection</h3>
      <a class="product-btn">View Product</a>
    </div>
  </div>
</section>

<section>
  <h2>Why Choose Us</h2>
  <p>Designed for speed, durability and comfort.</p>
</section>

<footer>© 2026 Performance Gear</footer>

<!-- ===== Lightbox Modal ===== -->
<div id="lightboxModal">
  <span class="close">&times;</span>
  <span class="prev">&#10094;</span>
  <span class="next">&#10095;</span>
  <img src="" alt="Product Image">
</div>

<script>
// ===== Lightbox JS =====
let currentImages = [];
let currentIndex = 0;

const modal = document.getElementById("lightboxModal");
const modalImg = modal.querySelector("img");
const closeBtn = modal.querySelector(".close");
const prevBtn = modal.querySelector(".prev");
const nextBtn = modal.querySelector(".next");

document.querySelectorAll(".product-btn").forEach((btn, i) => {
  btn.addEventListener("click", () => {
    const card = btn.closest(".card");
    currentImages = JSON.parse(card.dataset.images);
    currentIndex = 0;
    modalImg.src = currentImages[currentIndex];
    modal.style.display = "flex";
  });
});

closeBtn.onclick = () => modal.style.display = "none";
prevBtn.onclick = () => {
  currentIndex = (currentIndex - 1 + currentImages.length) % currentImages.length;
  modalImg.src = currentImages[currentIndex];
};
nextBtn.onclick = () => {
  currentIndex = (currentIndex + 1) % currentImages.length;
  modalImg.src = currentImages[currentIndex];
};

// Close on click outside image
modal.addEventListener("click", e => {
  if(e.target === modal) modal.style.display="none";
});
</script>

</div>
</body>
</html>

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
