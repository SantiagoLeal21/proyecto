<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Simulador de Elasticidad: Resorte en Movimiento</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

  body {
    font-family: 'Roboto', sans-serif;
    background: linear-gradient(120deg, #2b5876, #4e4376);
    color: #eee;
    margin: 0;
    padding: 0;
    display: flex;
    flex-direction: column;
    min-height: 100vh;
  }
  
  header {
    padding: 1.5rem 2rem;
    background: rgba(0,0,0,0.3);
    text-align: center;
    box-shadow: 0 2px 8px rgba(0,0,0,0.3);
  }
  header h1 {
    margin: 0;
    font-weight: 700;
    font-size: 2.5rem;
    letter-spacing: 1.5px;
  }
  
  main {
    flex: 1;
    display: flex;
    flex-wrap: wrap;
    padding: 2rem;
    gap: 2rem;
    max-width: 1200px;
    margin: 0 auto;
  }
  
  section#intro {
    flex: 1 1 350px;
    background: rgba(255,255,255,0.1);
    border-radius: 12px;
    padding: 1.5rem 2rem;
    box-shadow: 0 8px 16px rgba(0,0,0,0.3);
    overflow-y: auto;
    max-height: 600px;
  }
  section#intro h2 {
    border-bottom: 2px solid #a679dd;
    padding-bottom: 0.5rem;
    margin-bottom: 1rem;
    color: #a679dd;
  }
  section#intro p {
    line-height: 1.5;
    font-size: 1rem;
  }
  section#intro code {
    background: rgba(255, 255, 255, 0.15);
    padding: 2px 6px;
    border-radius: 4px;
    font-family: monospace;
  }
  section#intro ul {
    margin-left: 1.2rem;
  }

  section#simulator {
    flex: 2 1 600px;
    background: rgba(255,255,255,0.1);
    border-radius: 12px;
    padding: 1.5rem 2rem;
    box-shadow: 0 8px 16px rgba(0,0,0,0.3);
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  
  #canvas-container {
    background: #1a202c;
    border-radius: 12px;
    width: 100%;
    height: 300px;
    box-shadow: inset 0 0 30px #9a7ade;
    margin-bottom: 1rem;
    position: relative;
  }

  canvas {
    display: block;
    width: 100%;
    height: 100%;
    border-radius: 12px;
  }

  form#controls {
    width: 100%;
    max-width: 600px;
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 1.2rem;
    margin-bottom: 1.5rem;
  }
  form#controls label {
    display: flex;
    flex-direction: column;
    font-weight: 600;
    font-size: 0.95rem;
    color: #cdbfff;
  }
  form#controls input[type="range"], form#controls input[type="number"] {
    margin-top: 0.4rem;
    -webkit-appearance: none;
    background: #654ea3;
    height: 6px;
    border-radius: 5px;
    outline: none;
    cursor: pointer;
  }
  form#controls input[type="range"]::-webkit-slider-thumb {
    -webkit-appearance: none;
    appearance: none;
    width: 24px;
    height: 24px;
    background: #b595f7;
    cursor: pointer;
    border-radius: 50%;
    border: none;
    box-shadow: 0 0 12px #d8b3ff;
    transition: 0.25s ease;
  }
  form#controls input[type="range"]:hover::-webkit-slider-thumb {
    background: #d7bfff;
    box-shadow: 0 0 18px #debbff;
  }
  
  #calculations {
    background: rgba(0,0,0,0.3);
    border-radius: 12px;
    width: 100%;
    max-width: 600px;
    padding: 1rem 1.5rem;
    color: #d1c7ff;
    font-size: 1rem;
    font-weight: 500;
    box-shadow: inset 0 0 15px #865ed4;
  }
  #calculations h3 {
    margin-top: 0;
    color: #b195ee;
  }

  footer {
    text-align: center;
    padding: 1rem;
    font-size: 0.9rem;
    color: #aaa;
    background: rgba(0,0,0,0.2);
    user-select: none;
  }

  /* Scrollbar for intro */
  section#intro::-webkit-scrollbar {
    width: 8px;
  }
  section#intro::-webkit-scrollbar-thumb {
    background-color: #a679dd99;
    border-radius: 4px;
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
  <h1>Simulador de Elasticidad: Resorte en Movimiento</h1>
