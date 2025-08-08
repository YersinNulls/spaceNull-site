<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Космос</title>
<style>
    body {
        margin: 0;
        font-family: Arial, sans-serif;
        background-color: #000;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        height: 100vh;
        color: white;
    }
    h1 {
        margin-bottom: 30px;
        text-shadow: 0 0 10px cyan, 0 0 20px blue;
    }
    .button-container {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 20px;
    }
    .neon-button {
        padding: 15px 30px;
        font-size: 18px;
        color: white;
        background: transparent;
        border: 2px solid cyan;
        border-radius: 10px;
        cursor: pointer;
        text-shadow: 0 0 5px cyan, 0 0 10px blue;
        box-shadow: 0 0 10px cyan, 0 0 20px blue;
        transition: 0.3s;
    }
    .neon-button:hover {
        background-color: cyan;
        color: black;
        box-shadow: 0 0 20px cyan, 0 0 40px blue;
    }
</style>
</head>
<body>

<h1>Мир Космоса</h1>
<div class="button-container">
    <button class="neon-button" onclick="openWindow('Галактики', 'Огромные системы звезд, газа и туманностей.')">Галактики</button>
    <button class="neon-button" onclick="openWindow('Планеты', 'Мир, где могут быть океаны, горы и жизнь.')">Планеты</button>
    <button class="neon-button" onclick="openWindow('Звезды', 'Огненные шары, дающие свет и тепло.')">Звезды</button>
    <button class="neon-button" onclick="openWindow('Чёрные дыры', 'Объекты с гравитацией, из которой ничто не уходит.')">Чёрные дыры</button>
    <button class="neon-button" onclick="openWindow('Кометы', 'Ледяные странники, пролетающие мимо солнца.')">Кометы</button>
    <button class="neon-button" onclick="openWindow('Туманности', 'Красивые облака газа и пыли в космосе.')">Туманности</button>
</div>

<script>
function openWindow(title, description) {
    const newWin = window.open("", "_blank", "width=400,height=300");
    newWin.document.write(`
        <html>
        <head>
            <title>${title}</title>
            <style>
                body {
                    font-family: Arial;
                    background-color: black;
                    color: white;
                    text-align: center;
                    padding: 20px;
                }
                h2 { color: cyan; }
            </style>
        </head>
        <body>
            <h2>${title}</h2>
            <p>${description}</p>
        </body>
        </html>
    `);
}
</script>

</body>
</html>
