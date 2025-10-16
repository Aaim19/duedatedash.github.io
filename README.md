
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Grade 9A DueDateDash</title>
  <link href="https://fonts.googleapis.com/css2?family=Baloo+2:wght@700&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      height: 100vh;
      font-family: 'Baloo 2', cursive;
      overflow: hidden;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      align-items: center;
      background: #3e2c1c;
      color: #fff;
    }
    /* Animated gradient background */
    body::before {
      content: '';
      position: absolute;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background: linear-gradient(270deg, #3e2c1c, #8b5e3c, #d4a373, #8b5e3c, #3e2c1c);
      background-size: 1000% 1000%;
      animation: gradientFlow 30s ease infinite;
      z-index: -3;
    }
    body::after {
      content: '';
      position: absolute;
      top: -50%; left: -50%;
      width: 200%; height: 200%;
      background: radial-gradient(circle at 30% 30%, rgba(255,255,255,0.05), transparent 60%);
      animation: lightMove 40s linear infinite;
      z-index: -1;
    }
    @keyframes gradientFlow {
      0% { background-position: 0% 50%; }
      25% { background-position: 50% 100%; }
      50% { background-position: 100% 50%; }
      75% { background-position: 50% 0%; }
      100% { background-position: 0% 50%; }
    }
    @keyframes lightMove {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }
    /* Floating particles */
    .particle {
      position: absolute;
      width: 10px; height: 10px;
      background: rgba(255,255,255,0.05);
      border-radius: 50%;
      animation: floatParticle linear infinite;
    }
    @keyframes floatParticle {
      0% { transform: translateY(100vh) translateX(0) rotate(0deg); opacity: 0; }
      10% { opacity: 0.2; }
      50% { transform: translateY(-50vh) translateX(50px) rotate(180deg); opacity: 0.5; }
      90% { opacity: 0.2; }
      100% { transform: translateY(-100vh) translateX(0) rotate(360deg); opacity: 0; }
    }
    .header-container {
      margin-top: 60px;
      text-align: center;
      z-index: 1;
      display: flex;
      flex-direction: column;
      gap: 25px;
    }
    /* Interactive bubble buttons */
    .heading-box {
      background: rgba(139, 94, 60, 0.85);
      border-radius: 25px;
      padding: 25px 50px;
      box-shadow: 5px 5px 20px rgba(0,0,0,0.6), inset 0 0 10px rgba(255,255,255,0.05);
      transition: transform 0.3s, box-shadow 0.3s;
      display: inline-block;
      cursor: pointer;
      animation: floatBubble 6s ease-in-out infinite alternate;
    }
    .heading-box:hover {
      transform: scale(1.1);
      box-shadow: 0 0 30px rgba(255, 255, 200, 0.6), 8px 8px 30px rgba(0,0,0,0.8), inset 0 0 15px rgba(255,255,255,0.1);
    }
    .heading-box:active {
      transform: scale(0.95);
      box-shadow: 0 0 15px rgba(255, 255, 200, 0.4), 5px 5px 20px rgba(0,0,0,0.6), inset 0 0 8px rgba(255,255,255,0.05);
    }
    h1 {
      font-size: 3rem;
      color: #fff;
      margin: 0;
      text-shadow: 4px 4px 15px rgba(0,0,0,0.7), 0 0 20px rgba(255,255,255,0.1);
    }
    a {
      color: #fff;
      text-decoration: none;
    }
    a:hover {
      text-decoration: underline;
    }
    @keyframes floatBubble {
      0% { transform: translateY(0px); }
      50% { transform: translateY(-15px); }
      100% { transform: translateY(0px); }
    }
    /* Footer */
    footer {
      margin-bottom: 30px;
      text-align: center;
      color: #d4a373;
      font-size: 1.2rem;
      text-shadow: 1px 1px 5px rgba(0,0,0,0.4);
      z-index: 1;
    }
    footer p { margin: 5px; }
    @media (max-width: 768px) {
      h1 { font-size: 2.2rem; }
      .heading-box { padding: 15px 25px; }
    }
  </style>
</head>
<body>

  <!-- Particles -->
  <div class="particle" style="left: 10%; width:8px; height:8px; animation-duration:18s;"></div>
  <div class="particle" style="left: 25%; width:12px; height:12px; animation-duration:22s;"></div>
  <div class="particle" style="left: 50%; width:6px; height:6px; animation-duration:16s;"></div>
  <div class="particle" style="left: 70%; width:10px; height:10px; animation-duration:20s;"></div>
  <div class="particle" style="left: 85%; width:14px; height:14px; animation-duration:25s;"></div>

  <!-- Header with interactive bubble buttons -->
  <div class="header-container">
    <div class="heading-box">
      <h1>Business Grade 9</h1>
    </div>
    <div class="heading-box" onclick="window.location.href='inside.html'">
      <h1><i>Grade 9A’s DueDateDash</i></h1>
    </div>
  </div>

  <!-- Footer -->
  <footer>
    <p>By:</p>
    <p>Aaim</p>
    <p>Shadhan</p>
    <p>Yuaan</p>
    <p>"Push your limits"</p>
  </footer>

</body>
</html>
