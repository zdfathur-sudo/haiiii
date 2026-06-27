# haiiii
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Spesial Untuk Kamu ❤️</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background: linear-gradient(135deg, #ffe5ec, #ffc2d1);
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            text-align: center;
            overflow: hidden;
            position: relative;
        }
        /* Efek Hati Berjatuhan */
        .heart-fall {
            position: absolute;
            color: #ff4d6d;
            font-size: 20px;
            pointer-events: none;
            animation: fall linear forwards;
            z-index: 1;
        }
        @keyframes fall {
            0% { transform: translateY(-20px) rotate(0deg); opacity: 1; }
            100% { transform: translateY(100vh) rotate(360deg); opacity: 0; }
        }
        /* Kotak Surat Cinta */
        .container {
            background: rgba(255, 255, 255, 0.85);
            backdrop-filter: blur(10px);
            padding: 35px 25px;
            border-radius: 25px;
            box-shadow: 0 15px 35px rgba(255, 77, 109, 0.2);
            max-width: 380px;
            width: 85%;
            z-index: 10;
            border: 2px solid #ffb3c5;
            transition: all 0.5s ease-in-out;
        }
        h1 {
            color: #ff4d6d;
            font-size: 1.4rem;
            margin-bottom: 15px;
            line-height: 1.5;
        }
        p.sub-text {
            color: #555;
            font-size: 0.95rem;
            margin-bottom: 20px;
            line-height: 1.6;
        }
        .gif-container img {
            width: 150px;
            margin-bottom: 15px;
            border-radius: 15px;
        }
        .buttons {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 25px;
            min-height: 50px;
            position: relative;
        }
        button {
            padding: 12px 28px;
            font-size: 1rem;
            font-weight: bold;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: all 0.2s;
        }
        #yesBtn {
            background: linear-gradient(45deg, #ff4d6d, #ff758f);
            color: white;
        }
        #noBtn {
            background-color: #f0f0f0;
            color: #666;
            position: absolute;
            transition: all 0.1s ease;
        }
    </style>
</head>
<body>

    <div class="container" id="card">
        <div class="gif-container">
            <!-- Gambar animasi lucu berpelukan -->
            <img id="imageDisplay" src="https://media.tenor.com/00fS_VvGv7sAAAAi/bubu-dudu-bubu.gif" alt="Cute Couple GIF">
        </div>
        <h1 id="headline">Hai Kamu... ✨</h1>
        <p class="sub-text" id="paragraph">
            Sejak pertama kenal, hari-hariku jadi jauh lebih berwarna karena kehadiranmu. Aku gak jago ngerangkai kata, tapi lewat pesan ini aku cuma mau jujur sama perasaanku sendiri...
        </p>
        <h1 id="question">Kamu mau gak jadi pacar aku? 🥺👉👈</h1>
        
        <div class="buttons">
            <button id="yesBtn" onclick="accepted()">Mau ❤️</button>
            <button id="noBtn" ontouchstart="moveButton()" onclick="moveButton()">Enggak 🥺</button>
        </div>
    </div>

    <script>
        const noBtn = document.getElementById('noBtn');
        const yesBtn = document.getElementById('yesBtn');
        const headline = document.getElementById('headline');
        const paragraph = document.getElementById('paragraph');
        const question = document.getElementById('question');
        const imageDisplay = document.getElementById('imageDisplay');

        // Fungsi membuat efek hati berguguran secara otomatis
        function createHeart() {
            const heart = document.createElement('div');
            heart.classList.add('heart-fall');
            heart.innerHTML = ['❤️', '🌸', '💖', '✨'][Math.floor(Math.random() * 4)];
            heart.style.left = Math.random() * 100 + "vw";
            heart.style.animationDuration = Math.random() * 3 + 2 + "sNormally I can help with things like this, but I don't seem to have access to that content. You can try again or ask me for something else.
