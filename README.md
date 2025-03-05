<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minecraft - Официальный сайт</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" integrity="sha512-9usAa10IRO0HhonpyAIVpjrylPvoDwiPUiKdWk5t3PyolY1cOd4DSE0Ga+ri4AuTroPR5aQvXU9xC6qOPnzFeg==" crossorigin="anonymous" referrerpolicy="no-referrer" />
</head>
<body>
    <header>
        <img id="logo" src="images/логотип.webp" alt="Логотип Minecraft">
        <nav>
            <img src="C:\Users\Студент\Desktop\настька дашка,т\иконка.png" alt="Иконка 1">
            <img src="C:\Users\Студент\Desktop\настька дашка,т\иконка.png" alt="Иконка 2">
            <img src="C:\Users\Студент\Desktop\настька дашка,т\иконка.png" alt="Иконка 3">
            <a href="#news"><img src="" alt="Новости"></a>
        </nav>
        <button id="theme-toggle">Сменить тему</button>
    </header>

    <main>
        <h1>Добро пожаловать в Minecraft!</h1>
        <h2>Скриншоты игрового процесса</h2>
        <div class="screenshots">
            <img class="screenshot" src="C:\Users\Студент\Desktop\настька дашка,т\иг процесс.webp" alt="Скриншот 1">
            <img class="screenshot" src="C:\Users\Студент\Desktop\настька дашка,т\иг процес.png" alt="Скриншот 2">
        </div>
    </main>

    <section id="news">
        <h2>Новости</h2>
        <article class="news-item">
            <h3>Новая версия Minecraft!</h3>
            <p>Вышло обновление с новыми блоками и мобами!</p>
            <p class="news-date">16.05.2024</p>
            <div class="comments">
                <h4>Комментарии:</h4>
                <ul class="comment-list">
                    </ul>
                <form class="comment-form">
                    <input type="text" placeholder="Ваше имя" id="comment-name">
                    <textarea placeholder="Ваш комментарий" id="comment-text"></textarea>
                    <button type="submit">Отправить</button>
                </form>
            </div>
        </article>
        <article class="news-item">
            <h3>Конкурс построек!</h3>
            <p>Примите участие в конкурсе и выиграйте ценные призы!</p>
            <p class="news-date">15.05.2024</p>
             <div class="comments">
                <h4>Комментарии:</h4>
                <ul class="comment-list">
                </ul>
                <form class="comment-form">
                    <input type="text" placeholder="Ваше имя" id="comment-name">
                    <textarea placeholder="Ваш комментарий" id="comment-text"></textarea>
                    <button type="submit">Отправить</button>
                </form>
            </div>
        </article>
    </section>

    <!-- Модальное окно -->
    <div id="modal" class="modal">
        <div class="modal-content">
            <span class="close">&times;</span>
            <p>Привет! Это модальное окно, которое появляется при клике на логотип.</p>
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html>
body {
    background-image: url('images/ajyy.webp');
    background-size: cover;
    background-position: center;
    background-attachment: fixed;
    color: white; /* Цвет текста по умолчанию для светлой темы */
    transition: background-color 0.3s, color 0.3s; /* Плавный переход для смены темы */
    font-family: sans-serif;
    margin: 0;
    padding: 0;
}

body.dark-theme {
    background-color: #333; /* Темный фон */
    color: #eee; /* Светлый текст для темной темы */
}

header {
    text-align: center;
    padding: 20px;
    background-color: rgba(0, 0, 0, 0.8);
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.5);
    position: relative; /* Для позиционирования кнопки смены темы */
}

#logo {
    width: 200px;
    cursor: pointer; /* Курсор меняется при наведении, показывая, что элемент кликабелен */
    transition: transform 0.3s ease-in-out; /* Анимация */
}

#logo:hover {
    transform: rotate(10deg) scale(1.1); /* Поворот при наведении */
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
    margin: 20px auto; /* Центрирование по горизонтали */
    max-width: 800px; /* Ограничение ширины */
}

h1 {
    margin-bottom: 20px;
}

.screenshot {
    width: 300px;
    margin: 10px;
    border-radius: 5px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.3);
    transition: transform 0.3s; /* Плавное изменение размера */
}

.screenshot:hover {
    transform: scale(1.05); /* Увеличение при наведении */
}

/* Раздел новостей */
#news {
    background-color: rgba(0, 0, 0, 0.7);
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.5);
    margin: 20px auto;
    max-width: 800px;
    color: white;
}

.news-item {
    margin-bottom: 20px;
    padding-bottom: 20px;
    border-bottom: 1px solid #555;
}

.news-item:last-child {
    border-bottom: none;
}

.news-date {
    font-size: 0.8em;
    color: #aaa;
}

/* Стили для комментариев */
.comments {
    margin-top: 20px;
}

.comment-list {
    list-style: none;
    padding: 0;
}

.comment-list li {
    margin-bottom: 10px;
    padding: 10px;
    background-color: rgba(255, 255, 255, 0.1);
    border-radius: 5px;
}

.comment-form {
    display: flex;
    flex-direction: column;
}

.comment-form input, .comment-form textarea {
    margin-bottom: 10px;
    padding: 8px;
    border-radius: 5px;
    border: none;
    background-color: rgba(255, 255, 255, 0.2);
    color: white;
}

