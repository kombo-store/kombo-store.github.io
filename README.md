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
  /* الخلفية الجديدة من جهازك مباشرة */
  background: url('background.jpg') no-repeat center center fixed;
  background-size: cover;
  color: #fff;
  font-family: Arial, sans-serif;
}

/* ===== Neon Glow Animation ===== */
@keyframes neon-glow {
  0%, 100% {
    text-shadow: 0 0 4px #ff0000, 0 0 8px #ff0000, 0 0 12px #ff5555, 0 0 18px #ff5555;
  }
  50% {
    text-shadow: 0 0 6px #ff5555, 0 0 12px #ff0000, 0 0 18px #ff0000, 0 0 24px #ff5555;
  }
}

/* ===== Neon Frame ===== */
.neon-frame {
  position: relative;
  max-width: 1200px;
  min-height: 100vh;
  margin: 20px auto;
  border: 3px solid red;
  box-shadow: 0 0 15px red, 0 0 40px red;
  background-color: rgba(0,0,0,0.6);
  border-radius: 12px;
  padding-bottom: 80px;
}

/* ===== Header ===== */
header {
  padding: 16px 0;
  text-align: center;
}

header img {
  width: 140px;
  filter: drop-shadow(0 0 20px red);
}

/* ===== Hero ===== */
.hero {
  padding: 60px 20px;
  text-align: center;
}

.hero h1 {
  font-size: 2.8rem;
  color: red;
  animation: neon-glow 1.5s ease-in-out infinite alternate;
}

.hero p {
  margin-top: 10px;
  opacity: 0.85;
  animation: neon-glow 2s ease-in-out infinite alternate;
}

.hero button {
  margin-top: 22px;
  padding: 12px 28px;
  border: 2px solid red;
  background: transparent;
  color: red;
  cursor: pointer;
  animation: neon-glow 1.8s ease-in-out infinite alternate;
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
  animation: neon-glow 1.5s ease-in-out infinite alternate;
}

/* ===== Cards ===== */
.cards {
  disp
