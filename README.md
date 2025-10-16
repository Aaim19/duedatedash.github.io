/* Apply to the whole page */
body {
  height: 100vh;
  margin: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  font-family: Arial, sans-serif;
  color: #fff;
  background: linear-gradient(270deg, #3e2c1c, #8b5e3c, #d4a373, #8b5e3c, #3e2c1c);
  background-size: 1000% 1000%;
  animation: brownFlow 20s ease infinite;
  text-align: center;
  overflow: hidden;
}

/* Smooth flowing gradient animation */
@keyframes brownFlow {
  0% { background-position: 0% 50%; }
  25% { background-position: 50% 100%; }
  50% { background-position: 100% 50%; }
  75% { background-position: 50% 0%; }
  100% { background-position: 0% 50%; }
}

/* Example heading */
h1 {
  font-size: 3rem;
  font-style: italic;
  text-shadow: 2px 2px 8px rgba(0,0,0,0.6);
  animation: pulseText 3s ease-in-out infinite alternate;
}

/* Subtle pulsing animation for text */
@keyframes pulseText {
  0% { text-shadow: 2px 2px 8px rgba(0,0,0,0.6), 0 0 0px rgba(255,255,255,0); }
  50% { text-shadow: 2px 2px 12px rgba(0,0,0,0.7), 0 0 10px rgba(255,255,255,0.2); }
  100% { text-shadow: 2px 2px 8px rgba(0,0,0,0.6), 0 0 0px rgba(255,255,255,0); }
}

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
