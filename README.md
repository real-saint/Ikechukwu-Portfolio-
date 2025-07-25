<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ikechukwu Ugochukwu's Portfolio</title>
    <style>
        body {
            font-family: 'Segoe UI', Arial, sans-serif;
            margin: 0;
            padding: 40px;
            background-color: #1a2b4c; /* Dark blue background */
            color: #e0e0e0;
            overflow-x: hidden;
            position: relative;
        }
        #particles-js {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1; /* Behind content */
        }
        header {
            text-align: center;
            background: rgba(0, 0, 0, 0.3);
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.5);
            margin-bottom: 40px;
            animation: fadeIn 1s ease-in;
        }
        h1 {
            color: #ffffff;
            font-size: 2.5em;
            margin: 0;
        }
        header p {
            color: #b0c4de;
            font-size: 1.2em;
        }
        section {
            background: rgba(255, 255, 255, 0.1);
            padding: 20px;
            margin: 20px auto;
            border-radius: 10px;
            max-width: 600px;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.3);
            opacity: 0; /* For fade-in effect */
            animation: fadeInUp 1s ease forwards;
            animation-delay: calc(var(--order) * 0.3s); /* Staggered animation */
            transition: transform 0.3s ease;
        }
        section:hover {
            transform: translateY(-10px);
        }
        section:nth-child(2) { --order: 1; animation: float1 5s ease-in-out infinite; }
        section:nth-child(3) { --order: 2; animation: float2 6s ease-in-out infinite; }
        section:nth-child(4) { --order: 3; animation: float3 7s ease-in-out infinite; }
        h2 {
            color: #00b7eb;
            font-size: 1.8em;
            margin-top: 0;
        }
        p, a {
            line-height: 1.6;
            color: #d3d3d3;
        }
        a {
            color: #00b7eb;
            text-decoration: none;
        }
        a:hover {
            text-decoration: underline;
        }
        /* Animation keyframes */
        @keyframes float1 {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-15px); }
            100% { transform: translateY(0px); }
        }
        @keyframes float2 {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
            100% { transform: translateY(0px); }
        }
        @keyframes float3 {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-25px); }
            100% { transform: translateY(0px); }
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(50px); }
            to { opacity: 1; transform: translateY(0); }
        }
        /* Responsive design */
        @media (max-width: 600px) {
            body { padding: 20px; }
            h1 { font-size: 2em; }
            section { max-width: 100%; }
        }
    </style>
</head>
<body>
    <div id="particles-js"></div> <!-- Particle background -->
    <header>
        <h1>Ikechukwu Ugochukwu</h1>
        <p>Matric No: 24/208CSC/898 | Computer Science, University of Abuja</p>
    </header>
    <section>
        <h2>Past Experiences</h2>
        <p>Developed skills in web design and Python programming through self-study and hands-on projects, including small-scale websites and automation scripts.</p>
    </section>
    <section>
        <h2>Current Studies</h2>
        <p>Pursuing a degree in Computer Science at the University of Abuja, focusing on software development, algorithms, and cybersecurity fundamentals.</p>
    </section>
    <section>
        <h2>Future Goals</h2>
        <p>Aspiring to become a cybersecurity expert, specializing in secure software solutions and contributing to innovative tech projects.</p>
    </section>
    <section>
        <h2>Contact</h2>
        <p>Email: <a href="mailto:ikechukwuperfect759@gmail.com">ikechukwuperfect759@gmail.com</a></p>
    </section>
    <script src="https://cdn.jsdelivr.net/particles.js/2.0.0/particles.min.js"></script>
    <script>
        // Particle.js configuration
        particlesJS("particles-js", {
            particles: {
                number: { value: 80, density: { enable: true, value_area: 800 } },
                color: { value: "#00b7eb" }, // Cyan particles
                shape: { type: "circle" },
                opacity: { value: 0.5, random: true },
                size: { value: 3, random: true },
                line_linked: { enable: false },
                move: { enable: true, speed: 2, direction: "none", random: true }
            },
            interactivity: {
                detect_on: "canvas",
                events: { onhover: { enable: true, mode: "repulse" }, onclick: { enable: true, mode: "push" } },
                modes: { repulse: { distance: 100, duration: 0.4 }, push: { particles_nb: 4 } }
            }
        });
        // Intersection Observer for fade-in animations
        const sections = document.querySelectorAll('section');
        const observer = new IntersectionObserver(entries => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.animationPlayState = 'running';
                }
            });
        }, { threshold: 0.2 });
        sections.forEach(section => observer.observe(section));
    </script>
</body>
</html>