</header>
<main>
  <section id="intro" tabindex="0">
    <h2>Introducción</h2>
    <p>Este simulador muestra el comportamiento de un resorte elástico en movimiento, visualizando su oscilación armónica simple. Está basado en principios físicos de elasticidad y cinemática para calcular y representar el movimiento.</p>
    <p>Un resorte se deforma y genera una fuerza restauradora proporcional a su desplazamiento, originando un movimiento oscilatorio cuando se une a una masa.</p>
    <h2>Fórmulas Utilizadas</h2>
    <ul>
      <li><strong>Ley de Hooke:</strong><br>
      <code>F = -k × x</code><br>
      Donde <em>F</em> es la fuerza restauradora, <em>k</em> la constante del resorte, y <em>x</em> el desplazamiento respecto al equilibrio.</li>
      <li><strong>Energía potencial elástica:</strong><br>
      <code>U = (1/2) × k × x²</code><br>
      Energía almacenada en el resorte deformado.</li>
      <li><strong>Periodo de oscilación:</strong><br>
      <code>T = 2π × √(m / k)</code><br>
      <em>m</em> es la masa unida al resorte, <em>k</em> la constante.</li>
      <li><strong>Frecuencia:</strong><br>
      <code>f = 1 / T</code><br>
      Frecuencia de oscilación.</li>
    </ul>
    <p>Modificando los parámetros del resorte y la masa adherida, puede observar visualmente cómo cambia el movimiento de oscilación y cómo se reflejan los cálculos.</p>
  </section>
  <section id="simulator" aria-label="Simulador de resorte elástico en movimiento">
    <div id="canvas-container" aria-live="polite">
      <canvas id="springCanvas" width="800" height="300" role="img" aria-label="Animación de un resorte elástico en movimiento"></canvas>
    </div>
    <form id="controls" aria-describedby="controls-desc">
      <div>
        <label for="kRange">Constante del resorte (k) N/m: <output id="kOutput">50</output></label>
        <input type="range" min="10" max="150" step="1" value="50" id="kRange" name="k" />
      </div>
      <div>
        <label for="massRange">Masa (m) kg: <output id="massOutput">2.0</output></label>
        <input type="range" min="0.5" max="10" step="0.1" value="2.0" id="massRange" name="mass" />
      </div>
      <div>
        <label for="amplitudeRange">Amplitud (A) en metros: <output id="ampOutput">0.1</output></label>
        <input type="range" min="0.02" max="0.3" step="0.01" value="0.1" id="amplitudeRange" name="amplitude" />
      </div>
      <div>
        <label for="dampingRange">Amortiguamiento (b) (coeficiente): <output id="dampingOutput">0.05</output></label>
        <input type="range" min="0" max="0.2" step="0.005" value="0.05" id="dampingRange" name="damping" />
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
  const canvas = document.getElementById('springCanvas');
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

  const springStartX = 80;
  const springEndX = canvas.width - 150;
  const springY = canvas.height / 2;
  const springCoils = 25;

  let k = parseFloat(kRange.value);
  let mass = parseFloat(massRange.value);
  let amplitude = parseFloat(amplitudeRange.value);
  let damping = parseFloat(dampingRange.value);

  // Oscillation properties
  // Angular frequency w0 = sqrt(k / m)
  function angularFrequency(k, m) {
    return Math.sqrt(k / m);
  }

  // Period T = 2π sqrt(m/k)
  function calcPeriod(k, m) {
    return 2 * Math.PI * Math.sqrt(m / k);
  }

  // Frequency f = 1 / T
  function calcFrequency(T) {
    if (T === 0) return 0;
    return 1 / T;
  }

  // Maximum force Fmax = k × A
  function maxForce(k, A) {
    return k * A;
  }

  // Potential energy U = 0.5 * k * A^2
  function potentialEnergy(k, A) {
    return 0.5 * k * A * A;
  }

  function drawSpring(xOffset) {
    // Draw fixed support block on left
    ctx.fillStyle = '#9a7ade';
    ctx.shadowColor = '#bc9fff';
    ctx.shadowBlur = 10;
    ctx.fillRect(springStartX - 70, springY - 40, 50, 80);

    ctx.shadowBlur = 0;

    // Draw spring as a zig-zag line oscillating horizontally
    ctx.strokeStyle = '#b39dec';
    ctx.lineWidth = 6;
    ctx.beginPath();

    let springLength = springEndX - springStartX;
    let coilSpacing = springLength / springCoils;
    let amplitudePixels = 25;

    ctx.moveTo(springStartX, springY);
    for (let i = 0; i <= springCoils; i++) {
      let x = springStartX + i * coilSpacing;
      let offsetY = ((i % 2) === 0) ? -amplitudePixels : amplitudePixels;
      ctx.lineTo(x, springY + offsetY);
    }
    ctx.lineTo(springEndX, springY);

    ctx.stroke();

    // Draw mass: a rectangle attached to spring end that oscillates horizontally
    let massX = springEndX + xOffset;
    let massY = springY - 40;
    ctx.fillStyle = '#a679dd';
    ctx.shadowColor = '#ccaaff';
    ctx.shadowBlur = 15;
    ctx.fillRect(massX, massY, 80, 80);
    ctx.shadowBlur = 0;

    // Draw mass label
    ctx.fillStyle = '#ddd';
    ctx.font = 'bold 20px Roboto, sans-serif';
    ctx.textAlign = 'center';
    ctx.fillText('Masa', massX + 40, massY + 45);
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

    // Update calculations
    const period = calcPeriod(k, mass);
    const freq = calcFrequency(period);
    const fMax = maxForce(k, amplitude);
    const uMax = potentialEnergy(k, amplitude);

    periodCalc.textContent = period.toFixed(3);
    frequencyCalc.textContent = freq.toFixed(3);
    forceCalc.textContent = fMax.toFixed(2);
    energyCalc.textContent = uMax.toFixed(3);
  }

  // Animate simple harmonic motion with damping
  // x(t) = A * e^(-bt) * cos(w*t)
  let startTime = null;

  function animate(t) {
    if (!startTime) startTime = t;
    const elapsed = (t - startTime) / 1000;

    ctx.clearRect(0, 0, canvas.width, canvas.height);

    // Angular frequency w = sqrt(k / m)
    const w0 = angularFrequency(k, mass);
    // Position with damping
    const x = amplitude * Math.exp(-damping * elapsed) * Math.cos(w0 * elapsed);

    // Convert meters displacement to pixels for mass oscillation
    const metersToPixels = 400; // scale factor chosen for good visual effect

    drawSpring(x * metersToPixels);

    requestAnimationFrame(animate);
  }

  kRange.addEventListener('input', () => {
    updateParameters();
  });
  massRange.addEventListener('input', () => {
    updateParameters();
  });
  amplitudeRange.addEventListener('input', () => {
    updateParameters();
  });
  dampingRange.addEventListener('input', () => {
    updateParameters();
  });

  // Initialize
  updateParameters();
  requestAnimationFrame(animate);
})();
</script>
</body>
</html>

