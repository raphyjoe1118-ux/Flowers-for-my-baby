# Flowers-for-my-baby
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Happy Valentine’s Day, Eunice ❤️</title>
  <style>
    body {
      margin: 0;
      font-family: 'Georgia', serif;
      background: linear-gradient(180deg, #ffe6f0, #fff0f5);
      color: #8b1c3d;
      overflow-x: hidden;
    }

    header {
      text-align: center;
      padding: 80px 20px;
      background: radial-gradient(circle, #ffb6c1, #ff69b4);
      color: white;
    }

    header h1 {
      font-size: 3.5em;
      margin: 0;
    }

    header p {
      font-size: 1.4em;
      margin-top: 15px;
    }

    .flowers {
      font-size: 2.5em;
      text-align: center;
      margin: 40px 0;
    }

    section {
      max-width: 900px;
      margin: auto;
      padding: 40px 20px;
      text-align: center;
    }

    section h2 {
      font-size: 2.2em;
      margin-bottom: 20px;
    }

    section p {
      font-size: 1.2em;
      line-height: 1.8;
    }

    .bouquet {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
      gap: 20px;
      font-size: 3em;
      margin-top: 40px;
    }

    footer {
      text-align: center;
      padding: 30px;
      background: #ff69b4;
      color: white;
      font-size: 1.1em;
    }

    /* Floating flowers animation */
    .floating {
      position: fixed;
      top: -50px;
      animation: fall linear infinite;
      opacity: 0.8;
    }

    @keyframes fall {
      to {
        transform: translateY(110vh) rotate(360deg);
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>Happy Valentine’s Day, Eunice ❤️</h1>
    <p>A day filled with love, beauty, and endless flowers just for you</p>
  </header>

  <div class="flowers">
    🌸 🌹 🌷 💐 🌺 🌻 🌼 🌸 🌹 🌷 💐
  </div>

  <section>
    <h2>For Eunice</h2>
    <p>
      This little website is made just for you — a celebration of love,
      warmth, and all the beautiful moments that make Valentine’s Day special.
      May your day be as bright as these flowers and as sweet as every smile
      you bring into the world.
    </p>
  </section>

  <section>
    <h2>A Bouquet of Love</h2>
    <div class="bouquet">
      🌹 🌸 🌷 🌺 🌻 🌼 💐 🌹 🌸 🌷 🌺 🌻 🌼 💐
    </div>
  </section>

  <section>
    <h2>With All My Heart ❤️</h2>
    <p>
      Valentine’s Day is about love in every form — kindness, joy, laughter,
      and the simple beauty of caring for someone special. Today is your day,
      Eunice, and these flowers bloom just for you.
    </p>
  </section>

  <footer>
    Made with love 💖 | Happy Valentine’s Day
  </footer>

  <script>
    const flowers = ["🌸","🌹","🌷","🌺","🌻","🌼","💐"];

    for (let i = 0; i < 30; i++) {
      const f = document.createElement("div");
      f.className = "floating";
      f.textContent = flowers[Math.floor(Math.random() * flowers.length)];
      f.style.left = Math.random() * 100 + "vw";
      f.style.fontSize = 20 + Math.random() * 30 + "px";
      f.style.animationDuration = 5 + Math.random() * 10 + "s";
      document.body.appendChild(f);
    }
  </script>

</body>
</html>
