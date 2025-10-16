
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Animated Brown Background</title>
  <style>
    /* Apply to entire page */
    body {
      height: 100vh;
      margin: 0;
      background: linear-gradient(120deg, #4b2e2e, #b8916e, #4b2e2e);
      background-size: 300% 300%;
      animation: gradientAnimation 10s ease infinite;
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: Arial, sans-serif;
      color: #fff;
    }

    /* Animation for smooth fading gradient */
    @keyframes gradientAnimation {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    /* Example heading to show on the page */
    h1 {
      font-size: 3rem;
      text-shadow: 2px 2px 5px rgba(0,0,0,0.5);
    }
  </style>
  </head>
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
