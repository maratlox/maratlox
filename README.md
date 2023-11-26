<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>marat lox</title>
    <style>
        .cube-container {
            perspective: 800px;
            width: 200px;
            height: 200px;
            margin: 100px auto;
        }

        .cube {
            width: 100%;
            height: 100%;
            transform-style: preserve-3d;
            animation: rotateCube 5s infinite linear;
        }

        .face {
            position: absolute;
            width: 200px;
            height: 200px;
            background-color: #3498db;
            line-height: 200px;
            text-align: center;
            font-size: 24px;
            color: #fff;
        }

        .face:nth-child(1) { transform: rotateY(0deg) translateZ(10px); }
        .face:nth-child(2) { transform: rotateY(90deg) translateZ(10px); }
        .face:nth-child(3) { transform: rotateY(180deg) translateZ(10px); }
        .face:nth-child(4) { transform: rotateY(-90deg) translateZ(10px); }
        .face:nth-child(5) { transform: rotateX(90deg) translateZ(10px); }
        .face:nth-child(6) { transform: rotateX(-90deg) translateZ(10px); }

        @keyframes rotateCube {
            from { transform: rotateY(0deg); }
            to { transform: rotateY(360deg); }
        }
    </style>
</head>
<body>
    <div class="cube-container">
        <div class="cube">
            <div class="face">Марат лох!!!</div>
            <div class="face">Марат лох!!!</div>
            <div class="face">Марат лох!!!</div>
            <div class="face">Марат лох!!!</div>
            <div class="face">Марат лох!!!</div>
            <div class="face">Марат лох!!!</div>
        </div>
    </div>
</body>
</html>
