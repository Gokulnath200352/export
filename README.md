# Ex01 Portfolio
## Date:28.07.2026

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <style>
        /* CSS Reset and Base Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #f8f9fa;
            color: #333;
            line-height: 1.6;
        }

        /* Navigation Bar */
        header {
            background-color: #0967ff;
            color: #fff;
            padding: 1rem 5%;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        nav .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: #032f42;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 1.5rem;
        }

        nav a {
            color: #fff;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }

        nav a:hover {
            color: #022736;
        }

        /* Hero Section */
        .hero {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding: 5rem 1rem;
            background: linear-gradient(135deg, #1e293b, #0f172a);
            color: #fff;
        }

        /* Profile Picture Styling */
        .profile-pic {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            object-fit: cover;
            border: 4px solid #022f42;
            margin-bottom: 1.5rem;
            box-shadow: 0 4px 15px rgba(56, 189, 248, 0.3);
        }

        .hero h1 {
            font-size: 2.8rem;
            margin-bottom: 0.5rem;
        }

        .hero span {
            color: #c5d0d4;
        }

        .hero p {
            font-size: 1.2rem;
            color: #216eda;
            margin-bottom: 1.5rem;
        }

        .btn {
            display: inline-block;
            padding: 0.75rem 1.5rem;
            background-color: #022635;
            color: #1b4ab6;
            font-weight: bold;
            text-decoration: none;
            border-radius: 6px;
            transition: background 0.3s;
        }

        .btn:hover {
            background-color: #373939;
            color: #fff;
        }

        /* Main Container */
        .container {
            max-width: 1000px;
            margin: auto;
            padding: 3rem 1.5rem;
        }

        section {
            margin-bottom: 3rem;
        }

        h2 {
            font-size: 2rem;
            margin-bottom: 1rem;
            color: #1d3572;
            border-bottom: 3px solid #2c2c2deb;
            display: inline-block;
            padding-bottom: 0.2rem;
        }

        /* About Section */
        .about p {
            font-size: 1.1rem;
            color: #397ad6;
        }

        /* Skills Section */
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
            gap: 1rem;
            margin-top: 1rem;
        }

        .skill-card {
            background-color: #fff;
            padding: 1rem;
            text-align: center;
            border-radius: 8px;
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
            font-weight: 600;
            color: #245fbe;
        }

        /* Projects Section */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 1.5rem;
            margin-top: 1rem;
        }

        .project-card {
            background-color: #fff;
            padding: 1.5rem;
            border-radius: 8px;
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
        }

        .project-card h3 {
            margin-bottom: 0.5rem;
            color: #b98325;
        }

        .project-card p {
            color: #c96d34;
            font-size: 0.95rem;
            margin-bottom: 1rem;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 1.5rem;
            background-color: #da730c;
            color: #2974dd;
            font-size: 0.9rem;
        }
    </style>
</head>
<body>

    <!-- Header / Navbar -->
    <header>
        <nav>
            <div class="logo">MyPortfolio</div>
            <ul>
                <li><a href="#about">About</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <img src="WhatsApp Image 2026-07-28 at 2.34.57 PM.jpeg" alt="GOKULNATH R" class="profile-pic">
        <h1>Hi, I'm <span>GOKULNATH</span></h1>
        <p>Web Developer & Student</p>
        <a href="#projects" class="btn">View Work</a>
    </section>

    <!-- Main Content -->
    <div class="container">
        
        <!-- About Section -->
        <section id="about" class="about">
            <h2>About Me</h2>
            <p>Welcome to my portfolio! I am a passionate developer eager to build innovative web applications. I enjoy learning new technologies and solving complex problems with clean code.</p>
        </section>

        <!-- Skills Section -->
        <section id="skills">
            <h2>Skills</h2>
            <div class="skills-grid">
                <div class="skill-card">HTML5</div>
                <div class="skill-card">CSS3</div>
                <div class="skill-card">JavaScript</div>
                <div class="skill-card">Git & GitHub</div>
            </div>
        </section>

        <!-- Projects Section -->
        <section id="projects">
            <h2>Projects</h2>
            <div class="projects-grid">
                <div class="project-card">
                    <h3>Portfolio Website</h3>
                    <p>A responsive personal portfolio website built using HTML and CSS to showcase projects and skills.</p>
                </div>
                <div class="project-card">
                    <h3>Landing Page</h3>
                    <p>A modern product landing page design optimized for all screen sizes and mobile responsiveness.</p>
                </div>
            </div>
        </section>

        <!-- Contact Section -->
        <section id="contact">
            <h2>Contact</h2>
            <p>Feel free to reach out to me via email or GitHub:</p>
            <p style="margin-top: 0.5rem;"><strong>Email:</strong>rg4860179@gmail.com</p>
        </section>

    </div>

    <!-- Footer -->
    <footer>
        <p>&copy; 2026 GOKULNATH. All rights reserved.</p>
    </footer>

</body>
</html>
```

## OUTPUT

<img width="1920" height="1200" alt="Screenshot 2026-07-28 144828" src="https://github.com/user-attachments/assets/23b55e59-0549-408a-8643-8868ec912f00" />
<img width="1920" height="1200" alt="Screenshot 2026-07-28 144847" src="https://github.com/user-attachments/assets/b34f4fbd-46c9-4d74-9e23-add5d6cb1a53" />



## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
