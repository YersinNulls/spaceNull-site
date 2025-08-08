<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Space Null</title>
<style>
    body {
        margin: 0;
        font-family: Arial, sans-serif;
        text-align: center;
        color: white;
        background: url('https://www.nasa.gov/wp-content/uploads/2023/03/hs-2015-02-a-xlarge_web.jpg') no-repeat center center fixed;
        background-size: cover;
    }
    h1 {
        margin-top: 20px;
        text-shadow: 0 0 10px #0ff;
    }
    .button-container {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 20px;
        margin-top: 40px;
    }
    .neon-button {
        background: transparent;
        border: 2px solid #0ff;
        color: #0ff;
        padding: 15px 25px;
        font-size: 18px;
        cursor: pointer;
        border-radius: 8px;
        text-shadow: 0 0 5px #0ff;
        box-shadow: 0 0 20px #0ff;
        transition: 0.3s;
        width: 200px;
    }
    .neon-button:hover {
        background: rgba(0, 255, 255, 0.1);
        box-shadow: 0 0 30px #0ff;
    }
    .description {
        font-size: 14px;
        margin-top: 5px;
        color: #ddd;
    }
    .presentation {
        display: none;
        margin-top: 30px;
        padding: 20px;
        background: rgba(0, 0, 0, 0.7);
        border-radius: 10px;
        width: 80%;
        margin-left: auto;
        margin-right: auto;
        box-shadow: 0 0 20px #0ff;
    }
</style>
</head>
<body>

<h1>🌌 Космический проект Space Null 🌌</h1>

<div class="button-container">
    <div>
        <button class="neon-button" onclick="showPresentation(1)">Планеты</button>
        <div class="description">Интересные факты о планетах</div>
    </div>
    <div>
        <button class="neon-button" onclick="showPresentation(2)">Звёзды</button>
        <div class="description">Как рождаются и умирают звёзды</div>
    </div>
    <div>
        <button class="neon-button" onclick="showPresentation(3)">Галактики</button>
        <div class="description">Миллиарды миров во Вселенной</div>
    </div>
    <div>
        <button class="neon-button" onclick="showPresentation(4)">Чёрные дыры</button>
        <div class="description">Тайны гравитационных монстров</div>
    </div>
    <div>
        <button class="neon-button" onclick="showPresentation(5)">Космические миссии</button>
        <div class="description">Путешествия за пределы Земли</div>
    </div>
    <div>
        <button class="neon-button" onclick="showPresentation(6)">Будущее космоса</button>
        <div class="description">Колонизация других планет</div>
    </div>
</div>

<div id="presentation" class="presentation"></div>

<script>
    const presentations = {
        1: "<h2>Планеты</h2><p>В нашей Солнечной системе 8 планет, каждая уникальна. Например, Юпитер — самый большой, а Венера вращается в обратную сторону.</p>",
        2: "<h2>Звёзды</h2><p>Звёзды рождаются из облаков газа и пыли. Когда топливо заканчивается, они могут взрываться как сверхновые.</p>",
        3: "<h2>Галактики</h2><p>Галактики содержат миллиарды звёзд. Наша галактика — Млечный Путь, но есть и другие, например, Андромеда.</p>",
        4: "<h2>Чёрные дыры</h2><p>Это объекты с гравитацией настолько сильной, что даже свет не может вырваться. Они формируются после гибели массивных звёзд.</p>",
        5: "<h2>Космические миссии</h2><p>От «Аполлона-11» до марсохода Perseverance — люди уже много раз исследовали космос и продолжают открывать новое.</p>",
        6: "<h2>Будущее космоса</h2><p>Учёные планируют колонизацию Луны и Марса. Возможно, в будущем люди будут жить за пределами Земли.</p>"
    };

    function showPresentation(id) {
        const block = document.getElementById('presentation');
        block.innerHTML = presentations[id];
        block.style.display = 'block';
    }
</script>

</body>
</html>
