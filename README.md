<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Calculadora de Amor</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      margin: 50px;
    }
  </style>
</head>
<body>
  <h1>Calculadora de Amor</h1>
  <!-- Establecer el valor predeterminado para el primer nombre -->
  <label for="nombre1">Nombre 1:</label>
  <input type="text" id="nombre1" value="Ariadna" disabled>
  <br>
  <label for="nombre2">Nombre 2:</label>
  <input type="text" id="nombre2" placeholder="Ingrese el segundo nombre" required>
  <br>
  <button onclick="calcularPorcentaje()">Calcular Amor</button>
  <p id="resultado"></p>

  <script>
    function calcularPorcentaje() {
      // Obtiene el valor del segundo nombre
      const nombre2 = document.getElementById('nombre2').value.toLowerCase();

      // Lógica para calcular el porcentaje (puedes personalizar esto según tus preferencias)
      let porcentajeAmor = 50; // Valor base

      // Ejemplo de nombre1 
      if (nombre2 === 'gerard' || nombre2 === 'gericabot' || nombre2 === 'gerardcabot' ||nombre2 === 'Gerard Cabot' || nombre2 === 'Gerard Cabot Agustin') {
        porcentajeAmor = 100;
      }
      else porcentajeAmor = 0;



      // Mostrar el resultado
      document.getElementById('resultado').innerText = `El porcentaje de amor entre Ariadna y ${nombre2} es ${porcentajeAmor}%`;
    }
  </script>
</body>
</html>
