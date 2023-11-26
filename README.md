<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    .cube-container {
      perspective: 800px;
      width: 200px;
      height: 200px;
      margin: 50px auto;
    }

    .cube {
      width: 100%;
      height: 100%;
      transform-style: preserve-3d;
      transform: rotateX(45deg) rotateY(45deg);
      animation: rotateCube 5s infinite linear;
    }

    .face {
      position: absolute;
      width: 200px;
      height: 200px;
      display: flex;
      justify-content: center;
      align-items: center;
      font-size: 24px;
      font-weight: bold;
      color: white;
      background-color: #3498db;
      border: 1px solid #2980b9;
    }

    .face:nth-child(1) { transform: translateZ(100px); }
    .face:nth-child(2) { transform: rotateY(90deg) translateZ(100px); }
    .face:nth-child(3) { transform: rotateY(180deg) translateZ(100px); }
    .face:nth-child(4) { transform: rotateY(-90deg) translateZ(100px); }
    .face:nth-child(5) { transform: rotateX(90deg) translateZ(100px); }
    .face:nth-child(6) { transform: rotateX(-90deg) translateZ(100px); }

    @keyframes rotateCube {
      from { transform: rotateX(0) rotateY(0); }
      to { transform: rotateX(360deg) rotateY(360deg); }
    }
  </style>
</head>
<body>

<div class="cube-container">
  <div class="cube">
    <div class="face">Привет</div>
    <div class="face">Привет</div>
    <div class="face">Привет</div>
    <div class="face">Привет</div>
    <div class="face">Привет</div>
    <div class="face">Привет</div>
  </div>
</div>

</body>
</html>
