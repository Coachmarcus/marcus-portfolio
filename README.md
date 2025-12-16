<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Great Ola In Wealth - Portfolio</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, sans-serif;
    }

    body {
      line-height: 1.6;
      color: #333;
    }

    header {
      background-color: #1a1a2e;
      color: #fff;
      padding: 1rem 0;
    }

    nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      width: 90%;
      margin: auto;
    }

    nav ul {
      display: flex;
      list-style: none;
    }

    nav ul li {
      margin-left: 1.5rem;
    }

    nav ul li a {
      color: #fff;
      text-decoration: none;
      font-weight: bold;
    }

    #hero {
      text-align: center;
      padding: 5rem 2rem;
      background: linear-gradient(135deg, #f6d365, #fda085);
      color: #1a1a2e;
    }

    #hero h2 {
      font-size: 2.8rem;
      margin-bottom: 1rem;
    }

    .btn {
      display: inline-block;
      padding: 0.8rem 2rem;
      background: #1a1a2e;
      color: #fff;
      text-decoration: none;
      border-radius: 8px;
      margin-top: 1rem;
      transition: background 0.3s;
    }

    .btn:hover {
      background: #ff6f61;
    }

    section {
      width: 90%;
      max-width: 1000px;
      margin: 4rem auto;
      padding: 2rem;
      border-radius: 10px;
    }

    #about {
      background-color: #e0f7fa;
    }

    #services {
      background-color: #f1f8e9;
    }

    #contact {
      background-color: #fff3e0;
    }

    h2 {
      text-align: center;
      margin-bottom: 2rem;
      color: #1a1a2e;
    }

    .service-card {
      background: #fff;
      padding: 1.5rem;
      margin-bottom: 1.5rem;
      border-radius: 10px;
      box-shadow: 0 4px 6px rgba(0,0,0,0.1);
    }

    footer {
      text-align: center;
      padding: 2rem 0;
      background: #1a1a2e;
      color: #fff;
      margin-top: 2rem;
    }

    @media (max-width: 768px) {
      nav {
        flex-direction: column;
      }
      nav ul {
        flex-direction: column;
        margin-top: 1rem;
      }
      nav ul li {
        margin-left: 0;
        margin-bottom: 0.5rem;
      }
    }
  </style>
</head>
<body>
  <header>
    <nav>
      <h1>Great Ola In Wealth</h1>
      <ul>
        <li><a href="#about">About</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section id="hero">
    <h2>Hi, I'm a Full Stack Developer</h2>
    <p>I create simple and clean web experiences for individuals and businesses.</p>
    <a href="#contact" class="btn">Hire Me</a>
  </section>

  <section id="about">
    <h2>About Me</h2>
    <p>I am a full stack web developer skilled in building websites, landing pages, and web applications. My goal is to deliver clean, responsive, and functional solutions for my clients.</p>
  </section>

  <section id="services">
    <h2>Services</h2>
    <div class="service-card">
      <h3>Frontend Development</h3>
      <p>HTML, CSS, JavaScript, React — creating interactive and responsive UIs.</p>
    </div>
    <div class="service-card">
      <h3>Backend Development</h3>
      <p>Node.js, Express, MongoDB — building robust server-side applications.</p>
    </div>
    <div class="service-card">
      <h3>Full Stack Projects</h3>
      <p>Combining frontend and backend to deliver complete web solutions.</p>
    </div>
  </section>

  <section id="contact">
    <h2>Contact Me</h2>
    <p>Email: greatola@example.com</p>
    <p>Phone: +234 123 456 7890</p>
  </section>

  <footer>
    <p>&copy; 2025 Great Ola In Wealth. All rights reserved.</p>
  </footer>
</body>
</html>
