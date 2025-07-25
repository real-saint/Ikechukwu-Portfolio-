<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Portfolio Quest</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css" crossorigin="anonymous" />
  <link href="https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap" rel="stylesheet">
  <style>
    /* styles remain unchanged for brevity */
  </style>
</head>
<body>
<div class="background-layer"></div>
<div class="lightning float-bg">
  <div class="flash"></div>
</div>
<audio id="bgMusic">
  <source src="https://files.catbox.moe/8pue4c.mp3" type="audio/mpeg">
</audio>
<div class="start-screen" id="startScreen">
  <h1>🎮 Perfect Ikechukwu's Portfolio Quest</h1>
  <button class="start-button" onclick="startGame()">Press Start</button>
</div>
<div class="game-container" id="gameContainer">
  <img src="https://api.dicebear.com/7.x/pixel-art/svg?seed=Perfect" alt="avatar" class="avatar" />
  <div class="level" id="about">
    <h2>👤 About Me</h2>
    <p>Hi, my name is Perfect Ikechukwu. I'm a passionate Computer Science student at the University of Abuja. My journey in tech started with curiosity and has grown into a love for solving problems with code.</p>
    <p>Over the years, I've built strong foundations in programming, algorithms, and system design. But where I truly shine is web development — I've become skilled in creating clean, responsive, and interactive websites using HTML, CSS, and JavaScript.</p>
    <p>I believe in continuous learning and have already taken big steps forward in both frontend and backend design. Whether it's building static pages or integrating backend systems, I’m all in.</p>
    <div class="xp-bar"><div class="xp-fill" style="width: 85%"></div></div>
  </div>
  <div class="level" id="past">
    <h2>🕹️ Level 1: Past</h2>
    <p>I started learning the ropes of web design, building pages with HTML and CSS. It was like trying to teach a fish to climb a tree—awkward at first, but now I'm swimming in code!</p>
    <div class="xp-bar"><div class="xp-fill" style="width: 60%"></div></div>
  </div>
  <div class="level" id="present">
    <h2>⚔️ Level 2: Present</h2>
    <p>Currently a Computer Science student at the University of Abuja, sharpening my programming skills like a ninja with a keyboard. I’m building projects, debugging life, and drinking coffee like it’s a superpower.</p>
    <div class="xp-bar"><div class="xp-fill" style="width: 80%"></div></div>
  </div>
  <div class="level" id="future">
    <h2>🚀 Level 3: Future</h2>
    <p>I'm heading toward a career in cybersecurity—because what’s cooler than being a digital bodyguard? My dream is to become the guy who stops the bad guys with just a terminal window and a smirk.</p>
    <div class="xp-bar"><div class="xp-fill" style="width: 90%"></div></div>
  </div>
</div>
<footer>
  <p>Email: <a href="mailto:ikechukwuperfect759@gmail.com" style="color:#0ff;">ikechukwuperfect759@gmail.com</a></p>
  <div class="social-icons">
    <a href="#"><i class="fab fa-instagram"></i></a>
    <a href="#"><i class="fab fa-x-twitter"></i></a>
    <a href="#"><i class="fab fa-facebook-f"></i></a>
  </div>
  <p style="margin-top: 1rem;">© 2025 Perfect Ikechukwu. All rights reserved.</p>
</footer>
<script>
  function startGame() {
    document.getElementById("startScreen").style.display = "none";
    document.getElementById("gameContainer").style.display = "block";
    const music = document.getElementById("bgMusic");
    if (music) {
      music.play().catch(e => console.log("Autoplay failed:", e));
    }
  }
</script>
</body>
</html>
