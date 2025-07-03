# FPS-criador-por-IA
Esse e um game criador por IA
<!DOCTYPE html>
<html>
<head>
  <title>FPS Mobile Web Game</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body, html {
      margin: 0;
      padding: 0;
      overflow: hidden;
      touch-action: none;
    }
    canvas {
      display: block;
      width: 100vw;
      height: 100vh;
      background: #333;
    }
    #joystick {
      position: absolute;
      bottom: 20px;
      left: 20px;
      width: 100px;
      height: 100px;
      background: rgba(255,255,255,0.1);
      border-radius: 50%;
      touch-action: none;
    }
  </style>
</head>
<body>
  <canvas id="gameCanvas"></canvas>
  <div id="joystick"></div>

  <script>
    const canvas = document.getElementById("gameCanvas");
    const ctx = canvas.getContext("2d");
    canvas.width = window.innerWidth;
    canvas.height = window.innerHeight;

    let player = {
      x: canvas.width / 2,
      y: canvas.height / 2,
      angle: 0
    };

    let joystick = document.getElementById("joystick");
    let joyCenter = { x: 70, y: window.innerHeight - 70 };
    let move = { x: 0, y: 0 };

    joystick.addEventListener("touchmove", (e) => {
      let touch = e.touches[0];
      let dx = touch.clientX - joyCenter.x;
      let dy = touch.clientY - joyCenter.y;
      move.x = dx / 50;
      move.y = dy / 50;
      e.preventDefault();
    });

    joystick.addEventListener("touchend", () => {
      move = { x: 0, y: 0 };
    });

    function gameLoop() {
      ctx.clearRect(0, 0, canvas.width, canvas.height);
      player.x += move.x * 5;
      player.y += move.y * 5;
      ctx.fillStyle = "lime";
      ctx.fillRect(player.x - 10, player.y - 10, 20, 20);
      requestAnimationFrame(gameLoop);
    }

    gameLoop();
  </script>
</body>
</html>
<!DOCTYPE html>
<html>
<head>
  <title>FPS Mobile Web Game</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body, html {
      margin: 0;
      padding: 0;
      overflow: hidden;
      touch-action: none;
    }
    canvas {
      display: block;
      width: 100vw;
      height: 100vh;
      background: #333;
    }
    #joystick {
      position: absolute;
      bottom: 20px;
      left: 20px;
      width: 100px;
      height: 100px;
      background: rgba(255,255,255,0.1);
      border-radius: 50%;
      touch-action: none;
    }
  </style>
</head>
<body>
  <canvas id="gameCanvas"></canvas>
  <div id="joystick"></div>

  <script>
    const canvas = document.getElementById("gameCanvas");
    const ctx = canvas.getContext("2d");
    canvas.width = window.innerWidth;
    canvas.height = window.innerHeight;

    let player = {
      x: canvas.width / 2,
      y: canvas.height / 2,
      angle: 0
    };

    let joystick = document.getElementById("joystick");
    let joyCenter = { x: 70, y: window.innerHeight - 70 };
    let move = { x: 0, y: 0 };

    joystick.addEventListener("touchmove", (e) => {
      let touch = e.touches[0];
      let dx = touch.clientX - joyCenter.x;
      let dy = touch.clientY - joyCenter.y;
      move.x = dx / 50;
      move.y = dy / 50;
      e.preventDefault();
    });

    joystick.addEventListener("touchend", () => {
      move = { x: 0, y: 0 };
    });

    function gameLoop() {
      ctx.clearRect(0, 0, canvas.width, canvas.height);
      player.x += move.x * 5;
      player.y += move.y * 5;
      ctx.fillStyle = "lime";
      ctx.fillRect(player.x - 10, player.y - 10, 20, 20);
      requestAnimationFrame(gameLoop);
    }

    gameLoop();
  </script>
</body>
</html>
<!DOCTYPE html>
<html>
<head>
  <title>FPS Mobile Web Game</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body, html {
      margin: 0;
      padding: 0;
      overflow: hidden;
      touch-action: none;
    }
    canvas {
      display: block;
      width: 100vw;
      height: 100vh;
      background: #333;
    }
    #joystick {
      position: absolute;
      bottom: 20px;
      left: 20px;
      width: 100px;
      height: 100px;
      background: rgba(255,255,255,0.1);
      border-radius: 50%;
      touch-action: none;
    }
  </style>
</head>
<body>
  <canvas id="gameCanvas"></canvas>
  <div id="joystick"></div>

  <script>
    const canvas = document.getElementById("gameCanvas");
    const ctx = canvas.getContext("2d");
    canvas.width = window.innerWidth;
    canvas.height = window.innerHeight;

    let player = {
      x: canvas.width / 2,
      y: canvas.height / 2,
      angle: 0
    };

    let joystick = document.getElementById("joystick");
    let joyCenter = { x: 70, y: window.innerHeight - 70 };
    let move = { x: 0, y: 0 };

    joystick.addEventListener("touchmove", (e) => {
      let touch = e.touches[0];
      let dx = touch.clientX - joyCenter.x;
      let dy = touch.clientY - joyCenter.y;
      move.x = dx / 50;
      move.y = dy / 50;
      e.preventDefault();
    });

    joystick.addEventListener("touchend", () => {
      move = { x: 0, y: 0 };
    });

    function gameLoop() {
      ctx.clearRect(0, 0, canvas.width, canvas.height);
      player.x += move.x * 5;
      player.y += move.y * 5;
      ctx.fillStyle = "lime";
      ctx.fillRect(player.x - 10, player.y - 10, 20, 20);
      requestAnimationFrame(gameLoop);
    }

    gameLoop();
  </script>
</body>
</html>
