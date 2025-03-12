<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minecraft - Официальный сайт</title>
    <style>
        body {
    background-image: url('фон2.jpg'); /* Укажите путь к вашему изображению */
    background-size: cover; /* Растягиваем изображение на весь экран */
    background-position: center; /* Центрируем изображение */
    background-attachment: fixed; /* Фон остается фиксированным при прокрутке */   
        }
        header {
            text-align: center;
            padding: 20px;
            background-color: rgba(0, 0, 0, 0.8);
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.5);
        }
        #logo {
            width: 200px; /* Размер логотипа */ 
        }
        nav {
            margin: 20px 0;
        }
        nav img {
            width: 50px; /* Размер иконок меню */
            margin: 0 10px;
            cursor: pointer;
            transition: transform 0.3s;
        }
        nav img:hover {
            transform: scale(1.1);
        }
        main {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 20px;
            background-color: rgba(0, 0, 0, 0.7);
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.5);
        }
        h1 {
            margin-bottom: 20px;
        }
        .screenshot {
            width: 300px; /* Размер скриншотов */
            margin: 10px;
            border-radius: 5px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.3);
        }
if (category === 'all') {
screenshots. forEach(img => img-classList.add('show'));
} else if (category == 'category1') {
 if (screenshots [0]) {
screenshots[0].classList.add('show'); 
} else if (category === 'category2') {
if (screenshots[1]) screenshots [1].classlist.add('show'); 
if (screenshots[2]) screenshots [2].classList.add('show'); 
else if (category === 'category3') {
if (screenshots[3]) screenshots[3] classList.add('show');
    </style>
</head>
<body>
    <header>
        <img id="logo" src="логотип.webp"> <!-- Логотип -->
        <nav>
            <img src="иконка.png"> <!-- Иконка 1 -->
            <img src="л.webp" alt="Иконка 2"> <!-- Иконка 2 -->
        </nav>
    </header>
    <main>
        <h1>Добро пожаловать в Minecraft!</h1>
        <h2>Скриншоты игрового процесса</h2>
        <img class="screenshot" src="иг процес.png"> <!-- Скриншот 1 -->
        <img class="screenshot" src="игг.webp"> <!-- Скриншот 2 -->
    </main>
</body>
</html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minecraft - Официальный сайт</title>
    <style>
        /* Основные стили */
        body {
            background-image: url('images/ajyy.webp');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            font-family: Arial, sans-serif;
            color: #333; /* Цвет текста по умолчанию */
        }
        header {
            text-align: center;
            padding: 20px;
            background-color: rgba(0, 0, 0, 0.8);
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.5);
        }
        #logo {
            width: 200px;
            cursor: pointer; /* Изменяем курсор на руку */
        }
        nav {
            margin: 20px 0;
        }
        nav img {
            width: 50px;
            margin: 0 10px;
            cursor: pointer;
            transition: transform 0.3s;
        }
        nav img:hover {
            transform: scale(1.1);
        }
        main {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 20px;
            background-color: rgba(0, 0, 0, 0.7);
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.5);
            color: white; /* Цвет текста в main */
        }
        h1 {
            margin-bottom: 20px;
        }
        .screenshot {
            width: 300px;
            margin: 10px;
            border-radius: 5px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.3);
        }
        /* Стили для модального окна */
        .modal {
            display: none; /* Скрыто по умолчанию */
            position: fixed; /* Фиксированное положение */
            z-index: 1; /* Поверх всего */
            left: 0;
            top: 0;
            width: 100%; /* Полная ширина */
            height: 100%; /* Полная высота */
            overflow: auto; /* Включаем прокрутку, если много контента */
            background-color: rgba(0, 0, 0, 0.4); /* Полупрозрачный фон */
        }
        .modal-content {
            background-color: #fefefe;
            margin: 15% auto; /* Центрируем по вертикали и горизонтали */
            padding: 20px;
            border: 1px solid #888;
            width: 80%; /* Ширина контента */
color: black;
        }
       .close {
            color: #aaa;
            float: right;
            font-size: 28px;
            font-weight: bold;
        }
        .close:hover,
        .close:focus {
            color: black;
            text-decoration: none;
            cursor: pointer;
        }
        /* Стили для тёмной темы */
        .dark-mode {
            background-color: #333;
            color: #fff;
        }
        .dark-mode main {
            background-color: rgba(0, 0, 0, 0.9);
        }
        /* Стили для новостей и комментариев */
        #news-section {
            width: 80%;
            margin: 20px auto;
            padding: 20px;
            background-color: rgba(0, 0, 0, 0.7);
            color: white;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.5);
        }
        .news-item {
            margin-bottom: 20px;
        }
        .comment {
            margin-top: 10px;
            padding: 5px;
            border-left: 3px solid #ccc;
        }
        /* Стили для формы комментариев */
        #comment-form {
            margin-top: 20px;
        }
        #comment-form input[type="text"],
        #comment-form textarea {
            width: 100%;
            padding: 8px;
            margin-bottom: 10px;
            border: 1px solid #ddd;
            border-radius: 4px;
        }
        #comment-form button {
            background-color: #5cb85c;
            color: white;
            padding: 10px 15px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        #comment-form button:hover {
            background-color: #449d44;
        }
        /* Стили для переключателя темы */
        #theme-toggle {
            position: fixed;
            top: 20px;
            right: 20px;
            background-color: #4CAF50;
            color: white;
            padding: 10px 15px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            z-index: 500; /* Чтобы кнопка была поверх всего */
        }
        #theme-toggle:hover {
            background-color: #367c39;
        }
    </style>
