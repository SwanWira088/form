<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Form Animasi Rapi</title>
  <style>
    body {
      font-family: "Segoe UI", Arial, sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      background: linear-gradient(135deg, #7f53b9, #1e48ff);
    }

    .form-container {
      background: #ffffff;
      padding: 40px 30px;
      border-radius: 20px;
      box-shadow: 0 10px 2px rgba(0,0,0,0.15);
      width: 350px;
      animation: fadeSlide 0.8s ease forwards;
      opacity: 0;
      transform: translateY(40px);
    }

    @keyframes fadeSlide {
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    .form-container h2 {
      margin: 0 0 25px;
      font-size: 22px;
      text-align: center;
      color: rgb(69, 16, 129);
    }

    label {
      font-weight: 600;
      display: block;
      margin-bottom: 6px;
      color: #6200ff;
    }

    input[type="text"],
    input[type="password"] {
      width: 92%;
      padding: 12px;
      margin-bottom: 20px;
      border: 2px solid #ddd;
      border-radius: 10px;
      font-size: 14px;
      transition: 0.3s;
    }

    input[type="date"] {
      width: 92%;
      padding: 12px;
      margin-bottom: 20px;
      border: 2px solid #ddd;
      border-radius: 10px;
      font-size: 14px;
      transition: 0.3s;
    }

    input:focus {
      border-color: #6a85b6;
      box-shadow: 0 0 8px rgba(106,133,182,0.4);
      outline: none;
    }

    input[type="submit"] {
      width: 100%;
      background: linear-gradient(135deg, #667eea, #764ba2);
      color: whitesmoke;
      border: none;
      padding: 14px;
      border-radius: 10px;
      font-size: 16px;
      font-weight: bold;
      cursor: pointer;
      transition: 0.3s;
    }

    input[type="submit"]:hover {
      background: linear-gradient(135deg, #ff00f2, #570ce2);
      transform: translateY(-2px);
      box-shadow: 0 5px 15px rgba(0,0,0,0.15);
    }
  </style>
</head>
<body>
  <div class="form-container">
    <h2>Login Swan Sucker's</h2>
    <form name="contoh" action="form-submit.html" method="get">
      <label for="nama">Name</label>
      <input type="text" id="nama" name="nama" required>
      <label for="password">Password</label>
      <input type="password" id="password" name="password" required>
      <label for="tanggal">Date Birth</label>
      <input type="date" id="tanggal" name="tanggal" required>
      <input type="submit" value="Send Ident">
    </form>
  </div>
</body>
</html>
