# Giovanni-s-World
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Giovanni's Secrets</title>
    <style>
        body {
            font-family: 'Times New Roman', Times, serif;
            background-color: white; /* Fundo branco */
            display: flex;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
        }

        .container {
            text-align: center;
        }

        button {
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            font-family: 'Times New Roman', Times, serif;
        }

        #secretMessage {
            margin-top: 20px;
            display: none;
        }

        #gatoImg {
            max-width: 100%;
            height: auto;
            max-height: 100%; /* Altura máxima ajustada */
            display: none;
        }

        .italic-text {
            font-size: 15px;
            font-style: italic;
            z-index: 1; /* Garante que o texto fique acima da imagem */
            position: relative; /* Define o posicionamento em relação ao contêiner pai */
        }

        #booText {
            font-size: 20px;
            font-weight: bold;
        }

        #welcomeText {
            display: block; /* Garante que o texto de boas-vindas seja visível inicialmente */
        }
    </style>
</head>
<body>
    <div class="container">
        <h1 id="welcomeText">Welcome to Giovanni's World</h1>
        <button id="revealButton" onclick="revealSecret()">Clique aqui</button>
        <div id="secretMessage" class="hidden">
            <p id="booText">BOOO!</p>
            <p><span class="italic-text">A curiosidade matou o gato,</span> agora restam-lhe seis chances.</p>
            <img id="gatoImg" src="https://i.pinimg.com/originals/ad/e0/8c/ade08c4fc1f0237db5de58923126c05b.jpg" alt="Gato Preto Assustado">
        </div>
    </div>

    <script>
        function revealSecret() {
            document.getElementById('welcomeText').style.display = 'none'; // Oculta o texto de boas-vindas
            document.getElementById('secretMessage').style.display = 'block';
            document.getElementById('gatoImg').style.display = 'block';
            document.getElementById('revealButton').style.display = 'none';
        }
    </script>
</body>
</html>

