
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Perfect Ikechukwu - Portfolio</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css" integrity="sha512-z3gLpd7yknf1YoNbCzqRKc4qyor8gaKU1qmn+CShxbuBusANI9QpRohGBreCFkKxLhei6S9CQXFEbbKuqLg0DA==" crossorigin="anonymous" referrerpolicy="no-referrer" />
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&display=swap" rel="stylesheet">
    <style>
        /* General Styling */
        body {
            font-family: 'Roboto', Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: rgba(26, 38, 57, 0.8); /* Semi-transparent dark blue for overlay */
            color: #e6d5b8; /* Light beige text */
            scroll-behavior: smooth;
            perspective: 1000px; /* Enable 3D space */
            overflow-x: hidden; /* Prevent horizontal scroll from 3D elements */
            position: relative;
        }

        /* 3D Background Animation */
        .background-3d {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: #1a2639; /* Base dark blue */
            transform-style: preserve-3d;
            animation: rotate3D 20s infinite linear;
            z-index: -1; /* Behind content */
        }

        .background-3d::before,
        .background-3d::after {
            content: '';
            position: absolute;
            width: 200px;
            height: 200px;
            background: linear-gradient(45deg, #2c3e50, #0d1b2a);
            border-radius: 50%;
            animation: orbit 10s infinite linear;
        }

        .background-3d::after {
            animation-delay: -5s; /* Staggered animation */
            width: 150px;
            height: 150px;
            background: linear-gradient(45deg, #0d1b2a, #2c3e50);
        }

        @keyframes rotate3D {
            0% { transform: rotateX(0deg) rotateY(0deg); }
            100% { transform: rotateX(360deg) rotateY(360deg); }
        }

        @keyframes orbit {
            0% { transform: translate(-50%, -50%) rotate(0deg); }
            100% { transform: translate(-50%, -50%) rotate(360deg); }
        }

        /* Header Styling */
        header {
            background-color: #0d1b2a; /* Darker blue for header */
            color: #e6d5b8;
            text-align: center;
            padding: 3rem 2rem;
            position: relative;
            overflow: hidden;
        }

        .profile-pic {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            object-fit: cover;
            margin-bottom: 1rem;
            border: 3px solid #2c3e50; /* Lighter blue border */
            animation: float 3s ease-in-out infinite;
            transition: transform 0.3s ease;
        }

        .profile-pic:hover {
            transform: rotateY(15deg) rotateX(15deg) scale(1.1); /* 3D rotation on hover */
        }

        header h1 {
            margin: 0;
            font-size: 2.8rem;
            font-weight: 700;
            animation: typing 2.5s steps(30, end), blink-caret 0.75s step-end infinite, shadow3D 2s ease-out;
        }

        .typing-effect {
            overflow: hidden;
            white-space: nowrap;
            text-shadow: 0 0 10px rgba(244, 162, 97, 0.7);
        }

        header p {
            margin: 0.5rem 0;
            font-size: 1.2rem;
            font-weight: 300;
            animation: slideIn 1.2s ease-out;
        }

        header a {
            color: #f4a261; /* Warm orange for email link */
            text-decoration: none;
            transition: color 0.3s ease;
        }

        header a:hover {
            color: #e6d5b8; /* Beige on hover */
        }

        /* Social Media Links Styling */
        .social-links {
            margin-top: 1.5rem;
            animation: slideIn 1.4s ease-out;
        }

        .social-links a {
            color: #e6d5b8;
            font-size: 2rem;
            margin: 0 0.7rem;
            display: inline-block;
            transition: transform 0.3s ease;
            position: relative;
        }

        .social-links a:nth-child(1) { animation: float 2.5s ease-in-out infinite; }
        .social-links a:nth-child(2) { animation: float 2.5s ease-in-out infinite 0.3s; }
        .social-links a:nth-child(3) { animation: float 2.5s ease-in-out infinite 0.6s; }

        .social-links a:hover {
            transform: rotateY(180deg); /* 3D flip on hover */
            color: #2c3e50; /* Lighter blue on hover */
        }

        /* Main Content Styling */
        main {
            max-width: 900px;
            margin: 3rem auto;
            padding: 0 1.5rem;
            position: relative;
            z-index: 1; /* Above background */
        }

        section {
            background-color: #2c3e50; /* Lighter blue for sections */
            padding: 2rem;
            margin-bottom: 2rem;
            border-radius: 12px;
            border: 2px solid #0d1b2a; /* Darker blue border */
            box-shadow: 0 6px 20px rgba(0, 0, 0, 0.4);
            transition: transform 0.3s ease;
            transform-style: preserve-3d; /* Enable 3D transforms */
        }

        section:hover {
            transform: translateY(-12px) rotateX(5deg) rotateY(5deg); /* 3D tilt on hover */
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.5);
        }

        section h2 {
            color: #f4a261;
            font-size: 1.8rem;
            margin-top: 0;
            font-weight: 700;
        }

        /* Fade-In Animation for Sections */
        .fade-in {
            opacity: 0;
            animation: fadeIn 1s ease-in forwards;
        }

        .fade-in:nth-child(1) { animation-delay: 0.4s; }
        .fade-in:nth-child(2) { animation-delay: 0.8s; }
        .fade-in:nth-child(3) { animation-delay: 1.2s; }

        /* Footer Styling */
        footer {
            text-align: center;
            padding: 1.5rem;
            background-color: #0d1b2a;
            color: #e6d5b8;
            position: fixed;
            bottom: 0;
            width: 100%;
            animation: slideUp 1s ease-out;
            z-index: 1; /* Above background */
        }

        /* Keyframe Animations */
        @keyframes float {
            0% { transform: translateY(0); }
            50% { transform: translateY(-8px); }
            100% { transform: translateY(0); }
        }

        @keyframes fadeIn {
            0% { opacity: 0; transform: translateY(30px) rotateX(-10deg); }
            100% { opacity: 1; transform: translateY(0) rotateX(0); }
        }

        @keyframes slideIn {
            0% { opacity: 0; transform: translateX(-30px); }
            100% { opacity: 1; transform: translateX(0); }
        }

        @keyframes slideUp {
            0% { opacity: 0; transform: translateY(30px); }
            100% { opacity: 1; transform: translateY(0); }
        }

        @keyframes typing {
            from { width: 0; }
            to { width: 100%; }
        }

        @keyframes blink-caret {
            from, to { border-color: transparent; }
            50% { border-color: #f4a261; }
        }

        @keyframes shadow3D {
            0% { text-shadow: 0 0 0 rgba(244, 162, 97, 0); transform: translateZ(0); }
            100% { text-shadow: 5px 5px 10px rgba(244, 162, 97, 0.7); transform: translateZ(10px); }
        }

        /* Responsive Design */
        @media (max-width: 600px) {
            header h1 {
                font-size: 2.2rem;
            }

            .profile-pic {
                width: 100px;
                height: 100px;
            }

            section {
                padding: 1.5rem;
            }

            .social-links a {
                font-size: 1.7rem;
                margin: 0 0.5rem;
            }
        }
    </style>
</head>
<body>
    <div class="background-3d"></div> <!-- 3D background layer -->
    <header>
        <img src="profile-placeholder.jpg" alt="Profile Picture" class="profile-pic">
        <h1 class="typing-effect">Perfect Ikechukwu</h1>
        <p>Matric Number: 24/208/CSC898</p>
        <p>Email: <a href="mailto:ikechukwuperfect759@gmail.com">ikechukwuperfect759@gmail.com</a></p>
        <div class="social-links">
            <a href="https://instagram.com/yourusername" target="_blank" title="Instagram"><i class="fab fa-instagram"></i></a>
            <a href="https://x.com/yourusername" target="_blank" title="Twitter (X)"><i class="fab fa-x-twitter"></i></a>
            <a href="https://facebook.com/yourusername" target="_blank" title="Facebook"><i class="fab fa-facebook-f"></i></a>
        </div>
    </header>
    <main>
        <section class="fade-in" id="past">
            <h2>Past: What I Have Done</h2>
            <p>I have developed skills in <strong>web designing</strong>, creating responsive and user-friendly webpages using HTML and CSS.</p>
        </section>
        <section class="fade-in" id="present">
            <h2>Present: What I Am Doing</h2>
            <p>Currently a <strong>Computer Science student</strong> at the University of Abuja, focusing on coursework and advancing my programming and design skills.</p>
        </section>
        <section class="fade-in" id="future">
            <h2>Future: What I Plan to Do</h2>
            <p>I aim to pursue a career in <strong>cybersecurity</strong>, specializing in areas like ethical hacking and network security.</p>
        </section>
    </main>
    <footer>
        <p>© 2025 Perfect Ikechukwu. All rights reserved.</p>
    </footer>
</body>
</html>
