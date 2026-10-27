<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=800&size=42&pause=2000&color=00FFE0&center=true&vCenter=true&width=700&height=80&lines=LEONARDO+%F0%9F%A4%96;WhatsApp+Bot+Creator;Bots+%7C+Automation+%7C+2026" alt="LEONARDO"/>
</div><div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=14&pause=2000&color=ffffff&center=true&vCenter=true&width=700&lines=Creador+de+bots+de+WhatsApp+%E2%80%A2+Baileys+%E2%80%A2+Node.js+%E2%80%A2+Multi-Device" alt="subtitle"/>
</div><br/><div align="center">
  <img src="https://img.shields.io/badge/-Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white"/>
  <img src="https://img.shields.io/badge/-WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white"/>
  <img src="https://img.shields.io/badge/-Baileys-00FFE0?style=for-the-badge&logo=whatsapp&logoColor=white"/>
  <img src="https://img.shields.io/badge/-Git-F05032?style=for-the-badge&logo=git&logoColor=white"/>
</div><br/><div align="center">
  <img src="https://img.shields.io/badge/creador-LEONARDO-00ffe0?style=flat-square"/>
  <img src="https://img.shields.io/badge/año-2026-00ff88?style=flat-square"/>
  <img src="https://img.shields.io/badge/plataforma-WhatsApp-black?style=flat-square"/>
  <img src="https://img.shields.io/badge/estado-activo-00ff88?style=flat-square"/>
</div>

---

👨‍💻 LEONARDO

<div align="center">🤖 Creador y desarrollador de bots de WhatsApp

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


«⚡ Automatización • 🤖 Inteligencia • 📱 WhatsApp • 🚀 Desarrollo»

</div>

---

🤖 Mis Bots

🌸 Hinata-Bot

<div align="center"><img src="https://img.shields.io/badge/HINATA--BOT-ff69b4?style=for-the-badge&logo=whatsapp&logoColor=white"/></div>Bot de WhatsApp desarrollado por LEONARDO, diseñado para ofrecer diferentes herramientas, comandos y funciones automatizadas dentro de WhatsApp.

Tecnologías principales:

- 🟢 Node.js
- 📱 WhatsApp Multi-Device
- ⚡ Baileys
- 🛠️ JavaScript

---

👹 Alastor-WA-Bot

<div align="center"><img src="https://img.shields.io/badge/ALASTOR--WA--BOT-8A2BE2?style=for-the-badge&logo=whatsapp&logoColor=white"/></div>Bot de WhatsApp creado por LEONARDO, con una arquitectura orientada a automatización, comandos personalizados y herramientas multimedia.

Características:

- 🤖 Sistema de comandos
- 📥 Descargas y herramientas multimedia
- 🎵 Conversión de audio
- 🖼️ Procesamiento de imágenes
- 🎬 Procesamiento de vídeo
- 👥 Funciones para grupos
- ⚙️ Automatización de tareas
- 📱 Compatible con WhatsApp Multi-Device

---

🧰 Tecnologías

Tecnología| Uso
🟢 Node.js| Motor principal
⚡ Baileys| Conexión con WhatsApp
🟨 JavaScript| Desarrollo del bot
🎬 FFmpeg| Procesamiento multimedia
🐙 Git| Control de versiones
📱 WhatsApp| Plataforma principal

---

📊 Proyectos

<div align="center">🤖 Proyecto| 👨‍💻 Creador| 📅 Año
🌸 Hinata-Bot| LEONARDO| 2026
👹 Alastor-WA-Bot| LEONARDO| 2026

</div>

---

💬 Comunidad

<div align="center"><a href="#">
  <img src="https://img.shields.io/badge/Hinata--Bot-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="Hinata-Bot"/>
</a> 

<a href="#">
  <img src="https://img.shields.io/badge/Alastor--WA--Bot-8A2BE2?style=for-the-badge&logo=whatsapp&logoColor=white" alt="Alastor-WA-Bot"/>
</a></div><br/><div align="center">⚡ LEONARDO • BOT DEVELOPER • 2026 ⚡

<img src="https://img.shields.io/badge/WhatsApp-Bot%20Developer-25D366?style=for-the-badge&logo=whatsapp&logoColor=white"/></div>

---

⭐ Sobre el proyecto


Hinata-Bot y Alastor-WA-Bot representan dos proyectos independientes enfocados en ofrecer diferentes herramientas y sistemas automatizados para usuarios y comunidades de WhatsApp.

---

<div align="center">Made with ⚡ by LEONARDO

"2026 • WhatsApp Bot Developer"

</div>