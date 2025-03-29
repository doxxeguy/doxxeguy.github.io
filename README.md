# doxxeguy.github.io
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Estrellas en GitHub Pages</title>
  <style>
    /* Estilos para el fondo de estrellas */
    body {
      margin: 0;
      height: 100vh;
      background: black;
      overflow: hidden;
    }

    .estrella {
      position: absolute;
      border-radius: 50%;
      background-color: white;
      opacity: 0.7;
      animation: parpadeo 1.5s infinite alternate;
    }

    @keyframes parpadeo {
      0% { opacity: 0.5; }
      100% { opacity: 1; }
    }

    /* Estilo para centrar el contenido */
    .contenido {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      color: white;
      font-family: 'Arial', sans-serif;
      text-align: center;
    }
  </style>
</head>
<body>

  <div class="contenido">
    <h1>Bienvenidos a mi página de estrellas</h1>
    <p>Este es un fondo de estrellas en GitHub Pages</p>
  </div>

  <script>
    // Crear estrellas en el fondo
    for (let i = 0; i < 100; i++) {
      let estrella = document.createElement('div');
      estrella.classList.add('estrella');
      
      let tamaño = Math.random() * 3 + 1; // Estrella de tamaño entre 1px y 3px
      let x = Math.random() * window.innerWidth;
      let y = Math.random() * window.innerHeight;

      estrella.style.width = `${tamaño}px`;
      estrella.style.height = `${tamaño}px`;
      estrella.style.left = `${x}px`;
      estrella.style.top = `${y}px`;

      document.body.appendChild(estrella);
    }
  </script>
</body>
</html>
