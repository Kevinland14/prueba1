<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Bienvenido</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background: linear-gradient(to bottom, #ADD8E6, #ffffff);
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }
        .container {
            text-align: center;
            background-color: #0000FF;
            padding: 150px;
            border-radius: 12px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        h1 {
            margin-bottom: 30px;
        }
        .btn {
            display: block;
            width: 200px;
            padding: 12px;
            margin: 10px auto;
            font-size: 28px;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }
        .login-btn {
            background-color: #4CAF50;
            color: white;
        }
        .login-btn:hover {
            background-color: #45a049;
        }
        .register-btn {
            background-color: #2196F3;
            color: white;
        }
        .register-btn:hover {
            background-color: #1e87dc;
        }
    </style>
</head>
<body>

<div class="container">
    <h1>Bienvenido</h1>
    <button class="btn login-btn" onclick="location.href='Login.html'">Iniciar Sesión</button>
    <button class="btn register-btn" onclick="location.href='Registro.html'">Crear Cuenta</button>
</div>

</body>
</html>
