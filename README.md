<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Snake Game - Play Now</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <!-- Opening Animation Screen -->
        <div id="openingScreen" class="screen opening-screen">
            <div class="opening-content">
                <h1 class="opening-title">🐍 SNAKE GAME</h1>
                <p class="opening-subtitle">Classic Game with Modern Twist</p>
                <div class="animated-snake"></div>
                <button id="startBtn" class="btn btn-primary">START GAME</button>
                <p class="opening-hint">Or press SPACEBAR to begin</p>
            </div>
        </div>

        <!-- Game Screen -->
        <div id="gameScreen" class="screen game-screen" style="display: none;">
            <div class="game-header">
                <div class="score-container">
                    <h2>Score: <span id="score">0</span></h2>
                    <h3>High Score: <span id="highScore">0</span></h3>
                </div>
                <button id="quitBtn" class="btn btn-secondary">QUIT</button>
            </div>

            <div class="canvas-container">
                <canvas id="gameCanvas" width="400" height="400"></canvas>
            </div>

            <div class="controls-info">
                <p>Use ARROW KEYS to move • SPACEBAR to pause</p>
            </div>
        </div>

        <!-- Game Over Screen -->
        <div id="gameOverScreen" class="screen game-over-screen" style="display: none;">
            <div class="game-over-content">
                <h1>GAME OVER</h1>
                <div class="final-stats">
                    <p>Final Score: <span id="finalScore">0</span></p>
                    <p>High Score:  <span id="gameOverHighScore">0</span></p>
                </div>
                <button id="restartBtn" class="btn btn-primary">PLAY AGAIN</button>
                <button id="quitToMenuBtn" class="btn btn-secondary">MAIN MENU</button>
                <p class="hint">Or press SPACEBAR</p>
            </div>
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html>
