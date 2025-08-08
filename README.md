<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Space Null</title>
<style>
    body {
        background-color: #000;
        color: white;
        font-family: Arial, sans-serif;
        text-align: center;
        padding: 50px;
    }
    h1 {
        font-size: 2.5em;
        margin-bottom: 20px;
    }
    .button-container {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 20px;
    }
    .neon-button {
        background: none;
        border: 2px solid #0ff;
        color: #0ff;
        padding: 15px 30px;
        font-size: 1.2em;
        cursor: pointer;
        border-radius: 10px;
        text-shadow: 0 0 5px #0ff, 0 0 10px #0ff;
        box-shadow: 0 0 5px #0ff, 0 0 20px #0ff inset;
        transition: 0.3s;
    }
    .neon-button:hover {
        background: #0ff;
        color: black;
        box-shadow: 0 0 20px #0ff, 0 0 40px #0ff;
    }
    .desc {
        font-size: 0.9em;
        color: #ccc;
        margin-top: 5px;
    }
</style>
</head>
<body>
    <h1>🚀 Space Null</h1>
    <div class="button-container">
        <div>
            <button class="neon-button" onclick="alert('Информация о галактиках')">Галактики</button>
            <div class="desc">Узнай о далеких звездных системах</div>
        </div>
        <div>
            <button class="neon-button" onclick="alert('Информация о планетах')">Планеты</button>
            <div class="desc">Исследуй миры в нашей Вселенной</div>
        </div>
        <div>
            <button class="neon-button" onclick="alert('Информация о звездах')">Звезды</button>
            <div class="desc">Огромные шары плазмы в космосе</div>
        </div>
        <div>
            <button class="neon-button" onclick="alert('Информация о черных дырах')">Черные дыры</button>
            <div class="desc">Тайны гравитационных монстров</div>
        </div>
        <div>
            <button class="neon-button" onclick="alert('Информация о космонавтах')">Космонавты</button>
            <div class="desc">Люди, исследующие космос</div>
        </div>
        <div>
            <button class="neon-button" onclick="alert('Информация о миссиях в космосе')">Космические миссии</button>
            <div class="desc">Истории великих полетов</div>
        </div>
    </div>
</body>
</html>
