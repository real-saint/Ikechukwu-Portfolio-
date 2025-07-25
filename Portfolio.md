<!DOCTYPE html><html lang="en">
<link rel="icon" href="https://cdn-icons-png.flaticon.com/512/3064/3064197.png" type="image/png">
<meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Perfect's Cyber World</title>
  <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }
    body {
      font-family: 'Inter', sans-serif;
      background-color: #000;
      color: #e2e8f0;
      display: flex;
      min-height: 100vh;
      overflow-x: hidden;
      animation: fadeInBody 1s ease-in;
    }@keyframes fadeInBody {
  0% { opacity: 0; }
  100% { opacity: 1; }
}

nav {
  position: fixed;
  top: 0;
  left: 0;
  width: 240px;
  height: 100vh;
  background-color: #1e293b;
  padding: 2rem 1.5rem;
  display: flex;
  flex-direction: column;
  box-shadow: 2px 0 10px rgba(0, 0, 0, 0.4);
  animation: slideInNav 1.2s ease forwards;
}

@keyframes slideInNav {
  0% { transform: translateX(-100%); }
  100% { transform: translateX(0); }
}

nav a {
  color: #cbd5e1;
  text-decoration: none;
  margin: 1rem 0;
  font-size: 1rem;
  transition: all 0.3s;
}
nav a:hover {
  color: #38bdf8;
  padding-left: 5px;
}

main {
  margin-left: 240px;
  padding: 3rem 2rem;
  flex: 1;
  animation: slideInMain 1.2s ease forwards;
}

@keyframes slideInMain {
  0% { transform: translateY(20px); opacity: 0; }
  100% { transform: translateY(0); opacity: 1; }
}

section {
  margin-bottom: 4rem;
  padding: 2rem;
  background-color: #000;
  color: #e2e8f0;
  border-radius: 12px;
  box-shadow: 0 4px 25px rgba(0,0,0,0.2);
  transition: transform 0.3s;
  animation: fadeUp 1s ease-in-out;
}

section:hover {
  transform: translateY(-5px);
}

@keyframes fadeUp {
  0% { opacity: 0; transform: translateY(40px); }
  100% { opacity: 1; transform: translateY(0); }
}

section h2 {
  font-size: 1.4rem;
  margin-bottom: 1rem;
  font-weight: 600;
}

#past h2, #present h2, #future h2 {
  color: #22c55e;
}

footer {
  margin-left: 240px;
  padding: 2rem;
  text-align: center;
  background-color: #1e293b;
  color: #94a3b8;
  animation: fadeInFooter 1.5s ease;
}

@keyframes fadeInFooter {
  0% { opacity: 0; }
  100% { opacity: 1; }
}

.social-icons a {
  color: #38bdf8;
  font-size: 1.3rem;
  margin: 0 0.5rem;
  text-decoration: none;
}

.email a {
  color: #38bdf8;
  text-decoration: none;
}

@media (max-width: 768px) {
  nav {
    width: 100%;
    height: auto;
    flex-direction: row;
    justify-content: space-around;
    align-items: center;
    position: static;
  }
  main, footer {
    margin-left: 0;
    padding: 2rem 1rem;
  }
  section {
    margin: 2rem 0;
  }
}

  </style>
</head>
<body>
  <nav>
    <a href="#about">About</a>
    <a href="#past">Past</a>
    <a href="#present">Present</a>
    <a href="#future">Future</a>
    <a href="#contact">Contact</a>
  </nav>
  <main>
    <section id="about">
      <h2>About Me</h2>
      <p>Hello! I'm Perfect Ikechukwu, a passionate Computer Science student from the University of Abuja. My journey in technology began with curiosity and evolved into a commitment to mastering web design and cybersecurity. I enjoy building websites that not only look good but also function effectively. From basic HTML pages to responsive layouts and backend integrations — I love the process.</p>
      <p><strong>Matric Number:</strong> 24/208CSC/898</p>
    </section>
    <section id="past">
      <h2>Past</h2>
      <p>I started by learning HTML and CSS to create simple web pages. Over time, I expanded my skill set to include JavaScript, Python, and version control using Git. The early projects weren’t perfect — but they taught me how to solve real-world problems using code.</p>
    </section>
    <section id="present">
      <h2>Present</h2>
      <p>Currently, I’m balancing coursework and personal projects. I’m improving my understanding of frontend and backend frameworks, building tools, and exploring how cybersecurity plays a role in every digital product. I’m also studying systems, networks, and ethical hacking in preparation for my future goals.</p>
    </section>
    <section id="future">
      <h2>Future</h2>
      <p>I see myself advancing into the cybersecurity field — protecting systems, securing data, and ensuring trust in digital platforms. I aim to earn industry certifications and contribute to a world where privacy and digital integrity are prioritized.</p>
    </section>
    <section id="contact">
      <h2>Contact</h2>
      <p class="email">Email: <a href="mailto:ikechukwuperfect759@gmail.com">ikechukwuperfect759@gmail.com</a></p>
      <div class="social-icons">
        <a href="#"><i class="fab fa-instagram"></i></a>
        <a href="#"><i class="fab fa-x-twitter"></i></a>
        <a href="#"><i class="fab fa-facebook-f"></i></a>
      </div>
    </section>
  </main>
  <footer>
    <p>© 2025 Perfect Ikechukwu. All rights reserved.</p>
  </footer>
</body>
</html>
