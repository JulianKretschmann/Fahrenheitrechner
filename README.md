# Fahrenheitrechner
<html lang="en" dir="ltr">
  <head>
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
    <script>
      "use strict";

      function fTemperatur() {
        var vMenge;
        var vFahrenheit;
        var vAusgabe;

        vMenge = document.getElementById("idMenge").value;
        vMenge = parseFloat(vMenge);

        vFahrenheit = vMenge * 1.8 + 32;

        vAusgabe = "";
        vAusgabe = vAusgabe + "Fahrenheit: ";
        vAusgabe = vAusgabe + vFahrenheit;
        vAusgabe = vAusgabe + "°F";

        document.getElementById("idAusgabe").innerHTML = vAusgabe;
      }
    </script>
    <title>Temperaturumrechner</title>
  </head>
  <body>
    <h1>Celsius - Fahrenheit Umrechnen</h1>
    Celsius °C: <input id="idMenge" type="text" value="10" />
    <button onClick="fTemperatur();">Berechne den Erlös!</button><br />
    <div id="idAusgabe">Fahrenheit:</div>
  </body>
</html>
