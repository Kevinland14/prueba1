<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Registro</title>
<style>
        body {
            background: linear-gradient(#ADD8E6);
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 50px;
        }
        h1 {
            color: #0000FF;
            margin-bottom: 70px;
        }
        p {
           text-align: left;
            color: #000000;

           }
    </style>

  <script>
    function guardarUsuario() {
      const usuario = document.getElementById('usuario').value;
      const contrasena = document.getElementById('contrasena').value;

      // Guardamos los datos en localStorage (para demo)
      localStorage.setItem('usuario', usuario);
      localStorage.setItem('contrasena', contrasena);

      alert('Usuario registrado correctamente.');
      window.location.href = "Login.html";  // Redirige al inicio de sesión
    }
  </script>
</head>
<body style="margin: 0; height: 80vh; display: flex; justify-content: center; align-items: center; background-color: #3e5f8a;">

  <div style="width: 300px; border: 2px solid black; padding: 30px; background-color: 	#0000FF; text-align: center;">

  <h2>Registrar Nueva Cuenta</h2>
  <form onsubmit="event.preventDefault(); guardarUsuario();">
    <label for="usuario">Usuario:</label>
    <input type="text" id="usuario" name="usuario" required><br><br>

    <label for="contrasena">Contraseña:</label>
    <input type="password" id="contrasena" name="contrasena" required><br><br>

    <button type="submit">Registrarse</button>
  </form>
</body>
</html>
