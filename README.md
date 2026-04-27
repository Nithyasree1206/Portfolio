# Ex01 Portfolio
## Date:27/04/2026

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
# index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nithyasree | Professional Portfolio</title>
    <meta name="description" content="Professional portfolio of Nithyasree - developer focused on modern web experiences.">
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header class="site-header">
        <nav class="navbar container">
            <a class="brand" href="#home">Nithyasree</a>
            <ul class="nav-links" id="navLinks">
                <li><a href="#about">About</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#experience">Experience</a></li>
                <li><a href="#achievements">Achievements</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
            <div class="nav-actions">
                <button class="theme-toggle" id="themeToggle" aria-label="Toggle theme">
                    <span class="theme-icon">🌙</span>
                </button>
                <button class="menu-btn" id="menuBtn" aria-label="Toggle menu">☰</button>
            </div>
        </nav>
    </header>

    <main>
        <section id="home" class="hero section">
            <div class="container hero-grid">
                <div class="hero-content">
                    <p class="eyebrow">Software Developer</p>
                    <h1>Building elegant digital products with a professional edge.</h1>
                    <p class="subtitle">
                        I am <strong>Nithyasree</strong>, a results-focused developer creating high-performing web experiences.
                        <span class="typing-wrap">I specialize in <span id="typingText"></span></span>
                    </p>
                    <div class="hero-cta">
                        <button class="btn btn-primary" id="downloadResumeBtn">Download Resume</button>
                        <a class="btn btn-ghost" href="#projects">View Projects</a>
                    </div>
                    <div class="stats">
                        <div class="stat-card">
                            <h3>20+</h3>
                            <p>Projects Delivered</p>
                        </div>
                        <div class="stat-card">
                            <h3>2+</h3>
                            <p>Years Learning & Building</p>
                        </div>
                        <div class="stat-card">
                            <h3>100%</h3>
                            <p>Focus on Quality</p>
                        </div>
                    </div>
                </div>
                <aside class="hero-image-wrap">
                    <img class="hero-image" src="profile.jpg" alt="Nithyasree profile image">
                </aside>
            </div>
        </section>

        <section id="about" class="section">
            <div class="container">
                <p class="eyebrow">Royal Profile</p>
                <h2 class="section-title">About Me</h2>
                <div class="about-royal-card">
                    <p class="section-text">
                        I am <strong>Nithyasree</strong>, a passionate developer with a refined approach to digital creation.
                        I craft elegant, high-performing web experiences that blend modern technology with premium visual quality.
                    </p>
                    <p class="section-text">
                        With a strong focus on clarity, consistency, and user delight, I aim to deliver products that feel both
                        professional and timeless - built with purpose, precision, and pride.
                    </p>
                    <div class="about-royal-points">
                        <span>Elegant UI Thinking</span>
                        <span>Professional Delivery</span>
                        <span>Quality-First Development</span>
                    </div>
                </div>
            </div>
        </section>

        <section id="skills" class="section alt">
            <div class="container">
                <h2 class="section-title">Tech Stack & Skills</h2>
                <div class="skills-board">
                    <div class="skills-group">
                        <h3>Languages</h3>
                        <div class="skill-grid">
                            <span class="skill-pill orange">HTML5</span>
                            <span class="skill-pill blue">CSS3</span>
                            <span class="skill-pill yellow">JavaScript</span>
                            <span class="skill-pill sky">Python</span>
                            <span class="skill-pill royal">C</span>
                            <span class="skill-pill steel">SQL</span>
                        </div>
                    </div>
                    <div class="skills-group">
                        <h3>Frameworks & Libraries</h3>
                        <div class="skill-grid">
                            <span class="skill-pill dark">Flask</span>
                            <span class="skill-pill violet">OpenCV</span>
                            <span class="skill-pill tangerine">DeepFace</span>
                        </div>
                    </div>
                    <div class="skills-group">
                        <h3>Databases & Tools</h3>
                        <div class="skill-grid">
                            <span class="skill-pill steel">MySQL</span>
                            <span class="skill-pill dark">JSON</span>
                            <span class="skill-pill blue">VS Code</span>
                            <span class="skill-pill dark">GitHub</span>
                            <span class="skill-pill amber">Google Colab</span>
                            <span class="skill-pill tangerine">Jupyter</span>
                            <span class="skill-pill cyan">Canva</span>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section id="projects" class="section">
            <div class="container">
                <h2 class="section-title">Featured Projects</h2>
                <div class="project-grid">
                    <article class="project-card" data-title="Frontend E-Commerce Website" data-description="A modern responsive e-commerce website with product listing, shopping cart flow, and smooth UI animations for a polished shopping experience.">
                        <div class="project-tags">
                            <span class="project-tag">Web</span>
                            <span class="project-tag">Frontend</span>
                        </div>
                        <h3>Frontend E-Commerce Website</h3>
                        <p>A modern responsive e-commerce website with product listing, cart system, and smooth UI animations.</p>
                        <button class="text-btn" type="button">View details</button>
                    </article>
                    <article class="project-card" data-title="Gesture Cricket" data-description="An interactive cricket game controlled using hand gestures, combining computer vision concepts and AI-based interaction for an engaging gameplay experience.">
                        <div class="project-tags">
                            <span class="project-tag">AI</span>
                            <span class="project-tag">Python</span>
                        </div>
                        <h3>Gesture Cricket</h3>
                        <p>An interactive cricket game controlled using hand gestures for a fun and AI-based experience.</p>
                        <button class="text-btn" type="button">View details</button>
                    </article>
                    <article class="project-card" data-title="FoodMood Recommender" data-description="A smart recommendation app that suggests food based on user mood using simple AI logic and sentiment-driven ideas.">
                        <div class="project-tags">
                            <span class="project-tag">App</span>
                            <span class="project-tag">AI</span>
                        </div>
                        <h3>FoodMood Recommender</h3>
                        <p>A smart system that recommends food based on user mood using simple AI logic and sentiment idea.</p>
                        <button class="text-btn" type="button">View details</button>
                    </article>
                    <article class="project-card" data-title="Invoice Billing System" data-description="A billing system that generates invoices, calculates totals, and manages customer transactions with a simple fullstack workflow.">
                        <div class="project-tags">
                            <span class="project-tag">Web</span>
                            <span class="project-tag">Fullstack</span>
                        </div>
                        <h3>Invoice Billing System</h3>
                        <p>A billing system that generates invoices, calculates totals, and manages customer transactions easily.</p>
                        <button class="text-btn" type="button">View details</button>
                    </article>
                    <article class="project-card" data-title="Photobooth App" data-description="A fun photobooth web app with filters, frames, and image download feature for capturing and saving memories.">
                        <div class="project-tags">
                            <span class="project-tag">Web</span>
                            <span class="project-tag">Flask</span>
                        </div>
                        <h3>Photobooth App</h3>
                        <p>A fun photobooth web app with filters, frames, and download feature for capturing memories.</p>
                        <button class="text-btn" type="button">View details</button>
                    </article>
                    <article class="project-card" data-title="Figma UI/UX Designs" data-description="A collection of modern UI/UX designs created in Figma with clean layout systems and user-friendly interaction patterns.">
                        <div class="project-tags">
                            <span class="project-tag">Design</span>
                            <span class="project-tag">UI/UX</span>
                        </div>
                        <h3>Figma UI/UX Designs</h3>
                        <p>Modern UI/UX designs created in Figma with clean layouts and user-friendly interfaces.</p>
                        <button class="text-btn" type="button">View details</button>
                    </article>
                </div>
            </div>
        </section>

        <section id="experience" class="section alt">
            <div class="container">
                <h2 class="section-title">Experience</h2>
                <div class="timeline">
                    <div class="timeline-item">
                        <h3>Frontend Developer</h3>
                        <p class="timeline-meta">Freelance | 2024 - Present</p>
                        <p>Developed responsive websites and UI components for client requirements using modern front-end standards.</p>
                    </div>
                    <div class="timeline-item">
                        <h3>Software Development Intern</h3>
                        <p class="timeline-meta">Internship | 2023 - 2024</p>
                        <p>Collaborated on feature implementations, bug fixes, and performance improvements in web applications.</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="achievements" class="section">
            <div class="container">
                <p class="eyebrow">Recognition</p>
                <h2 class="section-title">Achievements & Certifications</h2>
                <div class="achievement-grid">
                    <article class="achievement-card">
                        <h3>Winner - ASTRANOVA'26 UXPLORE</h3>
                        <p class="achievement-org">St. Joseph College of Engineering, Sriperumbudur</p>
                        <p>Secured winner position in a competitive UI/UX innovation event.</p>
                    </article>
                    <article class="achievement-card">
                        <h3>Infosys Certification</h3>
                        <p class="achievement-org">Infosys</p>
                        <p>Successfully completed professional certification program.</p>
                    </article>
                    <article class="achievement-card">
                        <h3>AWS Cloud Badges</h3>
                        <p class="achievement-org">Amazon Web Services</p>
                        <p>Earned badges demonstrating cloud computing knowledge.</p>
                    </article>
                    <article class="achievement-card">
                        <h3>Be10x AI Tools Workshop</h3>
                        <p class="achievement-org">Be10x</p>
                        <p>Completed training on modern AI tools and productivity techniques.</p>
                    </article>
                    <article class="achievement-card">
                        <h3>IBM Datathon Participation</h3>
                        <p class="achievement-org">IBM</p>
                        <p>Participated in a data-driven hackathon focused on analytics.</p>
                    </article>
                    <article class="achievement-card">
                        <h3>Spidy Bot Hackathon</h3>
                        <p class="achievement-org">Sairam Engineering College</p>
                        <p>Worked on innovative robotics and tech solutions in a hackathon.</p>
                    </article>
                    <article class="achievement-card">
                        <h3>Infyra Technical Event</h3>
                        <p class="achievement-org">Sairam Institute of Technology</p>
                        <p>Participated in a technical innovation and development event.</p>
                    </article>
                    <article class="achievement-card">
                        <h3>Coursera Certification - DBMS</h3>
                        <p class="achievement-org">Coursera</p>
                        <p>Completed course on Database Management Systems.</p>
                    </article>
                </div>
            </div>
        </section>

        <section id="contact" class="section">
            <div class="container contact-wrap">
                <div>
                    <h2 class="section-title">Contact</h2>
                    <p class="section-text">Ready to collaborate on your next project? Send a message and I will get back to you soon.</p>
                </div>
                <form class="contact-form" id="contactForm">
                    <input type="text" name="name" placeholder="Your Name" required>
                    <input type="email" name="email" placeholder="Your Email" required>
                    <textarea name="message" rows="5" placeholder="Tell me about your project" required></textarea>
                    <button class="btn btn-primary" type="submit">Send Message</button>
                </form>
            </div>
        </section>
    </main>

    <div id="projectModal" class="modal" aria-hidden="true">
        <div class="modal-content">
            <button class="close" id="closeModalBtn" aria-label="Close modal">&times;</button>
            <h3 id="modalTitle"></h3>
            <p id="modalDescription"></p>
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html>
```
# style.css
```
:root {
    --bg: #f3f6fb;
    --surface: #ffffff;
    --surface-muted: #eef2fa;
    --text: #172033;
    --text-muted: #5d6982;
    --primary: #3f63ff;
    --primary-dark: #2f4be6;
    --border: #d8e0ef;
    --shadow: 0 14px 35px rgba(21, 37, 89, 0.12);
}

