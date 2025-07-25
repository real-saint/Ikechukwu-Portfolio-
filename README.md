<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Perfect Ikechukwu - Cybersecurity Portfolio</title>
    <style>
        body {
            margin: 0;
            overflow: hidden;
            font-family: 'Exo 2', sans-serif;
            color: #fff;
        }
        #canvas {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
        }
        .content {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            text-align: center;
            width: 80%;
            max-width: 800px;
            pointer-events: none;
        }
        h1 {
            font-size: 3.5rem;
            text-shadow: 0 0 15px #00f, 0 0 30px #0ff;
            opacity: 0;
        }
        h2 {
            font-size: 1.5rem;
            text-shadow: 0 0 10px #0ff;
            opacity: 0;
        }
        p {
            font-size: 1.3rem;
            line-height: 1.7;
            opacity: 0;
            text-shadow: 0 0 10px #0ff;
        }
        .social-logos {
            margin-top: 2rem;
            display: flex;
            justify-content: center;
            gap: 2rem;
            pointer-events: auto;
        }
        .social-logos a img {
            width: 40px;
            opacity: 0;
            transition: transform 0.3s, filter 0.3s;
        }
        .social-logos a img:hover {
            transform: scale(1.2);
            filter: drop-shadow(0 0 10px #0ff);
        }
        #loader {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: #000;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #0ff;
            font-size: 1.5rem;
            z-index: 1000;
        }
        @media (max-width: 600px) {
            h1 { font-size: 2rem; }
            h2 { font-size: 1.2rem; }
            p { font-size: 1rem; }
            .social-logos a img { width: 30px; }
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Exo+2:wght@400;700&display=swap" rel="stylesheet">
</head>
<body>
    <div id="loader">Initializing Cyber Matrix...</div>
    <canvas id="canvas"></canvas>
    <div class="content">
        <h1 id="name">Perfect Ikechukwu</h1>
        <h2 id="matric">Matric No: 24/208CSC/898</h2>
        <p id="past">In my early journey, I immersed myself in the world of web designing and coding. From crafting visually stunning websites to mastering languages like HTML, CSS, and JavaScript, I honed my skills, laying a robust foundation for a career in technology.</p>
        <p id="present">Currently, I am a dedicated student at the University of Abuja, pursuing a degree in Computer Science. I am deepening my knowledge in advanced programming, algorithms, and emerging technologies, preparing to make a significant impact in the tech industry.</p>
        <p id="future">Looking to the future, I am driven to specialize in cybersecurity. My goal is to become an expert in protecting digital infrastructures, safeguarding data, and combating cyber threats, contributing to a secure and connected global ecosystem.</p>
        <div class="social-logos">
            <a href="https://instagram.com" target="_blank" id="instagram"><img src="https://upload.wikimedia.org/wikipedia/commons/a/a5/Instagram_icon.png" alt="Instagram"></a>
            <a href="https://x.com" target="_blank" id="twitter"><img src="https://upload.wikimedia.org/wikipedia/commons/5/5a/X_icon_2.svg" alt="X"></a>
            <a href="https://facebook.com" target="_blank" id="facebook"><img src="https://upload.wikimedia.org/wikipedia/commons/5/51/Facebook_f_logo_%282019%29.svg" alt="Facebook"></a>
        </div>
    </div>

    <script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r134/three.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.11.4/gsap.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r134/examples/js/controls/OrbitControls.js"></script>
    <script>
        // Three.js - Advanced Tech Background
        const scene = new THREE.Scene();
        const camera = new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);
        const renderer = new THREE.WebGLRenderer({ canvas: document.getElementById('canvas'), antialias: true });
        renderer.setSize(window.innerWidth, window.innerHeight);

        // Grid
        const gridHelper = new THREE.GridHelper(100, 50, 0x00ffff, 0x003333);
        gridHelper.position.y = -10;
        scene.add(gridHelper);

        // Wireframe Sphere
        const sphereGeometry = new THREE.SphereGeometry(15, 32, 16);
        const sphereMaterial = new THREE.MeshBasicMaterial({ color: 0x00ffff, wireframe: true, transparent: true, opacity: 0.3 });
        const sphere = new THREE.Mesh(sphereGeometry, sphereMaterial);
        scene.add(sphere);

        // Particles
        const particleCount = 2000;
        const particlesGeometry = new THREE.BufferGeometry();
        const posArray = new Float32Array(particleCount * 3);
        const velocities = new Float32Array(particleCount * 3);
        for (let i = 0; i < particleCount * 3; i += 3) {
            posArray[i] = (Math.random() - 0.5) * 100;
            posArray[i + 1] = (Math.random() - 0.5) * 100;
            posArray[i + 2] = (Math.random() - 0.5) * 100;
            velocities[i] = (Math.random() - 0.5) * 0.02;
            velocities[i + 1] = (Math.random() - 0.5) * 0.02;
            velocities[i + 2] = (Math.random() - 0.5) * 0.02;
        }
        particlesGeometry.setAttribute('position', new THREE.BufferAttribute(posArray, 3));
        const particleMaterial = new THREE.PointsMaterial({ size: 0.05, color: 0x00ffff, transparent: true, opacity: 0.7 });
        const particles = new THREE.Points(particlesGeometry, particleMaterial);
        scene.add(particles);

        // Lighting
        const ambientLight = new THREE.AmbientLight(0x404040);
        scene.add(ambientLight);
        const pointLight = new THREE.PointLight(0x00ffff, 1, 100);
        pointLight.position.set(10, 10, 10);
        scene.add(pointLight);

        camera.position.z = 20;

        // Mouse Interaction
        let mouseX = 0, mouseY = 0;
        document.addEventListener('mousemove', (e) => {
            mouseX = (e.clientX / window.innerWidth) * 2 - 1;
            mouseY = -(e.clientY / window.innerHeight) * 2 + 1;
        });

        // Animation Loop
        function animate() {
            requestAnimationFrame(animate);
            sphere.rotation.y += 0.002;
            gridHelper.rotation.x += 0.001;
            const positions = particlesGeometry.attributes.position.array;
            for (let i = 0; i < particleCount * 3; i += 3) {
                positions[i] += velocities[i] + mouseX * 0.01;
                positions[i + 1] += velocities[i + 1] + mouseY * 0.01;
                positions[i + 2] += velocities[i + 2];
                if (Math.abs(positions[i]) > 50) velocities[i] *= -1;
                if (Math.abs(positions[i + 1]) > 50) velocities[i + 1] *= -1;
                if (Math.abs(positions[i + 2]) > 50) velocities[i + 2] *= -1;
            }
            particlesGeometry.attributes.position.needsUpdate = true;
            renderer.render(scene, camera);
        }
        animate();

        // Resize Handler
        window.addEventListener('resize', () => {
            camera.aspect = window.innerWidth / window.innerHeight;
            camera.updateProjectionMatrix();
            renderer.setSize(window.innerWidth, window.innerHeight);
        });

        // GSAP Animations with Typewriter Effect
        function typeWriter(element, text, delay) {
            return gsap.to(element, {
                text: { value: text, delimiter: "" },
                duration: text.length / 20,
                ease: "none",
                delay: delay,
                onStart: () => element.innerHTML = "",
                opacity: 1
            });
        }

        gsap.timeline()
            .to("#loader", { opacity: 0, duration: 1, delay: 2, onComplete: () => loader.style.display = 'none'; })
            .to("#name", { opacity: 1, scale: 1.1, duration: 1, ease: "power2.out", textShadow: "0 0 30px #0ff" })
            .to("#name", { scale: 1, duration: 0.5 })
            .to("#matric", { opacity: 1, duration: 1 }, "-=0.5")
            .add(typeWriter("#past", document.getElementById("past").innerText, 1))
            .to("#past", { opacity: 0, duration: 1, delay: 5 })
            .add(typeWriter("#present", document.getElementById("present").innerText, 0))
            .to("#present", { opacity: 0, duration: 1, delay: 5 })
            .add(typeWriter("#future", document.getElementById("future").innerText, 0))
            .to("#future", { opacity: 0, duration: 1, delay: 5 })
            .to(".social-logos a img", { opacity: 1, scale: 1, stagger: 0.3, duration: 0.5, ease: "back.out(1.7)" });
    </script>
</body>
</html>
