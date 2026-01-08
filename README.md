<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Performance Gear for Riders & Athletes</title>

<style>
  * {
    box-sizing: border-box;
  }

  body {
    margin: 0;
    background: black;
    width: 100vw;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: hidden;
    font-family: Arial, sans-serif;
  }

  /* الفريم النيون */
  .neon-frame {
    width: calc(100vw - 40px);
    height: calc(100vh - 40px);
    border: 3px solid cyan;
    box-shadow:
      0 0 15px cyan,
      0 0 40px cyan,
      0 0 80px cyan;
    display: flex;
    justify-content: center;
    align-items: center;
    animation: neonGlow 2s ease-in-out infinite alternate;
  }

  @keyframes neonGlow {
    from {
      box-shadow:
        0 0 15px cyan,
        0 0 40px cyan,
        0 0 80px cyan;
    }
    to {
      box-shadow:
        0 0 25px cyan,
        0 0 60px cyan,
        0 0 120px cyan;
    }
  }

  /* اللوجو في النص */
  .center-logo {
    width: 220px;
    max-width: 70%;
    filter: drop-shadow(0 0 25px cyan);
  }
</style>
</head>

<body>

  <div class="neon-frame">
    <img src="logo.png" alt="Logo" class="center-logo">
  </div>

</body>
</html>
