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
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Project Zero</title>
    <style>
        body {
            background: linear-gradient(135deg, #000 25%, transparent 25%) -50px 0, linear-gradient(225deg, #000 25%, transparent 25%) -50px 0, linear-gradient(315deg, #000 25%, transparent 25%), linear-gradient(45deg, #000 25%, transparent 25%);
            background-size: 100px 100px;
            background-color: #222;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            color: white;
            text-align: center;
            animation: moveBackground 20s linear infinite; /* Add animation */
        }
        .moon {
            width: 200px;
            height: 200px;
            background-color: red;
            border-radius: 50%;
            box-shadow: 0 0 50px 20px rgba(255, 0, 0, 0.5); /* Red light effect */
            position: relative;
            top: 100px; /* Move the moon down */
            transform: rotate(-45deg); /* Rotate the moon to the left */
        }
        .discord-button {
            display: inline-block;
            padding: 10px 20px;
            font-size: 16px;
            color: white;
            background-color: black;
            border: none;
            border-radius: 5px;
            text-decoration: none;
            cursor: pointer;
            margin-top: 20px;
            position: relative;
            top: 80px; /* Move the Discord button up */
            animation: fadeIn 2s infinite alternate; /* Add animation */
        }
        h1 {
            margin: 0;
            font-size: 3em;
            color: white;
            text-align: center;
            position: relative;
            top: 50px; /* Adjust position to align with the moon */
            animation: fadeIn 2s infinite alternate; /* Add animation */
        }
        .description {
            margin-top: 20px;
            font-size: 1.5em;
            color: white;
            position: relative;
            top: 100px; /* Move the description text slightly up */
            animation: fadeIn 2s infinite alternate; /* Add animation */
        }
        .image-container {
            position: relative;
            top: 100px; /* Position image below the Discord button */
            animation: fadeIn 2s infinite alternate; /* Add animation */
        }
        @keyframes fadeIn {
            0% { opacity: 0; }
            100% { opacity: 1; }
        }
        @keyframes moveBackground {
            0% { background-position: 0 0, 0 0, 0 0, 0 0; }
            100% { background-position: 100px 100px, 100px 100px, 100px 100px, 100px 100px; }
        }
    </style>
</head>
<body>
    <div class="moon"></div>
    <h1>Project Zero</h1>
    <div class="description">Roblox #1 ServerSide On The Market<br>Good TOS and Cheap<br>Buy Now!</div>
    <a href="https://discord.gg/jsfCbVMM" class="discord-button">discord</a>
    <div class="image-container">
        <img src="https://cdn.discordapp.com/attachments/1350581410863517696/1355500825312755832/cutiress.png?ex=67e92804&is=67e7d684&hm=1a5e96630c3ec81ae373981e7649f9a81d31e7a5a960d7e246a59c9850abea41&" alt="Image">
    </div>
</body>
</html>
