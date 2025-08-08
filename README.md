<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Неоновые кнопки с окнами</title>
<style>
    body {
        background: #000;
        color: white;
        font-family: Arial, sans-serif;
        text-align: center;
        padding-top: 50px;
    }

    /* Стиль кнопок */
    .neon-btn {
        display: inline-block;
        padding: 15px 30px;
        margin: 10px;
        font-size: 18px;
        color: #fff;
        border: 2px solid #0ff;
        border-radius: 10px;
        background: transparent;
        cursor: pointer;
        text-shadow: 0 0 5px #0ff, 0 0 10px #0ff;
        box-shadow: 0 0 5px #0ff, 0 0 20px #0ff inset;
        transition: 0.3s;
    }

    .neon-btn:hover {
        background: #0ff;
        color: #000;
        box-shadow: 0 0 20px #0ff, 0 0 40px #0ff;
    }

    /* Модальное окно */
    .modal {
        display: none;
        position: fixed;
        z-index: 1000;
        left: 0; top: 0;
        width: 100%; height: 100%;
        background-color: rgba(0,0,0,0.8);
        justify-content: center;
        align-items: center;
    }

    .modal-content {
        background: #111;
        border: 2px solid #0ff;
        padding: 20px;
        border-radius: 10px;
        width: 300px;
        text-shadow: 0 0 5px #0ff;
        box-shadow: 0 0 20px #0ff;
    }

    .close {
        color: #0ff;
        float: right;
        font-size: 24px;
        cursor: pointer;
    }
</style>
</head>
<body>

<h1>Неоновые кнопки с окнами</h1>

<!-- 6 кнопок -->
<button class="neon-btn" onclick="openModal(1)">Кнопка 1</button>
<button class="neon-btn" onclick="openModal(2)">Кнопка 2</button>
<button class="neon-btn" onclick="openModal(3)">Кнопка 3</button>
<button class="neon-btn" onclick="openModal(4)">Кнопка 4</button>
<button class="neon-btn" onclick="openModal(5)">Кнопка 5</button>
<button class="neon-btn" onclick="openModal(6)">Кнопка 6</button>

<!-- Окна -->
<div id="modal1" class="modal"><div class="modal-content"><span class="close" onclick="closeModal(1)">&times;</span><h2>Платформа 1</h2><p>Описание платформы 1.</p></div></div>
<div id="modal2" class="modal"><div class="modal-content"><span class="close" onclick="closeModal(2)">&times;</span><h2>Платформа 2</h2><p>Описание платформы 2.</p></div></div>
<div id="modal3" class="modal"><div class="modal-content"><span class="close" onclick="closeModal(3)">&times;</span><h2>Платформа 3</h2><p>Описание платформы 3.</p></div></div>
<div id="modal4" class="modal"><div class="modal-content"><span class="close" onclick="closeModal(4)">&times;</span><h2>Платформа 4</h2><p>Описание платформы 4.</p></div></div>
<div id="modal5" class="modal"><div class="modal-content"><span class="close" onclick="closeModal(5)">&times;</span><h2>Платформа 5</h2><p>Описание платформы 5.</p></div></div>
<div id="modal6" class="modal"><div class="modal-content"><span class="close" onclick="closeModal(6)">&times;</span><h2>Платформа 6</h2><p>Описание платформы 6.</p></div></div>

<script>
function openModal(num) {
    document.getElementById("modal" + num).style.display = "flex";
}
function closeModal(num) {
    document.getElementById("modal" + num).style.display = "none";
}
</script>

</body>
</html>
