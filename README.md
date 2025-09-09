<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Reddi's Portfolio</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    /* Reset and base styles */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Segoe UI', sans-serif;
      background-color: #f9f9f9;
      color: #333;
      line-height: 1.6;
    }

    /* Navigation */
    header {
      background-color: #0077cc;
      color: white;
      padding: 20px 0;
      text-align: center;
    }
    nav a {
      color: white;
      margin: 0 15px;
      text-decoration: none;
      font-weight: bold;
    }

    /* Sections */
    section {
      padding: 40px 20px;
      max-width: 1000px;
      margin: auto;
    }
    h2 {
      color: #0077cc;
      margin-bottom: 20px;
    }

    /* Projects */
    .project {
      background-color: #fff;
      padding: 20px;
      margin-bottom: 20px;
      border-left: 5px solid #0077cc;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }

    /* Contact Form */
    form {
      background-color: #fff;
      padding: 20px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }
    input, textarea {
      width: 100%;
      padding: 10px;
      margin-bottom: 15px;
      border: 1px solid #ccc;
      border-radius: 4px;
    }
    button {
      background-color: #0077cc;
      color: white;
      border: none;
      padding: 10px 20px;
      border-radius: 4px;
      cursor: pointer;
    }
    button:hover {
      background-color: #005fa3;
    }

    /* Footer */
    footer {
      text-align: center;
      padding: 20px;
      background-color: #eee;
      font-size: 0.9em;
    }

    /* Responsive */
    @media (max-width: 600px) {
      nav a {
        display: block;
        margin: 10px 0;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>Reddi's Web Portfolio</h1>
    <nav>
      <a href="#about">About</a>
      <a href="#projects">Projects</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <section id="about">
    <h2>About Me</h2>
    <p>Hello! I'm Reddi Roopa Sree, a passionate web development intern at ApexPlanet Software Pvt. Ltd. I love building clean, responsive websites using HTML, CSS, and JavaScript. This portfolio showcases my learning journey and hands-on projects.</p>
  </section>

  <section id="projects">
    <h2>Projects</h2>
    <div class="project">
      <h3>Simple Landing Page</h3>
      <p>A responsive landing page built with HTML and CSS, featuring smooth scrolling and modern layout.</p>
    </div>
    <div class="project">
      <h3>Interactive Quiz App</h3>
      <p>JavaScript-powered quiz with dynamic scoring and feedback. Great for learning DOM manipulation.</p>
    </div>
  </section>

  <section id="contact">
    <h2>Contact Me</h2>
    <form id="contactForm">
      <input type="text" id="name" placeholder="Your Name" required>
      <input type="email" id="email" placeholder="Your Email" required>
      <textarea id="message" rows="5" placeholder="Your Message" required></textarea>
      <button type="submit">Send Message</button>
    </form>
  </section>

  <footer>
    &copy; 2025 Reddi | Built with ❤️ using HTML, CSS & JavaScript
  </footer>

  <script>
    // Contact form interactivity
    document.getElementById("contactForm").addEventListener("submit", function(e) {
      e.preventDefault();
      const name = document.getElementById("name").value;
      alert("Thank you, " + name + "! Your message has been sent.");
      this.reset();
    });
  </script>

</body>
</html>
