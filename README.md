<!DOCTYPE html>
<html>
<head>
  <title>AgriGrow - Agriculture Website</title>

  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background-color: #f4fff4;
    }

    header {
      background-color: #2e8b57;
      color: white;
      padding: 20px;
      text-align: center;
    }

    nav {
      background-color: #3cb371;
      padding: 10px;
      text-align: center;
    }

    nav a {
      color: white;
      margin: 0 15px;
      text-decoration: none;
      font-weight: bold;
    }

    section {
      padding: 20px;
    }

    .card {
      background-color: white;
      padding: 15px;
      margin: 10px 0;
      border-radius: 8px;
      box-shadow: 0 0 5px #ccc;
    }

    button {
      padding: 10px 15px;
      background-color: #2e8b57;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }

    footer {
      background-color: #2e8b57;
      color: white;
      text-align: center;
      padding: 10px;
    }
  </style>
</head>

<body>

  <header>
    <h1>AgriGrow</h1>
    <p>Helping Farmers Grow Better 🌾</p>
  </header>

  <nav>
    <a href="#about">About</a>
    <a href="#crops">Crops</a>
    <a href="#tips">Farming Tips</a>
    <a href="#contact">Contact</a>
  </nav>

  <section id="about">
    <h2>About Agriculture</h2>
    <div class="card">
      <p>
        Agriculture is the practice of growing crops and raising animals
        for food, fiber, and other products essential for life.
      </p>
    </div>
  </section>

  <section id="crops">
    <h2>Popular Crops</h2>
    <div class="card">🌾 Wheat</div>
    <div class="card">🌽 Corn</div>
    <div class="card">🍚 Rice</div>
    <div class="card">🥔 Potatoes</div>
  </section>

  <section id="tips">
    <h2>Farming Tips</h2>
    <div class="card">
      <p id="tip">Click the button to get a farming tip.</p>
      <button onclick="showTip()">Get Tip</button>
    </div>
  </section>

  <section id="contact">
    <h2>Contact Us</h2>
    <div class="card">
      <p>Email: agrigrow@example.com</p>
      <p>Phone: +123 456 7890</p>
    </div>
  </section>

  <footer>
    <p>© 2026 AgriGrow | Agriculture for a Better Future</p>
  </footer>

  <script>
    function showTip() {
      const tips = [
        "Water crops early in the morning.",
        "Use organic compost to improve soil.",
        "Rotate crops to keep soil healthy.",
        "Check soil moisture before irrigation."
      ];

      const randomTip = tips[Math.floor(Math.random() * tips.length)];
      document.getElementById("tip").innerText = randomTip;
    }
  </script>

</body>
</html>
