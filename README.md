
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Perfect Ikechukwu - Portfolio</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css" crossorigin="anonymous"/>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&display=swap" rel="stylesheet"/>
  <style>
    body {
      font-family: 'Roboto', Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: linear-gradient(135deg, #1a2639 0%, #0d1b2a 100%);
      color: #e6d5b8;
      scroll-behavior: smooth;
      overflow-x: hidden;
    }

    #particleCanvas {
      position: fixed;
      top: 0;
      left: 0;
      z-index: -1;
      width: 100vw;
      height: 100vh;
      pointer-events: none;
      background: transparent;
    }

    .background-anim {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: linear-gradient(135deg, rgba(26, 38, 57, 0.8) 0%, rgba(13, 27, 42, 0.8) 100%);
      z-index: -2;
    }

    header {
      background-color: #0d1b2a;
      color: #e6d5b8;
      text-align: center;
      padding: 3rem 2rem;
    }

    header h1 {
      margin: 0;
      font-size: 2.8rem;
      font-weight: 700;
      opacity: 0;
      animation: fadeInWave 2s ease-out forwards, waveText 3s infinite ease-in-out;
    }

    header p {
      margin: 0.5rem 0;
      font-size: 1.2rem;
      font-weight: 300;
      animation: slideIn 1.2s ease-out;
    }

    header a {
      color: #f4a261;
      text-decoration: none;
      transition: color 0.3s ease;
    }

    header a:hover {
      color: #e6d5b8;
    }

    .social-links {
      margin-top: 2rem;
      animation: slideIn 1.4s ease-out;
    }

    .social-links a {
      color: #e6d5b8;
      font-size: 2rem;
      margin: 0 0.7rem;
      display: inline-block;
      transition: transform 0.3s ease;
    }

    .social-links a:nth-child(1) { animation: float 2.5s ease-in-out infinite; }
    .social-links a:nth-child(2) { animation: float 2.5s ease-in-out infinite 0.3s; }
    .social-links a:nth-child(3) { animation: float 2.5s ease-in-out infinite 0.6s; }

    .social-links a:hover {
      transform: scale(1.2) translateY(-5px);
      color: #2c3e50;
    }

    main {
      max-width: 900px;
      margin: 3rem auto;
      padding: 0 1.5rem;
      position: relative;
      z-index: 1;
    }

    section {
      background-color: #2c3e50;
      padding: 2rem;
      margin-bottom: 2rem;
      border-radius: 12px;
      border: 2px solid #0d1b2a;
      box-shadow: 0 6px 20px rgba(0, 0, 0, 0.4);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      animation: fadeIn 1s ease-in forwards;
    }

    section:hover {
      transform: translateY(-10px);
      box-shadow: 0 10px 25px rgba(0, 0, 0, 0.5);
    }

    section h2 {
      color: #f4a261;
      font-size: 1.8rem;
      margin-top: 0;
      font-weight: 700;
    }

    .fade-in { opacity: 0; }
    .fade-in:nth-child(1) { animation-delay: 0.4s; }
    .fade-in:nth-child(2) { animation-delay: 0.8s; }
    .fade-in:nth-child(3) { animation-delay: 1.2s; }

    footer {
      text-align: center;
      padding: 1.5rem;
      background-color: #0d1b2a;
      color: #e6d5b8;
      position: fixed;
      bottom: 0;
      width: 100%;
      animation: slideUp 1s ease-out;
      z-index: 1;
    }

    @keyframes float {
      0% { transform: translateY(0); }
      50% { transform: translateY(-8px); }
      100% { transform: translateY(0); }
    }

    @keyframes fadeIn {
      0% { opacity: 0; transform: translateY(20px); }
      100% { opacity: 1; transform: translateY(0); }
    }

    @keyframes slideIn {
      0% { opacity: 0; transform: translateX(-30px); }
      100% { opacity: 1; transform: translateX(0); }
    }

    @keyframes slideUp {
      0% { opacity: 0; transform: translateY(30px); }
      100% { opacity: 1; transform: translateY(0); }
    }

    @keyframes fadeInWave {
      0% { opacity: 0; }
      100% { opacity: 1; }
    }

    @keyframes waveText {
      0% { transform: translateY(0); }
      50% { transform: translateY(-5px); }
      100% { transform: translateY(0); }
    }

    @media (max-width: 600px) {
      header h1 { font-size: 2.2rem; }
      section { padding: 1.5rem; }
      .social-links a { font-size: 1.7rem; margin: 0 0.5rem; }
    }
  </style>
