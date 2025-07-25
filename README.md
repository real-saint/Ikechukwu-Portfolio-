<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Ikechukwu Perfect - Portfolio</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700&display=swap" rel="stylesheet" />
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    html {
      scroll-behavior: smooth;
    }
    body {
      font-family: 'Inter', sans-serif;
      background: linear-gradient(to bottom, #aee2ff, #e0f7ff);
      color: #1e293b;
      overflow-x: hidden;
    }
    .background-diamonds {
      position: fixed;
      width: 100%;
      height: 100%;
      top: 0;
      left: 0;
      overflow: hidden;
      z-index: -1;
    }
    .diamond {
      position: absolute;
      width: 10px;
      height: 10px;
      background: rgba(255, 255, 255, 0.6);
      transform: rotate(45deg);
      animation: float 10s linear infinite;
    }
    @keyframes float {
      from { transform: translateY(100vh) rotate(45deg); }
      to { transform: translateY(-10vh) rotate(45deg); }
    }
    header {
      text-align: center;
      padding: 2rem 1rem;
    }
    header img {
      width: 150px;
      height: 150px;
      border-radius: 50%;
      object-fit: cover;
      border: 4px solid #2563eb;
      margin-bottom: 1rem;
    }
    h1 {
      font-size: 2rem;
      font-weight: 700;
    }
    p {
      font-size: 1rem;
      margin-bottom: 1rem;
    }
    nav {
      display: flex;
      justify-content: center;
      gap: 2rem;
      background-color: rgba(255, 255, 255, 0.6);
      padding: 1rem;
      position: sticky;
      top: 0;
      z-index: 10;
    }
    nav a {
      color: #1e293b;
      text-decoration: none;
      font-weight: bold;
    }
    nav a:hover {
      color: #2563eb;
    }
    section {
      max-width: 800px;
      margin: auto;
      padding: 2rem 1rem;
    }
    h2 {
      font-size: 1.5rem;
      color: #2563eb;
      margin-bottom: 0.5rem;
    }
    footer {
      text-align: center;
      background-color: #2563eb;
      color: white;
      padding: 1rem;
      margin-top: 3rem;
    }
    .contact {
      background-color: #e2e8f0;
      padding: 1.5rem;
      border-radius: 10px;
      margin-top: 2rem;
    }
  </style>
</head>
<body>

  <div class="background-diamonds">
    <!-- 20 floating diamonds -->
    <div class="diamond" style="left: 5%; animation-delay: 1s;"></div>
    <div class="diamond" style="left: 10%; animation-delay: 2s;"></div>
    <div class="diamond" style="left: 15%; animation-delay: 3s;"></div>
    <div class="diamond" style="left: 20%; animation-delay: 4s;"></div>
    <div class="diamond" style="left: 25%; animation-delay: 5s;"></div>
    <div class="diamond" style="left: 30%; animation-delay: 6s;"></div>
    <div class="diamond" style="left: 35%; animation-delay: 7s;"></div>
    <div class="diamond" style="left: 40%; animation-delay: 8s;"></div>
    <div class="diamond" style="left: 45%; animation-delay: 9s;"></div>
    <div class="diamond" style="left: 50%; animation-delay: 10s;"></div>
    <div class="diamond" style="left: 55%; animation-delay: 11s;"></div>
    <div class="diamond" style="left: 60%; animation-delay: 12s;"></div>
    <div class="diamond" style="left: 65%; animation-delay: 13s;"></div>
    <div class="diamond" style="left: 70%; animation-delay: 14s;"></div>
    <div class="diamond" style="left: 75%; animation-delay: 15s;"></div>
    <div class="diamond" style="left: 80%; animation-delay: 16s;"></div>
    <div class="diamond" style="left: 85%; animation-delay: 17s;"></div>
    <div class="diamond" style="left: 90%; animation-delay: 18s;"></div>
    <div class="diamond" style="left: 95%; animation-delay: 19s;"></div>
    <div class="diamond" style="left: 100%; animation-delay: 20s;"></div>
  </div>

  <header>
    <img src="https://upload.wikimedia.org/wikipedia/commons/1/18/Bald_Eagle_Portrait.jpg" alt="Eagle Image" />
    <h1>Ikechukwu Perfect</h1>
    <p>Matric Number: 24/208CSC/898</p>
  </header>

  <nav>
    <a href="#past">Past</a>
    <a href="#present">Present</a>
    <a href="#future">Future</a>
    <a href="#contact">Contact</a>
  </nav>

  <section id="past">
    <h2>🔙 Past</h2>
    <p>I learned web designing and began building simple websites. This gave me a solid foundation in front-end technologies like HTML and CSS.</p>
  </section>

  <section id="present">
    <h2>📍 Present</h2>
    <p>I'm currently a Computer Science student at the University of Abuja. I'm actively learning graphic design and exploring different areas of technology to broaden my skills.</p>
  </section>

  <section id="future">
    <h2>🔜 Future</h2>
    <p>I plan to deepen my knowledge in the field of cybersecurity. My goal is to become a cybersecurity professional, helping protect digital systems and information.</p>
  </section>

  <section id="contact" class="contact">
    <h2>📬 Contact</h2>
    <p>Email: <a href="mailto:ikechukwuperfect759@gmail.com">youremail@example.com</a></p>
    <p>GitHub: <a href="https://github.com/real-saint" target="_blank">github.com/real-saint</a></p>
  </section>

  <footer>
    <p>Submitted by Ikechukwu Perfect | 24/208CSC/898</p>
  </footer>

</body>
</html>
