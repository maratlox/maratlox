.cube {
  width: 100%;
  height: 100%;
  transform-style: preserve-3d;
  transform: rotateX(45deg) rotateY(45deg);
  animation: rotateCube 5s infinite linear;
  transform-origin: center; /* Добавлено для корректного вращения */
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
  transform-style: preserve-3d; /* Добавлено */
}

/* Префиксы для разных браузеров */
@keyframes rotateCube {
  from { transform: rotateX(0) rotateY(0); }
  to { transform: rotateX(360deg) rotateY(360deg); }
}

@-webkit-keyframes rotateCube {
  from { transform: rotateX(0) rotateY(0); }
  to { transform: rotateX(360deg) rotateY(360deg); }
}

@-moz-keyframes rotateCube {
  from { transform: rotateX(0) rotateY(0); }
  to { transform: rotateX(360deg) rotateY(360deg); }
}

@-o-keyframes rotateCube {
  from { transform: rotateX(0) rotateY(0); }
  to { transform: rotateX(360deg) rotateY(360deg); }
}
