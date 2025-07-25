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
  position: relative;
}

.lightning {
  position: fixed;
  top: 0;
  left: 0;
  width: 100vw;
  height: 100vh;
  pointer-events: none;
  z-index: -1;
}

.flash {
  animation: flashEffect 8s infinite;
  background: radial-gradient(circle, rgba(255,255,255,0.4) 0%, rgba(0,0,0,0.2) 70%);
  position: absolute;
  width: 100%;
  height: 100%;
  opacity: 0;
}

@keyframes flashEffect {
  0%, 98%, 100% {
    opacity: 0;
  }
  99% {
    opacity: 1;
  }
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

.level {
  background: #fff;
  color: #000;
  padding: 2rem;
  border-radius: 10px;
  margin-bottom: 2rem;
  position: relative;
  box-shadow: 0 0 15px #0ff;
  animation: fadeSlide 1s ease forwards;
}

.level h2 {
  color: #0d1b2a;
  margin-bottom: 1rem;
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
  height: 100%;
  transition: width 1s ease;
}

.skills-section, .projects-section, .map-section {
  background: #fff;
  color: #000;
  padding: 2rem;
  border-radius: 10px;
  box-shadow: 0 0 15px #0ff;
  margin-bottom: 2rem;
}

.skills-section h2, .projects-section h2, .map-section h2 {
  color: #0d1b2a;
  margin-bottom: 1rem;
}

.skill {
  margin-bottom: 1rem;
}

.skill-label {
  margin-bottom: 0.5rem;
}

.skill-bar {
  background: #222;
  height: 18px;
  border-radius: 9px;
  overflow: hidden;
}

.skill-fill {
  background: #0ff;
  height: 100%;
  transition: width 1s ease;
}

.project-item {
  margin: 1rem 0;
  border-left: 4px solid #0ff;
  padding-left: 1rem;
}

.map-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
}

.map-tile {
  flex: 1 1 30%;
  background: #0d1b2a;
  color: #0ff;
  border: 2px dashed #0ff;
  padding: 1rem;
  text-align: center;
  border-radius: 8px;
}

footer {
  text-align: center;
  padding: 2rem 1rem;
  background: #000;
  color: #0ff;
}

.social-icons {
  margin-top: 1rem;
}

.social-icons a {
  color: #0ff;
  font-size: 1.5rem;
  margin: 0 0.5rem;
  text-decoration: none;
}

@keyframes fadeSlide {
  0% { opacity: 0; transform: translateY(40px); }
  100% { opacity: 1; transform: translateY(0); }
}

  </style>
</head>
<body>
<div class="lightning">
  <div class="flash"></div>
</div>
<audio id="bgMusic" loop autoplay>
  <source src="https://files.catbox.moe/8pue4c.mp3" type="audio/mpeg">
</audio><div class="start-screen" id="startScreen">
  <h1>🎮 Perfect Ikechukwu's Portfolio Quest</h1>
  <button class="start-button" onclick="startGame()">Press Start</button>
</div><div class="game-container" id="gameContainer">
  <div class="level" id="past">
    <h2>🕹️ Level 1: Past</h2>
    <p>I started learning the ropes of web design, building pages with HTML and CSS. It was like trying to teach a fish to climb a tree—awkward at first, but now I'm swimming in code!</p>
    <div class="xp-bar"><div class="xp-fill" style="width: 60%"></div></div>
  </div>  <div class="level" id="present">
    <h2>⚔️ Level 2: Present</h2>
    <p>Currently a Computer Science student at the University of Abuja, sharpening my programming skills like a ninja with a keyboard. I’m building projects, debugging life, and drinking coffee like it’s a superpower.</p>
    <div class="xp-bar"><div class="xp-fill" style="width: 80%"></div></div>
  </div>  <div class="level" id="future">
    <h2>🚀 Level 3: Future</h2>
    <p>I'm heading toward a career in cybersecurity—because what’s cooler than being a digital bodyguard? My dream is to become the guy who stops the bad guys with just a terminal window and a smirk.</p>
    <div class="xp-bar"><div class="xp-fill" style="width: 90%"></div></div>
  </div>
</div><footer>
  <p>Email: <a href="mailto:ikechukwuperfect759@gmail.com" style="color:#0ff;">ikechukwuperfect759@gmail.com</a></p>
  <div class="social-icons">
    <a href="#"><i class="fab fa-instagram"></i></a>
    <a href="#"><i class="fab fa-x-twitter"></i></a>
    <a href="#"><i class="fab fa-facebook-f"></i></a>
  </div>
  <p style="margin-top: 1rem;">© 2025 Perfect Ikechukwu. All rights reserved.</p>
</footer><script>
  function startGame() {
    document.getElementById("startScreen").style.display = "none";
    document.getElementById("gameContainer").style.display = "block";
  }
</script></body>
</html>
