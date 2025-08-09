<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Nissan GT-R</title>
<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@500;700&display=swap" rel="stylesheet">
<style>
    body {
        margin: 0;
        font-family: 'Orbitron', sans-serif;
        background: black;
        color: white;
        overflow-x: hidden;
    }

    header {
        height: 100vh;
        background: url('https://upload.wikimedia.org/wikipedia/commons/0/07/Nissan_GT-R_Track_Edition.jpg') center/cover fixed;
        display: flex;
        justify-content: center;
        align-items: center;
        text-align: center;
    }

    header h1 {
        font-size: 4rem;
        color: #0ff;
        text-shadow: 0 0 10px #0ff, 0 0 20px #0ff;
    }

    section {
        padding: 60px 20px;
        text-align: center;
    }

    .stats {
        background: #111;
        padding: 50px 20px;
    }

    .stats h2 {
        font-size: 2.5rem;
        margin-bottom: 20px;
        color: #0ff;
        text-shadow: 0 0 5px #0ff;
    }

    .stats p {
        font-size: 1.3rem;
        line-height: 1.6;
    }

    .parallax {
        height: 80vh;
        background-attachment: fixed;
        background-size: cover;
        background-position: center;
    }

    .img1 { background-image: url('https://images.unsplash.com/photo-1614549323175-38ad2c7b8ca1'); }
    .img2 { background-image: url('https://images.unsplash.com/photo-1614549323180-f1b3b6ed8e2b'); }

    .buttons {
        display: flex;
        justify-content: center;
        gap: 20px;
        margin-top: 40px;
    }

    .neon-btn {
        padding: 15px 30px;
        font-size: 1.2rem;
        color: #0ff;
        border: 2px solid #0ff;
        background: transparent;
        cursor: pointer;
        text-shadow: 0 0 5px #0ff;
        box-shadow: 0 0 10px #0ff, inset 0 0 10px #0ff;
        transition: 0.3s;
    }

    .neon-btn:hover {
        background: #0ff;
        color: black;
        box-shadow: 0 0 20px #0ff, inset 0 0 20px #0ff;
    }
</style>
</head>
<body>

<header>
    <h1>Nissan GT-R</h1>
</header>

<section class="stats">
    <h2>Характеристики</h2>
    <p>Двигатель: 3.8L Twin-Turbo V6</p>
    <p>Мощность: 565 л.с. (NISMO: 600 л.с.)</p>
    <p>Разгон 0-100 км/ч: 2.9 секунды</p>
</section>

<div class="parallax img1"></div>

<section>
    <h2>Легенда скорости</h2>
    <p>Nissan GT-R — культовый японский спорткар, известный своей точной управляемостью и невероятным ускорением.</p>
</section>

<div class="parallax img2"></div>

<section>
    <h2>Действия</h2>
    <div class="buttons">
        <button class="neon-btn">Купить</button>
        <button class="neon-btn">Галерея</button>
        <button class="neon-btn">Контакты</button>
    </div>
</section>

</body>
</html>
