<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>spaceNull's</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      background: black;
      overflow: hidden;
      color: white;
      font-family: 'Segoe UI', sans-serif;
      display: flex;
      align-items: center;
      justify-content: center;
      flex-direction: column;
      text-align: center;
    }
[Uploading index.html…]()<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>spaceNull – Космос</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background: #000;
      color: #fff;
    }
    nav {
      background: #111;
      padding: 15px;
      text-align: center;
      position: sticky;
      top: 0;
      z-index: 999;
    }
    nav button {
      margin: 10px;
      padding: 10px 20px;
      background: #222;
      color: #fff;
      border: none;
      cursor: pointer;
      transition: 0.3s;
    }
    nav button:hover {
      background: #444;
    }
    section {
      padding: 100px 20px;
      border-bottom: 1px solid #333;
    }
    h2 {
      color: #0ff;
    }
  </style>
</head>
<body>

  <nav>
    <button onclick="location.href='#galaxies'">Галактики</button>
    <button onclick="location.href='#blackholes'">Чёрные дыры</button>
    <button onclick="location.href='#planets'">Планеты</button>
    <button onclick="location.href='#stars'">Звёзды</button>
    <button onclick="location.href='#missions'">Космические миссии</button>
    <button onclick="location.href='#future'">Будущее космоса</button>
  </nav>

  <section id="galaxies">
    <h2>Галактики</h2>
    <p>Галактики — это гигантские системы, состоящие из миллиардов звёзд, планет, газа и пыли. Самая известная — Млечный Путь.</p>
  </section>

  <section id="blackholes">
    <h2>Чёрные дыры</h2>
    <p>Чёрные дыры — области пространства с гравитацией настолько сильной, что ничто, даже свет, не может их покинуть.</p>
  </section>

  <section id="planets">
    <h2>Планеты</h2>
    <p>Планеты — небесные тела, вращающиеся вокруг звёзд. В нашей Солнечной системе их 8, включая Землю.</p>
  </section>

  <section id="stars">
    <h2>Звёзды</h2>
    <p>Звёзды — гигантские шары плазмы, испускающие свет и тепло. Солнце — ближайшая к нам звезда.</p>
  </section>

  <section id="missions">
    <h2>Космические миссии</h2>
    <p>Миссии вроде Apollo, Voyager и SpaceX расширили наши знания о Вселенной и возможностях путешествий в космос.</p>
  </section>

  <section id="future">
    <h2>Будущее космоса</h2>
    <p>В будущем нас ждёт освоение Марса, постройка орбитальных станций и, возможно, контакт с внеземными цивилизациями.</p>
  </section>

</body>
</html>


    h1 {
      font-size: 3em;
      text-shadow: 0 0 15px white;
    }

    .stars {
      position: absolute;
      width: 100%;
      height: 100%;
      background: url('https://raw.githubusercontent.com/VincentGarreau/particles.js/master/demo/media/stars.png') repeat;
      animation: moveStars 100s linear infinite;
      z-index: -1;
    }

    @keyframes moveStars {
      from { background-position: 0 0; }
      to { background-position: -10000px 5000px; }
    }

    .subtitle {
      font-size: 1.2em;
      color: #ccc;
      margin-top: 20px;
    }
  </style>
</head>
<body>
  <div class="stars"></div>
  <h1>Добро пожаловать в spaceNull's</h1>
  <div class="subtitle">Твое путешествие начинается здесь</div>
</body>
</html>
