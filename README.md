<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Неоновые кнопки с платформами</title>
<style>
    body {
        background-color: #000;
        color: white;
        font-family: Arial, sans-serif;
        text-align: center;
        padding-top: 100px;
    }

    .neon-button {
        font-size: 20px;
        color: #fff;
        padding: 15px 30px;
        margin: 15px;
        border: none;
        cursor: pointer;
        border-radius: 5px;
        background: none;
        box-shadow: 0 0 5px #0ff, 0 0 15px #0ff, 0 0 30px #0ff;
        transition: all 0.3s ease;
    }

    .neon-button:hover {
        box-shadow: 0 0 10px #0ff, 0 0 20px #0ff, 0 0 40px #0ff;
    }

    /* Стили модального окна */
    .modal {
        display: none;
        position: fixed;
        z-index: 1000;
        padding-top: 100px;
        left: 0;
        top: 0;
        width: 100%;
        height: 100%;
        overflow: auto;
        background-color: rgba(0,0,0,0.8);
    }

    .modal-content {
        background-color: #111;
        margin: auto;
        padding: 20px;
        border: 1px solid #0ff;
        width: 50%;
        box-shadow: 0 0 15px #0ff;
        border-radius: 10px;
        text-align: left;
    }

    .close {
        color: #0ff;
        float: right;
        font-size: 28px;
        font-weight: bold;
        cursor: pointer;
    }

    .close:hover {
        color: #fff;
    }
</style>
</head>
<body>

<h1>Неоновые кнопки с платформами</h1>

<!-- Кнопки -->
<button class="neon-button" onclick="openModal('modal1')">Платформа 1</button>
<button class="neon-button" onclick="openModal('modal2')">Платформа 2</button>
<button class="neon-button" onclick="openModal('modal3')">Платформа 3</button>

<!-- Модальные окна -->
<div id="modal1" class="modal">
    <div class="modal-content">
        <span class="close" onclick="closeModal('modal1')">&times;</span>
        <h2>Платформа 1</h2>
        <p>Описание первой платформы. Здесь можно рассказать, что она делает и какие функции есть.</p>
    </div>
</div>

<div id="modal2" class="modal">
    <div class="modal-content">
        <span class="close" onclick="closeModal('modal2')">&times;</span>
        <h2>Платформа 2</h2>
        <p>Описание второй платформы. Тут можно добавить преимущества и уникальные особенности.</p>
    </div>
</div>

<div id="modal3" class="modal">
    <div class="modal-content">
        <span class="close" onclick="closeModal('modal3')">&times;</span>
        <h2>Платформа 3</h2>
        <p>Описание третьей платформы. Опиши, чем она полезна и кому подойдёт.</p>
    </div>
</div>

<script>
function openModal(id) {
    document.getElementById(id).style.display = "block";
}

function closeModal(id) {
    document.getElementById(id).style.display = "none";
}
</script>

</body>
</html>
