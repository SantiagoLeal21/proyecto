<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Simulador de Elasticidad - Cuerda en Movimiento</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

  body {
    font-family: 'Roboto', sans-serif;
    background: linear-gradient(135deg, #667eea, #764ba2);
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
    border-bottom: 2px solid#4f2b97;
    padding-bottom: 0.5rem;
    margin-bottom: 1rem;
    color:hsl(0, 0.00%, 100.00%);
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
    box-shadow: inset 0 0 30px #7f87f4;
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
    color: #c3c3ff;
  }
  form#controls input[type="range"], form#controls input[type="number"] {
    margin-top: 0.4rem;
    -webkit-appearance: none;
    background: #4949a1;
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
    background: #9f7aea;
    cursor: pointer;
    border-radius: 50%;
    border: none;
    box-shadow: 0 0 10px #b99fff;
    transition: 0.25s ease;
  }
  form#controls input[type="range"]:hover::-webkit-slider-thumb {
    background: #d6bcfa;
    box-shadow: 0 0 15px #daaaff;
  }
  
  #calculations {
    background: rgba(0,0,0,0.3);
    border-radius: 12px;
    width: 100%;
    max-width: 600px;
    padding: 1rem 1.5rem;
    color: #bbd7ff;
    font-size: 1rem;
    font-weight: 500;
    box-shadow: inset 0 0 15px #5978ff;
  }
  #calculations h3 {
    margin-top: 0;
    color: #a596f9;
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
    background-color: #9f7aea96;
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
  <h1>Simulador de Elasticidad: Cuerda en Movimiento</h1>
</header>
<main>
  <section id="intro" tabindex="0">
    <h2>Introducción</h2>
    <p>Este simulador muestra el comportamiento de una cuerda elástica en movimiento, visualizando una onda que se desplaza a lo largo de la cuerda. Se basa en principios físicos de elasticidad y ondas mecánicas para calcular y representar el movimiento.</p>
    <p>Una cuerda estirada puede transmitir ondas cuando se deforma, y la velocidad y forma de estas ondas dependen de sus propiedades físicas.</p>
    <h2>Fórmulas Utilizadas</h2>
    <ul>
      <li><strong>Ley de Hooke</strong> para elasticidad: <code>F = -k x</code><br>
      Donde <em>F</em> es la fuerza restauradora, <em>k</em> la constante de elasticidad, y <em>x</em> la deformación.</li>
      <li><strong>Velocidad de la onda en la cuerda:</strong><br>
      <code>v = √(T / μ)</code><br>
      Donde <em>v</em> es la velocidad de la onda, <em>T</em> la tensión en la cuerda, y <em>μ</em> es la densidad lineal (masa por unidad de longitud) de la cuerda.</li>
      <li><strong>Relación entre frecuencia, longitud de onda y velocidad:</strong><br>
      <code>v = f × λ</code><br>
      Donde <em>f</em> es la frecuencia y <em>λ</em> la longitud de onda.</li>
    </ul>
    <p>Modificando los parámetros de la cuerda, puede observar visualmente cómo cambia la onda y cómo se ajustan los cálculos físicos asociados.</p>
  </section>
  <section id="simulator" aria-label="Simulador de movimiento de cuerda elástica">
    <div id="canvas-container" aria-live="polite">
      <canvas id="ropeCanvas" width="800" height="300" role="img" aria-label="Animación de una cuerda elástica en movimiento"></canvas>
    </div>
    <form id="controls" aria-describedby="controls-desc">
      <div>
        <label for="tensionRange">Tensión (T) en Newtons: <output id="tensionOutput">50</output></label>
        <input type="range" min="10" max="200" step="1" value="50" id="tensionRange" name="tension" />
      </div>
      <div>
        <label for="massRange">Masa lineal (μ) kg/m: <output id="massOutput">0.02</output></label>
        <input type="range" min="0.001" max="0.1" step="0.001" value="0.02" id="massRange" name="mass" />
      </div>
      <div>
        <label for="freqRange">Frecuencia (f) Hz: <output id="freqOutput">2</output></label>
        <input type="range" min="0.1" max="10" step="0.1" value="2" id="freqRange" name="frequency" />
      </div>
      <div>
        <label for="amplitudeRange">Amplitud (A) en metros: <output id="ampOutput">0.03</output></label>
        <input type="range" min="0.005" max="0.1" step="0.005" value="0.03" id="amplitudeRange" name="amplitude" />
      </div>
    </form>

    <section id="calculations" aria-live="polite" aria-atomic="true">
      <h3>Cálculos en tiempo real</h3>
      <p><strong>Velocidad de onda (v): </strong><span id="velocityCalc">-</span> m/s</p>
      <p><strong>Longitud de onda (λ): </strong><span id="wavelengthCalc">-</span> m</p>
      <p><strong>Constante de elasticidad (k) estimada: </strong><span id="elasticConstCalc">-</span> N/m</p>
    </section>
  </section>
</main>

