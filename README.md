
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Perfect Ikechukwu - Portfolio</title>
  <!-- Font Awesome for social icons -->
  <link
    rel="stylesheet"
    href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css"
    crossorigin="anonymous"
    referrerpolicy="no-referrer"
  />
  <style>
    html {
      scroll-behavior: smooth;
    }

    body {
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
      color: white;
      background: dark blue;
      background-image: url('https://cdn.pixabay.com/photo/2022/01/10/11/12/technology-6928592_1280.jpg');
      background-repeat: no-repeat;
      background-size: cover;
      background-position: center center;
      background-attachment: fixed;
      overflow-x: hidden;
      position: relative;
    }

    /* Floating black animations */
    .floating-bg span {
      position: absolute;
      display: block;
      width: 20px;
      height: 20px;
      background: rgba(255, 255, 255, 0.2);
      border-radius: 50%;
      animation: floatUp 15s linear infinite;
      bottom: -50px;
    }

    .floating-bg span:nth-child(1) { left: 10%; width: 15px; height: 15px; }
    .floating-bg span:nth-child(2) { left: 20%; }
    .floating-bg span:nth-child(3) { left: 35%; width: 25px; height: 25px; }
    .floating-bg span:nth-child(4) { left: 50%; }
    .floating-bg span:nth-child(5) { left: 65%; width: 10px; height: 10px; }
    .floating-bg span:nth-child(6) { left: 80%; width: 30px; height: 30px; }

    @keyframes floatUp {
      0% { transform: translateY(0) scale(1); opacity: 0.6; }
      50% { transform: translateY(-300px) scale(1.2); opacity: 0.3; }
      100% { transform: translateY(-1000px) scale(0.8); opacity: 0; }
    }

    .floating-bg {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 200%;
      z-index: 1;
      pointer-events: none;
    }

    header {
      background-color: rgba(0, 0, 0, 0.85);
      padding: 2rem 1rem 1rem;
      text-align: center;
      border-bottom: 2px solid #00bfff;
      position: relative;
      z-index: 2;
    }

    header h1 {
      font-size: 1.8rem;
      margin-bottom: 0.5rem;
    }

    .intro {
      font-size: 1rem;
      margin-top: 0.5rem;
    }

    nav {
      margin-top: 1rem;
    }

    nav a {
      color: #00bfff;
      text-decoration: none;
      margin: 0 15px;
      font-weight: bold;
      transition: color 0.3s;
    }

    nav a:hover {
      color: white;
    }

    section {
      max-width: 800px;
      margin: 2rem auto;
      padding: 2rem;
      background: rgba(0, 0, 0, 0.8);
      border-radius: 10px;
      box-shadow: 0 0 15px rgba(0,0,0,0.6);
      position: relative;
      z-index: 2;
    }

    h2 {
      color: #00bfff;
    }

    p {
      color: #e0f7ff;
    }

    .about-me {
      text-align: center;
      font-size: 1.2rem;
      line-height: 1.6;
      padding: 1rem 2rem;
    }

    footer {
      text-align: center;
      padding: 1rem;
      background: rgba(0, 0, 0, 0.9);
      color: #ccc;
      margin-top: 2rem;
      position: relative;
      z-index: 2;
    }

    .contact {
      margin-top: 1rem;
    }

    .social-icons {
      margin-top: 1rem;
    }

    .social-icons a {
      color: #00bfff;
      text-decoration: none;
      margin: 0 10px;
      font-size: 1.5rem;
      transition: transform 0.3s, color 0.3s;
    }

    .social-icons a:hover {
      color: #ffffff;
      transform: scale(1.2);
    }
  </style>
</head>
<body>

  <!-- Floating animation -->
  <div class="floating-bg">
    <span></span><span></span><span></span><span></span><span></span><span></span>
  </div>

  <!-- Header -->
  <header>
    <h1>Perfect Ikechukwu</h1>
    <p class="intro">Matric Number: 24/208CSC/898</p>
    <p class="intro">My Portfolio – Past • Present • Future</p>

    <!-- Navigation -->
    <nav>
      <a href="#about">About</a>
      <a href="#past">Past</a>
      <a href="#present">Present</a>
      <a href="#future">Future</a>
    </nav>
  </header>

  <!-- About Me -->
  <section id="about" class="about-me">
    <h2>About Me</h2>
    <p>Hi, I'm <strong>Perfect Ikechukwu</strong> — a creative mind passionate about tech, growth, and solving real-world problems.<br>
    I design, build, and protect in the digital world. <br>
    Watch this space — the <strong>future is loading...</strong></p>
  </section>

  <!-- Past -->
  <section id="past">
    <h2>Past</h2>
    <p>I learned web designing, which gave me the foundation to create beautiful and functional websites like this one.</p>
  </section>

  <!-- Present -->
  <section id="present">
    <h2>Present</h2>
    <p>I'm currently a Computer Science student at the University of Abuja, actively building my skills in technology and problem-solving.</p>
  </section>

  <!-- Future -->
  <section id="future">
    <h2>Future</h2>
    <p>I plan to pursue a career in Cybersecurity to protect systems, data, and people from digital threats.</p>
  </section>

  <!-- Footer -->
  <footer>
    <div class="contact">
      <p>Contact: ikechukwuperfect759@gmail.com</p>
    </div>
    <div class="social-icons">
      <a href="mailto:ikechukwuperfect759@gmail.com" title="Email"><i class="fas fa-envelope"></i></a>
      <a href="https://github.com/real-saint" title="GitHub"><i class="fab fa-github"></i></a>
      <a href="https://linkedin.com" title="LinkedIn"><i class="fab fa-linkedin"></i></a>
      <a href="https://instagram.com" title="Instagram"><i class="fab fa-instagram"></i></a>
    </div>
    <p>&copy; 2025 Perfect Ikechukwu. All rights reserved.</p>
  </footer>

</body>
</html>
