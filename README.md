<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>My Portfolio</h1>
        <nav>
            <ul>
                <li><a href="#about">About Me</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="about">
        <h2>About Me</h2>
        <p>Hi, I'm [Your Name], a web developer passionate about creating user-friendly websites.</p>
    </section>

    <section id="projects">
        <h2>Projects</h2>
        <div class="project">
            <h3>Project 1</h3>
            <p>Description of your project.</p>
            <a href="https://example.com">View Project</a>
        </div>
        <div class="project">
            <h3>Project 2</h3>
            <p>Description of your project.</p>
            <a href="https://example.com">View Project</a>
        </div>
    </section>

    <section id="skills">
        <h2>Skills</h2>
        <ul>
            <li>HTML</li>
            <li>CSS</li>
            <li>JavaScript</li>
        </ul>
    </section>

    <section id="contact">
        <h2>Contact Me</h2>
        <form>
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            <label for="message">Message:</label>
            <textarea id="message" name="message" required></textarea>
            <button type="submit">Send</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2024 My Portfolio</p>
    </footer>
    <script src="script.js"></script>
</body>
</html>


// Smooth scrolling for navigation links
document.querySelectorAll('nav a').forEach(anchor => {
    anchor.addEventListener('click', function(e) {
        e.preventDefault();
        document.querySelector(this.getAttribute('href')).scrollIntoView({
            behavior: 'smooth'
        });
    });
});


body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    margin: 0;
    padding: 0;
    color: #333;
}

header {
    background: #333;
    color: #fff;
    padding: 1rem 0;
    text-align: center;
}

header ul {
    list-style: none;
    padding: 0;
}

header ul li {
    display: inline;
    margin: 0 15px;
}

header a {
    color: #fff;
    text-decoration: none;
}

section {
    padding: 20px;
    margin: 10px auto;
    max-width: 800px;
}

.project {
    background: #f4f4f4;
    padding: 15px;
    margin: 10px 0;
    border-radius: 5px;
}

form input, form textarea {
    width: 100%;
    padding: 10px;
    margin: 5px 0;
    border: 1px solid #ccc;
    border-radius: 5px;
}

button {
    background: #333;
    color: #fff;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}