<script>
(() => {
  const canvas = document.getElementById('ropeCanvas');
  const ctx = canvas.getContext('2d');

  // Controls references
  const tensionRange = document.getElementById('tensionRange');
  const massRange = document.getElementById('massRange');
  const freqRange = document.getElementById('freqRange');
  const amplitudeRange = document.getElementById('amplitudeRange');

  // Outputs for values
  const tensionOutput = document.getElementById('tensionOutput');
  const massOutput = document.getElementById('massOutput');
  const freqOutput = document.getElementById('freqOutput');
  const ampOutput = document.getElementById('ampOutput');

  // Calculation display
  const velocityCalc = document.getElementById('velocityCalc');
  const wavelengthCalc = document.getElementById('wavelengthCalc');
  const elasticConstCalc = document.getElementById('elasticConstCalc');

  // Physical constants
  const length = 1.5; // meters, length of the rope represented visually
  const ropeSegments = 100; // segments to draw the rope wave
  const ropeBaselineY = canvas.height / 2;

  let tension = parseFloat(tensionRange.value);
  let massLinear = parseFloat(massRange.value);
  let frequency = parseFloat(freqRange.value);
  let amplitude = parseFloat(amplitudeRange.value);

  // Wave velocity v = sqrt(T/μ)
  function calculateVelocity(T, mu) {
    return Math.sqrt(T / mu);
  }

  // Wavelength λ = v / f
  function calculateWavelength(v, f) {
    if(f === 0) return 0;
    return v / f;
  }
  
  // Estimate elastic constant k from tension and elongation x (assumed from amplitude here)
  // Using Hooke's law: F = kx => k = F/x, here F = T (tension), x = amplitude
  function calculateElasticConstant(T, A) {
    if(A === 0) return 0;
    return T / A;
  }

  // Draw the rope wave on the canvas
  function drawRope(time) {
    ctx.clearRect(0, 0, canvas.width, canvas.height);

    ctx.lineWidth = 3;
    ctx.strokeStyle = '#9f7aea';
    ctx.shadowColor = '#bb99ff';
    ctx.shadowBlur = 10;
    ctx.beginPath();

    for (let i = 0; i <= ropeSegments; i++) {
      const x = (i / ropeSegments) * canvas.width;
      // Calculate the corresponding position in meters along the rope
      const posMeter = (i / ropeSegments) * length;

      // Wave function: y = A * sin(2π * (x/λ - f * t))
      // time in seconds, convert ms to s
      const v = calculateVelocity(tension, massLinear);
      const wavelength = calculateWavelength(v, frequency);
      const omega = 2 * Math.PI * frequency;
      const k = 2 * Math.PI / wavelength;

      // Wave displacement in meters scaled to pixels (scale factor)
      const scaleY = canvas.height * 0.15; // scaling amplitude visually
      const displacement = amplitude * Math.sin(k * posMeter - omega * time) * scaleY;

      const y = ropeBaselineY + displacement;

      if (i === 0) ctx.moveTo(x, y);
      else ctx.lineTo(x, y);
    }
    ctx.stroke();

    // Draw endpoints
    ctx.shadowBlur = 0;
    ctx.fillStyle = '#d6bcfa';
    ctx.beginPath();
    ctx.arc(0, ropeBaselineY, 6, 0, 2 * Math.PI, false);
    ctx.fill();
    ctx.beginPath();
    ctx.arc(canvas.width, ropeBaselineY, 6, 0, 2 * Math.PI, false);
    ctx.fill();
  }

  function updateCalculations() {
    const v = calculateVelocity(tension, massLinear);
    const wavelength = calculateWavelength(v, frequency);
    const k = calculateElasticConstant(tension, amplitude);

    velocityCalc.textContent = v.toFixed(2);
    wavelengthCalc.textContent = wavelength.toFixed(3);
    elasticConstCalc.textContent = k.toFixed(1);
  }

  function updateParameters() {
    tension = parseFloat(tensionRange.value);
    massLinear = parseFloat(massRange.value);
    frequency = parseFloat(freqRange.value);
    amplitude = parseFloat(amplitudeRange.value);

    tensionOutput.value = tension;
    massOutput.value = massLinear;
    freqOutput.value = frequency;
    ampOutput.value = amplitude;

    tensionOutput.textContent = tension;
    massOutput.textContent = massLinear.toFixed(3);
    freqOutput.textContent = frequency.toFixed(1);
    ampOutput.textContent = amplitude.toFixed(3);

    updateCalculations();
  }

  // Attach handlers for inputs
  tensionRange.addEventListener('input', updateParameters);
  massRange.addEventListener('input', updateParameters);
  freqRange.addEventListener('input', updateParameters);
  amplitudeRange.addEventListener('input', updateParameters);

  // Animation loop
  let startTime = null;
  function animate(timestamp) {
    if (!startTime) startTime = timestamp;
    const elapsed = (timestamp - startTime) / 1000; // seconds

    drawRope(elapsed);
    requestAnimationFrame(animate);
  }

  // Initialize
  updateParameters();
  requestAnimationFrame(animate);
})();
</script>
</body>
</html>

