<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Date and Time Button</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      padding-top: 50px;
    }
    button {
      padding: 10px 20px;
      font-size: 16px;
      border-radius: 8px;
      border: none;
      background-color: #4CAF50;
      color: white;
      cursor: pointer;
    }
    button:hover {
      background-color: #45a049;
    }
    #output {
      margin-top: 20px;
      font-size: 18px;
      color: #333;
    }
  </style>
</head>
<body>

  <h1>Show Current Date and Time</h1>
  <button id="showBtn">Click Me</button>
  <div id="output"></div>

  <script>
    // Attach event listener to button
    document.getElementById("showBtn").addEventListener("click", function() {
      const now = new Date();
      // Format date & time in a readable way
      document.getElementById("output").innerText = now.toLocaleString();
    });
  </script>

</body>
</html>
