<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <title>Генератор Безумия v1.0</title>
    <style>
        body {
            background: linear-gradient(45deg, #ff00ff, #00ffff, #ffff00);
            background-size: 400% 400%;
            animation: gradient 5s ease infinite;
            overflow: hidden;
            color: #fff;
            font-family: 'Comic Sans MS', cursive;
            text-align: center;
        }

        @keyframes gradient {
            0% {background-position: 0% 50%;}
            50% {background-position: 100% 50%;}
            100% {background-position: 0% 50%;}
        }

        .chaos-box {
            margin-top: 15vh;
            transform: rotate(-5deg);
            background: rgba(0, 0, 0, 0.8);
            padding: 50px;
            border: 10px dashed lime;
            display: inline-block;
        }

        h1 {
            font-size: 5rem;
            text-shadow: 5px 5px #ff0000;
            animation: shake 0.5s infinite;
        }

        @keyframes shake {
            0% { transform: translate(1px, 1px) rotate(0deg); }
            10% { transform: translate(-1px, -2px) rotate(-1deg); }
            20% { transform: translate(-3px, 0px) rotate(1deg); }
            50% { transform: translate(1px, 2px) rotate(0deg); }
            100% { transform: translate(1px, -2px) rotate(-1deg); }
        }

        .btn {
            padding: 20px 40px;
            font-size: 24px;
            background: red;
            color: white;
            border: none;
            cursor: pointer;
            box-shadow: 10px 10px 0px blue;
        }

        .btn:hover {
            transform: scale(2) rotate(360deg);
            transition: 0.5s;
            background: yellow;
            color: black;
        }
    </style>
</head>
<body>

    <div class="chaos-box">
        <h1>АБРАКАДАБРА!</h1>
        <p style="font-size: 20px;">Если ты это видишь, значит GitPages живой.</p>
        <p>Текущее время в параллельной вселенной: <span id="time"></span></p>
        <button class="btn" onclick="alert('ТЫ ТЫКНУЛ В КНОПКУ ИЗ ИНТЕРНЕТА!')">НЕ НАЖИМАТЬ</button>
    </div>

    <script>
        // Рандомные цифры для вида
        setInterval(() => {
            document.getElementById('time').innerText = Math.random().toString(36).substring(2, 15);
        }, 100);

        console.log("Windneiro, поздравляю! Ты заглянул в консоль!");
    </script>
</body>
</html>
