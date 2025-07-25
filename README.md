<!DOCTYPE html>
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
            background-color: #2f1b0f; /* Dark brown background */
            color: #e6d5b8; /* Light beige text */
            scroll-behavior: smooth;
        }

        /* Header Styling */
        header {
            background-color: #1a0f07; /* Darker brown for header */
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
            border: 3px solid #1a2639; /* Dark blue border */
            animation: float 3s ease-in-out infinite;
        }

        header h1 {
            margin: 0;
            font-size: 2.8rem;
            font-weight: 700;
        }

        .typing-effect {
            overflow: hidden;
            white-space: nowrap;
            animation: typing 2.5s steps(30, end), blink-caret 0.75s step-end infinite;
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
            color: #1a2639; /* Dark blue on hover */
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
            transition: transform 0.3s ease, color 0.3s ease;
            display: inline-block;
        }

        .social-links a:nth-child(1) { animation: float 2.5s ease-in-out infinite; }
        .social-links a:nth-child(2) { animation: float 2.5s ease-in-out infinite 0.3s; }
        .social-links a:nth-child(3) { animation: float 2.5s ease-in-out infinite 0.6s; }

        .social-links a:hover {
            transform: scale(1.3);
            color: #1a2639; /* Dark blue on hover */
        }

        /* Main Content Styling */
        main {
            max-width: 900px;
            margin: 3rem auto;
            padding: 0 1.5rem;
        }

        section {
            background-color: #3c2317; /* Slightly lighter brown for sections */
            padding: 2rem;
            margin-bottom: 2rem;
            border-radius: 12px;
            border: 2px solid #1a2639; /* Dark blue border */
            box-shadow: 0 6px 20px rgba(0, 0, 0, 0.4);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        section:hover {
            transform: translateY(-12px) scale(1.02); /* Lift and slight float on hover */
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
            background-color: #1a0f07;
            color: #e6d5b8;
            position: fixed;
            bottom: 0;
            width: 100%;
            animation: slideUp 1s ease-out;
        }

        /* Keyframe Animations */
        @keyframes float {
            0% { transform: translateY(0); }
            50% { transform: translateY(-8px); }
            100% { transform: translateY(0); }
        }

        @keyframes fadeIn {
            0% { opacity: 0; transform: translateY(30px); }
            100% { opacity: 1; transform: translateY(0); }
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
