<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Conexão de Amor</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f8ff;
            color: #333;
            text-align: center;
            padding: 20px;
        }
        .container {
            max-width: 600px;
            margin: 0 auto;
        }
        .message {
            margin: 20px 0;
            padding: 20px;
            background-color: #e6e6fa;
            border-radius: 10px;
        }
        .button {
            background-color: #4CAF50;
            color: white;
            padding: 15px 20px;
            margin: 10px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .button:hover {
            background-color: #45a049;
        }
        .hidden {
            display: none;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Conexão de Amor</h1>
        <p>Um jogo de caça ao tesouro virtual que celebra a nossa história de amor.</p>

        <div id="step1" class="message">
            <h2>Capítulo 1: O Primeiro Contato</h2>
            <p>Ana e Mariana se conheceram em um fórum sobre música. Encontre a música especial que as conectou.</p>
            <button class="button" onclick="revealStep('step2')">Ouvir Música</button>
        </div>

        <div id="step2" class="message hidden">
            <h2>Mensagem</h2>
            <p>A música nos uniu, e com ela, nosso coração começou a bater no mesmo ritmo.</p>
            <button class="button" onclick="revealStep('step3')">Próximo</button>
        </div>

        <div id="step3" class="message hidden">
            <h2>Capítulo 2: Mensagens Carinhosas</h2>
            <p>Ana e Mariana compartilham fotos de seus lugares favoritos. Encontre esses lugares no mapa interativo.</p>
            <button class="button" onclick="revealStep('step4')">Abrir Mapa</button>
        </div>

        <div id="step4" class="message hidden">
            <h2>Mensagem</h2>
            <p>Mesmo à distância, sinto que estou perto de você.</p>
            <button class="button" onclick="revealStep('step5')">Próximo</button>
        </div>

        <div id="step5" class="message hidden">
            <h2>Capítulo 3: O Primeiro Encontro Virtual</h2>
            <p>Ana e Mariana decidem ter seu primeiro encontro virtual. Ajude Mariana a escolher a roupa certa.</p>
            <button class="button" onclick="revealStep('step6')">Escolher Roupa</button>
        </div>

        <div id="step6" class="message hidden">
            <h2>Mensagem</h2>
            <p>Estar com você, mesmo que virtualmente, é o que mais desejo.</p>
            <button class="button" onclick="revealStep('step7')">Próximo</button>
        </div>

        <div id="step7" class="message hidden">
            <h2>Capítulo 4: Planejando o Futuro</h2>
            <p>Ana e Mariana fazem planos para se encontrarem. Complete o quebra-cabeça para ver onde elas irão.</p>
            <button class="button" onclick="revealStep('step8')">Resolver Quebra-Cabeça</button>
        </div>

        <div id="step8" class="message hidden">
            <h2>Mensagem</h2>
            <p>O futuro parece brilhante porque você está nele.</p>
            <button class="button" onclick="revealStep('step9')">Próximo</button>
        </div>

        <div id="step9" class="message hidden">
            <h2>Capítulo 5: A Grande Surpresa</h2>
            <p>Ana planeja uma surpresa especial para Mariana. Ajude-a a decifrar o código para descobrir o que é.</p>
            <button class="button" onclick="revealStep('step10')">Decifrar Código</button>
        </div>

        <div id="step10" class="message hidden">
            <h2>Mensagem Final</h2>
            <p>Nosso amor ultrapassou todas as barreiras, e agora estamos prestes a nos encontrar.</p>
            <button class="button" onclick="revealStep('end')">Finalizar</button>
        </div>

        <div id="end" class="message hidden">
            <h2>O Encontro</h2>
            <p>De todas as aventuras que já vivi, encontrar você foi a mais incrível. Mal posso esperar para viver o resto da minha vida ao seu lado.</p>
        </div>
    </div>

    <script>
        function revealStep(stepId) {
            document.querySelectorAll('.message').forEach(function(step) {
                step.classList.add('hidden');
            });
            document.getElementById(stepId).classList.remove('hidden');
        }
    </script>
</body>
</html>

