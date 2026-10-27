<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Leo ♥</title>
<style>
  html, body { height: 100%; margin: 0; background: #0d1117; }
  body { display: flex; align-items: center; justify-content: center; overflow: hidden; }

  .wrap {
    position: relative;
    width: min(92vw, 640px);
    aspect-ratio: 640 / 600;
    animation: latido 1.4s ease-in-out infinite;
  }
  @keyframes latido {
    0%, 100% { transform: scale(1); }
    15%      { transform: scale(1.07); }
    30%      { transform: scale(1); }
    45%      { transform: scale(1.05); }
    60%      { transform: scale(1); }
  }

  #corazon { position: absolute; inset: 0; }
  #corazon span {
    position: absolute;
    font: bold 14px/1 'Courier New', monospace;
    transform: translate(-50%, -50%);
    animation: parpadeo var(--d) ease-in-out var(--b) infinite;
  }
  @keyframes parpadeo {
    0%, 100% { opacity: 1; }
    50%      { opacity: .08; }
  }

  .leo {
    position: absolute;
    left: 50%; top: 46%;
    transform: translate(-50%, -50%);
    font: bold clamp(48px, 15vw, 96px) 'Courier New', monospace;
    color: #fff;
    text-shadow: 0 0 14px #00ffe0, 0 0 30px #ff4d8d;
    animation: brillo 1.4s ease-in-out infinite;
  }
  @keyframes brillo {
    0%, 100% { opacity: .85; }
    15%      { opacity: 1; }
  }
</style>
</head>
<body>
  <div class="wrap">
    <div id="corazon"></div>
    <div class="leo">Leo</div>
  </div>

<script>
  const cont = document.getElementById('corazon');
  const colores = ['#00ffe0', '#00ffe0', '#00ff88', '#ff4d8d', '#ff69b4'];
  const cols = 40, filas = 36;
  const celdas = [];

  for (let r = 0; r < filas; r++) {
    for (let c = 0; c < cols; c++) {
      // Coordenadas normalizadas para la ecuación del corazón
      const x = ((c - cols / 2 + 0.5) / (cols / 2)) * 1.45;
      const y = -((r - filas / 2 + 0.5) / (filas / 2)) * 1.45 + 0.1;
      if (Math.pow(x * x + y * y - 1, 3) - x * x * Math.pow(y, 3) > 0) continue;

      const px = (c + 0.5) / cols * 100;
      const py = (r + 0.5) / filas * 100;

      // Hueco en el centro para que se lea "Leo"
      if (Math.abs(px - 50) < 15 && Math.abs(py - 44) < 7) continue;

      const s = document.createElement('span');
      s.textContent = Math.random() < 0.5 ? '0' : '1';
      s.style.left = px + '%';
      s.style.top = py + '%';
      s.style.color = colores[Math.floor(Math.random() * colores.length)];
      s.style.setProperty('--d', (0.8 + Math.random() * 1.8).toFixed(2) + 's');
      s.style.setProperty('--b', (Math.random() * 2).toFixed(2) + 's');
      cont.appendChild(s);
      celdas.push(s);
    }
  }

  // Cambia aleatoriamente unos por ceros
  setInterval(() => {
    for (let i = 0; i < 25; i++) {
      const s = celdas[Math.floor(Math.random() * celdas.length)];
      s.textContent = s.textContent === '0' ? '1' : '0';
    }
  }, 120);
</script>
</body>
</html>
