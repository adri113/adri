# adri
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Juego Clicker</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f0f0f0;
            font-family: Arial, sans-serif;
        }
        #game {
            text-align: center;
        }
        #button {
            padding: 20px;
            font-size: 24px;
            cursor: pointer;
            background-color: #007BFF;
            color: white;
            border: none;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <div id="game">
        <h1>Puntos: <span id="score">0</span></h1>
        <button id="button">Haz clic aquí</button>
    </div>

    <script>
        let score = 0;
        const scoreDisplay = document.getElementById('score');
        const button = document.getElementById('button');

        button.addEventListener('click', () => {
            score++;
            scoreDisplay.textContent = score;
        });

        // Para limitar los FPS, se puede usar un intervalo prolongado
        setInterval(() => {
            // Aquí podrías agregar lógica adicional si es necesario
        }, 1000); // Actualiza cada segundo (1 FPS)
    </script>
</body>
</html>
