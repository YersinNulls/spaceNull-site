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
      margin-bottom: 40px;
      text-align: center;
      text-shadow: 0 0 10px #00f0ff;
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
    }

    .card-button::before {
      content: "";
      position: absolute;
      top: -50%;
      left: -50%;
      width: 200%;
      height: 200%;
      background: radial-gradient(circle, #00ffff33 10%, transparent 70%);
      animation: shine 3s linear infinite;
      z-index: 0;
    }

    .card-button h2,
    .card-button p {
      position: relative;
      z-index: 1;
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

    @keyframes shine {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }
  </style>
</head>
<body>

  <h1>SpaceNull — Космический портал</h1>

  <div class="button-grid">
    <a href="#" class="card-button">
      <h2>Планеты</h2>
      <p>Исследуй уникальные миры солнечной системы.</p>
    </a>
    <a href="#" class="card-button">
      <h2>Звёзды</h2>
      <p>Узнай, как рождаются, живут и умирают звёзды.</p>
    </a>
    <a href="#" class="card-button">
      <h2>Чёрные дыры</h2>
      <p>Открой тайны самых загадочных объектов космоса.</p>
    </a>
    <a href="#" class="card-button">
      <h2>Галактики</h2>
      <p>Погрузись в путешествие по миллиардам галактик.</p>
    </a>
    <a href="#" class="card-button">
      <h2>Космические миссии</h2>
      <p>Следи за историями NASA, SpaceX и других.</p>
    </a>
    <a href="#" class="card-button">
      <h2>Будущее человечества</h2>
      <p>Как мы будем жить и работать в космосе?</p>
    </a>
  </div>

</body>
</html>
