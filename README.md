<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Perfect Ikechukwu - Portfolio</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css" crossorigin="anonymous"/>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&display=swap" rel="stylesheet"/>
  <script src="https://cdn.jsdelivr.net/npm/typed.js@2.0.12"></script>
  <style>
    html {
      scroll-behavior: smooth;
    }body {
  font-family: 'Roboto', Arial, sans-serif;
  margin: 0;
  padding: 0;
  background: #0b1e3c; /* dark blue background */
  color: #ffffff; /* white font color */
  overflow-x: hidden;
  transition: background 0.4s, color 0.4s;
}

.navbar {
  display: flex;
  justify-content: center;
  background: rgba(0, 0, 0, 0.7);
  padding: 0.5rem 1rem;
  position: sticky;
  top: 0;
  z-index: 10;
}

.navbar a {
  color: #fff;
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
  color: #fff;
}

header p, .social-links {
  animation: slideIn 1.2s ease-out;
  color: #fff;
}

.social-links a {
  color: #fff;
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
  background-color: #ffffff;
  color: #111;
  padding: 2rem;
  margin-bottom: 2rem;
  border-radius: 12px;
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.2);
  opacity: 0;
  transform: translateY(40px);
  transition: opacity 0.8s ease, transform 0.8s ease;
}

section.reveal {
  opacity: 1;
  transform: translateY(0);
}

section h2 {
  color: #0b1e3c;
  font-size: 1.8rem;
}

footer {
  text-align: center;
  padding: 1.5rem;
  background-color: #000;
  color: #fff;
}

.background-animation {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(135deg, rgba(11, 30, 60, 0.8) 0%, rgba(5, 15, 30, 0.8) 100%);
  z-index: -1;
  animation: backgroundMove 10s ease-in-out infinite;
}

.back-to-top {
  position: fixed;
  bottom: 20px;
  right: 20px;
  background: #f4a261;
  color: white;
  border: none;
  padding: 10px 15px;
  border-radius: 50%;
  font-size: 18px;
  cursor: pointer;
  display: none;
  z-index: 1000;
}

.back-to-top.show {
  display: block;
}

@keyframes backgroundMove {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}

@keyframes fadeIn { 0% { opacity: 0; transform: translateY(20px); } 100% { opacity: 1; transform: translateY(0); } }
@keyframes slideIn { 0% { opacity: 0; transform: translateX(-30px); } 100% { opacity: 1; transform: translateX(0); } }

  </style>
</head>
<body><div class="background-animation"></div><header>
  <h1><span id="typed"></span></h1>
  <img src="https://images.unsplash.com/photo-1549921296-3a6b6b050b57?fit=crop&w=300&q=80" alt="Tech Avatar" class="profile-pic" />
  <p>Matric Number: 24/208CSC/898</p>
  <p>Email: <a href="mailto:ikechukwuperfect759@gmail.com" style="color: #f4a261;">ikechukwuperfect759@gmail.com</a></p>
  <div class="social-links">
    <a href="#"><i class="fab fa-instagram"></i></a>
    <a href="#"><i class="fab fa-x-twitter"></i></a>
    <a href="#"><i class="fab fa-facebook-f"></i></a>
  </div>
</header><main>
  <section id="past">
    <h2>Past: What I Have Done</h2>
    <p>I started learning the ropes of web design, building pages with HTML and CSS. It was like trying to teach a fish to climb a tree—awkward at first, but now I'm swimming in code!</p>
  </section>  <section id="present">
    <h2>Present: What I Am Doing</h2>
    <p>Currently a Computer Science student at the University of Abuja, sharpening my programming skills like a ninja with a keyboard. I’m building projects, debugging life, and drinking coffee like it’s a superpower.</p>
  </section>  <section id="future">
    <h2>Future: What I Plan to Do</h2>
    <p>I'm heading toward a career in cybersecurity—because what’s cooler than being a digital bodyguard? My dream is to become the guy who stops the bad guys with just a terminal window and a smirk.</p>
  </section>
</main><footer>
  <p>© 2025 Perfect Ikechukwu. All rights reserved.</p>
</footer><button class="back-to-top" id="backToTop">↑</button>

<script>
  // Typed effect
  new Typed("#typed", {
    strings: ["Perfect Ikechukwu"],
    typeSpeed: 60,
    showCursor: false,
  });

  // Reveal on scroll
  const sections = document.querySelectorAll("section");
  const revealOnScroll = () => {
    sections.forEach(sec => {
      const top = sec.getBoundingClientRect().top;
      if (top < window.innerHeight - 100) {
        sec.classList.add("reveal");
      }
    });
  };
  window.addEventListener("scroll", revealOnScroll);
  window.addEventListener("load", revealOnScroll);

  // Back to top button
  const backToTopBtn = document.getElementById("backToTop");
  window.addEventListener("scroll", () => {
    if (window.scrollY > 300) {
      backToTopBtn.classList.add("show");
    } else {
      backToTopBtn.classList.remove("show");
    }
  });
  backToTopBtn.addEventListener("click", () => {
    window.scrollTo({ top: 0, behavior: "smooth" });
  });
</script></body>
</html>
