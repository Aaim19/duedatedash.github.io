/* Apply to body or a specific container */
body {
  height: 100vh;
  margin: 0;
  background: linear-gradient(120deg, #4b2e2e, #b8916e, #4b2e2e);
  background-size: 300% 300%;
  animation: gradientAnimation 10s ease infinite;
  font-family: Arial, sans-serif;
}

/* Animation for smooth fading gradient */
@keyframes gradientAnimation {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}
