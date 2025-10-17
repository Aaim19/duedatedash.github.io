<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Grade 9A | DueDateDash</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600;700&family=Poppins:wght@400;500&display=swap" rel="stylesheet">
<style>
  /* Base */
  body {
    margin: 0;
    font-family: 'Poppins', sans-serif;
    color: #fff;
    overflow-x: hidden; /* Allow vertical scroll only */
    display: flex;
    flex-direction: column;
    align-items: center;
    background: radial-gradient(circle at top left, #1b1b1b, #000);
    position: relative;
    min-height: 100vh;
  }

  /* Elegant shimmer background */
  body::before {
    content: "";
    position: fixed;
    inset: 0;
    background: linear-gradient(135deg, rgba(255,215,150,0.07), rgba(80,50,20,0.08), rgba(255,215,150,0.07));
    animation: subtleGlow 25s ease-in-out infinite;
    z-index: 0;
    pointer-events: none;
  }

  @keyframes subtleGlow {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
  }

  /* Floating light particles */
  .particle {
    position: fixed;
    border-radius: 50%;
    background: rgba(255,215,150,0.06);
    animation: floatParticle linear infinite;
    z-index: 0;
  }

  @keyframes floatParticle {
    0% { transform: translateY(100vh) rotate(0deg); opacity: 0; }
    20% { opacity: 0.3; }
    50% { transform: translateY(-50vh) rotate(180deg); opacity: 0.6; }
    80% { opacity: 0.3; }
    100% { transform: translateY(-100vh) rotate(360deg); opacity: 0; }
  }

  /* Header Section */
  .header-container {
    margin-top: 100px;
    margin-bottom: 120px;
    display: flex;
    flex-direction: column;
    gap: 60px;
    align-items: center;
    z-index: 2;
  }

  .heading-box {
    background: rgba(30, 20, 10, 0.8);
    border: 1px solid rgba(212,163,115,0.5);
    border-radius: 25px;
    padding: 35px 70px;
    box-shadow: 0 0 25px rgba(212,163,115,0.15), inset 0 0 10px rgba(255,215,150,0.05);
    transition: all 0.4s ease;
    cursor: pointer;
    position: relative;
    backdrop-filter: blur(10px);
  }

  .heading-box::before {
    content: "";
    position: absolute;
    inset: 0;
    border-radius: 25px;
    padding: 2px;
    background: linear-gradient(145deg, rgba(255,215,150,0.5), rgba(139,94,60,0.4));
    -webkit-mask: linear-gradient(#fff 0 0) content-box, linear-gradient(#fff 0 0);
    -webkit-mask-composite: xor;
    mask-composite: exclude;
    pointer-events: none;
  }

  .heading-box:hover {
    transform: translateY(-8px) scale(1.05);
    box-shadow: 0 0 45px rgba(255,215,150,0.35);
  }

  .heading-box h1 {
    margin: 0;
    font-family: 'Playfair Display', serif;
    font-weight: 700;
    font-size: 3rem;
    background: linear-gradient(to right, #d4a373, #fff4c2);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    letter-spacing: 1.5px;
    text-shadow: 0 0 15px rgba(255,255,200,0.1);
  }

  .click-note {
    font-size: 1rem;
    color: #e0b98a;
    font-style: italic;
    margin-top: 10px;
    transition: 0.3s ease;
  }

  .heading-box:hover .click-note {
    color: #fff4c2;
  }

  /* Footer */
  footer {
    margin: 100px 0 40px;
    text-align: center;
    color: #d4a373;
    font-family: 'Playfair Display', serif;
    font-size: 1.1rem;
    z-index: 2;
  }

  footer p { margin: 4px 0; }

  footer p.quote {
    font-style: italic;
    color: #f8e3b6;
    margin-top: 10px;
  }

  .github-link {
    font-size: 0.85rem;
    color: #fff;
    text-decoration: none;
    opacity: 0.7;
    transition: 0.3s;
    display: inline-block;
    margin-top: 8px;
  }

  .github-link:hover {
    opacity: 1;
    text-decoration: underline;
  }

  @media(max-width: 768px) {
    .heading-box { padding: 25px 40px; }
    .heading-box h1 { font-size: 2.2rem; }
    footer { font-size: 0.95rem; }
  }
</style>
</head>
<body>

  <!-- Particles -->
  <div class="particle" style="left:10%; width:6px; height:6px; animation-duration:18s;"></div>
  <div class="particle" style="left:30%; width:10px; height:10px; animation-duration:22s;"></div>
  <div class="particle" style="left:50%; width:8px; height:8px; animation-duration:25s;"></div>
  <div class="particle" style="left:70%; width:12px; height:12px; animation-duration:28s;"></div>
  <div class="particle" style="left:85%; width:14px; height:14px; animation-duration:32s;"></div>

  <!-- Header -->
  <div class="header-container">
    <div class="heading-box" onclick="window.location.href='doubts.html'">
      <h1>Business Grade 9</h1>
      <span class="click-note">Click for notes</span>
    </div>
    <div class="heading-box" onclick="window.location.href='inside.html'">
      <h1>Grade 9A’s DueDateDash</h1>
      <span class="click-note">Click here</span>
    </div>
  </div>

  <!-- Footer -->
  <footer>
    <p>By: Aaim • Shadhan • Yuaan</p>
    <p class="quote">“Push your limits”</p>
    
  </footer>

</body>
</html>
