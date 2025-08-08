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
      background: linear-gradient(#000010, #000030);
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
    }

    .button-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 30px;
      width: 100%;
      max-width: 1000px;
    }

    .card-button {
      background-color: rgba(255, 255, 255, 0.05);
      border: 1px solid rgba(255, 255, 255, 0.1);
      border-radius: 15px;
      padding: 20px;
      text-align: center;
      transition: 0.3s;
      text-decoration: none;
      color: white;
    }

    .card-button:hover {
      background-color: rgba(30, 144, 255, 0.2);
      transform: scale(1.03);
    }

    .card-button h2 {
      margin: 0 0 10px;
      font-size: 1.3em;
      color: #00bfff;
    }

    .card-button p {
      margin: 0;
      font-size: 0.95em;
      color: #ccc;
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
