<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Ikechukwu Perfect - Portfolio</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700&display=swap" rel="stylesheet" />
  <style>
    html {
      scroll-behavior: smooth;
    }
    body {
      margin: 0;
      font-family: 'Inter', sans-serif;
      background-color: #f5f5f5;
      color: #333;
    }
    header {
      background-color: #1e293b;
      color: white;
      padding: 2rem 1rem;
      text-align: center;
    }
    header img {
      width: 120px;
      height: 120px;
      border-radius: 50%;
      object-fit: cover;
      border: 3px solid #38bdf8;
      margin-bottom: 1rem;
    }
    nav {
      background-color: #0f172a;
      display: flex;
      justify-content: center;
      gap: 2rem;
      padding: 1rem;
      position: sticky;
      top: 0;
      z-index: 100;
    }
    nav a {
      color: #f8fafc;
      text-decoration: none;
      font-weight: bold;
    }
    nav a:hover {
      color: #60a5fa;
    }
    section {
      max-width: 800px;
      margin: auto;
      padding: 2rem 1rem;
    }
    h2 {
      color: #2563eb;
      margin-top: 2rem;
    }
    p {
      font-size: 1.1rem;
      line-height: 1.6;
    }
    footer {
      background-color: #1e293b;
      color: white;
      text-align: center;
      padding: 1rem;
      margin-top: 3rem;
    }
    .contact {
      background: #e2e8f0;
      padding: 1.5rem;
      border-radius: 10px;
      margin-top: 2rem;
    }
    .contact h3 {
      color: #1e293b;
    }
    .contact p {
      font-size: 1rem;
      color: #334155;
    }
  </style>
</head>
<body>

  <header>
    <!-- 👇 Replace this link with your own image URL if you have one -->
    <img src="https://i.imgur.com/8Km9tLL.jpg" alt="Profile Photo" />
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
    <h3>📬 Contact</h3>
    <p>Email: <a href="mailto:youremail@example.com">ikechukwuperfect759@gmail.com</a></p>
    <p>GitHub: <a href="https://github.com/real-saint" target="_blank">github.com/real-saint</a></p>
  </section>

  <footer>
    <p>Submitted by Ikechukwu Perfect | 24/208CSC/898</p>
  </footer>

</body>
</html>
