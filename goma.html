<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Simulador de Elasticidad: Goma en Movimiento Realista</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

  body {
    font-family: 'Roboto', sans-serif;
    background: linear-gradient(135deg, #4b4372, #6f4f8f);
    color: #ececec;
    margin: 0;
    padding: 0;
    display: flex;
    flex-direction: column;
    min-height: 100vh;
  }

  header {
    padding: 1.6rem 2rem;
    background: rgba(0,0,0,0.3);
    text-align: center;
    box-shadow: 0 2px 7px rgba(0,0,0,0.4);
  }
  header h1 {
    margin: 0;
    font-weight: 700;
    font-size: 2.6rem;
    letter-spacing: 1.6px;
  }

  main {
    flex: 1;
    display: flex;
    flex-wrap: wrap;
    gap: 2rem;
    max-width: 1100px;
    margin: 0 auto;
    padding: 2rem 1rem;
  }

  section#intro {
    flex: 1 1 370px;
    background: rgba(255,255,255,0.1);
    border-radius: 14px;
    padding: 1.8rem 2.2rem;
    box-shadow: 0 7px 15px rgba(0,0,0,0.5);
    max-height: 650px;
    overflow-y: auto;
  }
  section#intro h2 {
    border-bottom: 3px solid #9f7aea;
    padding-bottom: 0.5rem;
    margin-bottom: 1rem;
    color: #bb99ff;
  }
  section#intro p, section#intro ul {
    font-size: 1rem;
    line-height: 1.6;
  }
  section#intro ul {
    margin-left: 1.4rem;
  }
  section#intro code {
    background: rgba(255, 255, 255, 0.2);
    padding: 3px 7px;
    font-family: monospace;
    border-radius: 4px;
  }

  section#simulator {
    flex: 2 1 650px;
    background: rgba(255,255,255,0.1);
    border-radius: 14px;
    padding: 1.8rem 2.2rem;
    box-shadow: 0 7px 15px rgba(0,0,0,0.5);

    display: flex;
    flex-direction: column;
    align-items: center;
  }

  #canvas-container {
    width: 100%;
    height: 300px;
    background: #2a2363;
    border-radius: 14px;
    box-shadow: inset 0 0 50px #705da9, inset 0 0 30px #997ae1;
    margin-bottom: 1.25rem;
    position: relative;
  }

  canvas {
    display: block;
    width: 100%;
    height: 100%;
    border-radius: 14px;
  }

  form#controls {
    width: 100%;
    max-width: 640px;
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 1.15rem;
    margin-bottom: 1.5rem;
  }
  form#controls label {
    display: flex;
    flex-direction: column;
    font-weight: 600;
    font-size: 0.95rem;
    color: #cdbaff;
  }
  form#controls input[type="range"] {
    margin-top: 0.35rem;
    -webkit-appearance: none;
    background: #6c5da5;
    height: 6px;
    border-radius: 6px;
    outline: none;
    cursor: pointer;
    box-shadow: inset 0 0 5px #876fd4;
  }
  form#controls input[type="range"]::-webkit-slider-thumb {
    -webkit-appearance: none;
    appearance: none;
    width: 26px;
    height: 26px;
    background: #bba0ff;
    border-radius: 50%;
    cursor: pointer;
    box-shadow: 0 0 18px #cab8ff;
    transition: 0.3s ease;
    border: none;
  }
  form#controls input[type="range"]:hover::-webkit-slider-thumb {
    background: #d3c4ff;
    box-shadow: 0 0 28px #d9cfff;
  }

  #calculations {
    background: rgba(0,0,0,0.3);
    border-radius: 14px;
    width: 100%;
    max-width: 640px;
    padding: 1.2rem 1.8rem;
    color: #d5cfff;
    font-size: 1rem;
    font-weight: 500;
    box-shadow: inset 0 0 25px #9a7aea;
  }
  #calculations h3 {
    margin-top: 0;
    color: #b7a9f7;
  }

  footer {
    text-align: center;
    padding: 1.15rem;
    font-size: 0.9rem;
    color: #a9a0da;
    background: rgba(0,0,0,0.25);
    user-select: none;
  }

  /* Scrollbar style for intro */
  section#intro::-webkit-scrollbar {
    width: 7px;
  }
  section#intro::-webkit-scrollbar-thumb {
    background-color: #9f7aea88;
    border-radius: 5px;
  }
  .volver-btn {
  position: absolute;
  top: 20px;
  left: 20px;
  background-color: #6f4f8f;
  color: #ffffff;
  text-decoration: none;
  font-weight: 600;
  padding: 0.5rem 1rem;
  border-radius: 8px;
  box-shadow: 0 3px 6px rgba(0,0,0,0.4);
  transition: background-color 0.3s ease;
  font-size: 1rem;
}
.volver-btn:hover {
  background-color: #8b6cb3;
}
header {
  position: relative; /* Necesario para posicionar el botón */
}


