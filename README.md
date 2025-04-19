<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>Iniciar Sesión</title>
<style>
         body {
            background: linear-gradient(#ADD8E6);
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 50px;
        }
        h1 {
            color: blue;
            margin-bottom: 70px;
        }
        p {
           text-align: left;
            color: #000000;
           }
    </style>
  <script>
    function iniciarSesion() {
      const usuario = document.getElementById('usuario').value;
      const contrasena = document.getElementById('contrasena').value;

      // Obtener datos guardados del localStorage
      const usuarioGuardado = localStorage.getItem('usuario');
      const contrasenaGuardada = localStorage.getItem('contrasena');

      if (usuario === usuarioGuardado && contrasena === contrasenaGuardada) {
        // Redirige a la página de bienvenida si es correcto
        window.location.href = "index.html";
      } else {
        // Muestra un mensaje de error si es incorrecto
        alert('Usuario o contraseña incorrectos.');
      }
    }
  </script>
</head>
<body style="margin: 0; height: 80vh; display: flex; justify-content: center; align-items: center; background-color: #3e5f8a;">

  <div style="width: 300px; border: 2px solid black; padding: 30px; background-color: 	#0000FF; text-align: center;">
  <h2>Iniciar Sesión</h2>
  <form onsubmit="event.preventDefault(); iniciarSesion();">
    <label for="usuario">Usuario:</label>
    <input type="text" id="usuario" name="usuario" required><br><br>

    <label for="contrasena">Contraseña:</label>
    <input type="password" id="contrasena" name="contrasena" required><br><br>

    <button type="submit">Iniciar Sesión</button>
</div>
  </form>
</body>
</html>
