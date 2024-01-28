<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Simple Calculator</title>
  <style>
    input {
      width: 100%;
      margin-bottom: 10px;
    }
  </style>
</head>
<body>

  <h2>Simple Calculator</h2>
  
  <input type="text" id="display" disabled>
  <br>
  <button onclick="clearDisplay()">C</button>
  <button onclick="appendToDisplay('1')">1</button>
  <button onclick="appendToDisplay('2')">2</button>
  <button onclick="appendToDisplay('3')">3</button>
  <button onclick="appendToDisplay('+')">+</button>
  <br>
  <button onclick="appendToDisplay('4')">4</button>
  <button onclick="appendToDisplay('5')">5</button>
  <button onclick="appendToDisplay('6')">6</button>
  <button onclick="appendToDisplay('-')">-</button>
  <br>
  <button onclick="appendToDisplay('7')">7</button>
  <button onclick="appendToDisplay('8')">8</button>
  <button onclick="appendToDisplay('9')">9</button>
  <button onclick="appendToDisplay('*')">*</button>
  <br>
  <button onclick="appendToDisplay('0')">0</button>
  <button onclick="calculateResult()">=</button>
  <button onclick="appendToDisplay('/')">/</button>

  <script>
    function appendToDisplay(value) {
      document.getElementById('display').value += value;
    }

    function clearDisplay() {
      document.getElementById('display').value = '';
    }

    function calculateResult() {
      try {
        document.getElementById('display').value = eval(document.getElementById('display').value);
      } catch (error) {
        document.getElementById('display').value = 'Error';
      }
    }
  </script>

</body>
</html>

![image](https://github.com/hardik5555/Simple-Calculator/assets/103363985/c7cf5de7-4ae2-49a4-9574-19c4349e2abc)

