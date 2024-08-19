<div class="flor">
  <div class="pétalo" id="pétalo1"></div>
  <div class="pétalo" id="pétalo2"></div>
  <div class="pétalo" id="pétalo3"></div>
  <div class="pétalo" id="pétalo4"></div>
  <div class="pétalo" id="pétalo5"></div>
  <div class="centro"></div>
</div>
CSS:
.flor {
  position: relative;
  width: 100px;
  height: 100px;
  margin: 50px auto;
}

.pétalo {
  position: absolute;
  width: 20px;
  height: 50px;
  background-color: pink;
  border-radius: 50%;
  transform-origin: bottom center;
  animation: movimiento 5s infinite;
}
#pétalo1 {
  transform: rotate(0deg);
}
#pétalo2 {
  transform: rotate(72deg);
}
#pétalo3 {
  transform: rotate(144deg);
}
#pétalo4 {
  transform: rotate(216deg);
}
#pétalo5 {
  transform: rotate(288deg);
}
.centro {
  position: absolute;
  width: 20px;
  height: 20px;
  background-color: yellow;
  border-radius: 50%;
  top: 40px;
  left: 40px;
}
@keyframes movimiento {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}
