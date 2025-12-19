<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Great Ola In Wealth Portfolio</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    * { margin:0; padding:0; box-sizing:border-box; font-family:'Poppins', sans-serif; }
    body { background: linear-gradient(135deg, #0f2027, #203a43, #2c5364); color:#fff; }
    a { text-decoration:none; color:inherit; }
    .container { width:90%; max-width:1200px; margin:0 auto; padding:50px 0; }

    /* Hero Section */
    .hero { text-align:center; padding:100px 20px; }
    .hero img { width:180px; height:180px; border-radius:50%; border:4px solid #fff; transition:transform 0.3s; }
    .hero img:hover { transform:scale(1.1); }
    .hero h1 { font-size:3rem; margin:20px 0 10px; text-shadow:2px 2px 8px rgba(0,0,0,0.5); }
    .hero p { font-size:1.2rem; color:#ccc; margin-bottom:20px; }
    .hero .buttons { display:flex; justify-content:center; gap:15px; flex-wrap:wrap; }
    .hero .buttons a { padding:12px 25px; border-radius:10px; background:linear-gradient(45deg,#6a11cb,#2575fc); color:#fff; font-weight:600; transition:0.3s; }
    .hero .buttons a:hover { background:linear-gradient(45deg,#2575fc,#6a11cb); }

    /* About / Skills */
    .about { text-align:center; padding:60px 20px; }
    .about h2 { font-size:2.5rem; margin-bottom:20px; color:#fff; }
    .about p { font-size:1.1rem; color:#ddd; max-width:800px; margin:0 auto 30px; line-height:1.6; }
    .skills { display:flex; justify-content:center; flex-wrap:wrap; gap:15px; }
    .skills span { background:rgba(255,255,255,0.1); padding:10px 20px; border-radius:10px; transition:0.3s; }
    .skills span:hover { background:linear-gradient(45deg,#2575fc,#6a11cb); color:#fff; }

    /* Projects Section */
    .projects { padding:60px 20px; }
    .projects h2 { text-align:center; font-size:2.5rem; margin-bottom:40px; }
    .project-cards { display:grid; grid-template-columns:repeat(auto-fit,minmax(280px,1fr)); gap:25px; }
    .card { background:rgba(255,255,255,0.05); border-radius:15px; overflow:hidden; transition:transform 0.3s, box-shadow 0.3s; backdrop-filter:blur(5px); }
    .card:hover { transform:translateY(-10px); box-shadow:0 15px 25px rgba(0,0,0,0.5); }
    .card img { width:100%; display:block; }
    .card-content { padding:20px; }
    .card-content h3 { margin-bottom:10px; font-size:1.5rem; }
    .card-content p { font-size:1rem; color:#ccc; line-height:1.5; }
    .card-content a { display:inline-block; margin-top:10px; padding:8px 18px; border-radius:8px; background:#2575fc; color:#fff; transition:0.3s; }
    .card-content a:hover { background:#6a11cb; }

    /* Contact Section */
    .contact { text-align:center; padding:60px 20px; background:rgba(0,0,0,0.2); border-radius:20px; margin-top:50px; }
    .contact h2 { font-size:2.5rem; margin-bottom:20px; }
    .contact p { font-size:1.1rem; margin-bottom:10px; }
    .contact a { display:inline-block; margin:10px; padding:12px 25px; border-radius:10px; background:linear-gradient(45deg,#6a11cb,#2575fc); color:#fff; transition:0.3s; }
    .contact a:hover { background:linear-gradient(45deg,#2575fc,#6a11cb); }

    /* Footer */
    footer { text-align:center; padding:20px; color:#ccc; }

    /* Responsive */
    @media(max-width:768px){ .hero h1{font-size:2.2rem;} .about h2,.projects h2,.contact h2{font-size:2rem;} }
  </style>
</head>
<body>

  <div class="container">

    <!-- Hero Section -->
    <section class="hero">
      <img src="https://avatars.githubusercontent.com/u/171789491?v=4" alt="Profile Picture">
      <h1>Great Ola In Wealth</h1>
      <p>Luxury Portfolio | Web & Creative Design | Osun State, Nigeria</p>
      <div class="buttons">
        <a href="https://wa.me/2348144466868?text=Greetings" target="_blank">WhatsApp</a>
        <a href="mailto:assistancepromoter@gmail.com">Email Me</a>
        <a href="https://www.behance.net/olamilemarcus" target="_blank">Behance</a>
      </div>
    </section>

    <!-- About Section -->
    <section class="about">
      <h2>About Me</h2>
      <p>Hello! I’m Great Ola In Wealth, a passionate web and creative designer. I specialize in creating sharp, interactive, and luxury digital experiences that stand out. My work combines creativity, technology, and precision to deliver professional results for clients worldwide.</p>
      <div class="skills">
        <span>UI/UX Design</span>
        <span>Web Development</span>
        <span>Branding</span>
        <span>Animation</span>
        <span>Creative Direction</span>
      </div>
    </section>

    <!-- Projects Section -->
    <section class="projects">
      <h2>My Projects</h2>
      <div class="project-cards">
        <div class="card">
          <img src="https://via.placeholder.com/400x250.png?text=Project+1" alt="Project 1">
          <div class="card-content">
            <h3>Project One</h3>
            <p>Interactive and responsive web design highlighting modern UI patterns.</p>
            <a href="#">View Project</a>
          </div>
        </div>
        <div class="card">
          <img src="https://via.placeholder.com/400x250.png?text=Project+2" alt="Project 2">
          <div class="card-content">
            <h3>Project Two</h3>
            <p>Luxury creative design combining animation, typography, and interactivity.</p>
            <a href="#">View Project</a>
          </div>
        </div>
        <div class="card">
          <img src="https://via.placeholder.com/400x250.png?text=Project+3" alt="Project 3">
          <div class="card-content">
            <h3>Project Three</h3>
            <p>Professional digital solution delivering a sharp, modern user experience.</p>
            <a href="#">View Project</a>
          </div>
        </div>
      </div>
    </section>

    <!-- Contact Section -->
    <section class="contact">
      <h2>Get in Touch</h2>
      <p>Location: Osun State, Nigeria</p>
      <a href="https://wa.me/2348144466868?text=Greetings" target="_blank">WhatsApp Me</a>
      <a href="mailto:assistancepromoter@gmail.com">Email Me</a>
      <a href="https://www.behance.net/olamilemarcus" target="_blank">View My Behance</a>
    </section>

  </div>

  <footer>
    &copy; 2025 Great Ola In Wealth | All Rights Reserved
  </footer>

</body>
</html>