</style>
</head>
<body>
<header>
  <a href="index.html" class="volver-btn">← Volver</a>

  <h1>Simulador de Elasticidad: Goma en Movimiento </h1>
</header>

<main>
  <section id="intro" tabindex="0">
    <h2>Introducción</h2>
    <p>Este simulador presenta una goma elástica en movimiento con una representación visual más realista, mostrando cómo se estira y se contrae generando oscilaciones causadas por la elasticidad del material y la masa aplicada.</p>
    <p>Aunque la goma responde a principios similares a la Ley de Hooke, su comportamiento visual aquí imita mejor la deformación y la textura de una banda elástica real.</p>
    <h2>Fórmulas usadas</h2>
    <ul>
      <li><strong>Ley de Hooke:</strong><br>
        <code>F = -k × x</code><br>
        Donde <em>F</em> es la fuerza restauradora, <em>k</em> es la constante elástica efectiva, y <em>x</em> el estiramiento o compresión.</li>
      <li><strong>Energía potencial:</strong><br>
        <code>U = 1/2 × k × x²</code><br>
        La energía almacenada debido a la deformación.</li>
      <li><strong>Periodo:</strong><br>
        <code>T = 2π × √(m / k)</code><br>
        Tiempo que tarda un ciclo de oscilación completo.</li>
      <li><strong>Frecuencia:</strong><br>
        <code>f = 1 / T</code><br>
        Número de oscilaciones por segundo.</li>
    </ul>
    <p>Modificando los parámetros puedes observar cómo la goma responde con distintas velocidades y amplitudes.</p>
  </section>

  <section id="simulator" aria-label="Simulador de goma elástica en movimiento">
    <div id="canvas-container" aria-live="polite">
      <canvas id="rubberCanvas" width="800" height="300" role="img" aria-label="Animación de una goma elástica en movimiento"></canvas>
    </div>

    <form id="controls" aria-describedby="controls-desc">
      <div>
        <label for="kRange">Constante elástica (k) N/m: <output id="kOutput">40</output></label>
        <input type="range" min="5" max="150" step="1" value="40" id="kRange" name="k"/>
      </div>
      <div>
        <label for="massRange">Masa (m) kg: <output id="massOutput">1.5</output></label>
        <input type="range" min="0.3" max="10" step="0.1" value="1.5" id="massRange" name="mass"/>
      </div>
      <div>
        <label for="amplitudeRange">Amplitud (A) metros: <output id="ampOutput">0.1</output></label>
        <input type="range" min="0.01" max="0.3" step="0.01" value="0.1" id="amplitudeRange" name="amplitude"/>
      </div>
      <div>
        <label for="dampingRange">Amortiguamiento (b) coeficiente: <output id="dampingOutput">0.04</output></label>
        <input type="range" min="0" max="0.15" step="0.005" value="0.04" id="dampingRange" name="damping"/>
      </div>
    </form>

    <section id="calculations" aria-live="polite" aria-atomic="true">
      <h3>Cálculos en tiempo real</h3>
      <p><strong>Periodo (T): </strong><span id="periodCalc">-</span> s</p>
      <p><strong>Frecuencia (f): </strong><span id="frequencyCalc">-</span> Hz</p>
      <p><strong>Fuerza máxima (F): </strong><span id="forceCalc">-</span> N</p>
      <p><strong>Energía potencial máxima (U): </strong><span id="energyCalc">-</span> J</p>
    </section>
  </section>
</main>


