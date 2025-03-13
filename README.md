
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minecraft - Официальный сайт</title>
    <style>
        body {
            background-image: url('фон2.jpg');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            font-family: Arial, sans-serif;
            color: #333;
        }
        header {
            text-align: center;
            padding: 20px;
            background-color: rgba(0, 0, 0, 0.8);
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.5);
        }
        #logo {
            width: 200px;
            cursor: pointer;
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
            color: white;
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
        /* Стили для кнопки переключения темы */
        #theme-toggle {
            position: fixed;
            top: 20px;
            right: 20px;
            background-color: #4CAF50;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
            transition: background-color 0.3s, transform 0.2s;
            z-index: 500;
        }
        #theme-toggle:hover {
            background-color: #367c39;
            transform: scale(1.05);
        }
        /* Остальные стили остаются без изменений */
        .modal {
            display: none; /* Скрыто по умолчанию */
            position: fixed;
            z-index: 1000;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            overflow: auto;
            background-color: rgb(0,0,0);
            background-color: rgba(0,0,0,0.4);
        }
        .modal-content {
            background-color: #fefefe;
            margin: 15% auto;
            padding: 20px;
            border: 1px solid #888;
            width: 80%;
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
    </style>
</head>
<body>
    <button id="theme-toggle">поменять тему</button>
    <header>
        <img id="logo" src="логотип.webp" alt="Логотип"> <!-- Логотип -->
        <nav>
            <img src="иконка.png" alt="Иконка 1"> <!-- Иконка 1 -->
            <img src="л.webp" alt="Иконка 2"> <!-- Иконка 2 -->
        </nav>
    </header>
    <main>
        <h1>Добро пожаловать в Minecraft!</h1>
        <h2>Информация</h2>
        <p>Это страница с дополнительной информацией.</p>
        <p><a href="2part" style="color: #7FFF00; font-size: 20px;">О игре</a></p>
        <h2>Скриншоты игрового процесса</h2>
        <img class="screenshot" src="иг процесс.png" alt="Скриншот 1
        <img class="screenshot" src="иг процесс.png" alt="Скриншот 1"> <!-- Скриншот 1 -->
        <img class="screenshot" src="игг.webp" alt="Скриншот 2"> <!-- Скриншот 2 -->
    </main>
    <!-- Модальное окно -->
    <div id="myModal" class="modal">
        <div class="modal-content">
            <span class="close">&times;</span>
            <p>Добро пожаловать в наш великолепный сайт!</p>
        </div>
    </div>
    <!-- Раздел новостей и комментариев -->
    <section id="news-section">
        <h2>Новости</h2>
        <div class="news-item">
            <h3>Вышло новое обновление Minecraft!</h3>
            <p>1. У свиней появились новые окрасы</p>
            <p>2. Листья начали опадать</p>
            <div class="comments">
                <h4>Комментарии:</h4>
                <div class="comment">
                    <b>игрок1:</b> шикарное обновление!
                </div>
                <div class="comment">
                    <b>игрок2:</b> жду новых возможностей!
                </div>
            </div>
        </div>
    </section>
    <script>
        // Переключение темы
        const themeToggleButton = document.getElementById('theme-toggle');
        let isDarkTheme = false;
        themeToggleButton.addEventListener('click', () => {
            isDarkTheme = !isDarkTheme;
            document.body.style.backgroundColor = isDarkTheme ? '#333' : '#fff';
            document.body.style.color = isDarkTheme ? '#fff' : '#333';
            themeToggleButton.style.backgroundColor = isDarkTheme ? '#555' : '#4CAF50';
        });
        // Модальное окно
        const modal = document.getElementById("myModal");
        const span = document.getElementsByClassName("close")[0];
        // Показать модальное окно при нажатии на логотип
        const logo = document.getElementById("logo");
        logo.onclick = function() {
            modal.style.display = "block";
        }
        // Закрытие модального окна
        span.onclick = function() {
            modal.style.display = "none";
        }
        window.onclick = function(event) {
            if (event.target == modal) {
                modal.style.display = "none";
            }
        }
    </script>
</body>
</html>
