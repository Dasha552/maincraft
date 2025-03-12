<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>О игре</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            background-color: #f4f4f4;
            margin: 0;
            padding: 20px;
        }
        h1, h2 {
            color: #333;
        }
        img {
            max-width: 100%;
            height: auto;
            transition: transform 0.2s;
        }
        img:hover {
            transform: scale(1.05);
        }
        .gallery img {
            cursor: pointer;
            max-width: 200px;
            margin: 10px;
        }
        .form-container {
            background: #fff;
            padding: 20px;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            margin-top: 20px;
        }
        .form-container input, .form-container textarea {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        .form-container button {
            background: #5cb85c;
            color: #fff;
            border: none;
            padding: 10px 15px;
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s;
        }
        .form-container button:hover {
            background: #4cae4c;
        }
        .faq {
            margin-top: 20px;
        }
        .faq h3 {
            cursor: pointer;
        color: #007bff;
        }
        .faq p {
            display: none;
            margin: 0;
            padding: 10px 0;
        }
    </style>
</head>
<body>
    <h1>О нашей игре</h1>
    <p>Творческая игра, в которой основное внимание уделяется строительству.</p>
    <img src="лох.png" alt="Изображение игры">
    <h2>Трейлер игры</h2>
    <video width="600" controls>
        <source src="ScreenRecording_03-12-2025 12-12-14_1.mov" type="vid">
        Ваш браузер не поддерживает видео.
    </video>
    <div class="form-container">
        <h2>Обратная связь</h2>
        <form id="contact-form">
            <input type="text" id="name" placeholder="Имя" required>
            <input type="email" id="email" placeholder="Email" required>
            <textarea id="message" rows="4" placeholder="Сообщение" required></textarea>
            <button type="submit">Отправить</button>
        </form>
        <p id="response-message" style="color: green; display: none;">Ваше сообщение принято, мы скоро ответим!</p>
    </div>
    <div class="gallery">
        <h2>Галерея</h2>
        <img src="image1.jpg" alt="Изображение 1" onclick="фон2.jpg">
        <img src="image2.jpg" alt="Изображение 2" onclick="openImage(this.src)">
        <img src="image3.jpg" alt="Изображение 3" onclick="openImage(this.src)">
        <img src="image4.jpg" alt="Изображение 4" onclick="openImage(this.src)">
        <img src="image5.jpg" alt="Изображение 5" onclick="openImage(this.src)">
    </div>
    <div class="faq">
        <h2>Часто задаваемые вопросы (FAQ)</h2>
        <h3 onclick="toggleFAQ(1)">Как установить игру?</h3>
        <p id="faq-answer-1">Инструкции по установке игры можно найти на странице загрузки.</p>
        <h3 onclick="toggleFAQ(2)">Есть ли системные требования?</h3>
        <p id="faq-answer-2">Да, минимальные системные требования указаны на странице игры.</p>
        <h3 onclick="toggleFAQ(3)">Как связаться с поддержкой?</h3>
        <p id="faq-answer-3">Вы можете связаться с нами через форму обратной связи или по email.</p>
    </div>
    <script>
        document.getElementById('contact-form').addEventListener('submit', function(event) {
            event.preventDefault();
            document.getElementById('response-message').style.display = 'block';
            this.reset();
        });
function toggleFAQ(number) {
            const answer = document.getElementById(faq-answer-${number});
            answer.style.display = answer.style.display === 'block' ? 'none' : 'block';
        }
        function openImage(src) {
            const imgWindow = window.open("", "_blank");
            imgWindow.document.write(<img src="${src}" style="max-width:100%;"/>);
        }
    </script>
</body>
</html>