</head>
<body>
  <canvas id="particleCanvas"></canvas>
  <div class="background-anim"></div>

  <header>
    <h1 class="typing-effect">Perfect Ikechukwu</h1>
    <p>Matric Number: 24/208CSC/898</p>
    <p>Email: <a href="mailto:ikechukwuperfect759@gmail.com">ikechukwuperfect759@gmail.com</a></p>
    <div class="social-links">
      <a href="https://instagram.com/yourusername" target="_blank"><i class="fab fa-instagram"></i></a>
      <a href="https://x.com/yourusername" target="_blank"><i class="fab fa-x-twitter"></i></a>
      <a href="https://facebook.com/yourusername" target="_blank"><i class="fab fa-facebook-f"></i></a>
    </div>
  </header>

  <main>
    <section class="fade-in" id="past">
      <h2>Past: What I Have Done</h2>
      <p>
        I have developed skills in <strong>web designing</strong>, creating responsive and user-friendly webpages using HTML and CSS.
        <br><br>
        <em>"I started with <strong>&lt;div&gt; confusion</strong> and <strong>border-radius frustration</strong> — now I style like a boss. Every bug was just a misunderstood feature."</em>
      </p>
    </section>

    <section class="fade-in" id="present">
      <h2>Present: What I Am Doing</h2>
      <p>
        Currently a <strong>Computer Science student</strong> at the University of Abuja, focusing on coursework and advancing my programming and design skills.
        <br><br>
        <em>"Some people binge-watch Netflix... I debug code at 2AM and cry in CSS. But hey, learning is progress!"</em>
      </p>
    </section>

    <section class="fade-in" id="future">
      <h2>Future: What I Plan to Do</h2>
      <p>
        I aim to pursue a career in <strong>cybersecurity</strong>, specializing in areas like ethical hacking and network security.
        <br><br>
        <em>"I don't just want to hack the system... I want to ethically scare people into using strong passwords. Future me wears a hoodie, types fast, and saves the world one firewall at a time."</em>
      </p>
    </section>
  </main>

  <footer>
    <p>© 2025 Perfect Ikechukwu. All rights reserved.</p>
  </footer>

  <script>
    const canvas = document.getElementById("particleCanvas");
    const ctx = canvas.getContext("2d");
    let particles = [];

    function resizeCanvas() {
      canvas.width = window.innerWidth;
      canvas.height = window.innerHeight;
    }

    window.addEventListener("resize", resizeCanvas);
    resizeCanvas();

    function createParticle(x = Math.random() * canvas.width, y = Math.random() * canvas.height) {
      return {
        x: x,
        y: y,
        size: Math.random() * 2 + 1,
        speedX: (Math.random() - 0.5) * 0.5,
        speedY: (Math.random() - 0.5) * 0.5,
        opacity: Math.random() * 0.5 + 0.3
      };
    }

    for (let i = 0; i < 100; i++) {
      particles.push(createParticle());
    }

    function drawParticles() {
      ctx.clearRect(0, 0, canvas.width, canvas.height);
      particles.forEach(p => {
        ctx.save();
        ctx.translate(p.x, p.y);
        ctx.rotate(Math.PI / 4);
        ctx.fillStyle = `rgba(255, 255, 255, ${p.opacity})`;
        ctx.beginPath();
        ctx.moveTo(0, -p.size);
        ctx.lineTo(p.size, 0);
        ctx.lineTo(0, p.size);
        ctx.lineTo(-p.size, 0);
        ctx.closePath();
        ctx.fill();
        ctx.restore();

        p.x += p.speedX;
        p.y += p.speedY;

        if (p.x < -10 || p.x > canvas.width + 10 || p.y < -10 || p.y > canvas.height + 10) {
          Object.assign(p, createParticle());
        }
      });
      requestAnimationFrame(drawParticles);
    }

    canvas.addEventListener("click", (e) => {
      const rect = canvas.getBoundingClientRect();
      for (let i = 0; i < 5; i++) {
        particles.push(createParticle(e.clientX - rect.left, e.clientY - rect.top));
      }
    });

    canvas.addEventListener("touchstart", (e) => {
      const touch = e.touches[0];
      const rect = canvas.getBoundingClientRect();
      for (let i = 0; i < 5; i++) {
        particles.push(createParticle(touch.clientX - rect.left, touch.clientY - rect.top));
      }
    });

    drawParticles();
  </script>
</body>
</html>
