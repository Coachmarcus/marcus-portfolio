<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Great Ola In Wealth - Web Developer Portfolio</title>
<style>
/* Reset */
* {margin:0;padding:0;box-sizing:border-box;font-family: Arial, sans-serif;}
body {line-height:1.6;color:#333;}

/* Moving background */
body::before {
  content:"";
  position:fixed;
  top:0;left:0;width:100%;height:100%;
  background: url('https://cdn.pixabay.com/photo/2017/03/22/22/59/computer-2168546_1280.jpg') repeat;
  background-size:cover;
  opacity:0.08;
  animation: moveBackground 60s linear infinite;
  z-index:-1;
}
@keyframes moveBackground {
  0% {background-position:0 0;}
  100% {background-position:2000px 1000px;}
}

/* Header */
header {
  background: rgba(26,26,46,0.95);
  color: #fff;
  padding: 1rem 0;
  position: sticky;
  top:0;
  z-index:10;
}
nav {
  display:flex;
  justify-content: space-between;
  align-items:center;
  width:90%;
  margin:auto;
}
nav img {height:50px; margin-right:10px;}
nav ul {display:flex; list-style:none;}
nav ul li {margin-left:1.5rem;}
nav ul li a {color:#fff;text-decoration:none;font-weight:bold;}
nav ul li a:hover {color:#ff6f61;}

/* Transparent sections */
section {
  width: 90%;
  max-width: 1000px;
  margin: 4rem auto;
  padding: 2rem;
  border-radius: 10px;
  background: rgba(255,255,255,0.85);
  box-shadow: 0 4px 15px rgba(0,0,0,0.1);
}

/* Hero / Introducing Me */
#hero {
  text-align:center;
  padding:4rem 2rem;
  background: rgba(246,211,101,0.2);
  color:#1a1a2e;
}
#hero img {
  width:180px;
  height:180px;
  border-radius:50%;
  border:3px solid #1a1a2e;
  margin-bottom:1.5rem;
}
#hero h2 {font-size:2.5rem;margin-bottom:1rem;}
.btn {
  display:inline-block;
  padding:0.8rem 2rem;
  background:#1a1a2e;
  color:#fff;
  text-decoration:none;
  border-radius:8px;
  margin-top:1rem;
  transition:0.3s;
}
.btn:hover {background:#ff6f61;}

/* Section headers */
h2 {text-align:center; margin-bottom:2rem; color:#1a1a2e;}

/* Service Cards */
.service-card {
  background: rgba(255,255,255,0.9);
  padding:1.5rem;
  margin-bottom:1.5rem;
  border-radius:10px;
  box-shadow:0 4px 6px rgba(0,0,0,0.1);
  text-align:center;
}
.service-card img {
  width:60px;
  margin:0 auto 1rem;
  display:block;
}

/* Client Satisfaction / Comments */
.comments {
  display:flex;
  flex-direction:column;
  gap:1.5rem;
}
.comment-card {
  background: rgba(240,240,240,0.9);
  padding:1rem;
  border-radius:8px;
  box-shadow:0 2px 6px rgba(0,0,0,0.1);
}

/* Office / Work Picture */
.office-pic {
  width:100%;
  max-height:400px;
  object-fit:cover;
  border-radius:10px;
  margin-top:2rem;
  box-shadow:0 4px 10px rgba(0,0,0,0.2);
}

/* Footer */
footer {
  text-align:center;
  padding:2rem 0;
  background: rgba(26,26,46,0.95);
  color:#fff;
  margin-top:2rem;
}

/* Responsive */
@media (max-width:768px){
  nav{flex-direction:column;}
  nav ul{flex-direction:column;margin-top:1rem;}
  nav ul li{margin-left:0;margin-bottom:0.5rem;}
  .comments{flex-direction:column;}
}
</style>
</head>
<body>

<!-- Header -->
<header>
  <nav>
    <div style="display:flex;align-items:center;">
      <img src="https://cdn-icons-png.flaticon.com/512/1055/1055646.png" alt="Logo">
      <h1>Great Ola In Wealth</h1>
    </div>
    <ul>
      <li><a href="#hero">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#services">Services</a></li>
      <li><a href="#comments">Clients</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
</header>

<!-- Hero / Introducing Me -->
<section id="hero">
  <img src="https://via.placeholder.com/180" alt="Your Picture">
  <h2>Hello, I'm Great Ola In Wealth</h2>
  <p>A full stack web developer delivering clean, professional web solutions.</p>
  <a href="#contact" class="btn">Hire Me</a>
</section>

<!-- About Section -->
<section id="about">
  <h2>About Me</h2>
  <p>I am a full stack web developer with experience building websites, landing pages, and web applications. I focus on clean design, responsiveness, and client satisfaction.</p>
</section>

<!-- Services Section -->
<section id="services">
  <h2>Services</h2>
  <div class="service-card">
    <img src="https://cdn-icons-png.flaticon.com/512/1055/1055646.png" alt="Frontend">
    <h3>Frontend Development</h3>
    <p>HTML, CSS, JavaScript, React — creating interactive and responsive UIs.</p>
  </div>
  <div class="service-card">
    <img src="https://cdn-icons-png.flaticon.com/512/1006/1006554.png" alt="Backend">
    <h3>Backend Development</h3>
    <p>Node.js, Express, MongoDB — building robust server-side applications.</p>
  </div>
  <div class="service-card">
    <img src="https://cdn-icons-png.flaticon.com/512/3163/3163470.png" alt="Full Stack">
    <h3>Full Stack Projects</h3>
    <p>Combining frontend and backend to deliver complete web solutions.</p>
  </div>
</section>

<!-- Client Satisfaction / Comments -->
<section id="comments">
  <h2>Client Satisfaction</h2>
  <div class="comments">
    <div class="comment-card">
      <p>"Great Ola delivered our website on time and exceeded our expectations!"</p>
      <strong>- Client A</strong>
    </div>
    <div class="comment-card">
      <p>"Professional, responsive, and very creative. Highly recommend!"</p>
      <strong>- Client B</strong>
    </div>
    <div class="comment-card">
      <p>"Our full stack project was handled efficiently and beautifully."</p>
      <strong>- Client C</strong>
    </div>
  </div>
</section>

<!-- Office Picture at Bottom -->
<section id="office">
  <h2>Work Environment</h2>
  <img class="office-pic" src="https://via.placeholder.com/1000x400" alt="Office / Laptop">
</section>

<!-- Contact Section -->
<section id="contact">
  <h2>Contact Me</h2>
  <p>Email: greatola@example.com</p>
  <p>Phone: +234 123 456 7890</p>
</section>

<!-- Footer -->
<footer>
  <p>&copy; 2025 Great Ola In Wealth. All rights reserved.</p>
</footer>

</body>
</html>nav ul li a:hover {color:#ff6f61;}

/* Hero Section */
#hero {
  text-align:center;
  padding:5rem 2rem;
  background: rgba(246,211,101,0.2);
  color: #1a1a2e;
}
#hero h2 {font-size:2.8rem;margin-bottom:1rem;}
.btn {
  display:inline-block;
  padding:0.8rem 2rem;
  background:#1a1a2e;
  color:#fff;
  text-decoration:none;
  border-radius:8px;
  margin-top:1rem;
  transition:0.3s;
}
.btn:hover {background:#ff6f61;}

/* Sections Headers */
h2 {text-align:center; margin-bottom:2rem; color:#1a1a2e;}

/* Service Cards */
.service-card {
  background: rgba(255,255,255,0.9);
  padding:1.5rem;
  margin-bottom:1.5rem;
  border-radius:10px;
  box-shadow:0 4px 6px rgba(0,0,0,0.1);
  text-align:center;
}
.service-card img {
  width:60px;
  margin:0 auto 1rem;
  display:block;
}

/* Profile Pictures */
.profile {
  display:flex;
  justify-content:center;
  gap:2rem;
  margin-top:2rem;
}
.profile img {
  width:150px;
  height:150px;
  object-fit:cover;
  border-radius:50%;
  border:3px solid #1a1a2e;
  box-shadow:0 4px 10px rgba(0,0,0,0.2);
}

/* Footer */
footer {
  text-align:center;
  padding:2rem 0;
  background: rgba(26,26,46,0.95);
  color:#fff;
  margin-top:2rem;
}

/* Responsive */
@media (max-width:768px){
  nav{flex-direction:column;}
  nav ul{flex-direction:column;margin-top:1rem;}
  nav ul li{margin-left:0;margin-bottom:0.5rem;}
  .profile {flex-direction:column;}
}
</style>
</head>
<body>

<!-- Header -->
<header>
  <nav>
    <div style="display:flex;align-items:center;">
      <img src="https://cdn-icons-png.flaticon.com/512/1055/1055646.png" alt="Logo">
      <h1>Great Ola In Wealth</h1>
    </div>
    <ul>
      <li><a href="#about">About</a></li>
      <li><a href="#services">Services</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
</header>

<!-- Hero Section -->
<section id="hero">
  <h2>Hi, I'm a Full Stack Developer</h2>
  <p>I create clean, modern, and professional web experiences.</p>
  <a href="#contact" class="btn">Hire Me</a>
</section>

<!-- About Section -->
<section id="about">
  <h2>About Me</h2>
  <p>I am a full stack web developer with experience building websites, landing pages, and web applications. My goal is to deliver professional, responsive, and functional solutions for clients.</p>
  
  <!-- Profile Pictures -->
  <div class="profile">
    <img src="https://via.placeholder.com/150" alt="Your Picture 1">
    <img src="https://via.placeholder.com/150" alt="Your Picture 2">
  </div>
</section>

<!-- Services Section -->
<section id="services">
  <h2>Services</h2>
  <div class="service-card">
    <img src="https://cdn-icons-png.flaticon.com/512/1055/1055646.png" alt="Frontend">
    <h3>Frontend Development</h3>
    <p>HTML, CSS, JavaScript, React — creating interactive and responsive UIs.</p>
  </div>
  <div class="service-card">
    <img src="https://cdn-icons-png.flaticon.com/512/1006/1006554.png" alt="Backend">
    <h3>Backend Development</h3>
    <p>Node.js, Express, MongoDB — building robust server-side applications.</p>
  </div>
  <div class="service-card">
    <img src="https://cdn-icons-png.flaticon.com/512/3163/3163470.png" alt="Full Stack">
    <h3>Full Stack Projects</h3>
    <p>Combining frontend and backend to deliver complete web solutions.</p>
  </div>
</section>

<!-- Contact Section -->
<section id="contact">
  <h2>Contact Me</h2>
  <p>Email: greatola@example.com</p>
  <p>Phone: +234 123 456 7890</p>
</section>

<!-- Footer -->
<footer>
  <p>&copy; 2025 Great Ola In Wealth. All rights reserved.</p>
</footer>

</body>
</html>
