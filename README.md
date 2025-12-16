<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Great Ola In Wealth - Portfolio</title>
<style>
/* Reset */
* {margin:0;padding:0;box-sizing:border-box;font-family: Arial, sans-serif;}
body {line-height:1.6;color:#333;}

/* Moving background effect */
body::before {
  content:"";
  position:fixed;
  top:0;left:0;width:100%;height:100%;
  background: url('https://cdn.pixabay.com/photo/2017/03/22/22/59/computer-2168546_1280.jpg') no-repeat center center;
  background-size:cover;
  opacity:0.05;
  z-index:-1;
}

/* Header */
header {
  background-color: #1a1a2e;
  color: #fff;
  padding: 1rem 0;
  position: sticky;
  top: 0;
  z-index: 10;
}
nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 90%;
  margin: auto;
}
nav img {height:50px; margin-right:10px;}
nav ul {display:flex; list-style:none;}
nav ul li {margin-left:1.5rem;}
nav ul li a {color:#fff;text-decoration:none;font-weight:bold;}
nav ul li a:hover {color:#ff6f61;}

/* Hero Section */
#hero {
  text-align: center;
  padding: 5rem 2rem;
  background: linear-gradient(135deg, #f6d365, #fda085);
  color: #1a1a2e;
}
#hero h2 {font-size:2.8rem; margin-bottom:1rem;}
.btn {
  display: inline-block;
  padding:0.8rem 2rem;
  background:#1a1a2e;
  color:#fff;
  text-decoration:none;
  border-radius:8px;
  margin-top:1rem;
  transition:0.3s;
}
.btn:hover {background:#ff6f61;}

/* Sections */
section {
  width: 90%;
  max-width: 1000px;
  margin: 4rem auto;
  padding: 2rem;
  border-radius: 10px;
}
#about {background-color:#e0f7fa;}
#services {background-color:#f1f8e9;}
#contact {background-color:#fff3e0;}
h2 {text-align:center; margin-bottom:2rem; color:#1a1a2e;}

/* Service Cards */
.service-card {
  background:#fff;
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

/* Footer */
footer {
  text-align:center;
  padding:2rem 0;
  background:#1a1a2e;
  color:#fff;
  margin-top:2rem;
}

/* Responsive */
@media (max-width:768px){
  nav{flex-direction:column;}
  nav ul{flex-direction:column;margin-top:1rem;}
  nav ul li{margin-left:0;margin-bottom:0.5rem;}
}
</style>
</head>
<body>

<!-- Header with Logo -->
<header>
  <nav>
    <div style="display:flex; align-items:center;">
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
  <p>I create simple, clean, and professional web experiences.</p>
  <a href="#contact" class="btn">Hire Me</a>
</section>

<!-- About Section -->
<section id="about">
  <h2>About Me</h2>
  <p>I am a full stack web developer with experience building websites, landing pages, and web applications. My goal is to deliver clean, responsive, and functional solutions that impress clients.</p>
</section>

<!-- Services Section -->
<section id="services">
  <h2>Services</h2>
  <div class="service-card">
    <img src="https://cdn-icons-png.flaticon.com/512/1055/1055646.png" alt="Frontend">
    <h3>Frontend Development</h3>
    <p>HTML, CSS, JavaScript, React — creating interactive and responsive user interfaces.</p>
  </div>
  <div class="service-card">
    <img src="https://cdn-icons-png.flaticon.com/512/1006/1006554.png" alt="Backend">
    <h3>Backend Development</h3>
    <p>Node.js, Express, MongoDB — building robust server-side applications.</p>
  </div>
  <div class="service-card">
    <img src="https://cdn-icons-png.flaticon.com/512/3163/3163470.png" alt="Full Stack">
    <h3>Full Stack Projects</h3>
    <p>Combining frontend and backend to deliver complete web solutions for clients.</p>
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
