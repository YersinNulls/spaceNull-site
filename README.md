<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>SpaceNull — Космический портал</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: radial-gradient(ellipse at top, #020024, #090979, #000);
      color: #ffffff;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 50px 20px;
      min-height: 100vh;
    }

    h1 {
      font-size: 3em;
      margin-bottom: 10px;
      text-align: center;
      text-shadow: 0 0 15px #00f0ff;
    }

    .subtitle {
      font-size: 1.2em;
      color: #ccc;
      margin-bottom: 30px;
      text-align: center;
      max-width: 700px;
    }

    .intro-box {
      background-color: rgba(255, 255, 255, 0.05);
      border: 1px solid rgba(255, 255, 255, 0.1);
      border-radius: 15px;
      padding: 20px;
      margin-bottom: 50px;
      box-shadow: 0 0 10px #00ffff44;
      max-width: 800px;
      text-align: center;
    }

    .button-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 30px;
      width: 100%;
      max-width: 1000px;
    }

    .card-button {
      background: #0a0a0a;
      border: 2px solid #00ffff;
      border-radius: 15px;
      padding: 20px;
      text-align: center;
      text-decoration: none;
      color: #ffffff;
      transition: 0.4s;
      box-shadow: 0 0 10px #00ffff, 0 0 30px #00ffff33, inset 0 0 10px #00ffff55;
      position: relative;
      overflow: hidden;
      cursor: pointer;
    }

    .card-button h2 {
      margin: 0 0 10px;
      font-size: 1.3em;
      color: #00ffff;
      text-shadow: 0 0 5px #00ffff, 0 0 10px #00ffffaa;
    }

    .card-button p {
      margin: 0;
      font-size: 0.95em;
      color: #ccc;
    }

    .card-button:hover {
      transform: scale(1.05);
      box-shadow: 0 0 15px #00ffff, 0 0 40px #00ffff88, inset 0 0 15px #00ffff55;
    }

    .presentation {
      display: none;
      max-width: 700px;
      background-color: rgba(255, 255, 255, 0.07);
      border-radius: 15px;
      padding: 20px;
      margin-top: 40px;
      box-shadow: 0 0 15px #00ffff33;
    }
  </style>
</head>
<body>

  <h1>SpaceNull</h1>
  <div class="subtitle">Твоя цифровая станция для путешествия по вселенной</div>

  <div class="intro-box">
    <p>
      Добро пожаловать в <strong>SpaceNull</strong> — космический портал, созданный для всех, кто мечтает заглянуть за пределы Земли.
    </p>
  </div>

  <div class="button-grid">
    <div class="card-button" onclick="showText('planets')">
      <h2>Планеты</h2>
      <p>Исследуй уникальные миры солнечной системы.</p>
    </div>
    <div class="card-button" onclick="showText('stars')">
      <h2>Звёзды</h2>
      <p>Как рождаются и умирают светила?</p>
    </div>
    <div class="card-button" onclick="showText('blackholes')">
      <h2>Чёрные дыры</h2>
      <p>Загадочные монстры пространства и времени.</p>
    </div>
    <div class="card-button" onclick="showText('galaxies')">
      <h2>Галактики</h2>
      <p>Миллиарды звёзд в каждом космическом острове.</p>
    </div>
    <div class="card-button" onclick="showText('missions')">
      <h2>Космические миссии</h2>
      <p>NASA, SpaceX и будущее человечества.</p>
    </div>
    <div class="card-button" onclick="showText('future')">
      <h2>Будущее</h2>
      <p>Как мы будем жить и работать в космосе?</p>
    </div>
  </div>

  <div id="presentation" class="presentation"></div>

  <script>
    const texts = {
      planets: "Планеты — это уникальные миры, от горячего Меркурия до ледяного Нептуна. Каждая из них имеет свои тайны, спутники и загадки.",
      stars: "Звёзды — гигантские шары плазмы, рождающиеся в туманностях. Они создают свет, тепло и в итоге — элементы жизни.",
      blackholes: "Чёрные дыры — плотные области, из которых не может вырваться даже свет. Они деформируют пространство и время.",
      galaxies: "Галактики — огромные системы звёзд, пыли и тьмы. Мы живём в одной из них — Млечном Пути.",
      missions: "Космические миссии, такие как Apollo, Voyager или Starship, продвигают нас к будущему среди звёзд.",
      future: "Будущее человечества — это колонии на Марсе, орбитальные станции, космические города. Всё только начинается."
    };

    function showText(key) {
      const box = document.getElementById('presentation');
      box.style.display = 'block';
      box.innerText = texts[key];
    }
  </script>

</body>
</html>
