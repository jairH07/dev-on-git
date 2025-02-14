<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Number Adder</title>
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css"
    />
    <link rel="stylesheet" href="styles.css" />
  </head>
  <style>
    body {
      font-family: Arial, sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      background-color: #f0f0f0;
    }
    .container {
      background-color: white;
      padding: 30px;
      border-radius: 8px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
      text-align: center;
      max-width: 400px;
      width: 100%;
    }
    h1 {
      color: #333;
      margin-bottom: 10px;
    }
    p {
      color: #666;
      margin-bottom: 20px;
    }
    .input-group {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 15px;
    }
    input {
      width: 45%;
      padding: 10px;
      border: 1px solid #ddd;
      border-radius: 4px;
      font-size: 16px;
    }
    button {
      width: 100%;
      padding: 10px;
      background-color: #4caf50;
      color: white;
      border: none;
      border-radius: 4px;
      cursor: pointer;
      font-size: 16px;
      transition: background-color 0.3s;
    }
    button:hover {
      background-color: #45a049;
    }
    #result {
      margin-top: 20px;
      font-weight: bold;
      font-size: 18px;
    }
    .icon {
      font-size: 24px;
      margin: 0 10px;
      color: #4caf50;
    }
  </style>
  <body>
    <div class="container">
      <h1><i class="fas fa-plus-circle icon"></i> Number Adder</h1>
      <p>Enter two numbers below and click the button to add them together.</p>
      <div class="input-group">
        <input
          type="number"
          id="num1"
          placeholder="Enter first number"
          required
        />
        <i class="fas fa-plus icon"></i>
        <input
          type="number"
          id="num2"
          placeholder="Enter second number"
          required
        />
      </div>
      <button id="addButton">Add Numbers</button>
      <div id="result"></div>
    </div>
    <script src="script.js">
            addButton.addEventListener('click', function(){
          let num1 = document.getElementById("num1").value;
          let num2 = document.getElementById("num2").value;
          let addButton = document.getElementById("addButton").value;
          let result = document.getElementById("result");

      let sum =parseFloat(num1) + parseFloat(num2);

          result.innerHTML = sum;
      });
    </script>
  </body>
</html>