</head>
<body>
    <button id="theme-toggle">поменять тему</button>
    <main>
    <!-- Модальное окно -->
    <div id="myModal" class="modal">
        <div class="modal-content">
            <span class="close">&times;</span>
            <p>Добро пожаловать в наш великолепный сайт!!!!!!!!!!!</p>
        </div>
    </div>
    <!-- Раздел новостей и комментариев -->
    <section id="news-section">
        <h2>Новости</h2>
        <div class="news-item">
            <h3>Вышло новое обновление Minecraft!</h3>
            <p>1.у свиней появились новые окрасы</p>
            <p>2.листья начали опадать</p>
            <div class="comments">
                <h4>Комментарии:</h4>
                <div class="comment">
                    <b>игрок1:</b> шикарное обновление!
                </div>
                <div class="comment">
                    <b>игрок2:</b> очень понравилось!
                </div>
            </div>
            <!-- Форма для добавления комментария -->
            <form id="comment-form">
                <input type="text" id="comment-name" placeholder="Ваше имя">
                <textarea id="comment-text" placeholder="Ваш комментарий"></textarea>
                <button type="button" onclick="addComment()">Отправить</button>
            </form>
        </div>
    </section>
    <script>
        // Модальное окно
        var modal = document.getElementById("myModal");
        var logo = document.getElementById("logo");
        var span = document.getElementsByClassName("close")[0];
        logo.onclick = function() {
            modal.style.display = "block";
        }
        span.onclick = function() {
            modal.style.display = "none";
        }
        window.onclick = function(event) {
            if (event.target == modal) {
                modal.style.display = "none";
            }
        }
        // Тёмная тема
        const themeToggle = document.getElementById('theme-toggle');
        const body = document.querySelector('body');
        themeToggle.addEventListener('click', function() {
            body.classList.toggle('dark-mode');
        });
        // Добавление комментария
        function addComment() {
            var name = document.getElementById('comment-name').value;
            var text = document.getElementById('comment-text').value;
            if (name && text) {
                var commentDiv = document.createElement('div');
                commentDiv.classList.add('comment');
                commentDiv.innerHTML = '<b>' + name + ':</b> ' + text;
                var commentsContainer = document.querySelector('.comments');
                commentsContainer.appendChild(commentDiv);
                // Очищаем поля формы
                document.getElementById('comment-name').value = '';
                document.getElementById('comment-text').value = '';
            } else {
                alert('Пожалуйста, заполните все поля!');
            }
        }
    </script>
<body>
    <h1>Информация</h1>
    <p>Это страница с дополнительной информацией.</p>
    <p><a href="2part" style="color: #7FFF00; font-size: 20px;">  тык</a></p>
</body>
