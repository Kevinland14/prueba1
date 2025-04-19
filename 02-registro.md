<html lang="es">
<head>
  <meta charset="UTF-8">
</head>
<body style="margin: 0; height: 80vh; display: flex; justify-content: center; align-items: center; background-color: #3e5f8a;">

  <div style="width: 300px; border: 2px solid black; padding: 30px; background-color: 	#0000FF; text-align: center;">

  <h2>Registrar Nueva Cuenta</h2>
  <form onsubmit="event.preventDefault(); guardarUsuario();">
    <label for="usuario">Usuario:</label>
    <input type="text" id="usuario" name="usuario" required><br><br>
    
  </form>
</body>
</html>
