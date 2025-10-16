
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Grade 9A’s DueDateDash</title>
  <style>
    /* Full-screen body */
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: 'Arial', sans-serif;
      overflow: hidden;
      background: #3e2c1c; /* fallback color */
    }

    /* Animated gradient background using pseudo-element */
    body::before {
      content: '';
      position: absolute;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background: linear-gradient(270deg, #3e2c1c, #8b5e3c, #d4a373, #8b5e3c, #3e2c1c);
      background-size: 1000% 1000%;
      animation: gradientFlow 30s ease infinite;
      z-index: -2;
    }

    /* Floating particles */
    .particle {
      position: absolute;
      width: 10px; height: 10px;
      background: rgba(255, 255, 255, 0.05);
      border-radius: 50%;
      animation: floatParticle 20s linear infinite;
    }

    @keyframes gradientFlow {
      0% { background-position: 0% 50%; }
      25% { background-position: 50% 100%; }
      50% { background-position: 100% 50%; }
      75% { background-position: 50% 0%; }
      100% { background-position: 0% 50%; }
    }

    @keyframes floatParticle {
      0% { transform: translateY(100vh) translateX(0) rotate(0deg); opacity: 0; }
      10% { opacity: 0.2; }
      50% { transform: translateY(-50vh) translateX(50px) rotate(180deg); opacity: 0.5; }
      90% { opacity: 0.2; }
      100% { transform: translateY(-100vh) translateX(0) rotate(360deg); opacity: 0; }
    }

    /* Central heading */
    h1 {
      position: relative;
      z-index: 1;
      font-size: 4rem;
      color: #fff;
      font-style: italic;
      text-shadow: 2px 2px 15px rgba(0,0,0,0.7), 0 0 20px rgba(255,255,255,0.1);
      animation: pulseText 3s ease-in-out infinite alternate;
      text-align: center;
    }

    @keyframes pulseText {
      0% { text-shadow: 2px 2px 15px rgba(0,0,0,0.7), 0 0 20px rgba(255,255,255,0.1); }
      50% { text-shadow: 2px 2px 25px rgba(0,0,0,0.8), 0 0 30px rgba(255,255,255,0.3); }
      100% { text-shadow: 2px 2px 15px rgba(0,0,0,0.7), 0 0 20px rgba(255,255,255,0.1); }
    }
  </style>
</head>
<body>

  <!-- Heading -->
  <h1> Business Grade 9 </h1>

  <!-- Floating particles -->
  <div class="particle" style="left: 10%; width:8px; height:8px; animation-duration:18s;"></div>
  <div class="particle" style="left: 25%; width:12px; height:12px; animation-duration:22s;"></div>
  <div class="particle" style="left: 50%; width:6px; height:6px; animation-duration:16s;"></div>
  <div class="particle" style="left: 70%; width:10px; height:10px; animation-duration:20s;"></div>
  <div class="particle" style="left: 85%; width:14px; height:14px; animation-duration:25s;"></div>

</body>
</html>

<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Grade 9A DueDateDash</title>
  <style>
    body {
      height: 100vh;
      margin: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(120deg, #4b2e2e, #b8916e, #4b2e2e);
      background-size: 300% 300%;
      animation: gradientAnimation 10s ease infinite;
      font-family: Arial, sans-serif;
      color: #fff;
    }

    @keyframes gradientAnimation {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    h1 {
      font-style: italic; /* makes the heading italic */
      text-shadow: 2px 2px 5px rgba(0,0,0,0.5);
    }

    a {
      color: #fff; /* make link white */
      text-decoration: none; /* remove underline */
    }

    a:hover {
      text-decoration: underline; /* underline on hover */
    }
  </style>
</head>
<body>
  <h1>
    <a href="inside.html"><i>Grade 9A’s DueDateDash</i></a>
  </h1>
</body>
</html>
