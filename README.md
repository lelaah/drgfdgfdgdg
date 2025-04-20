<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
    <title>Escolha seu Jogo</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 50px;
        }
        h1 {
            margin-bottom: 30px;
        }
        .jogo {
            display: inline-block;
            width: 200px;
            height: 150px;
            margin: 10px;
            padding: 20px;
            background-color: #4CAF50;
            color: white;
            font-size: 1.2em;
            border-radius: 8px;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        .jogo:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <h1>Escolha seu Jogo</h1>
    <div id="listaJogos">
        <div class="jogo" onclick="abrirJogo('velha')">Jogo da Velha</div>
        <!-- Você pode adicionar mais jogos aqui -->
        <div class="jogo" onclick="abrirJogo('quebra-cabeca')">Quebra-Cabeça</div>
        <div class="jogo" onclick="abrirJogo('snake')">Snake</div>
    </div>

    <script>
        function abrirJogo(nomeJogo) {
            // Aqui você pode redirecionar para a página do jogo correspondente
            if (nomeJogo === 'velha') {
                window.location.href = 'velha.html'; // Crie essa página depois
            } else if (nomeJogo === 'quebra-cabeca') {
                // window.location.href = 'quebra-cabeca.html';
                alert('Em breve!');
            } else if (nomeJogo === 'snake') {
                // window.location.href = 'snake.html';
                alert('Em breve!');
            }
        }
    </script>
</body>
</html>
