<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Weather Forecasting Model</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
    }
    .container {
      width: 80%;
      margin: auto;
      text-align: center;
    }
    h1 {
      margin-bottom: 20px;
    }
    .input-group {
      margin-bottom: 20px;
    }
    .input-group label {
      display: block;
      margin-bottom: 5px;
    }
    .input-group input {
      width: 100%;
      padding: 8px;
      border: 1px solid #ccc;
      border-radius: 4px;
      box-sizing: border-box;
    }
    button {
      background-color: #4CAF50;
      color: white;
      padding: 10px 20px;
      border: none;
      border-radius: 4px;
      cursor: pointer;
    }
    button:hover {
      background-color: #45a049;
    }
    .forecast {
      margin-top: 20px;
      padding: 20px;
      border: 1px solid #ccc;
      border-radius: 4px;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Weather Forecasting Model</h1>
    <div class="input-group">
      <label for="temperature">Temperature (°C):</label>
      <input type="number" id="temperature" placeholder="Enter temperature">
    </div>
    <div class="input-group">
      <label for="humidity">Humidity (%):</label>
      <input type="number" id="humidity" placeholder="Enter humidity">
    </div>
    <div class="input-group">
      <label for="wind-speed">Wind Speed (km/h):</label>
      <input type="number" id="wind-speed" placeholder="Enter wind speed">
    </div>
    <button onclick="forecastWeather()">Get Forecast</button>
    <div class="forecast" id="forecast-result"></div>
  </div>

  <script>
    function forecastWeather() {
      var temperature = parseFloat(document.getElementById("temperature").value);
      var humidity = parseFloat(document.getElementById("humidity").value);
      var windSpeed = parseFloat(document.getElementById("wind-speed").value);

      // Perform weather forecasting calculations here
      // Example: Generate forecast based on input parameters

      // Display forecast result
      var forecastResult = document.getElementById("forecast-result");
      forecastResult.innerHTML = "Forecasted Weather:<br>";
      forecastResult.innerHTML += "Temperature: " + temperature + " °C<br>";
      forecastResult.innerHTML += "Humidity: " + humidity + " %<br>";
      forecastResult.innerHTML += "Wind Speed: " + windSpeed + " km/h";
    }
  </script>
</body>
</html>
