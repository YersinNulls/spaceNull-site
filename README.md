<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SpaceNull</title>
<style>
    body {
        margin: 0;
        height: 100vh;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        font-family: Arial, sans-serif;
        color: white;
        overflow: hidden;
    }

    /* Анимированный фон космоса */
    body::before {
        content: "";
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: url('https://cdn.pixabay.com/photo/2017/08/30/01/05/space-2694031_1280.jpg') repeat;
        background-size: cover;
        animation: moveBg 60s linear infinite;
        z-index: -1;
    }

    @keyframes moveBg {
        0% { background-position: 0 0; }
        100% { background-position: -1000px 1000px; }
    }

    h1 {
        text-shadow: 0 0 20px #0ff;
        margin-bottom: 30px;
    }

    .buttons {
        display: flex;
        flex-direction: column;
        gap: 15px;
    }

    .btn {
        background: transparent;
        border: 2px solid #0ff;
        padding: 15px 30px;
        color: white;
        font-size: 18px;
        text-transform: uppercase;
        letter-spacing: 2px;
        border-radius: 10px;
        cursor: pointer;
        transition: all 0.3s ease;
        text-shadow: 0 0 5px #0ff;
        box-shadow: 0 0 20px #0ff;
    }

    .btn:hover {
        background: #0ff;
        color: black;
        box-shadow: 0 0 30px #0ff, 0 0 60px #0ff;
    }
</style>
</head>
<body>
    <h1>🚀 SpaceNull Project</h1>
    <div class="buttons">
        <button class="btn" onclick="openPresentation(1)">Планеты</button>
        <button class="btn" onclick="openPresentation(2)">Звёзды</button>
        <button class="btn" onclick="openPresentation(3)">Галактики</button>
        <button class="btn" onclick="openPresentation(4)">Чёрные дыры</button>
        <button class="btn" onclick="openPresentation(5)">Космические миссии</button>
        <button class="btn" onclick="openPresentation(6)">Будущее космоса</button>
    </div>

<script>
function openPresentation(num) {
    const links = {
        1: "https://example.com/planets",
        2: "https://example.com/stars",
        3: "https://example.com/galaxies",
        4: "https://example.com/blackholes",
        5: "https://example.com/missions",
        6: "https://example.com/future"
    };
    window.open(links[num], "_blank");
}
</script>
</body>
</html>
