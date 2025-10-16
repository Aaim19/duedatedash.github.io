
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Grade 9A DueDateDash</title>
<link href="https://fonts.googleapis.com/css2?family=Baloo+2:wght@400;700&family=Roboto:wght@400;500&display=swap" rel="stylesheet">
<style>
  /* Base setup */
  body {
    margin: 0;
    height: 100vh;
    font-family: 'Roboto', sans-serif;
    color: #fff;
    overflow: hidden;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    background: linear-gradient(135deg, #3e2c1c, #8b5e3c, #d4a373, #8b5e3c, #3e2c1c);
    background-size: 500% 500%;
    animation: bgFlow 40s ease infinite;
    position: relative;
  }
  /* Gradient animation */
  @keyframes bgFlow {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
  }
  /* Particles */
  .particle {
    position: absolute;
    border-radius: 50%;
    background: rgba(255,255,255,0.08);
    animation: floatParticle linear infinite;
  }
  @keyframes floatParticle {
    0% { transform: translateY(100vh) translateX(0) rotate(0deg); opacity: 0; }
    10% { opacity: 0.2; }
    50% { transform: translateY(-50vh) translateX(50px) rotate(180deg); opacity: 0.5; }
    90% { opacity: 0.2; }
    100% { transform: translateY(-100vh) translateX(0) rotate(360deg); opacity: 0; }
  }
  /* Bottom overlay for footer */
  .bottom-overlay {
    position: absolute;
    bottom: 0;
    width: 100%;
    height: 35%;
    background: linear-gradient(to top, rgba(0,0,0,0.75), transparent);
    z-index: -1;
  }
  /* Header container */
  .header-container {
    margin-top: 60px;
    display: flex;
    flex-direction: column;
    gap: 30px;
    align-items: center;
    z-index: 1;
    width: 100%;
  }
  /* Branded bubble buttons */
  .heading-box {
    background: rgba(139,94,60,0.9);
    border-radius: 30px;
    padding: 25px 60px;
    box-shadow: 5px 5px 20px rgba(0,0,0,0.6), inset 0 0 15px rgba(255,255,255,0.07);
    display: flex;
    flex-direction: column;
    align-items: center;
    transition: all 0.4s ease;
    cursor: pointer;
    position: relative;
    animation: floatBubble 5s ease-in-out infinite alternate;
  }
  .heading-box:hover {
    transform: translateY(-8px) scale(1.08);
    box-shadow: 0 0 35px rgba(255, 255, 200,0.6), 10px 10px 30px rgba(0,0,0,0.85), inset 0 0 18px rgba(255,255,255,0.1);
  }
  .heading-box:active {
    transform: scale(0.95);
    box-shadow: 0 0 20px rgba(255, 255, 200,0.4), 5px 5px 18px rgba(0,0,0,0.6), inset 0 0 10px rgba(255,255,255,0.05);
  }
  .heading-box h1 {
    margin: 0;
    font-family: 'Baloo 2', cursive;
    font-weight: 700;
    font-size: 3rem;
    text-shadow: 3px 3px 15px rgba(0,0,0,0.6);
    letter-spacing: 1px;
  }
  .click-note {
    font-size: 1rem;
    color: #ffe0b2;
    font-style: italic;
    margin-top: 8px;
    text-shadow: 1px 1px 4px rgba(0,0,0,0.5);
    transition: all 0.3s ease;
  }
  .heading-box:hover .click-note {
    color: #fff2d1;
    transform: translateY(-2px);
  }
  @keyframes floatBubble {
    0% { transform: translateY(0); }
    50% { transform: translateY(-12px); }
    100% { transform: translateY(0); }
  }
  /* Footer styling */
  footer {
    margin-bottom: 30px;
    text-align: center;
    color: #d4a373;
    font-family: 'Baloo 2', cursive;
    font-size: 1.2rem;
    text-shadow: 1px 1px 5px rgba(0,0,0,0.45);
    display: flex;
    flex-direction: column;
    gap: 4px;
    z-index: 1;
  }
  footer p:nth-child(1) { font-weight: 500; font-size: 1.1rem; }
  footer p:nth-child(5) { font-size: 1.1rem; font-style: italic; color: #e0b98a; }
  /* Responsive adjustments */
  @media(max-width: 768px){
    .heading-box h1 { font-size: 2rem; }
    .heading-box { padding: 18px 35px; }
    footer { font-size: 1rem; }
  
  }
</style>
</head>
<body>

  <!-- Particles -->
  <div class="particle" style="left:10%; width:8px; height:8px; animation-duration:18s;"></div>
  <div class="particle" style="left:25%; width:12px; height:12px; animation-duration:22s;"></div>
  <div class="particle" style="left:50%; width:6px; height:6px; animation-duration:16s;"></div>
  <div class="particle" style="left:70%; width:10px; height:10px; animation-duration:20s;"></div>
  <div class="particle" style="left:85%; width:14px; height:14px; animation-duration:25s;"></div>

  <!-- Bottom overlay -->
  <div class="bottom-overlay"></div>

  <!-- Header -->
  <div class="header-container">
    <div class="heading-box">
      <h1>Business Grade 9</h1>
    </div>
    <div class="heading-box" onclick="window.location.href='inside.html'">
      <h1><i>Grade 9A’s DueDateDash</i></h1>
      <span class="click-note">Click here</span>
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
