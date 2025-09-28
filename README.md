# lab-1

<!-- 
Lab 1 - Personal Portfolio Website
File: index.html
Author: S Aradhana
-->


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>S Aradhana - Beginner Portfolio</title>
    <style>
        /* Basic Reset and Global Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: #f4f4f4;
        }

        a {
            text-decoration: none;
            color: #007bff;
        }

        a:hover {
            text-decoration: underline;
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
        }

        /* Header */
        header {
            background: #fff;
            padding: 10px 0;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.5em;
            font-weight: bold;
        }

        .nav-links {
            list-style: none;
            display: flex;
        }

        .nav-links li {
            margin-left: 20px;
        }

        .nav-links a {
            color: #333;
            font-weight: bold;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(to right, #007bff, #0056b3);
            color: white;
            text-align: center;
            padding: 100px 0 50px;
            margin-top: 60px; /* Account for fixed header */
        }

        .hero h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
        }

        .hero p {
            font-size: 1.2em;
            margin-bottom: 20px;
        }

        .btn {
            display: inline-block;
            background: #fff;
            color: #007bff;
            padding: 10px 20px;
            border-radius: 5px;
            font-weight: bold;
            margin-top: 10px;
        }

        .btn:hover {
            background: #f8f9fa;
        }

        /* Section Styles */
        section {
            padding: 50px 0;
            background: #fff;
        }

        .section-title {
            text-align: center;
            font-size: 2em;
            margin-bottom: 30px;
            color: #333;
        }

        /* About Section */
        .about-content {
            text-align: center;
            max-width: 600px;
            margin: 0 auto;
        }

        .about-content p {
            font-size: 1.1em;
            margin-bottom: 20px;
        }

        /* Skills Section */
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .skill-item {
            background: #f8f9fa;
            padding: 20px;
            border-radius: 8px;
            text-align: center;
            border-left: 4px solid #007bff;
        }

        .skill-item h3 {
            color: #007bff;
            margin-bottom: 10px;
        }

        .skill-item p {
            color: #666;
        }

        /* Projects Section */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .project-card {
            background: #f8f9fa;
            padding: 20px;
            border-radius: 8px;
            text-align: center;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        .project-card h3 {
            color: #333;
            margin-bottom: 10px;
        }

        .project-card p {
            color: #666;
            margin-bottom: 15px;
        }

        .project-link {
            color: #007bff;
            font-weight: bold;
        }

        /* Contact Section */
        .contact-content {
            text-align: center;
            max-width: 600px;
            margin: 0 auto;
        }

        .contact-info {
            margin-bottom: 20px;
        }

        .contact-info p {
            margin-bottom: 10px;
        }

        form {
            max-width: 500px;
            margin: 0 auto;
        }

        input, textarea {
            width: 100%;
            padding: 10px;
            margin-bottom: 15px;
            border: 1px solid #ddd;
            border-radius: 4px;
            font-family: Arial, sans-serif;
        }

        button {
            background: #007bff;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-size: 1em;
        }

        button:hover {
            background: #0056b3;
        }

        /* Footer */
        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 20px 0;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .nav-links {
                flex-direction: column;
                position: absolute;
                top: 60px;
                left: -100%;
                width: 100%;
                background: #fff;
                padding: 20px 0;
                box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            }

            .nav-links.active {
                left: 0;
            }

            .nav-links li {
                margin: 10px 0;
            }

            .hero h1 {
                font-size: 2em;
            }

            .container {
                padding: 10px;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <nav class="container">
            <div class="logo">S Aradhana</div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="container">
            <h1>Hi, I'm S Aradhana</h1>
            <p>A beginner programmer passionate about learning coding and building simple projects.</p>
            <a href="#projects" class="btn">See My Projects</a>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="container">
        <h2 class="section-title">About Me</h2>
        <div class="about-content">
            <p>Hello! I'm S Aradhana, a beginner in the world of programming. I'm currently learning the basics of computer science and software development through online courses and personal projects.</p>
            <p>I enjoy solving problems with code and am excited to start my journey in tech. My goal is to become a full-stack developer one day!</p>
            <p>When not coding, I like reading books and exploring new technologies.</p>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="container">
        <h2 class="section-title">My Skills</h2>
        <div class="skills-grid">
            <div class="skill-item">
                <h3>Python</h3>
                <p>Basic programming concepts, loops, functions, and simple scripts.</p>
            </div>
            <div class="skill-item">
                <h3>C</h3>
                <p>Understanding pointers, arrays, and basic data structures.</p>
            </div>
            <div class="skill-item">
                <h3>C++</h3>
                <p>Object-oriented programming basics, classes, and inheritance.</p>
            </div>
            <div class="skill-item">
                <h3>HTML </h3>
                <p>Building simple web pages.</p>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="container">
        <h2 class="section-title">My Projects</h2>
        <div class="projects-grid">
            <div class="project-card">
                <h3>Simple Calculator (Python)</h3>
                <p>A basic command-line calculator that performs addition, subtraction, multiplication, and division.</p>
                <a href="https://github.com/aradhana-bit/arithematic-calculator-.git" class="project-link">View Code on GitHub</a>
            </div>
            <div class="project-card">
                <h3>Student Grade Tracker (C)</h3>
                <p>A program to input student names and grades, then calculate averages and display results.</p>
                <a href="https://github.com/aradhana-bit/student-grade-tracker.git" class="project-link">View Code on GitHub</a>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="container">
        <h2 class="section-title">Get In Touch</h2>
        <div class="contact-content">
            <div class="contact-info">
                <p><strong>Email:</strong> aru10072007@gmail.com</p>
                <p><strong>LinkedIn:</strong> <a href="#">https://www.linkedin.com/in/s-aradhana-a9ab51306?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app</a></p>
                <p><strong>GitHub:</strong> <a href="#">https://github.com/aradhana-bit</a></p>
            </div>
            <form>
                <input type="text" placeholder="Your Name" required>
                <input type="email" placeholder="Your Email" required>
                <textarea placeholder="Your Message" required></textarea>
                <button type="submit">Send Message</button>
            </form>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p>&copy; 2023 S Aradhana. All rights reserved.</p>
        </div>
    </footer>

    <script>
        // Simple smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
