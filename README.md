<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Great Ola In Wealth - Portfolio</title>
<style>
/* Reset */
* {margin:0;padding:0;box-sizing:border-box;font-family: Arial, sans-serif;}
body {line-height:1.6;color:#333;scroll-behavior:smooth;position:relative;background:#f2f2f2;}

/* Background */
body::before {
  content:"";
  position:fixed;
  top:0; left:0;
  width:100%; height:100%;
  background: url('https://cdn.pixabay.com/photo/2017/03/22/22/59/computer-2168546_1280.jpg') repeat;
  background-size:cover;
  opacity:0.08;
  animation: moveBG 120s linear infinite;
  z-index:-1;
}
@keyframes moveBG {0% {background-position:0 0;} 100% {background-position:2000px 1000px;}}

/* Sections */
section {
  width:90%;
  max-width:900px;
  margin:4rem auto;
  padding:2rem;
  border-radius:12px;
  background: rgba(255,255,255,0.95);
  box-shadow: 0 5px 20px rgba(0,0,0,0.1);
  text-align:center;
  position:relative;
}

/* Hero */
#hero img {
  width:180px;
  height:180px;
  border-radius:50%;
  border:3px solid #2a2a72;
  margin-bottom:1.5rem;
}
#hero h2 {font-size:2.5rem;margin-bottom:0.5rem;color:#2a2a72;}
#hero p {margin-bottom:1.5rem;color:#444;}
.btn {
  display:inline-block;
  padding:0.8rem 2rem;
  background:#2a2a72;
  color:#fff;
  border-radius:8px;
  font-weight:bold;
  text-decoration:none;
  transition:0.3s;
  margin:0.5rem;
  animation: pulse 2s infinite;
}
.btn:hover {background:#ff6f61;}
@keyframes pulse {0%,100%{transform: scale(1);}50%{transform: scale(1.1);}}

/* Services */
.service-card {
  background: rgba(240,240,250,0.95);
  padding:1.5rem;
  border-radius:10px;
  margin-bottom:1.5rem;
  display:flex;
  flex-direction:column;
  align-items:center;
}
.service-card img {
  width:80px;
  margin-bottom:1rem;
}

/* Testimonials */
.comments {
  display:flex;
  flex-wrap:wrap;
  justify-content:center;
  gap:1rem;
}
.comment-card {
  width:220px;
  background: rgba(250,250,250,0.95);
  padding:1rem;
  border-radius:10px;
  box-shadow:0 2px 6px rgba(0,0,0,0.1);
  text-align:center;
}
.comment-card img {
  width:60px;height:60px;border-radius:50%;margin-bottom:0.5rem;border:2px solid #2a2a72;
}

/* Floating WhatsApp button */
.customer-service {
  position:fixed;
  bottom:20px;
  right:20px;
  z-index:50;
}
.customer-service img {
  width:60px;
  height:60px;
  cursor:pointer;
  transition: transform 0.3s;
}
.customer-service img:hover {transform: scale(1.2);}

/* Office picture */
.office-pic {
  width:100%;
  max-height:400px;
  object-fit:cover;
  border-radius:10px;
  box-shadow:0 4px 12px rgba(0,0,0,0.1);
  margin-top:1.5rem;
}

/* Contact Form */
#contact form {
  display:flex;
  flex-direction:column;
  gap:1rem;
  max-width:500px;
  margin:auto;
}
#contact input, #contact textarea {
  padding:0.8rem;
  border-radius:8px;
  border:1px solid #ccc;
  width:100%;
}
#contact button {
  padding:0.8rem 2rem;
  border:none;
  background:#2a2a72;
  color:#fff;
  border-radius:8px;
  font-weight:bold;
  cursor:pointer;
}
#contact button:hover {background:#ff6f61;}

/* Footer */
footer {
  text-align:center;
  padding:2rem 0;
  background:#2a2a72;
  color:#fff;
  margin-top:3rem;
  font-size:14px;
}

/* Hamburger Menu Top-Left */
#menu-btn {
  position: fixed;
  top:20px;
  left:20px;
  width:50px;
  height:50px;
  background:#ff6f61;
  border-radius:50%;
  display:flex;
  flex-direction:column;
  justify-content:space-around;
  align-items:center;
  padding:10px;
  cursor:pointer;
  z-index:30;
  box-shadow:0 4px 12px rgba(0,0,0,0.3);
  animation: bounce 2s infinite;
}
#menu-btn div {
  width:25px;
  height:3px;
  background:#fff;
  border-radius:2px;
}
@keyframes bounce {0%,100%{transform: translateY(0);}50%{transform: translateY(-5px);}}

/* Top-left menu */
#top-menu {
  position: fixed;
  top:80px;
  left:20px;
  background: rgba(255,255,255,0.95);
  border-radius:10px;
  overflow:hidden;
  display:none;
  flex-direction: column;
  box-shadow:0 4px 15px rgba(0,0,0,0.2);
}
#top-menu a {
  padding:0.8rem 2rem;
  display:block;
  text-decoration:none;
  color:#2a2a72;
  font-weight:bold;
  border-bottom:1px solid #ddd;
}
#top-menu a:last-child{border-bottom:none;}
#top-menu a:hover{background:#ff6f61;color:#fff;}

