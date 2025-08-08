<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>spaceNull — Космос</title>
  <style>
    /* ОБЩИЕ СТИЛИ */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }

    body {
      font-family: 'Segoe UI', sans-serif;
      background: url('https://images.unsplash.com/photo-1477201389074-1863f668fac5?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80') no-repeat center center fixed;
      background-size: cover;
      color: #fff;
    }

    header {
      text-align: center;
      padding: 100px 20px 60px;
      background: rgba(0, 0, 0, 0.7);
    }

    header h1 {
      font-size: 3em;
      color: #00ffff;
      text-shadow: 0 0 15px #00ffff;
    }

    header p {
      font-size: 1.2em;
      color: #aaa;
    }

    /* НАВИГАЦИЯ */
    nav {
      text-align: center;
      background-color: rgba(0, 0, 0, 0.85);
      padding: 15px;
      position: sticky;
      top: 0;
      z-index: 999;
    }

    nav .nav-button {
      margin: 10px;
      padding: 12px 20px;
      background: none;
      border: 2px solid #0ff;
      color: #0ff;
      font-size: 1em;
      border-radius: 30px;
      cursor: pointer;
      transition: 0.3s ease;
    }

    nav .nav-button:hover {
      background: #0ff;
      color: #000;
      box-shadow: 0 0 10px #0ff;
    }

    /* РАЗДЕЛЫ */
    section {
      padding: 100px 20px;
      background: rgba(0, 0, 0, 0.6);
      border-bottom: 1px solid #444;
    }

    section h2 {
      color: #00ffff;
      text-shadow: 0 0 10px #0ff;
      margin-bottom: 10px;
    }

    /* КНОПКИ ВВЕРХ/ВНИЗ */
    .scroll-btn {
      position: fixed;
      right: 20px;
      background: rgba(0, 0, 0, 0.6);
      color: #0ff;
      border: 2px solid #0ff;
      border-radius: 50%;
      width: 45px;
      height: 45px;
      text-align: center;
      line-height: 40px;
      font-size: 20px;
      cursor: pointer;
      z-index: 1000;
      transition: 0.3s;
    }

    .scroll-btn:hover {
      background: #0ff;
      color: #000;
    }

    #scroll-up {
      bottom: 80px;
    }

    #scroll-down {
      bottom: 20px;
    }
  </style>
</head>
<body>

  <!-- Шапка -->
  <header>
    <h1>spaceNull</h1>
    <p>Твоё путешествие в космос начинается здесь</p>
  </header>

  <!-- Навигация -->
  <nav>
    <button class="nav-button" onclick="location.href='#galaxies'">Галактики</button>
    <button class="nav-button" onclick="location.href='#blackholes'">Чёрные дыры</button>
    <button class="nav-button" onclick="location.href='#planets'">Планеты</button>
    <button class="nav-button" onclick="location.href='#stars'">Звёзды</button>
    <button class="nav-button" onclick="location.href='#missions'">Миссии</button>
    <button class="nav-button" onclick="location.href='#future'">Будущее</button>
  </nav>

  <!-- Разделы -->
  <section id="galaxies">
    <h2>Галактики</h2>
    <p>Массивные системы из звёзд, газа, пыли и тёмной материи. Мы живём в Млечном Пути — спиральной галактике.</p>
  </section>

  <section id="blackholes">
    <h2>Чёрные дыры</h2>
    <p>Небесные объекты с колоссальной гравитацией. Даже свет не может вырваться из их горизонта событий.</p>
  </section>

  <section id="planets">
    <h2>Планеты</h2>
    <p>Планеты — тела, вращающиеся вокруг звёзд. У Земли — жизнь, у Юпитера — мощные бури, у Марса — загадочное прошлое.</p>
  </section>

  <section id="stars">
    <h2>Звёзды</h2>
    <p>Гигантские огненные шары. Их свет доходит до нас спустя миллионы лет, а некоторые уже давно угасли.</p>
  </section>

  <section id="missions">
    <h2>Космические миссии</h2>
    <p>От «Восток-1» до «Starship» — человечество покоряет космос, отправляя зонды, спутники и людей за пределы Земли.</p>
  </section>

  <section id="future">
    <h2>Будущее космоса</h2>
    <p>Новая эра — освоение Марса, космические станции, искусственный интеллект и контакт с внеземным разумом.</p>
  </section>

  <!-- Кнопки вверх/вниз -->
  <div id="scroll-up" class="scroll-btn" onclick="scrollToTop()">🔼</div>
  <div id="scroll-down" class="scroll-btn" onclick="scrollToBottom()">🔽</div>

  <script>
    function scrollToTop() {
      window.scrollTo({ top: 0, behavior: 'smooth' });
    }

    function scrollToBottom() {
      window.scrollTo({ top: document.body.scrollHeight, behavior: 'smooth' });
    }
  </script>

