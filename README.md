<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Perfect Ikechukwu - Portfolio</title>
  <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&display=swap" rel="stylesheet">
  <style>
    * { box-sizing: border-box; margin: 0; padding: 0; }
    body {
      font-family: 'Roboto', sans-serif;
      background-color: #0d1b2a;
      color: #fff;
      display: flex;
    }
    nav {
      position: fixed;
      left: 0;
      top: 0;
      width: 220px;
      height: 100vh;
      background-color: #1a2639;
      padding: 2rem 1rem;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      box-shadow: 2px 0 10px rgba(0, 0, 0, 0.3);
    }
    nav h1 {
      font-size: 1.2rem;
      color: #0ff;
      margin-bottom: 2rem;
    }
    nav a {
      color: #fff;
      text-decoration: none;
      margin: 1rem 0;
      font-weight: 400;
      transition: color 0.3s;
    }
    nav a:hover {
      color: #0ff;
    }
    main {
      margin-left: 220px;
      padding: 3rem 2rem;
      flex: 1;
    }
    section {
      margin-bottom: 4rem;
      padding: 2rem;
      background-color: #fff;
      color: #000;
      border-radius: 12px;
      box-shadow: 0 0 20px rgba(0,0,0,0.2);
      transition: transform 0.3s;
    }
    section:hover {
      transform: translateY(-5px);
    }
    section h2 {
      color: #0d1b2a;
      margin-bottom: 1rem;
    }
    footer {
      margin-left: 220px;
      padding: 2rem;
      text-align: center;
      color: #0ff;
      background-color: #1a2639;
    }
    .social-icons a {
      color: #0ff;
      font-size: 1.5rem;
      margin: 0 0.5rem;
      text-decoration: none;
    }
    @media (max-width: 768px) {
      nav {
        width: 100%;
        height: auto;
        position: relative;
        flex-direction: row;
        justify-content: space-around;
      }
      main, footer {
        margin-left: 0;
      }
      section {
        margin: 2rem 0;
      }
    }
  </style>
</head>
<body>
  <nav>
    <h1>🚀 Perfect Ikechukwu</h1>
    <a href="#about">About Me</a>
    <a href="#past">Past</a>
    <a href="#present">Present</a>
    <a href="#future">Future</a>
    <a href="#contact">Contact</a>
  </nav>
  <main>
    <section id="about">
      <h2>About Me</h2>
      <p>Hi, I'm Perfect Ikechukwu, a Computer Science student at the University of Abuja. I'm deeply passionate about technology, especially web design and cybersecurity. I've built responsive websites and sharpened my skills in both frontend and backend development.</p>
    </section>
    <section id="past">
      <h2>Past</h2>
      <p>Started with the basics — HTML, CSS, and JavaScript. I spent time mastering the foundations of web development and gradually began building personal projects. Every error was a lesson in disguise.</p>
    </section>
    <section id="present">
      <h2>Present</h2>
      <p>Currently studying Computer Science while actively working on small-scale projects. I’m improving my coding skills and diving deeper into programming, databases, and security protocols. I also enjoy working on visual interfaces.</p>
    </section>
    <section id="future">
      <h2>Future</h2>
      <p>My ambition is to become a cybersecurity expert. I plan to further explore ethical hacking, penetration testing, and network defense. I’m driven to protect systems and data from digital threats.</p>
    </section>
    <section id="contact">
      <h2>Contact</h2>
      <p>Email: <a href="mailto:ikechukwuperfect759@gmail.com">ikechukwuperfect759@gmail.com</a></p>
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
