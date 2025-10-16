# myportfoilo
index.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>B. Likhitha | Portfolio</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <!-- Navigation Bar -->
  <nav class="navbar">
    <div class="logo">B. Likhitha</div>
    <ul class="nav-links">
      <li><a href="#about">About</a></li>
      <li><a href="#skills">Skills</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <!-- Main Container -->
  <div class="container">
    <section id="about" class="section-card">
      <h2>About Me</h2>
      <p>
        I’m pursuing my B.Tech in Artificial Intelligence & Data Science at Mother Theresa 
        Institute of Engineering and Technology with a CGPA of 8.7. I’m passionate about 
        building intelligent web applications, exploring machine learning, and solving 
        real-world data problems creatively.
      </p>
    </section>

    <section id="skills" class="section-card">
      <h2>Skills</h2>
      <ul>
        <li>Web Development: HTML, CSS, JavaScript</li>
        <li>Programming: Python, C</li>
        <li>Data Analysis: Pandas, NumPy (Basic Level)</li>
      </ul>
    </section>

    <section id="projects" class="section-card">
      <h2>Projects</h2>
      <ul>
        <li><strong>Portfolio Website</strong> – A responsive personal website showcasing skills and achievements.</li>
        <li><strong>Web Page Designs</strong> – Custom UI pages with creative color palettes and modern layouts.</li>
      </ul>
    </section>

    <section id="contact" class="section-card">
      <h2>Contact</h2>
      <p>Email: <a href="mailto:likhitha301@gmail.com">likhitha301@gmail.com</a></p>
      <p>Location: Mother Theresa Institute of Engineering and Technology</p>
    </section>
  </div>

  <footer>
    © 2025 <span>B. Likhitha</span> | All Rights Reserved
  </footer>
</body>
</html>                                                                                                                                                                                                                                                        
style.css
/* Reset and Base Styles */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Poppins', sans-serif;
  color: #fff;
  background: radial-gradient(circle at top left, #ff9ff3, #00d2d3, #5f27cd);
  background-size: 200% 200%;
  animation: bgShift 10s ease-in-out infinite alternate;
  scroll-behavior: smooth;
}

/* Background Animation */
@keyframes bgShift {
  0% { background-position: left top; }
  100% { background-position: right bottom; }
}

/* Navigation Bar */
.navbar {
  width: 100%;
  padding: 15px 30px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: rgba(255, 255, 255, 0.1);
  backdrop-filter: blur(8px);
  position: fixed;
  top: 0;
  z-index: 1000;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
}

.logo {
  font-size: 1.6rem;
  font-weight: bold;
  color: #ffeaa7;
}

.nav-links {
  list-style: none;
  display: flex;
  gap: 20px;
}

.nav-links li a {
  color: #fff;
  text-decoration: none;
  font-size: 1rem;
  transition: 0.3s;
}

.nav-links li a:hover {
  color: #74b9ff;
  text-shadow: 0 0 8px rgba(255,255,255,0.7);
}

/* Container */
.container {
  padding: 120px 30px 60px;
  width: 90%;
  max-width: 1000px;
  margin: auto;
}

/* Cards for Sections */
.section-card {
  background: rgba(255, 255, 255, 0.12);
  border-radius: 20px;
  backdrop-filter: blur(12px);
  box-shadow: 0 0 25px rgba(255, 255, 255, 0.2);
  padding: 40px;
  margin-bottom: 30px;
  animation: fadeIn 1.5s ease-in-out;
}

@keyframes fadeIn {
  from { opacity: 0; transform: scale(0.95); }
  to { opacity: 1; transform: scale(1); }
}

h2 {
  font-size: 1.8rem;
  margin-bottom: 15px;
  border-left: 4px solid #fff;
  padding-left: 10px;
}

p, li {
  font-size: 1rem;
  line-height: 1.6;
  color: #e4e4e4;
}

ul {
  margin-top: 10px;
  margin-left: 25px;
  list-style-type: square;
}

li strong {
  color: #ffeaa7;
}

a {
  color: #74b9ff;
  text-decoration: none;
  transition: 0.3s;
}

a:hover {
  color: #00cec9;
  text-shadow: 0 0 8px rgba(255,255,255,0.7);
}

/* Footer */
footer {
  text-align: center;
  padding: 20px;
  font-size: 0.9rem;
  opacity: 0.85;
}

footer span {
  color: #81ecec;
}

/* Responsive */
@media (max-width: 600px) {
  .navbar {
    flex-direction: column;
    gap: 10px;
  }
  .nav-links {
    flex-direction: column;
    gap: 10px;
  }
  h2 { font-size: 1.4rem; }
}
