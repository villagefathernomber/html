<!DOCTYPE html>
<html>
<head>
  <title>Digital Clock</title>
  <style>
    body {
      background: white;
      color: cyan;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      font-family: monospace;
    }
    h1 {
      border: 50px solid black;
      padding: 100px;
      border-radius: 100px;
    }
    h2 {
        background-color:blue;
        color:brown;
        border: 10px solid blue;
      padding: 100px;
      border-radius: 100px;
    }
    
  </style>
</head>
<body>
  <h1 id="clock nitish"></h1><br><br/>
   <h2>THIS IS MY TIME </h2>
  <script>
    function updateClock() {
      const now = new Date();
      const time = now.toLocaleTimeString();
      document.getElementById("clock nitish").textContent = time;
    }
    setInterval(updateClock, 1000);
    updateClock();
  </script>
</body>
</html>