/* Responsive */
@media(max-width:768px){.comments{flex-direction:column;align-items:center;}}
</style>
</head>
<body>

<!-- Hero Section -->
<section id="hero">
  <img src="YOUR_PICTURE.jpg" alt="Your Picture">
  <h2>Hello, I'm Great Ola In Wealth</h2>
  <p>A full stack web developer delivering clean, professional web solutions.</p>
  <a href="https://wa.me/2348144466868?text=Hi,%20I'm%20[Your Name]%20from%20your%20portfolio.%20I%20have%20a%20deal%20for%20you" class="btn" target="_blank">Hire Me</a>
</section>

<!-- About -->
<section id="about">
  <h2>About Me</h2>
  <p>I build websites, landing pages, and web apps with clean design, responsive layouts, and great client satisfaction.</p>
  <p>Email: <a href="mailto:assistancepromoter@gmail.com">assistancepromoter@gmail.com</a></p>
</section>

<!-- Services -->
<section id="services">
  <h2>Services</h2>
  <div class="service-card">
    <img src="https://cdn-icons-png.flaticon.com/512/919/919847.png" alt="Web design icon">
    <h3>Web & Frontend Development</h3>
    <p>HTML, CSS, JavaScript, React, responsive design, and more.</p>
  </div>
  <div class="service-card">
    <img src="https://cdn-icons-png.flaticon.com/512/919/919825.png" alt="Backend icon">
    <h3>Backend & APIs</h3>
    <p>Node.js, Express, database integration, server work, and more.</p>
  </div>
  <div class="service-card">
    <img src="https://cdn-icons-png.flaticon.com/512/919/919836.png" alt="Full stack icon">
    <h3>Full Stack Solutions</h3>
    <p>Complete web applications and deployable projects.</p>
  </div>
</section>

<!-- Testimonials -->
<section id="comments">
  <h2>Client Satisfaction</h2>
  <div class="comments">
    <div class="comment-card">
      <img src="https://randomuser.me/api/portraits/men/11.jpg" alt="Client A">
      <p>"Great Ola delivered our website on time!"</p>
      <strong>- John D.</strong>
    </div>
    <div class="comment-card">
      <img src="https://randomuser.me/api/portraits/women/21.jpg" alt="Client B">
      <p>"Professional, responsive, highly recommend!"</p>
      <strong>- Sarah K.</strong>
    </div>
    <div class="comment-card">
      <img src="https://randomuser.me/api/portraits/men/31.jpg" alt="Client C">
      <p>"Full stack project handled beautifully."</p>
      <strong>- Michael R.</strong>
    </div>
  </div>
</section>

<!-- Office Image -->
<section id="office">
  <h2>Work Environment</h2>
  <img class="office-pic" src="https://unsplash.com/photos/black-and-brown-chairs-and-tables-DyFjxmHt3Es.jpg" alt="Tech work environment">
</section>

<!-- Contact Form -->
<section id="contact">
  <h2>Contact Me</h2>
  <form action="mailto:assistancepromoter@gmail.com" method="post" enctype="text/plain">
    <input type="text" name="name" placeholder="Your Name" required>
    <input type="email" name="email" placeholder="Your Email" required>
    <textarea name="message" placeholder="Your Message" rows="5" required></textarea>
    <button type="submit">Send Message</button>
  </form>
</section>

<!-- Footer -->
<footer>
  <p>⭐⭐⭐ 4.8/5 Client Rating • 120+ Daily Visits</p>
  <p>&copy; 2025 Great Ola In Wealth. All rights reserved.</p>
</footer>

<!-- Top-Left Hamburger -->
<div id="menu-btn">
  <div></div><div></div><div></div>
</div>
<div id="top-menu">
  <a href="#hero">Home</a>
  <a href="#about">About</a>
  <a href="#services">Services</a>
  <a href="#comments">Clients</a>
  <a href="#office">Work</a>
  <a href="#contact">Contact</a>
</div>

<!-- Floating WhatsApp Button -->
<div class="customer-service">
  <img src="https://cdn-icons-png.flaticon.com/512/733/733585.png" alt="WhatsApp" 
  onclick="window.open('https://wa.me/2348144466868?text=Hi,%20I\'m%20[Your Name]%20from%20your%20portfolio.%20I%20have%20a%20deal%20for%20you','_blank')">
</div>

<script>
const menuBtn = document.getElementById('menu-btn');
const topMenu = document.getElementById('top-menu');
menuBtn.addEventListener('click', ()=>{
  topMenu.style.display = topMenu.style.display === 'flex' ? 'none' : 'flex';
  topMenu.style.flexDirection = 'column';
});
</script>

</body>
</html>
