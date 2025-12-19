<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Great Ola In Wealth Portfolio</title>
<style>
  /* Reset & Base */
  *{margin:0;padding:0;box-sizing:border-box;font-family:sans-serif;}
  body{background:linear-gradient(135deg,#2bc0e4,#eaecc6);color:#111;line-height:1.6;}
  a{text-decoration:none;color:inherit;}

  /* Container */
  .container{width:90%;max-width:1200px;margin:0 auto;padding:50px 0;}

  /* Hero */
  .hero{text-align:center;padding:80px 20px;}
  .hero img{width:180px;height:180px;border-radius:50%;border:3px solid #fff;transition:transform 0.3s;}
  .hero img:hover{transform:scale(1.1);}
  .hero h1{font-size:3rem;margin:20px 0;color:#111;}
  .hero p{font-size:1.2rem;color:#333;margin-bottom:20px;}
  .hero .buttons{display:flex;justify-content:center;gap:15px;flex-wrap:wrap;}
  .hero .buttons a{padding:12px 25px;border-radius:10px;background:#111;color:#fff;font-weight:600;transition:0.3s;}
  .hero .buttons a:hover{background:#444;}

  /* About */
  .about{text-align:center;padding:60px 20px;}
  .about h2{font-size:2.5rem;margin-bottom:20px;color:#111;}
  .about p{font-size:1.1rem;color:#222;max-width:800px;margin:0 auto 30px;}
  .skills{display:flex;justify-content:center;flex-wrap:wrap;gap:15px;}
  .skills span{background:#fff;padding:10px 20px;border-radius:10px;color:#111;transition:0.3s;}
  .skills span:hover{background:#444;color:#fff;}

  /* Projects */
  .projects{padding:60px 20px;}
  .projects h2{text-align:center;font-size:2.5rem;margin-bottom:40px;color:#111;}
  .project-cards{display:grid;grid-template-columns:repeat(auto-fit,minmax(280px,1fr));gap:25px;}
  .card{background:#fff;border-radius:15px;overflow:hidden;transition:transform 0.3s,box-shadow 0.3s;cursor:pointer;}
  .card:hover{transform:translateY(-10px);box-shadow:0 10px 25px rgba(0,0,0,0.3);}
  .card img{width:100%;display:block;}
  .card-content{padding:20px;}
  .card-content h3{margin-bottom:10px;font-size:1.5rem;color:#111;}
  .card-content p{font-size:1rem;color:#333;}
  .card-content a{display:inline-block;margin-top:10px;padding:8px 18px;border-radius:8px;background:#111;color:#fff;transition:0.3s;}
  .card-content a:hover{background:#444;}

  /* Contact */
  .contact{text-align:center;padding:60px 20px;background:rgba(255,255,255,0.2);border-radius:20px;margin-top:50px;}
  .contact h2{font-size:2.5rem;margin-bottom:20px;color:#111;}
  .contact p{font-size:1.1rem;margin-bottom:10px;color:#111;}
  .contact a{display:inline-block;margin:10px;padding:12px 25px;border-radius:10px;background:#111;color:#fff;transition:0.3s;}
  .contact a:hover{background:#444;}

  footer{text-align:center;padding:20px;color:#111;}

  /* Responsive */
  @media(max-width:768px){.hero h1{font-size:2.2rem;}.about h2,.projects h2,.contact h2{font-size:2rem;}}
</style>
</head>
<body>
<div class="container">

  <!-- Hero -->
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

  <!-- About -->
  <section class="about">
    <h2>About Me</h2>
    <p>Hello! I’m Great Ola In Wealth, a passionate web and creative designer. I specialize in creating interactive and luxury digital experiences that stand out. My work combines creativity, technology, and precision to deliver professional results.</p>
    <div class="skills">
      <span>UI/UX Design</span>
      <span>Web Development</span>
      <span>Branding</span>
      <span>Animation</span>
      <span>Creative Direction</span>
    </div>
  </section>

  <!-- Projects -->
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

  <!-- Contact -->
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