<script>
(() => {
  const canvas = document.getElementById('rubberCanvas');
  const ctx = canvas.getContext('2d');

  const kRange = document.getElementById('kRange');
  const massRange = document.getElementById('massRange');
  const amplitudeRange = document.getElementById('amplitudeRange');
  const dampingRange = document.getElementById('dampingRange');

  const kOutput = document.getElementById('kOutput');
  const massOutput = document.getElementById('massOutput');
  const ampOutput = document.getElementById('ampOutput');
  const dampingOutput = document.getElementById('dampingOutput');

  const periodCalc = document.getElementById('periodCalc');
  const frequencyCalc = document.getElementById('frequencyCalc');
  const forceCalc = document.getElementById('forceCalc');
  const energyCalc = document.getElementById('energyCalc');

  const rubberStartX = 130;
  const rubberEndX = canvas.width - 130;
  const rubberY = canvas.height / 2;
  const rubberHeight = 32;

  let k = parseFloat(kRange.value);
  let mass = parseFloat(massRange.value);
  let amplitude = parseFloat(amplitudeRange.value);
  let damping = parseFloat(dampingRange.value);

  // Physics functions
  function period(k, m) {
    return 2 * Math.PI * Math.sqrt(m / k);
  }
  function frequency(T) {
    return T === 0 ? 0 : 1 / T;
  }
  function fMax(k, A) {
    return k * A;
  }
  function potentialEnergy(k, A) {
    return 0.5 * k * A * A;
  }

  // Draw realistic rubber band with better shading and a subtle wave bulge
  function drawRubberBand(xOffset) {
    ctx.clearRect(0, 0, canvas.width, canvas.height);

    // Draw left fixed support circle
    ctx.fillStyle = '#9f7aea';
    ctx.shadowColor = '#bb99ff';
    ctx.shadowBlur = 18;
    ctx.beginPath();
    ctx.arc(rubberStartX - 40, rubberY, 34, 0, 2 * Math.PI);
    ctx.fill();
    ctx.shadowBlur = 0;

    // Draw right fixed support circle
    ctx.beginPath();
    ctx.arc(rubberEndX + 40, rubberY, 34, 0, 2 * Math.PI);
    ctx.fill();

    // Define band max width and centerX shifts with xOffset
    const totalLength = rubberEndX - rubberStartX;
    // Center point moves with oscillation offset horizontally
    const centerX = rubberStartX + totalLength / 2 + xOffset;

    // Rubber band colors: gradient for shiny and translucent look
    const gradient = ctx.createLinearGradient(rubberStartX, rubberY - rubberHeight, rubberEndX, rubberY + rubberHeight);
    gradient.addColorStop(0, 'rgba(158, 130, 231, 0.9)');
    gradient.addColorStop(0.3, 'rgba(140, 112, 215, 0.85)');
    gradient.addColorStop(0.5, 'rgba(180, 155, 240, 0.95)');
    gradient.addColorStop(0.7, 'rgba(140, 112, 215, 0.85)');
    gradient.addColorStop(1, 'rgba(158, 130, 231, 0.9)');

    ctx.fillStyle = gradient;
    ctx.shadowColor = 'rgba(180, 155, 240, 0.8)';
    ctx.shadowBlur = 28;
    ctx.lineJoin = 'round';

    ctx.beginPath();

    // Upper edge: create a smooth bulging curve simulating stretch with subtle sinusoidal and quadratic shape
    const bulgeHeight = rubberHeight * 0.9;
    ctx.moveTo(rubberStartX, rubberY - rubberHeight / 2);
    ctx.bezierCurveTo(
      rubberStartX + totalLength * 0.15, rubberY - bulgeHeight,
      centerX - totalLength * 0.1, rubberY - bulgeHeight * 1.15,
      centerX, rubberY - bulgeHeight * 0.6
    );
    ctx.bezierCurveTo(
      centerX + totalLength * 0.1, rubberY - bulgeHeight * 1.15,
      rubberEndX - totalLength * 0.15, rubberY - bulgeHeight,
      rubberEndX, rubberY - rubberHeight / 2
    );

    // Right side down
    ctx.lineTo(rubberEndX, rubberY + rubberHeight / 2);

    // Lower edge mirroring the upper edge for realism with smooth bulge
    ctx.bezierCurveTo(
      rubberEndX - totalLength * 0.15, rubberY + bulgeHeight,
      centerX + totalLength * 0.1, rubberY + bulgeHeight * 1.15,
      centerX, rubberY + bulgeHeight * 0.6
    );
    ctx.bezierCurveTo(
      centerX - totalLength * 0.1, rubberY + bulgeHeight * 1.15,
      rubberStartX + totalLength * 0.15, rubberY + bulgeHeight,
      rubberStartX, rubberY + rubberHeight / 2
    );

    ctx.closePath();
    ctx.fill();

    // Draw subtle inner highlight shape to simulate translucency and rounded shape
    ctx.shadowBlur = 0;
    const highlightGradient = ctx.createLinearGradient(rubberStartX, rubberY - rubberHeight / 2, rubberEndX, rubberY + rubberHeight / 2);
    highlightGradient.addColorStop(0, 'rgba(255, 255, 255, 0.2)');
    highlightGradient.addColorStop(0.5, 'rgba(255, 255, 255, 0.05)');
    highlightGradient.addColorStop(1, 'rgba(255, 255, 255, 0.2)');

    ctx.fillStyle = highlightGradient;
    ctx.beginPath();
    ctx.moveTo(rubberStartX + 10, rubberY - rubberHeight / 2.5);
    ctx.bezierCurveTo(
      rubberStartX + totalLength * 0.2, rubberY - bulgeHeight * 0.5,
      centerX - totalLength * 0.15, rubberY - bulgeHeight * 0.8,
      centerX, rubberY - bulgeHeight * 0.52
    );
    ctx.bezierCurveTo(
      centerX + totalLength * 0.15, rubberY - bulgeHeight * 0.8,
      rubberEndX - totalLength * 0.2, rubberY - bulgeHeight * 0.5,
      rubberEndX - 10, rubberY - rubberHeight / 2.5
    );
    ctx.lineTo(rubberEndX - 10, rubberY - rubberHeight / 4);
    ctx.bezierCurveTo(
      rubberEndX - totalLength * 0.2, rubberY - bulgeHeight * 0.3,
      centerX + totalLength * 0.15, rubberY - bulgeHeight * 0.3,
      centerX, rubberY - bulgeHeight * 0.2
    );
    ctx.bezierCurveTo(
      centerX - totalLength * 0.15, rubberY - bulgeHeight * 0.3,
      rubberStartX + totalLength * 0.2, rubberY - bulgeHeight * 0.3,
      rubberStartX + 10, rubberY - rubberHeight / 4
    );
    ctx.closePath();
    ctx.fill();

    // Draw label text on rubber band
    ctx.fillStyle = 'rgba(230, 220, 255, 0.85)';
    ctx.font = 'bold 22px Roboto, sans-serif';
    ctx.textAlign = 'center';
    ctx.shadowColor = 'rgba(150, 120, 250, 0.4)';
    ctx.shadowBlur = 10;
    ctx.fillText('Goma Elástica', centerX, rubberY + 6);
  }

  function updateParameters() {
    k = parseFloat(kRange.value);
    mass = parseFloat(massRange.value);
    amplitude = parseFloat(amplitudeRange.value);
    damping = parseFloat(dampingRange.value);

    kOutput.textContent = k;
    massOutput.textContent = mass.toFixed(1);
    ampOutput.textContent = amplitude.toFixed(2);
    dampingOutput.textContent = damping.toFixed(3);

    const T = period(k, mass);
    const f = frequency(T);
    const Fmax = fMax(k, amplitude);
    const Umax = potentialEnergy(k, amplitude);

    periodCalc.textContent = T.toFixed(3);
    frequencyCalc.textContent = f.toFixed(3);
    forceCalc.textContent = Fmax.toFixed(2);
    energyCalc.textContent = Umax.toFixed(3);
  }

  // Physics helpers
  function period(k, m) {
    return 2 * Math.PI * Math.sqrt(m / k);
  }
  function frequency(T) {
    return T === 0 ? 0 : 1 / T;
  }
  function fMax(k, A) {
    return k * A;
  }
  function potentialEnergy(k, A) {
    return 0.5 * k * A * A;
  }

  // Animate horizontal oscillation with exponential damping and cosine wave
  let startTime = null;
  function animate(t) {
    if (!startTime) startTime = t;
    const elapsed = (t - startTime) / 1000;

    const w0 = Math.sqrt(k / mass);
    const x = amplitude * Math.exp(-damping * elapsed) * Math.cos(w0 * elapsed);

    drawRubberBand(x * 400);
    requestAnimationFrame(animate);
  }

  // Attach event listeners
  [kRange, massRange, amplitudeRange, dampingRange].forEach(elem => {
    elem.addEventListener('input', updateParameters);
  });

  // Initialize values and start animation
  updateParameters();
  requestAnimationFrame(animate);

})();
</script>
</body>
</html>

