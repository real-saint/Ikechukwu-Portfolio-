<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Perfect Ikechukwu's Portfolio</title>
    <style>
        body {
            font-family: 'Roboto', Arial, sans-serif;
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
            z-index: -1;
        }
        header {
            text-align: center;
            background: rgba(0, 0, 0, 0.4);
            padding: 40px;
            border-radius: 15px;
            box-shadow: 0 6px 20px rgba(0, 0, 0, 0.6);
            margin-bottom: 50px;
            animation: fadeIn 1.5s ease-in;
        }
        h1 {
            color: #ffffff;
            font-size: 3em;
            margin: 0;
            display: inline-block;
            overflow: hidden; /* For typewriter effect */
            white-space: nowrap;
            border-right: 0.15em solid #00b7eb;
            animation: typewriter 3s steps(40, end) forwards, blink-caret 0.75s step-end infinite;
        }
        header p {
            color: #b0c4de;
            font-size: 1.3em;
            margin-top: 10px;
        }
        section {
            background: rgba(255, 255, 255, 0.15);
            padding: 25px;
            margin: 30px auto;
            border-radius: 15px;
            max-width: 700px;
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.4);
            opacity: 0;
            animation: fadeInUp 1.2s ease forwards;
            animation-delay: calc(var(--order) * 0.4s);
            transition: transform 0.3s ease;
            transform-style: preserve-3d; /* For 3D tilt */
        }
        section:hover {
            transform: translateY(-15px) rotateX(5deg) rotateY(5deg);
        }
        section:nth-child(2) { --order: 1; animation: float1 5s ease-in-out infinite, fadeInUp 1.2s ease forwards; }
        section:nth-child(3) { --order: 2; animation: float2 6s ease-in-out infinite, fadeInUp 1.2s ease forwards; }
        section:nth-child(4) { --order: 3; animation: float3 7s ease-in-out infinite, fadeInUp 1.2s ease forwards; }
        section:nth-child(5) { --order: 4; animation: float1 5.5s ease-in-out infinite, fadeInUp 1.2s ease forwards; }
        h2 {
            color: #00b7eb;
            font-size: 2em;
            margin-top: 0;
            position: relative;
        }
        h2::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 50px;
            height: 3px;
            background: #00b7eb;
            animation: slideIn 1s ease forwards;
        }
        p, a {
            line-height: 1.7;
            color: #d3d3d3;
            font-size: 1.1em;
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
            0% { transform: translateY(0px) rotateX(0deg); }
            50% { transform: translateY(-20px) rotateX(3deg); }
            100% { transform: translateY(0px) rotateX(0deg); }
        }
        @keyframes float2 {
            0% { transform: translateY(0px) rotateY(0deg); }
            50% { transform: translateY(-25px) rotateY(4deg); }
            100% { transform: translateY(0px) rotateY(0deg); }
        }
        @keyframes float3 {
            0% { transform: translateY(0px) rotateX(0deg) rotateY(0deg); }
            50% { transform: translateY(-30px) rotateX(5deg) rotateY(5deg); }
            100% { transform: translateY(0px) rotateX(0deg) rotateY(0deg); }
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(60px); }
            to { opacity: 1; transform: translateY(0); }
        }
        @keyframes typewriter {
            from { width: 0; }
            to { width: 100%; }
        }
        @keyframes blink-caret {
            from, to { border-color: transparent; }
            50% { border-color: #00b7eb; }
        }
        @keyframes slideIn {
            from { width: 0; }
            to { width: 50px; }
        }
        /* Responsive design */
        @media (max-width: 600px) {
            body { padding: 20px; }
            h1 { font-size: 2.2em; }
            section { max-width: 100%; }
            header { padding: 20px; }
        }
    </style>
</head>
<body>
    <div id="particles-js"></div>
    <header>
        <h1>Perfect Ikechukwu</h1>
        <p>Matric No: 24/208CSC/898 | Computer Science, University of Abuja</p>
    </header>
    <section>
        <h2>Past Experiences</h2>
        <p>Embarked on a self-driven journey in software development, mastering web design with HTML, CSS, and JavaScript to create responsive, user-friendly websites. Developed proficiency in Python through projects like automation scripts, data analysis tools, and small-scale web applications. Contributed to open-source repositories and collaborated on team projects, honing skills in version control with Git and problem-solving in real-world coding scenarios.</p>
    </section>
    <section>
        <h2>Current Studies</h2>
        <p>Actively pursuing a Bachelor’s degree in Computer Science at the University of Abuja, delving into advanced topics such as data structures, algorithms, database management, and cybersecurity principles. Engaged in practical coursework, including developing full-stack applications and exploring machine learning fundamentals. Leading a study group within the CSC department to foster peer learning and collaborative coding projects.</p>
    </section>
    <section>
        <h2>Future Goals</h2>
        <p>Aspiring to become a globally recognized cybersecurity expert, specializing in ethical hacking, penetration testing, and secure software architecture. Plan to contribute to cutting-edge cybersecurity solutions, protecting digital infrastructures against emerging threats. Aim to pursue advanced certifications (e.g., CEH, OSCP) and lead innovative projects that integrate AI with cybersecurity for robust defense mechanisms.</p>
    </section>
    <section>
        <h2>Contact</h2>
        <p>Email: <a href="mailto:ikechukwuperfect759@gmail.com">ikechukwuperfect759@gmail.com</a></p>
    </section>
    <script src="https://cdn.jsdelivr.net/particles.js/2.0.0/particles.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/vanilla-tilt/1.7.0/vanilla-tilt.min.js"></script>
    <script>
        // Enhanced Particle.js configuration
        particlesJS("particles-js", {
            particles: {
                number: { value: 100, density: { enable: true, value_area: 800 } },
                color: { value: ["#00b7eb", "#ffffff", "#b0c4de"] }, // Multi-color particles
                shape: { type: ["circle", "triangle", "star"], stroke: { width: 0 } },
                opacity: { value: 0.6, random: true, anim: { enable: true, speed: 1 } },
                size: { value: 4, random: true, anim: { enable: true, speed: 2 } },
                line_linked: { enable: true, distance: 150, color: "#00b7eb", opacity: 0.3, width: 1 },
                move: { enable: true, speed: 3, direction: "random", random: true, out_mode: "out" }
            },
            interactivity: {
                detect_on: "canvas",
                events: {
                    onhover: { enable: true, mode: "grab" },
                    onclick: { enable: true, mode: "push" },
                    resize: true
                },
                modes: {
                    grab: { distance: 200, line_linked: { opacity: 0.5 } },
                    push: { particles_nb: 5 }
                }
            }
        });
        // Vanilla Tilt for 3D tilt effect on sections
        VanillaTilt.init(document.querySelectorAll("section"), {
            max: 15,
            speed: 400,
            glare: true,
            "max-glare": 0.3
        });
        // Intersection Observer for fade-in animations
        const sections = document.querySelectorAll('section');
        const observer = new IntersectionObserver(entries => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.animationPlayState = 'running';
                }
            });
        }, { threshold: 0.3 });
        sections.forEach(section => observer.observe(section));
    </script>
</body>
</html>
