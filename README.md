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
# INDEX.HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nithyasree | Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>

    <!-- HEADER -->
    <header>
        <div class="container">
            <div class="header-wrapper">

                <div>
                    <h1 class="brand">Nithyasree</h1>
                    <p class="tagline">Web Developer</p>
                </div>

                <div class="social-links">
                    <img src="profile.jpg" alt="Profile" class="header-img">

                    <a href="https://github.com/Nithyasree1206/" target="_blank" title="GitHub">
                        GitHub
                    </a>

                    <a href="https://www.linkedin.com/in/nithyasree-learner" target="_blank" title="LinkedIn">
                        LinkedIn
                    </a>

                    <a href="https://www.instagram.com/ms_nithyasree" target="_blank" title="Instagram">
                        Instagram
                    </a>
                </div>

            </div>
        </div>
    </header>

    <!-- MAIN CONTENT -->
    <main class="container">

        <div class="accordion">

            <!-- HOME -->
            <div class="item">
                <button class="header" onclick="toggle(this)">▶ Home</button>
                <div class="content">
                    <div class="home-wrapper">
                        <div>
                            <p>Building elegant digital products with modern web technologies.</p>
                            <a href="#contact" class="btn">Get Started</a>
                        </div>
                        <img src="profile.jpg" alt="Nithyasree" class="profile-img">
                    </div>
                </div>
            </div>

            <!-- ABOUT -->
            <div class="item">
                <button class="header" onclick="toggle(this)">▶ About</button>
                <div class="content">
                    <p>
                        Passionate developer crafting high-performing web experiences.
                        Focused on responsive design and clean code.
                    </p>
                </div>
            </div>

            <!-- SKILLS -->
            <div class="item">
                <button class="header" onclick="toggle(this)">▶ Skills</button>
                <div class="content">
                    <div class="skills">
                        <span>HTML5</span>
                        <span>CSS3</span>
                        <span>JavaScript</span>
                        <span>Python</span>
                        <span>Flask</span>
                        <span>MySQL</span>
                        <span>GitHub</span>
                        <span>VS Code</span>
                    </div>
                </div>
            </div>

            <!-- CONTACT -->
            <div class="item">
                <button class="header" onclick="toggle(this)">▶ Contact</button>
                <div class="content">
                    <form>
                        <input type="text" placeholder="Name" required>
                        <input type="email" placeholder="Email" required>
                        <textarea placeholder="Message" rows="3" required></textarea>
                        <button type="submit" class="btn">Send</button>
                    </form>
                </div>
            </div>

        </div>

    </main>

    <!-- FOOTER -->
    <footer>
        <p>&copy; 2026 Nithyasree</p>
    </footer>
</body>
</html>
```

## STYLE.CSS

````
/* RESET */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* BODY */
body {
    font-family: "Segoe UI", Geneva, sans-serif;
    background: #f3f6fb;
    color: #172033;
    line-height: 1.6;
}

/* CONTAINER */
.container {
    width: min(1100px, 92%);
    margin: 0 auto;
}

/* HEADER */
header {
    background: #fff;
    border-bottom: 1px solid #e0e0e0;
    padding: 1.5rem 0;
}

.header-wrapper {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

/* SOCIAL LINKS */
.social-links {
    display: flex;
    gap: 1.5rem;
    align-items: center;
}

.header-img {
    width: 50px;
    height: 50px;
    border-radius: 50%;
    object-fit: cover;
    border: 2px solid #3f63ff;
}

.social-links a {
    text-decoration: none;
    color: #3f63ff;
    font-weight: 600;
    font-size: 0.9rem;
    transition: color 0.3s;
}

.social-links a:hover {
    color: #2f4be6;
}

/* BRAND */
.brand {
    font-size: 1.8rem;
    font-weight: 700;
}

.tagline {
    font-size: 0.9rem;
    color: #5d6982;
    margin-top: 0.5rem;
}

/* MAIN */
main {
    padding: 2rem 0;
}

/* ACCORDION */
.accordion {
    display: flex;
    flex-direction: column;
    gap: 1rem;
}

.item {
    border: 1px solid #d8e0ef;
    border-radius: 8px;
    overflow: hidden;
}

.header {
    width: 100%;
    padding: 1rem;
    background: #f9f9f9;
    border: none;
    cursor: pointer;
    font-weight: 600;
    text-align: left;
    font-size: 1rem;
}

.header:hover {
    background: #f0f0f0;
}

.content {
    padding: 1rem;
    display: none;
    background: #fff;
    border-top: 1px solid #e0e0e0;
}

/* HOME SECTION */
.home-wrapper {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 2rem;
}

.profile-img {
    width: 150px;
    height: 150px;
    border-radius: 50%;
    object-fit: cover;
    border: 3px solid #3f63ff;
    flex-shrink: 0;
}

/* SKILLS */
.skills {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
    margin-top: 0.5rem;
}

.skills span {
    background: #3f63ff;
    color: #fff;
    padding: 0.5rem 1rem;
    border-radius: 20px;
    font-size: 0.85rem;
    font-weight: 600;
}

/* FORM */
form {
    display: flex;
    flex-direction: column;
    gap: 0.8rem;
    max-width: 500px;
}

input,
textarea {
    border: 1px solid #d8e0ef;
    padding: 0.75rem;
    border-radius: 6px;
    font-family: inherit;
    font-size: 0.95rem;
}

/* BUTTON */
.btn {
    background: #3f63ff;
    color: #fff;
    border: 0;
    padding: 0.75rem 1.5rem;
    border-radius: 6px;
    cursor: pointer;
    font-weight: 600;
    display: inline-block;
}

.btn:hover {
    background: #2f4be6;
}

/* FOOTER */
footer {
    border-top: 1px solid #e0e0e0;
    padding: 1.5rem;
    text-align: center;
    color: #5d6982;
    background: #f3f6fb;
    margin-top: 2rem;
}
````

## OUTPUT
<img width="1897" height="898" alt="image" src="https://github.com/user-attachments/assets/7d0725d7-4d8e-4aec-b278-7b200f5b542f" />
`

<img width="1882" height="823" alt="image" src="https://github.com/user-attachments/assets/ae3a7a0c-a491-4429-acd0-01e4835d6917" />
`

<img width="1870" height="905" alt="image" src="https://github.com/user-attachments/assets/42deae66-5c34-494c-ae05-1e331680d00d" />


## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