</body>
</html>
<section id="galaxies">
  <h2>Галактики</h2>
  <img src="https://upload.wikimedia.org/wikipedia/commons/4/4c/Messier51_sRGB.jpg" alt="Галактика" width="100%" style="max-width:600px;">
  <p>Галактики — гигантские системы звёзд, газа и пыли. Мы живём в Млечном Пути.</p>
  <a href="https://ru.wikipedia.org/wiki/Галактика" target="_blank">Читать на Википедии</a>
</section>

<section id="blackholes">
  <h2>Чёрные дыры</h2>
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d2/Black_hole_-_Messier_87_crop_max_res.jpg/640px-Black_hole_-_Messier_87_crop_max_res.jpg" alt="Чёрная дыра" width="100%" style="max-width:600px;">
  <p>Чёрные дыры — области с сильнейшей гравитацией, которые "поглощают" всё вокруг.</p>
  <a href="https://ru.wikipedia.org/wiki/Чёрная_дыра" target="_blank">Читать на Википедии</a>
</section>

<section id="planets">
  <h2>Планеты</h2>
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/6f/Solar_sys8.jpg/640px-Solar_sys8.jpg" alt="Планеты" width="100%" style="max-width:600px;">
  <p>Планеты — тела, вращающиеся вокруг звёзд. Земля, Марс, Юпитер — всё это планеты.</p>
  <a href="https://ru.wikipedia.org/wiki/Планета" target="_blank">Читать на Википедии</a>
</section>

<section id="stars">
  <h2>Звёзды</h2>
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/65/ESO_-_Stars.jpg/640px-ESO_-_Stars.jpg" alt="Звёзды" width="100%" style="max-width:600px;">
  <p>Звёзды — шары из плазмы, испускающие свет и тепло. Солнце — ближайшая к нам звезда.</p>
  <a href="https://ru.wikipedia.org/wiki/Звезда" target="_blank">Читать на Википедии</a>
</section>

<section id="missions">
  <h2>Космические миссии</h2>
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/7e/Apollo_11_Lunar_Module_on_the_Moon.jpg/640px-Apollo_11_Lunar_Module_on_the_Moon.jpg" alt="Космическая миссия" width="100%" style="max-width:600px;">
  <p>Миссии, как Apollo или SpaceX, двигают человечество к новым планетам и звёздам.</p>
  <a href="https://ru.wikipedia.org/wiki/Космонавтика" target="_blank">Читать на Википедии</a>
</section>

<section id="future">
  <h2>Будущее космоса</h2>
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/95/Mars_Colony_-_SpaceX_Vision.jpg/640px-Mars_Colony_-_SpaceX_Vision.jpg" alt="Будущее космоса" width="100%" style="max-width:600px;">
  <p>Марс, космические города, инопланетяне — всё это не фантастика, а возможное будущее.</p>
  <a href="https://ru.wikipedia.org/wiki/Колонизация_космоса" target="_blank">Читать на Википедии</a>
</section>
