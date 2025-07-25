
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Portfolio Quest</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css" crossorigin="anonymous" />
  <link href="https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap" rel="stylesheet">
  <style>
    * { box-sizing: border-box; margin: 0; padding: 0; }
    body {
      font-family: 'Press Start 2P', monospace;
      background: linear-gradient(135deg, #0d1b2a, #1a2639);
      background-size: 400% 400%;
      animation: gradientShift 30s ease infinite;
      color: #fff;
      overflow-x: hidden;
      position: relative;
    }
    @keyframes gradientShift {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    .lightning { position: fixed; top: 0; left: 0; width: 100vw; height: 100vh; pointer-events: none; z-index: -1; }
    .flash {
      animation: flashEffect 8s infinite;
      background: white;
      position: absolute;
      width: 100%;
      height: 100%;
      opacity: 0;
      z-index: -1;
    }
    @keyframes flashEffect {
      0%, 97%, 100% { opacity: 0; }
      98% { opacity: 0.8; }
      99% { opacity: 0.2; }
    }

    .background-layer {
      position: fixed;
      top: 0;
      left: 0;
      width: 100vw;
      height: 100vh;
      z-index: -2;
      background-image: url('https://www.transparenttextures.com/patterns/cubes.png');
      opacity: 0.03;
      animation: floatPattern 20s linear infinite;
    }
    @keyframes floatPattern {
      0% { transform: translateY(0); }
      100% { transform: translateY(-50px); }
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
    .start-screen h1 { font-size: 1.5rem; margin-bottom: 2rem; }
    .start-button {
      background: #0ff; color: #000;
      padding: 1rem 2rem;
      border: none;
      font-size: 1rem;
      cursor: pointer;
      border-radius: 8px;
      transition: transform 0.2s;
    }
    .start-button:hover { transform: scale(1.1); }

    .game-container {
      display: none;
      padding: 2rem;
      max-width: 1000px;
      margin: auto;
    }

    .level, .side-quest {
      background: #fff;
      color: #000;
      padding: 2rem;
      border-radius: 10px;
      margin-bottom: 2rem;
      position: relative;
      box-shadow: 0 0 15px #0ff;
      animation: fadeSlide 1s ease forwards;
    }
    .level h2, .side-quest h2 {
      color: #0d1b2a;
      margin-bottom: 1rem;
    }
    @keyframes fadeSlide {
      0% { opacity: 0; transform: translateY(40px); }
      100% { opacity: 1; transform: translateY(0); }
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

    .avatar {
      display: block;
      margin: 2rem auto;
      max-width: 120px;
      border-radius: 50%;
      border: 3px solid #0ff;
      box-shadow: 0 0 15px rgba(0, 255, 255, 0.5);
    }

    .terminal {
      background: #000;
      color: #0f0;
      font-family: monospace;
      padding: 1rem;
      margin-top: 1rem;
      border-radius: 8px;
      box-shadow: 0 0 10px #0f0;
    }

    .badge {
      display: inline-block;
      background: #0ff;
      color: #000;
      padding: 0.4rem 1rem;
      margin: 0.3rem;
      border-radius: 20px;
      font-size: 0.8rem;
      font-weight: bold;
      box-shadow: 0 0 5px #0ff;
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
  </style>
</head>
<body>
<div class="background-layer"></div>
<div class="lightning"><div class="flash"></div></div>
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

  <div class="side-quest">
    <h2>🎯 Side Quests</h2>
    <ul>
      <li>🔐 Took free courses on cybersecurity basics and ethical hacking</li>
      <li>📜 Certified in Responsive Web Design</li>
      <li>🎨 Designed and deployed personal web projects</li>
      <li>🎧 Sometimes codes to lo-fi beats or rain sounds</li>
    </ul>
  </div>

  <div class="side-quest">
    <h2>💻 Terminal Simulation</h2>
    <div class="terminal">
      >_ npm install my-skills<br />
      Installing...<br />
      ✔ HTML, CSS, JavaScript<br />
      ✔ Git & GitHub<br />
      ✔ Python, Node.js<br />
      ✔ Cybersecurity<br />
      ✔ Deployment Complete 🎉
    </div>
  </div>

  <div class="side-quest">
    <h2>🏆 Badges & Achievements</h2>
    <span class="badge">Web Dev Master</span>
    <span class="badge">Cybersecurity Explorer</span>
    <span class="badge">Frontend Ninja</span>
    <span class="badge">Debugging Pro</span>
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
    if (music) music.play().catch(e => console.log("Autoplay failed:", e));
  }
</script>
</body>
</html>
