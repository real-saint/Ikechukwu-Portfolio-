<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Perfect Ikechukwu - Portfolio</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css" crossorigin="anonymous"/>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&display=swap" rel="stylesheet"/>
  <script src="https://cdn.jsdelivr.net/npm/typed.js@2.0.12"></script>
  <style>
    body {
      font-family: 'Roboto', Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: linear-gradient(135deg, #1a2639 0%, #0d1b2a 100%);
      color: #e6d5b8;
      scroll-behavior: smooth;
      overflow-x: hidden;
      transition: background 0.4s, color 0.4s;
    }.dark-mode {
  background: #fff;
  color: #111;
}

.dark-mode section {
  background: #eee;
  color: #111;
}

.mode-toggle {
  position: fixed;
  top: 1rem;
  right: 1rem;
  background: #f4a261;
  border: none;
  padding: 0.5rem 1rem;
  border-radius: 20px;
  color: #fff;
  font-weight: bold;
  cursor: pointer;
  z-index: 1000;
}

.navbar {
  display: flex;
  justify-content: center;
  background: rgba(13, 27, 42, 0.9);
  padding: 0.5rem 1rem;
  position: sticky;
  top: 0;
  z-index: 10;
}

.navbar a {
  color: #e6d5b8;
  text-decoration: none;
  margin: 0 1rem;
  padding: 0.5rem;
  font-weight: 500;
  transition: color 0.3s;
}

.navbar a:hover {
  color: #f4a261;
}

.profile-pic {
  width: 150px;
  height: 150px;
  object-fit: cover;
  border-radius: 50%;
  margin-top: 1rem;
  border: 4px solid #f4a261;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.6);
  animation: fadeIn 1.5s ease-out;
}

header {
  text-align: center;
  padding: 3rem 2rem;
}

header h1 {
  margin: 0;
  font-size: 2.8rem;
  font-weight: 700;
}

header p, .social-links {
  animation: slideIn 1.2s ease-out;
}

.social-links a {
  color: #e6d5b8;
  font-size: 2rem;
  margin: 0 0.7rem;
  display: inline-block;
  transition: transform 0.3s ease;
}

.social-links a:hover {
  transform: scale(1.2) translateY(-5px);
  color: #f4a261;
}

main {
  max-width: 900px;
  margin: 3rem auto;
  padding: 0 1.5rem;
}

section {
  background-color: #2c3e50;
  padding: 2rem;
  margin-bottom: 2rem;
  border-radius: 12px;
  box-shadow: 0 6px 20px rgba(0, 0, 0, 0.4);
  animation: fadeIn 1s ease-in forwards;
}

section h2 {
  color: #f4a261;
  font-size: 1.8rem;
}

footer {
  text-align: center;
  padding: 1.5rem;
  background-color: #0d1b2a;
  color: #e6d5b8;
}

.cv-button {
  display: inline-block;
  margin-top: 1rem;
  padding: 0.6rem 1.2rem;
  background: #f4a261;
  color: white;
  text-decoration: none;
  border-radius: 8px;
  font-weight: bold;
  transition: background 0.3s;
}

.cv-button:hover {
  background: #e76f51;
}

input, textarea {
  width: 100%;
  padding: 0.7rem;
  margin-bottom: 1rem;
  border-radius: 8px;
  border: 1px solid #ccc;
}

button[type="submit"] {
  background: #f4a261;
  color: #fff;
  border: none;
  padding: 0.7rem 1.2rem;
  border-radius: 8px;
  cursor: pointer;
}

@keyframes fadeIn { 0% { opacity: 0; transform: translateY(20px); } 100% { opacity: 1; transform: translateY(0); } }
@keyframes slideIn { 0% { opacity: 0; transform: translateX(-30px); } 100% { opacity: 1; transform: translateX(0); } }

  </style>
</head>
<body>
  <button class="mode-toggle" onclick="document.body.classList.toggle('dark-mode')">🌓 Toggle Mode</button>  <header>
    <h1><span id="typed"></span></h1>
    <img src="me.jpg" alt="Perfect Ikechukwu" class="profile-pic" />
    <p>Matric Number: 24/208CSC/898</p>
    <p>Email: <a href="mailto:ikechukwuperfect759@gmail.com">ikechukwuperfect759@gmail.com</a></p>
    <div class="social-links">
      <a href="#"><i class="fab fa-instagram"></i></a>
      <a href="#"><i class="fab fa-x-twitter"></i></a>
      <a href="#"><i class="fab fa-facebook-f"></i></a>
    </div>
  </header>  <nav class="navbar">
    <a href="#past">Past</a>
    <a href="#present">Present</a>
    <a href="#future">Future</a>
    <a href="#projects">Projects</a>
    <a href="#contact">Contact</a>
  </nav>  <main>
    <section>
      <h2>Quote of the Day</h2>
      <p id="quoteBox"></p>
    </section><section class="fade-in" id="past">
  <h2>Past: What I Have Done</h2>
  <p>I have developed skills in <strong>web designing</strong>, creating responsive and user-friendly webpages using HTML and CSS.<br><br><em>"I started with &lt;div&gt; confusion and border-radius frustration — now I style like a boss. Every bug was just a misunderstood feature."</em></p>
</section>

<section class="fade-in" id="present">
  <h2>Present: What I Am Doing</h2>
  <p>Currently a <strong>Computer Science student</strong> at the University of Abuja, focusing on coursework and advancing my programming and design skills.<br><br><em>"Some people binge-watch Netflix... I debug code at 2AM and cry in CSS. But hey, learning is progress!"</em></p>
</section>

<section class="fade-in" id="future">
  <h2>Future: What I Plan to Do</h2>
  <p>I aim to pursue a career in <strong>cybersecurity</strong>, specializing in ethical hacking and network security.<br><br><em>"I don't just want to hack the system... I want to ethically scare people into using strong passwords."</em></p>
</section>

<section class="fade-in" id="projects">
  <h2>Projects</h2>
  <ul>
    <li><strong>My First Portfolio Website</strong> – Clean, responsive, and animated.</li>
    <li><strong>Student Login System</strong> – Login/signup system built with HTML/CSS.</li>
    <li><strong>Anime Download App (Concept)</strong> – UI design for anime lovers.</li>
  </ul>
  <a href="Perfect-Ikechukwu-CV.pdf" download class="cv-button">Download My CV</a>
</section>

<section class="fade-in" id="contact">
  <h2>Contact Me</h2>
  <form action="https://formspree.io/f/YOUR_ID" method="POST">
    <input type="email" name="email" placeholder="Your email" required>
    <textarea name="message" placeholder="Your message" rows="4" required></textarea>
    <button type="submit">Send</button>
  </form>
</section>

  </main>  <footer>
    <p>© 2025 Perfect Ikechukwu. All rights reserved.</p>
  </footer>  <script>
    new Typed('#typed', {
      strings: ["Perfect Ikechukwu", "Web Designer", "Future Cybersecurity Expert"],
      typeSpeed: 60,
      backSpeed: 40,
      loop: true
    });

    const quotes = [
      "Success is 99% failure – So keep failing upward.",
      "Don’t wait for opportunity. Create it.",
      "Even syntax errors teach you something.",
      "Discipline is remembering what you want.",
      "Dream big. Debug harder."
    ];
    document.getElementById("quoteBox").innerText = quotes[Math.floor(Math.random() * quotes.length)];
  </script></body>
</html>
