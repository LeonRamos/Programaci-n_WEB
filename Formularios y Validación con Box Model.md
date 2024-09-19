<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Formulario con Validación</title>
  <style>
    * {
      box-sizing: border-box;
    }
    body {
      font-family: Arial, sans-serif;
      background-color: #f4f4f4;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
    }
    .form-container {
      width: 400px;
      background-color: white;
      padding: 20px;
      border-radius: 8px;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
    }
    input, textarea {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
      border: 1px solid #ccc;
      border-radius: 4px;
    }
    button {
      padding: 10px 15px;
      background-color: #28a745;
      color: white;
      border: none;
      border-radius: 4px;
      cursor: pointer;
    }
    button:hover {
      background-color: #218838;
    }
    input:invalid {
      border-color: red;
    }
  </style>
</head>
<body>

<div class="form-container">
  <form id="formulario">
    <label for="nombre">Nombre completo:</label>
    <input type="text" id="nombre" name="nombre" required>

    <label for="email">Correo electrónico:</label>
    <input type="email" id="email" name="email" required>

    <label for="password">Contraseña:</label>
    <input type="password" id="password" name="password" required minlength="8">

    <label for="confirm_password">Confirmar contraseña:</label>
    <input type="password" id="confirm_password" name="confirm_password" required>

    <!-- Más campos aquí -->

    <button type="submit">Enviar</button>
    <button type="reset">Limpiar</button>
  </form>
</div>

</body>
</html>
