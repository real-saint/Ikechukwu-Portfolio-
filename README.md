
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Perfect Ikechukwu - Portfolio</title>
  <!-- Font Awesome for icons -->
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
      background: black;
      background-size: 400% 400%;
      animation: gradientShift 15s ease infinite;
      overflow-x: hidden;
      position: relative;
    }

    @keyframes gradientShift {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    /* Floating white bubbles */
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

    .floating-bg span:nth-child(1) { left: 10%; animation-delay: 0s; width: 15px; height: 15px; }
    .floating-bg span:nth-child(2) { left: 20%; animation-delay: 2s; }
    .floating-bg span:nth-child(3) { left: 35%; animation-delay: 4s; width: 25px; height: 25px; }
    .floating-bg span:nth-child(4) { left: 50%; animation-delay: 6s; }
    .floating-bg span:nth-child(5) { left: 65%; animation-delay: 8s; width: 10px; height: 10px; }
    .floating-bg span:nth-child(6) { left: 80%; animation-delay: 10s; width: 30px; height: 30px; }

    @keyframes floatUp {
      0% { transform: translateY(0) scale(1); opacity: 0.6; }
      50% { transform: translateY(-300px) scale(1.2); opacity: 0.3; }
      100% { transform: translateY(-600px) scale(0.8); opacity: 0; }
    }

    .floating-bg {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      z-index: 1;
      pointer-events: none;
    }

    header {
      background-color: rgba(0, 0, 0, 0.95);
      padding: 2rem 1rem 1rem;
      text-align: center;
      border-bottom: 2px solid #00bfff;
      position: relative;
      z-index: 2;
    }

    header h1 {
      font-size: 1.8rem; /* Reduced font size */
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
      background: rgba(0, 0, 0, 0.85);
      border-radius: 10px;
      box-shadow: 0 0 15px rgba(0,0,0,0.5);
      position: relative;
      z-index: 2;
    }

    h2 {
      color: #00bfff;
    }

    p {
      color: #e0f7ff;
    }

    footer {
      text-align: center;
      padding: 1rem;
      background: rgba(0, 0, 0, 0.95);
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

  <!-- Floating background animation -->
  <div class="floating-bg">
    <span></span><span></span><span></span><span></span><span></span><span></span>
  </div>

  <!-- Header -->
  <header>
    <h1>Perfect Ikechukwu</h1>
    <p class="intro">Matric Number: 24/208CSC/898</p>
    <p class="intro">My Portfolio – Past • Present • Future</p>

    <!-- Navigation links -->
    <nav>
      <a href="#past">Past</a>
      <a href="#present">Present</a>
      <a href="#future">Future</a>
    </nav>
  </header>

  <!-- Sections -->
  <section id="past">
    <h2>Past</h2>
    <p>I learned web designing, which gave me the foundation to create beautiful and functional websites like this one.</p>
  </section>

  <section id="present">
    <h2>Present</h2>
    <p>I'm currently a Computer Science student at the University of Abuja, actively building my skills in technology and problem-solving.</p>
  </section>

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
