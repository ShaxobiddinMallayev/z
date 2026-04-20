<!DOCTYPE html>
<html lang="uz">
<head>
  <meta charset="UTF-8">
  <title>3% Hisoblash</title>
  <style>
    body {
      font-family: Arial;
      background: #f4f4f4;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }
    .box {
      background: white;
      padding: 20px;
      border-radius: 12px;
      text-align: center;
      width: 300px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }
    input {
      width: 100%;
      padding: 10px;
      margin-top: 10px;
      font-size: 16px;
    }
    button {
      margin-top: 15px;
      padding: 10px;
      width: 100%;
      background: #4CAF50;
      color: white;
      border: none;
      font-size: 16px;
      border-radius: 8px;
    }
    .result {
      margin-top: 15px;
      font-weight: bold;
    }
  </style>
</head>
<body>

<div class="box">
  <h2>3% Hisoblash</h2>
  <p>Mijoz summasini kiriting (A):</p>
  
  <input type="number" id="inputA" placeholder="Masalan: 600000">
  
  <button onclick="hisobla()">Hisobla</button>
  
  <div class="result" id="natija"></div>
</div>

<script>
function hisobla() {
  let A = document.getElementById("inputA").value;
  let B = A / 1.03;

  document.getElementById("natija").innerText =
    "Ishchi yozishi kerak: " + Math.round(B) + " so'm";
}
</script>

</body>
</html>
