# onex.js
🎧 onex.js
onex.js es una librería ultra simple para agregar música o sonidos a tu página web con una sola línea de código.
Sin configuraciones raras, sin frameworks, solo puro flow sonoro en segundos. 🔊

🚀 ¿Cómo se usa?
1. Incluye la librería en tu HTML
Desde tu archivo local:
html
Copiar
Editar
<script src="onex.js"></script>
O desde CDN (cuando subas el repo):
html
Copiar
Editar
<script src="https://cdn.jsdelivr.net/gh/nubladoxd/onex.js@latest/onex.min.js"></script>
2. Inicia la música con una línea:
html
Copiar
Editar
<script>
  Onex.init("cancion.mp3", { loop: true, volume: 0.7 });
</script>
Eso es todo. ¡Ya tienes música! 😎

✅ Opciones de Onex.init
Parámetro	Tipo	Descripción	Default
src	String	Ruta al archivo .mp3	—
loop	Boolean	Si debe repetirse	true
volume	Número	Volumen inicial (0.0 a 1.0)	1.0

🕹️ Controles disponibles
js
Copiar
Editar
Onex.play();       // Reproduce el sonido
Onex.pause();      // Pausa el sonido
Onex.stop();       // Detiene y reinicia
Onex.toggle();     // Alterna entre play/pause
Onex.setVolume(0.5); // Cambia el volumen
💻 Ejemplo completo
html
Copiar
Editar
<!DOCTYPE html>
<html>
<head>
  <title>Demo onex.js</title>
</head>
<body>
  <h1>Mi web con música 🔊</h1>
  <button onclick="Onex.play()">▶️ Play</button>
  <button onclick="Onex.pause()">⏸️ Pause</button>
  <button onclick="Onex.stop()">⏹️ Stop</button>

  <script src="onex.js"></script>
  <script>
    Onex.init("cancion.mp3", { loop: true, volume: 0.7 });
  </script>
</body>
</html>
🧠 ¿Por qué usar onex.js?
Simple y directo

Sin dependencias

Perfecto para páginas personales, portfolios, juegos web, etc.

Funciona en todos los navegadores modernos

🗂 Archivos incluidos
onex.js – Código fuente original

onex.min.js – Versión lista para producción/CDN

index.html – Demo básica

demo.mp3 – Audio dummy de prueba (puedes reemplazarlo)

