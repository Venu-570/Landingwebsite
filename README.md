<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <link rel="stylesheet" href="styles.css">
    <style>
body {
    font-family: 'Arial', sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
    color: #333;
    line-height: 1.6;
    overflow-x: hidden;
}
/* Header Styles */
header {
    background-color: #333;
    color: #fff;
    padding: 1em 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 1000;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
    transition: background-color 0.3s ease;
}
header.scrolled {
    background-color: rgba(51, 51, 51, 0.9);
}
.logo h1 {
    margin: 0;
    padding-left: 20px;
    font-size: 1.8em;
    font-weight: bold;
}
nav ul {
    list-style: none;
    margin: 0;
    padding-right: 20px;
    display: flex;
    gap: 1em;
}
nav ul li {
    margin: 0;
}
nav ul li a {  
    color: #fff;
    text-decoration: none;
    font-weight: bold;
    padding: 0.5em 1em;
    transition: color 0.3s ease;
}
nav ul li a:hover {
    color: #ff6347;
}
/* Hero Section Styles */
#hero {
    height: 100vh;
    background-image: url('https://dl.dropbox.com/s/5vqcn5w81ki3bbl/FaceApp_1600785543600-01-05.jpeg?dl=0');
    background-size: cover;
    background-position: center;
    color: #fff;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 0 20px;
}
#hero h2 {
    font-size: 2.5em;
    margin-bottom: 0.5em;
    animation: fadeInDown 1s ease-out;
}
#hero p {
    font-size: 1.5em;
    margin-bottom: 1em;
    animation: fadeInUp 1s ease-out;
}
#hero .cta {
    padding: 0.8em 2em;
    background-color: #ff6347;
    color: #fff;
    text-decoration: none;
    font-weight: bold;
    border-radius: 5px;
    transition: background-color 0.3s ease, transform 0.3s ease;
    animation: fadeInUp 1.2s ease-out;
}
#hero .cta:hover {
    background-color: #e5533d;
    transform: scale(1.05);
}
/* Content Section Styles */
.content-section {
    padding: 4em 1em;
    max-width: 1100px;
    margin: 0 auto;
    text-align: center;
}
.content-section h2 {
    font-size: 2.5em;
    margin-bottom: 1em;
    position: relative;
    display: inline-block;
}
.content-section h2::after {
    content: '';
    width: 50px;
    height: 4px;
    background-color: #ff6347;
    display: block;
    margin: 0.5em auto;
    transition: width 0.4s ease;
}
.content-section h2:hover::after {
    width: 100px;
}
#skills .skills-grid {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 1em;
}
.skill {
    background-color: #fff;
    padding: 1.5em;
    border-radius: 5px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}
.skill:hover {
    transform: translateY(-5px);
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
}
#projects .projects-grid {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 1em;
}
.project-card {
    background-color: #fff;
    padding: 2em;
    border-radius: 5px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}
.project-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
}
/* Contact Section */
#contact p {
    font-size: 1.2em;
    color: #666;
}
#contact a {
    color: #ff6347;
    text-decoration: none;
    font-weight: bold;
    transition: color 0.3s ease;
}
#contact a:hover {
    color: #e5533d;
}
/* Footer Styles */
footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 1em 0;
}
/* Media Queries for Responsive Design */
@media (max-width: 768px) {
    nav ul {
        flex-direction: column;
        gap: 0.5em;
    }
  #hero h2 {
        font-size: 2em;
    }
  #hero p {
        font-size: 1.2em;
    }
   #skills .skills-grid,
    #projects .projects-grid {
        flex-direction: column;
    }
    #skills .skill,
    #projects .project-card {
        width: 100%;
    }
}

   </style>
</head>
<body>
    <header>
        <div class="logo">
            <h1>My Portfolio</h1>
        </div>
        <nav>
            <ul>
                <li><a href="#about">About</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

 <section id="hero">
        <h2>Hello, I'm a Web Developer</h2>
        <p>Crafting beautiful and functional websites with passion.</p>
        <a href="#contact" class="cta">Get in Touch</a>
    </section>

 <section id="about" class="content-section">
        <h2>About Me</h2>
        <p>I'm a passionate web developer with fresher  in building responsive and visually appealing websites.</p>
    </section>

 <section id="skills" class="content-section">
        <h2>Skills</h2>
        <div class="skills-grid">
            <div class="skill">
                <h3>HTML</h3>
                <p>Semantic and accessible markup.</p>
            </div>
            <div class="skill">
                <h3>CSS</h3>
                <p>Modern layouts and animations.</p>
            </div>
            <div class="skill">
                <h3>JavaScript</h3>
                <p>Interactive and dynamic interfaces.</p>
            </div>
            <div class="skill">
                <h3>Core </h3>
                <p>for backend</p>
            </div>
        </div>
    </section>

<section id="projects" class="content-section">
        <h2>Projects</h2>
        <div class="projects-grid">
            <div class="project-card">
                <h3>Project 1</h3>
                <p>Responsive e-commerce website.</p>
            </div>
            <div class="project-card">
                <h3>Project 2</h3>
                <p>Interactive portfolio site.</p>
            </div>
            <div class="project-card">
                <h3>Project 3</h3>
                <p>Gallery</p>
            </div>
            <div class="project-card">
                <h3>Project 4</h3>
                <p>education website</p>
            </div>
        </div>
    </section>

<section id="contact" class="content-section">
        <h2>Contact</h2>
        <p>If you'd like to collaborate or just say hi, feel free to reach out to me at <a href="mailto:venukanchiraju122@gmail.com">youremail@example.com</a>.</p>
    </section>

 <footer>
        <p>&copy; 2024 My Portfolio. All rights reserved.</p>
    </footer>

  <script src="script.js">
      
      // Sticky Header on Scroll
window.addEventListener('scroll', function() {
    const header = document.querySelector('header');
    header.classList.toggle('scrolled', window.scrollY > 0);
});

// Smooth Scrolling for Navigation Links
document.querySelectorAll('nav ul li a').forEach(anchor => {
    anchor.addEventListener('click', function(e) {
        e.preventDefault();

        const targetId = this.getAttribute('href').substring(1);
        const targetElement = document.getElementById(targetId);

        window.scrollTo({
            top: targetElement.offsetTop - document.querySelector('header').offsetHeight,
            behavior: 'smooth'
        });
    });
});

    </script>
</body>
</html>
