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
      background: #0d1b2a;
      color: #e6d5b8;
      scroll-behavior: smooth;
      overflow-x: hidden;
      transition: background 0.4s, color 0.4s;
      position: relative;
    }body::before {
  content: "";
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: repeating-linear-gradient(
    0deg,
    rgba(255, 255, 255, 0.02) 0px,
    rgba(255, 255, 255, 0.02) 1px,
    transparent 1px,
    transparent 4px
  ),
  repeating-linear-gradient(
    90deg,
    rgba(255, 255, 255, 0.02) 0px,
    rgba(255, 255, 255, 0.02) 1px,
    transparent 1px,
    transparent 4px
  );
  z-index: -1;
  animation: techScroll 30s linear infinite;
}

@keyframes techScroll {
  0% {
    transform: translate(0, 0);
  }
  100% {
    transform: translate(-100px, -100px);
  }
}

.dark-mode {
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
