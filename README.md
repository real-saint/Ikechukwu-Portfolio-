<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Perfect Ikechukwu - Portfolio Quest</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css" crossorigin="anonymous" />
  <link href="https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap" rel="stylesheet">
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }body {
  font-family: 'Press Start 2P', monospace;
  background-color: #0d1b2a;
  color: #fff;
  overflow-x: hidden;
}

.start-screen {
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background: #000;
  color: #0ff;
  text-align: center;
}

.start-screen h1 {
  font-size: 1.5rem;
  margin-bottom: 2rem;
}

.start-button {
  background: #0ff;
  color: #000;
  padding: 1rem 2rem;
  border: none;
  font-size: 1rem;
  cursor: pointer;
  border-radius: 8px;
  transition: transform 0.2s;
}

.start-button:hover {
  transform: scale(1.1);
}

.game-container {
  display: none;
  padding: 2rem;
  max-width: 1000px;
  margin: auto;
}

.profile {
  text-align: center;
  margin-bottom: 2rem;
}

.profile img {
  width: 150px;
  height: 150px;
  object-fit: cover;
  border-radius: 50%;
  border: 4px solid #0ff;
  margin-bottom: 1rem;
}

.level {
  background: #fff;
  color: #000;
  padding: 2rem;
  border-radius: 10px;
  margin-bottom: 2rem;
  position: relative;
  box-shadow: 0 0 15px #0ff;
  animation: slideIn 1s ease forwards;
}

.level h2 {
  color: #0d1b2a;
  margin-bottom: 1rem;
}

.social-icons {
  text-align: center;
  margin-top: 1.5rem;
}

.social-icons a {
  color: #0ff;
  font-size: 1.5rem;
  margin: 0 0.5rem;
  text-decoration: none;
}

.xp-bar {
  background: #222;
  height: 20px;
  border-radius: 10px;
  overflow: hidden;
  margin-top: 1rem;
}

.xp-fill {
  background: #0ff;
  width: 70%;
  height: 100%;
  transition: width 1s ease;
}

footer {
  text-align: center;
  padding: 1rem;
  background: #000;
  color: #0ff;
}

@keyframes slideIn {
  0% { opacity: 0; transform: translateY(30px); }
  100% { opacity: 1; transform: translateY(0); }
}

  </style>
</head>
<body><div class="start-screen" id="startScreen">
  <h1>🎮 Perfect Ikechukwu's Portfolio Quest</h1>
  <button class="start-button" onclick="startGame()">Press Start</button>
</div><div class="game-container" id="gameContainer">
  <div class="profile">
    <img src="https://images.unsplash.com/photo-1549921296-3a6b6b050b57?fit=crop&w=300&q=80" alt="Perfect's Photo">
    <h2>Perfect Ikechukwu</h2>
    <p>Matric Number: 24/208CSC/898</p>
    <p>Email: <a href="mailto:ikechukwuperfect759@gmail.com" style="color:#f4a261;">ikechukwuperfect759@gmail.com</a></p>
    <div class="social-icons">
      <a href="#"><i class="fab fa-instagram"></i></a>
      <a href="#"><i class="fab fa-x-twitter"></i></a>
      <a href="#"><i class="fab fa-facebook-f"></i></a>
    </div>
  </div>  <div class="level" id="level1">
    <h2>🕹️ Level 1: Past</h2>
    <p>I started learning the ropes of web design, building pages with HTML and CSS. It was like trying to teach a fish to climb a tree—awkward at first, but now I'm swimming in code!</p>
    <div class="xp-bar"><div class="xp-fill" style="width: 60%"></div></div>
  </div>  <div class="level" id="level2">
    <h2>⚔️ Level 2: Present</h2>
    <p>Currently a Computer Science student at the University of Abuja, sharpening my programming skills like a ninja with a keyboard. I’m building projects, debugging life, and drinking coffee like it’s a superpower.</p>
    <div class="xp-bar"><div class="xp-fill" style="width: 80%"></div></div>
  </div>  <div class="level" id="level3">
    <h2>🚀 Level 3: Future</h2>
    <p>I'm heading toward a career in cybersecurity—because what’s cooler than being a digital bodyguard? My dream is to become the guy who stops the bad guys with just a terminal window and a smirk.</p>
    <div class="xp-bar"><div class="xp-fill" style="width: 90%"></div></div>
  </div>
</div><footer>
  <p>© 2025 Perfect Ikechukwu. All rights reserved.</p>
</footer><script>
  function startGame() {
    document.getElementById("startScreen").style.display = "none";
    document.getElementById("gameContainer").style.display = "block";
  }
</script></body>
</html>
