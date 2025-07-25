
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
    /* Background Animation */
    body {
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
      color: white;
      background: linear-gradient(-45deg, #001f3f, #003366, #004080, #001f3f);
      background-size: 400% 400%;
      animation: gradientShift 15s ease infinite;
    }

    @keyframes gradientShift {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    header {
      background-color: rgba(0, 0, 51, 0.9);
      color: white;
      padding: 2rem;
      text-align: center;
      border-bottom: 4px solid #00bfff;
    }

    .intro {
      font-size: 1.2rem;
      margin-top: 0.5rem;
    }

    section {
      max-width: 800px;
      margin: 2rem auto;
      padding: 2rem;
      background: rgba(0, 51, 102, 0.8);
      border-radius: 10px;
      box-shadow: 0 0 15px rgba(0,0,0,0.3);
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
      background: rgba(0, 38, 77, 0.9);
      color: #ccc;
      margin-top: 2rem;
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

  <header>
    <h1>Perfect Ikechukwu</h1>
    <p class="intro">Matric Number: 24/208CSC/898</p>
    <p class="intro">My Portfolio – Past • Present • Future</p>
  </header>

  <section>
    <h2>Past</h2>
    <p>I learned web designing, which gave me the foundation to create beautiful and functional websites like this one.</p>
  </section>

  <section>
    <h2>Present</h2>
    <p>I'm currently a Computer Science student at the University of Abuja, actively building my skills in technology and problem-solving.</p>
  </section>

  <section>
    <h2>Future</h2>
    <p>I plan to pursue a career in Cybersecurity to protect systems, data, and people from digital threats.</p>
  </section>

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