.comment-form textarea {
    resize: vertical;
    height: 80px;
}

.comment-form button {
    padding: 10px 15px;
    background-color: #4CAF50;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.3s;
}

.comment-form button:hover {
    background-color: #367c39;
}

/* Стили для модального окна */
.modal {
    display: none; /* Скрыто по умолчанию */
    position: fixed;
    z-index: 1;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    overflow: auto;
    background-color: rgba(0, 0, 0, 0.4);
}

.modal-content {
    background-color: #fefefe;
    margin: 15% auto;
    padding: 20px;
    border: 1px solid #888;
    width: 80%;
    color: black;
    position: relative;
    border-radius: 5px;
}

.close {
    position: absolute;
    top: 0;
    right: 0;
    color: #aaa;
    font-size: 28px;
    font-weight: bold;
    padding: 5px;
    cursor: pointer;
}

.close:hover,
.close:focus {
    color: black;
    text-decoration: none;
    cursor: pointer;
}

/* Кнопка смены темы */
#theme-toggle {
    position: absolute;
    top: 10px;
    right: 10px;
    padding: 10px 15px;
    background-color: #428bca;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

/* Адаптивность */
@media (max-width: 600px) {
    #logo {
        width: 150px;
    }

    nav img {
        width: 40px;
        margin: 0 5px;
    }

    main {
        padding: 10px;
    }

    .screenshot {
        width: 100%; /* Занимает всю ширину на маленьких экранах */
    }
}
body {
    background-image: url('images/ajyy.webp');
    background-size: cover;
    background-position: center;
    background-attachment: fixed;
    color: white; /* Цвет текста по умолчанию для светлой темы */
    transition: background-color 0.3s, color 0.3s; /* Плавный переход для смены темы */
    font-family: sans-serif;
    margin: 0;
    padding: 0;
}

body.dark-theme {
    background-color: #333; /* Темный фон */
    color: #eee; /* Светлый текст для темной темы */
}

header {
    text-align: center;
    padding: 20px;
    background-color: rgba(0, 0, 0, 0.8);
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.5);
    position: relative; /* Для позиционирования кнопки смены темы */
}

#logo {
    width: 200px;
    cursor: pointer; /* Курсор меняется при наведении, показывая, что элемент кликабелен */
    transition: transform 0.3s ease-in-out; /* Анимация */
}

#logo:hover {
    transform: rotate(10deg) scale(1.1); /* Поворот при наведении */
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
    margin: 20px auto; /* Центрирование по горизонтали */
    max-width: 800px; /* Ограничение ширины */
}

h1 {
    margin-bottom: 20px;
}

.screenshot {
    width: 300px;
    margin: 10px;
    border-radius: 5px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.3);
    transition: transform 0.3s; /* Плавное изменение размера */
}

.screenshot:hover {
    transform: scale(1.05); /* Увеличение при наведении */
}

/* Раздел новостей */
#news {
    background-color: rgba(0, 0, 0, 0.7);
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.5);
    margin: 20px auto;
    max-width: 800px;
    color: white;
}

.news-item {
    margin-bottom: 20px;
    padding-bottom: 20px;
    border-bottom: 1px solid #555;
}

.news-item:last-child {
    border-bottom: none;
}

.news-date {
    font-size: 0.8em;
    color: #aaa;
}

/* Стили для комментариев */
.comments {
    margin-top: 20px;
}

.comment-list {
    list-style: none;
    padding: 0;
}

.comment-list li {
    margin-bottom: 10px;
    padding: 10px;
    background-color: rgba(255, 255, 255, 0.1);
    border-radius: 5px;
}

.comment-form {
    display: flex;
    flex-direction: column;
}

.comment-form input, .comment-form textarea {
    margin-bottom: 10px;
    padding: 8px;
    border-radius: 5px;
    border: none;
    background-color: rgba(255, 255, 255, 0.2);
    color: white;
}

.comment-form textarea {
    resize: vertical;
    height: 80px;
}

.comment-form button {
    padding: 10px 15px;
    background-color: #4CAF50;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.3s;
}

.comment-form button:hover {
    background-color: #367c39;
}

/* Стили для модального окна */
.modal {
    display: none; /* Скрыто по умолчанию */
    position: fixed;
    z-index: 1;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    overflow: auto;
    background-color: rgba(0, 0, 0, 0.4);
}

.modal-content {
    background-color: #fefefe;
    margin: 15% auto;
    padding: 20px;
    border: 1px solid #888;
    width: 80%;
    color: black;
    position: relative;
    border-radius: 5px;
}

.close {
    position: absolute;
    top: 0;
    right: 0;
    color: #aaa;
    font-size: 28px;
    font-weight: bold;
    padding: 5px;
    cursor: pointer;
}

.close:hover,
.close:focus {
    color: black;
    text-decoration: none;
    cursor: pointer;
}

/* Кнопка смены темы */
#theme-toggle {
    position: absolute;
    top: 10px;
    right: 10px;
    padding: 10px 15px;
    background-color: #428bca;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

/* Адаптивность */
@media (max-width: 600px) {
    #logo {
        width: 150px;
    }

    nav img {
        width: 40px;
        margin: 0 5px;
    }

    main {
        padding: 10px;
    }

    .screenshot {
        width: 100%; /* Занимает всю ширину на маленьких экранах */
    }
}
