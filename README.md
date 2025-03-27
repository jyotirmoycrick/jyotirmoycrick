<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jyotirmoy Malo - Professional Profile</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        :root {
            --primary-color: #3B82F6;
            --secondary-color: #2563EB;
            --text-color: #1F2937;
            --background-color: #F3F4F6;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            background-color: var(--background-color);
            line-height: 1.6;
            color: var(--text-color);
        }

        .profile-container {
            max-width: 1200px;
            margin: 2rem auto;
            background-color: white;
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
            border-radius: 15px;
            overflow: hidden;
            perspective: 1000px;
        }

        .header {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: white;
            padding: 3rem;
            text-align: center;
            position: relative;
            clip-path: polygon(0 0, 100% 0, 100% 85%, 0 100%);
            animation: headerSlideIn 1s ease-out;
        }

        @keyframes headerSlideIn {
            from {
                opacity: 0;
                transform: translateY(-50px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .profile-image {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            border: 5px solid white;
            object-fit: cover;
            margin-bottom: 1rem;
            box-shadow: 0 10px 25px rgba(0,0,0,0.2);
            transition: transform 0.5s ease;
        }

        .profile-image:hover {
            transform: scale(1.05) rotate(5deg);
        }

        .content {
            display: grid;
            grid-template-columns: 2fr 1fr;
            gap: 2rem;
            padding: 2rem;
        }

        .main-content {
            display: flex;
            flex-direction: column;
            gap: 2rem;
        }

        .section {
            background-color: white;
            border-radius: 10px;
            padding: 1.5rem;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
        }

        .section:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.15);
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 1rem;
        }

        .skill-category {
            background-color: var(--background-color);
            padding: 1rem;
            border-radius: 8px;
        }

        .skill-tag {
            display: inline-block;
            background-color: var(--primary-color);
            color: white;
            padding: 0.3rem 0.8rem;
            margin: 0.3rem;
            border-radius: 20px;
            font-size: 0.8rem;
            animation: tagPulse 2s infinite alternate;
        }

        @keyframes tagPulse {
            from { transform: scale(1); }
            to { transform: scale(1.05); }
        }

        .sidebar {
            display: flex;
            flex-direction: column;
            gap: 1.5rem;
        }

        .contact-card, .social-links {
            background-color: white;
            border-radius: 10px;
            padding: 1.5rem;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .social-links {
            display: flex;
            justify-content: space-around;
        }

        .social-link {
            color: var(--primary-color);
            font-size: 2rem;
            transition: transform 0.3s ease;
        }

        .social-link:hover {
            transform: scale(1.2) rotate(360deg);
        }

        @media (max-width: 768px) {
            .content {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="profile-container">
        <div class="header">
            <img src="/api/placeholder/200/200" alt="Jyotirmoy Malo" class="profile-image">
            <h1>Jyotirmoy Malo</h1>
            <p>Computer Science Engineering Student | Web Developer | Freelancer</p>
        </div>

        <div class="content">
            <div class="main-content">
                <section class="section about-me">
                    <h2>About Me</h2>
                    <p>A passionate computer science engineering student and freelance web developer with a keen interest in exploring cutting-edge technologies. Since 2020, I've been delivering high-quality web solutions and continuously expanding my technological expertise.</p>
                </section>

                <section class="section skills">
                    <h2>Skills</h2>
                    <div class="skills-grid">
                        <div class="skill-category">
                            <h3>Web Technologies</h3>
                            <div>
                                <span class="skill-tag">HTML5</span>
                                <span class="skill-tag">CSS3</span>
                                <span class="skill-tag">JavaScript</span>
                                <span class="skill-tag">PHP</span>
                                <span class="skill-tag">WordPress</span>
                            </div>
                        </div>
                        <div class="skill-category">
                            <h3>Design</h3>
                            <div>
                                <span class="skill-tag">Adobe Illustrator</span>
                                <span class="skill-tag">Photoshop</span>
                            </div>
                        </div>
                        <div class="skill-category">
                            <h3>Programming</h3>
                            <div>
                                <span class="skill-tag">Python</span>
                                <span class="skill-tag">Java</span>
                                <span class="skill-tag">C</span>
                            </div>
                        </div>
                        <div class="skill-category">
                            <h3>Cloud & Database</h3>
                            <div>
                                <span class="skill-tag">AWS</span>
                                <span class="skill-tag">MySQL</span>
                                <span class="skill-tag">Linux</span>
                            </div>
                        </div>
                    </div>
                </section>

                <section class="section projects">
                    <h2>Featured Projects</h2>
                    <div class="project-card">
                        <h3>Apollo Pharmacy Clone</h3>
                        <p>Comprehensive e-commerce platform mimicking pharmacy retail experience</p>
                        <div>
                            <span class="skill-tag">React</span>
                            <span class="skill-tag">Node.js</span>
                            <span class="skill-tag">Bootstrap</span>
                        </div>
                    </div>
                    <div class="project-card">
                        <h3>Sundarban Tour Expert</h3>
                        <p>Travel booking and information platform for tourism</p>
                        <div>
                            <span class="skill-tag">WordPress</span>
                            <span class="skill-tag">PHP</span>
                            <span class="skill-tag">MySQL</span>
                        </div>
                    </div>
                </section>
            </div>

            <div class="sidebar">
                <div class="contact-card">
                    <h2>Contact</h2>
                    <p><i class="fas fa-envelope"></i> malojyotirmoy@gmail.com</p>
                    <p><i class="fas fa-globe"></i> WebDesert.in</p>
                </div>

                <div class="social-links">
                    <a href="https://twitter.com/jyotirmoymalo" class="social-link">
                        <i class="fab fa-twitter"></i>
                    </a>
                    <a href="https://www.linkedin.com/in/jyotirmoy-malo-63827923b/" class="social-link">
                        <i class="fab fa-linkedin"></i>
                    </a>
                    <a href="https://github.com/jyotirmoycrick" class="social-link">
                        <i class="fab fa-github"></i>
                    </a>
                </div>

                <div class="section">
                    <h2>Continuous Learning</h2>
                    <p>Currently expanding knowledge in Computer Science Engineering at Adamas University</p>
                </div>
            </div>
        </div>
    </div>
</body>
</html>