body.dark {
    --bg: #0f1728;
    --surface: #172033;
    --surface-muted: #11192c;
    --text: #e5ecff;
    --text-muted: #aab7d6;
    --primary: #7f9aff;
    --primary-dark: #9ab0ff;
    --border: #2b3753;
    --shadow: 0 14px 40px rgba(0, 0, 0, 0.45);
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
    background: var(--bg);
    color: var(--text);
    line-height: 1.6;
    transition: background 0.3s ease, color 0.3s ease;
}

.container {
    width: min(1100px, 92%);
    margin: 0 auto;
}

.section {
    padding: 92px 0;
    min-height: 100vh;
    display: flex;
    align-items: center;
}

.section.alt {
    background: var(--surface-muted);
}

.section-title {
    font-size: 2rem;
    margin-bottom: 18px;
}

.section-text {
    color: var(--text-muted);
    max-width: 760px;
}

#about {
    background:
        radial-gradient(circle at 12% 20%, color-mix(in srgb, #cfa94f 20%, transparent), transparent 35%),
        radial-gradient(circle at 88% 80%, color-mix(in srgb, var(--primary) 14%, transparent), transparent 32%);
}

.about-royal-card {
    margin-top: 12px;
    padding: 26px;
    border-radius: 18px;
    border: 1px solid color-mix(in srgb, var(--border) 75%, #cfa94f 25%);
    background: linear-gradient(
        145deg,
        color-mix(in srgb, var(--surface) 92%, #cfa94f 8%),
        color-mix(in srgb, var(--surface-muted) 92%, #6d54d8 8%)
    );
    box-shadow: var(--shadow);
}

.about-royal-card .section-text + .section-text {
    margin-top: 12px;
}

.about-royal-points {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-top: 18px;
}

.about-royal-points span {
    border: 1px solid color-mix(in srgb, var(--border) 70%, #cfa94f 30%);
    border-radius: 999px;
    padding: 7px 12px;
    font-size: 0.86rem;
    font-weight: 700;
    color: color-mix(in srgb, var(--text) 88%, #b88b2f 12%);
    background: color-mix(in srgb, var(--surface) 86%, #cfa94f 14%);
}

.site-header {
    position: sticky;
    top: 0;
    z-index: 1000;
    backdrop-filter: blur(10px);
    background: color-mix(in srgb, var(--surface) 86%, transparent);
    border-bottom: 1px solid var(--border);
}

.navbar {
    min-height: 88px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 16px;
}

.brand {
    color: var(--text);
    font-weight: 700;
    font-size: 1.35rem;
    text-decoration: none;
}

.nav-links {
    list-style: none;
    display: flex;
    gap: 22px;
}

.nav-links a {
    text-decoration: none;
    color: var(--text-muted);
    font-weight: 600;
    font-size: 1.02rem;
}

.nav-links a:hover {
    color: var(--primary);
}

.nav-actions {
    display: flex;
    align-items: center;
    gap: 10px;
}

.theme-toggle,
.menu-btn {
    border: 1px solid var(--border);
    background: var(--surface);
    color: var(--text);
    width: 46px;
    height: 46px;
    border-radius: 10px;
    cursor: pointer;
}

.menu-btn {
    display: none;
    font-size: 1.15rem;
}

.hero {
    padding-top: 70px;
    min-height: calc(100vh - 88px);
    background: linear-gradient(135deg, color-mix(in srgb, var(--primary) 12%, var(--bg)), var(--bg));
}

.hero-grid {
    display: grid;
    grid-template-columns: 2fr 1fr;
    gap: 28px;
    align-items: stretch;
}

.hero-content h1 {
    font-size: clamp(2rem, 4vw, 3.2rem);
    line-height: 1.2;
    margin: 12px 0 16px;
    max-width: 750px;
}

.eyebrow {
    color: var(--primary);
    font-weight: 700;
    letter-spacing: 0.04em;
    text-transform: uppercase;
    font-size: 0.8rem;
}

.subtitle {
    max-width: 760px;
    color: var(--text-muted);
}

#typingText {
    color: var(--primary);
    font-weight: 700;
    border-right: 2px solid var(--primary);
    padding-right: 4px;
}

.hero-cta {
    margin: 28px 0;
    display: flex;
    flex-wrap: wrap;
    gap: 12px;
}

.btn {
    border: 0;
    border-radius: 12px;
    padding: 11px 18px;
    font-weight: 600;
    cursor: pointer;
    text-decoration: none;
    display: inline-block;
}

.btn-primary {
    background: var(--primary);
    color: #ffffff;
}

.btn-primary:hover {
    background: var(--primary-dark);
}

.btn-ghost {
    border: 1px solid var(--border);
    color: var(--text);
    background: var(--surface);
}

.stats {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 14px;
}

.stat-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 16px;
    padding: 16px;
    box-shadow: var(--shadow);
}

.stat-card h3 {
    font-size: 1.4rem;
}

.stat-card p {
    color: var(--text-muted);
    font-size: 0.9rem;
}

.hero-image-wrap {
    background: linear-gradient(160deg, var(--surface), var(--surface-muted));
    border: 1px solid var(--border);
    border-radius: 20px;
    padding: 14px;
    box-shadow: var(--shadow);
    display: flex;
    align-items: center;
    justify-content: center;
}

.hero-image {
    width: 100%;
    height: 100%;
    max-height: 460px;
    object-fit: cover;
    border-radius: 14px;
    display: block;
}

.skills-board {
    margin-top: 10px;
    background: #060c23;
    border: 1px solid #1c2446;
    border-radius: 18px;
    padding: 22px;
    box-shadow: 0 14px 34px rgba(4, 9, 28, 0.45);
}

.skills-group + .skills-group {
    margin-top: 18px;
}

.skills-group h3 {
    color: #d6e3ff;
    margin-bottom: 10px;
    font-size: 1.05rem;
}

.skill-grid {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
}

.skill-pill {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-height: 32px;
    padding: 7px 12px;
    border-radius: 6px;
    font-size: 0.77rem;
    font-weight: 700;
    letter-spacing: 0.06em;
    text-transform: uppercase;
    color: #ffffff;
}

.skill-pill.orange { background: #e45c27; }
.skill-pill.blue { background: #1f7ad6; }
.skill-pill.yellow { background: #f0ce2a; color: #2f2a10; }
.skill-pill.sky { background: #4a8dcb; }
.skill-pill.royal { background: #1060b5; }
.skill-pill.steel { background: #4e78a7; }
.skill-pill.dark { background: #0d0f15; border: 1px solid #2a324d; }
.skill-pill.violet { background: #5640cc; }
.skill-pill.tangerine { background: #f1841f; }
.skill-pill.amber { background: #efb100; color: #2f2a10; }
.skill-pill.cyan { background: #1fbec9; }

.project-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 18px;
}

.project-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 18px;
    padding: 22px;
    box-shadow: var(--shadow);
}

.project-card h3 {
    margin-bottom: 10px;
}

.project-card p {
    color: var(--text-muted);
}

.project-tags {
    display: flex;
    gap: 8px;
    margin-bottom: 12px;
}

.project-tag {
    font-size: 0.72rem;
    text-transform: uppercase;
    letter-spacing: 0.05em;
    border: 1px solid var(--border);
    border-radius: 999px;
    padding: 4px 9px;
    color: var(--primary);
    background: color-mix(in srgb, var(--primary) 10%, var(--surface));
    font-weight: 700;
}

.text-btn {
    margin-top: 14px;
    border: 0;
    background: transparent;
    color: var(--primary);
    cursor: pointer;
    font-weight: 700;
}

.timeline {
    display: grid;
    gap: 16px;
}

.timeline-item {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 14px;
    padding: 20px;
}

.timeline-meta {
    color: var(--primary);
    font-size: 0.92rem;
    margin-bottom: 8px;
}

.achievement-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 14px;
}

.achievement-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 14px;
    padding: 16px;
    box-shadow: var(--shadow);
}

.achievement-card h3 {
    margin-bottom: 8px;
    font-size: 1.02rem;
}

.achievement-org {
    color: var(--primary);
    font-weight: 600;
    margin-bottom: 8px;
    font-size: 0.9rem;
}

.achievement-card p {
    color: var(--text-muted);
}

.contact-wrap {
    display: grid;
    grid-template-columns: 1.2fr 1fr;
    gap: 24px;
    align-items: start;
}

.contact-form {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 16px;
    padding: 20px;
    box-shadow: var(--shadow);
}

.contact-form input,
.contact-form textarea {
    width: 100%;
    border: 1px solid var(--border);
    border-radius: 10px;
    background: var(--bg);
    color: var(--text);
    padding: 12px;
    margin-bottom: 12px;
}

.modal {
    display: none;
    position: fixed;
    inset: 0;
    background: rgba(0, 0, 0, 0.55);
    z-index: 2000;
    place-items: center;
    padding: 16px;
}

.modal.show {
    display: grid;
}

.modal-content {
    width: min(560px, 100%);
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 16px;
    padding: 22px;
}

.close {
    margin-left: auto;
    display: block;
    border: 0;
    background: transparent;
    color: var(--text-muted);
    font-size: 1.7rem;
    cursor: pointer;
}

@media (max-width: 900px) {
    .hero-grid,
    .contact-wrap {
        grid-template-columns: 1fr;
    }

    .project-grid,
    .achievement-grid {
        grid-template-columns: repeat(2, 1fr);
    }

    .stats {
        grid-template-columns: 1fr;
    }
}

@media (max-width: 700px) {
    .menu-btn {
        display: inline-grid;
        place-items: center;
    }

    .nav-links {
        position: absolute;
        top: 88px;
        right: 4%;
        width: min(260px, 92vw);
        background: var(--surface);
        border: 1px solid var(--border);
        border-radius: 12px;
        padding: 16px;
        display: none;
        flex-direction: column;
        gap: 12px;
    }

    .nav-links.open {
        display: flex;
    }

    .project-grid,
    .achievement-grid {
        grid-template-columns: 1fr;
    }
}
```
# script.js
```
const body = document.body;
const themeToggle = document.getElementById("themeToggle");
const themeIcon = document.querySelector(".theme-icon");
const menuBtn = document.getElementById("menuBtn");
const navLinks = document.getElementById("navLinks");
const typingText = document.getElementById("typingText");
const projectCards = document.querySelectorAll(".project-card");
const projectModal = document.getElementById("projectModal");
const modalTitle = document.getElementById("modalTitle");
const modalDescription = document.getElementById("modalDescription");
const closeModalBtn = document.getElementById("closeModalBtn");
const contactForm = document.getElementById("contactForm");
const downloadResumeBtn = document.getElementById("downloadResumeBtn");

const roles = [
    "Frontend Development",
    "Responsive UI Engineering",
    "Modern JavaScript Interfaces"
];

let roleIndex = 0;
let charIndex = 0;
let deleting = false;

function applyTheme(theme) {
    const isDark = theme === "dark";
    body.classList.toggle("dark", isDark);
    themeIcon.textContent = isDark ? "☀️" : "🌙";
    localStorage.setItem("portfolioTheme", theme);
}

themeToggle.addEventListener("click", () => {
    const nextTheme = body.classList.contains("dark") ? "light" : "dark";
    applyTheme(nextTheme);
});

const savedTheme = localStorage.getItem("portfolioTheme") || "light";
applyTheme(savedTheme);

menuBtn.addEventListener("click", () => {
    navLinks.classList.toggle("open");
});

document.querySelectorAll(".nav-links a").forEach((link) => {
    link.addEventListener("click", () => {
        navLinks.classList.remove("open");
    });
});

function typeEffect() {
    const current = roles[roleIndex];

    if (!deleting) {
        typingText.textContent = current.slice(0, charIndex + 1);
        charIndex += 1;
        if (charIndex === current.length) {
            deleting = true;
            setTimeout(typeEffect, 1300);
            return;
        }
    } else {
        typingText.textContent = current.slice(0, charIndex - 1);
        charIndex -= 1;
        if (charIndex === 0) {
            deleting = false;
            roleIndex = (roleIndex + 1) % roles.length;
        }
    }

    const delay = deleting ? 50 : 85;
    setTimeout(typeEffect, delay);
}

typeEffect();

function showModal(title, description) {
    modalTitle.textContent = title;
    modalDescription.textContent = description;
    projectModal.classList.add("show");
    projectModal.setAttribute("aria-hidden", "false");
}

function hideModal() {
    projectModal.classList.remove("show");
    projectModal.setAttribute("aria-hidden", "true");
}

projectCards.forEach((card) => {
    const button = card.querySelector(".text-btn");
    button.addEventListener("click", () => {
        showModal(card.dataset.title, card.dataset.description);
    });
});

closeModalBtn.addEventListener("click", hideModal);

projectModal.addEventListener("click", (event) => {
    if (event.target === projectModal) {
        hideModal();
    }
});

document.addEventListener("keydown", (event) => {
    if (event.key === "Escape") {
        hideModal();
    }
});

contactForm.addEventListener("submit", (event) => {
    event.preventDefault();
    alert("Thank you for your message. I will contact you soon.");
    contactForm.reset();
});

downloadResumeBtn.addEventListener("click", () => {
    alert("Resume download can be connected to your PDF file.");
});

```
## OUTPUT
# HOME PAGE
<img width="1915" height="963" alt="web1" src="https://github.com/user-attachments/assets/693e8299-a186-4afe-a15a-374582747eeb" />
## ABOUT PAGE
<img width="1918" height="956" alt="web2" src="https://github.com/user-attachments/assets/c9e8916a-2746-42ee-85aa-7e1c5fdea50e" />

# SKILLS PAGE
<img width="1918" height="956" alt="web3" src="https://github.com/user-attachments/assets/3973bf51-b61c-413d-aa90-63a66e8d8f9d" />

# PROJECTS PAGE
<img width="1918" height="935" alt="web4" src="https://github.com/user-attachments/assets/189f286e-6803-404b-baa1-a3e7a439b659" />

# EXPERIENCE PAGE
<img width="1916" height="927" alt="web5" src="https://github.com/user-attachments/assets/109ceb85-d571-4846-a924-2fb2abb0575d" />

# ACHIEVEMENTS PAGE
<img width="1918" height="955" alt="web6" src="https://github.com/user-attachments/assets/1bb9affc-0f76-4aa8-8c3a-91f115dc0008" />

# CONTACT PAGE
<img width="1910" height="905" alt="web7" src="https://github.com/user-attachments/assets/c27c4664-6c2c-4a9e-a294-58bbe5783a6b" />

## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
