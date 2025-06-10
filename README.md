<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <title>موقعي</title>
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: 'Segoe UI', sans-serif;
    }

    body, html {
      height: 100%;
      background-color: #000;
      color: #000;
      direction: rtl;
    }

    .content {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      min-height: 100vh;
      gap: 40px;
    }

    .main-box {
      background-color: white;
      padding: 30px;
      border-radius: 20px;
      box-shadow: 0 0 20px rgba(255, 255, 255, 0.2);
      text-align: center;
      width: 300px;
      max-width: 90%;
    }

    .main-box img {
      width: 100px;
      height: 100px;
      object-fit: cover;
      border-radius: 10px;
    }

    .boxes {
      display: flex;
      gap: 20px;
      flex-wrap: wrap;
      justify-content: center;
      animation: fadeInScale 1.5s ease-in-out forwards;
      opacity: 0;
    }

    .box {
      background-color: white;
      color: black;
      border-radius: 10px;
      padding: 15px;
      width: 160px;
      text-align: center;
      box-shadow: 0 0 15px rgba(255,255,255,0.1);
      transition: transform 0.4s ease, box-shadow 0.4s ease;
      overflow: hidden;
    }

    .box img {
      width: 100%;
      height: 120px;
      object-fit: cover;
      border-radius: 8px;
    }

    .box span {
      display: block;
      margin-top: 10px;
      font-size: 16px;
      font-weight: bold;
    }

    .box:hover {
      transform: translateY(-5px) scale(1.05);
      box-shadow: 0 10px 25px rgba(255,255,255,0.2);
    }

    @keyframes fadeInScale {
      0% {
        opacity: 0;
        transform: scale(0.9);
      }
      100% {
        opacity: 1;
        transform: scale(1);
      }
    }
  </style>
</head>
<body>

  <div class="content">

    <div class="main-box">
      <img src="logo.png" alt="شعار">
    </div>

    <div class="boxes">
      <div class="box">
        <img src="service1.jpg" alt="الخدمة 1">
        <span>الخدمة 1</span>
      </div>
      <div class="box">
        <img src="service2.jpg" alt="الخدمة 2">
        <span>الخدمة 2</span>
      </div>
      <div class="box">
        <img src="service3.jpg" alt="الخدمة 3">
        <span>الخدمة 3</span>
      </div>
      <div class="box">
        <img src="service4.jpg" alt="الخدمة 4">
        <span>الخدمة 4</span>
      </div>
    </div>

  </div>

</body>
</html>
