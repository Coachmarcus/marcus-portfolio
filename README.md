<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Great Ola In Wealth - Portfolio</title>
<style>
/* Reset */
*{margin:0;padding:0;box-sizing:border-box;font-family:'Segoe UI',sans-serif;}
body{background:#f4f6f8;color:#333;scroll-behavior:smooth;line-height:1.6;}

/* Hero Section */
#hero{
  background: linear-gradient(135deg,#1f2a63,#ff704d);
  color:#fff;text-align:center;padding:6rem 1rem;position:relative;overflow:hidden;
}
#hero::before{
  content:"";position:absolute;top:0;left:0;width:200%;height:200%;
  background:linear-gradient(45deg,#ff6f61,#2a2a72,#ffecde,#ff704d);
  animation:moveBG 15s linear infinite;opacity:0.3;z-index:0;
}
@keyframes moveBG{
  0%{transform:translate(0,0);}
  50%{transform:translate(-50%,-50%);}
  100%{transform:translate(0,0);}
}
#hero img{position:relative;width:160px;height:160px;border-radius:50%;border:3px solid #fff;margin-bottom:1.5rem;animation:float 4s ease-in-out infinite;z-index:1;}
@keyframes float{0%,100%{transform:translateY(0);}50%{transform:translateY(-10px);}}
#hero h1{position:relative;font-size:2.8rem;margin-bottom:0.5rem;font-weight:700;z-index:1;}
#hero p{position:relative;font-size:1.2rem;margin-bottom:1.5rem;z-index:1;}
.btn{display:inline-block;padding:1rem 2rem;background:#fff;color:#1f2a63;font-weight:600;border-radius:8px;text-decoration:none;transition:0.3s;position:relative;z-index:1;animation:pulse 2s infinite;}
@keyframes pulse{0%,100%{transform:scale(1);}50%{transform:scale(1.1);}}
.btn:hover{background:#ffecde;color:#1f2a63;transform:scale(1.05);}

/* About Section */
#about{display:flex;flex-wrap:wrap;align-items:center;justify-content:center;padding:5rem 1rem;background:#fff;}
#about img{width:250px;height:250px;border-radius:12px;margin:1rem;object-fit:cover;}
#about .text{max-width:600px;margin:1rem;}
#about h2{color:#1f2a63;margin-bottom:1rem;font-size:2rem;}
#about p{margin-bottom:0.8rem;font-size:1rem;color:#555;}

/* Services Section */
#services{padding:5rem 1rem;background:#fefefe;text-align:center;}
#services h2{color:#1f2a63;margin-bottom:2rem;font-size:2rem;}
.service-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:1.5rem;}
.service-card{background:#fff;padding:2rem;border-radius:12px;box-shadow:0 4px 15px rgba(0,0,0,0.08);transition:0.3s;}
.service-card:hover{transform:translateY(-5px);}
.service-card img{width:70px;margin-bottom:1rem;}
.service-card h3{color:#1f2a63;margin-bottom:0.5rem;}
.service-card p{color:#555;font-size:0.95rem;}

/* Work Experience Section */
#experience{padding:5rem 1rem;background:#f4f6f8;text-align:center;}
#experience h2{color:#1f2a63;margin-bottom:2rem;font-size:2rem;}
.experience-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:1.5rem;}
.experience-card{background:#fff;padding:1.5rem;border-radius:12px;box-shadow:0 4px 12px rgba(0,0,0,0.08);transition:0.3s;}
.experience-card img{width:100%;height:150px;border-radius:10px;margin-bottom:0.8rem;object-fit:cover;}
.experience-card h3{color:#1f2a63;margin-bottom:0.3rem;}
.experience-card p{color:#555;font-size:0.9rem;margin-bottom:0.5rem;}

/* Testimonials Section */
#comments{padding:5rem 1rem;background:#fff;text-align:center;}
#comments h2{color:#1f2a63;margin-bottom:2rem;font-size:2rem;}
.testimonials{display:flex;overflow-x:auto;gap:1rem;padding-bottom:1rem;scroll-snap-type:x mandatory;scroll-behavior:smooth;}
.comment-card{flex:0 0 250px;background:#f4f6f8;padding:1.5rem;border-radius:12px;box-shadow:0 4px 12px rgba(0,0,0,0.08);scroll-snap-align:start;text-align:center;transition:0.3s;}
.comment-card img{width:60px;height:60px;border-radius:50%;margin-bottom:0.5rem;border:2px solid #1f2a63;}
.comment-card:hover{transform:scale(1.05);}

/* Work Location */
#office{padding:5rem 1rem;text-align:center;}
.map-container{position:relative;width:100%;max-width:900px;height:450px;margin:auto;border-radius:12px;overflow:hidden;box-shadow:0 4px 15px rgba(0,0,0,0.1);}
.pin{position:absolute;top:50%;left:50%;transform:translate(-50%,-100%);width:45px;height:45px;background:#ff704d;border-radius:50%;border:3px solid #fff;animation:bouncePin 2s infinite;}
@keyframes bouncePin{0%,100%{transform:translate(-50%,-100%) scale(1);}50%{transform:translate(-50%,-110%) scale(1.2);}}
.pin::after{content:"📍 Jbo Hotel and Suite, Osun State, Nigeria";position:absolute;top:55px;left:50%;transform:translateX(-50%);background:rgba(255,255,255,0.95);padding:0.6rem 1.2rem;border-radius:8px;font-size:14px;color:#333;white-space:nowrap;}
.map-container::before{content:"";position:absolute;top:0;left:0;width:100%;height:100%;background:url('https://cdn.pixabay.com/photo/2016/10/07/07/01/map-1728385_1280.jpg') center/cover no-repeat;opacity:0.8;}

/* Contact Section */
#contact{display:flex;flex-wrap:wrap;justify-content:center;padding:5rem 1rem;background:#fefefe;}
#contact .form{flex:1;min-width:300px;max-width:450px;margin:1rem;}
#contact .info{flex:1;min-width:250px;max-width:400px;margin:1rem;padding:1.5rem;background:#f4f6f8;border-radius:12px;}
#contact h2{color:#1f2a63;margin-bottom:1.5rem;font-size:2rem;}
#contact input,#contact textarea{width:100%;padding:1rem;margin-bottom:1rem;border-radius:10px;border:1px solid #ccc;font-size:1rem;}
#contact button{padding:1rem 2rem;border:none;background:#1f2a63;color:#fff;border-radius:10px;font-weight:bold;cursor:pointer;transition:0.3s;animation:pulse 2s infinite;}
#contact button:hover{background:#ff704d;transform:scale(1.05);}

/* Footer */
footer{background:#1f2a63;color:#fff;text-align:center;padding:2rem 0;font-size:0.95rem;}

/* Hamburger Menu */
#menu-btn{position:fixed;top:20px;left:20px;width:50px;height:50px;background:#ff704d;border-radius:50%;display:flex;flex-direction:column;justify-content:space-around;align-items:center;padding:10px;cursor:pointer;z-index:50;box-shadow:0 4px 12px rgba(0,0,0,0.3);}
#menu-btn div{width:28px;height:3px;background:#fff;border-radius:2px;}
#top-menu{position:fixed;top:80px;left:20px;background:#fff;border-radius:10px;overflow:hidden;display:none;flex-direction:column;box-shadow:0 6px 20px rgba(0,0,0,0.2);}
#top-menu a{padding:0.9rem 2rem;display:block;text-decoration:none;color:#1f2a63;font-weight:600;border-bottom:1px solid #eee;transition:0.3s;}
#top-menu a:last-child{border-bottom:none;}
#top-menu a:hover{background:#ff704d;color:#fff;}

/* WhatsApp Floating Button */
.customer-service img{width:65px;height:65px;cursor:pointer;position:fixed;bottom:20px;right:20px;transition:transform 0.3s;}
.customer-service img:hover{transform:scale(1.2);}

/* Responsive */
@media(max-width:768px){#about{flex-direction:column;}#contact{flex-direction:column;}}
</style>
</head>
<body>

<!-- Hero -->
<section id="hero">
  <img src="https://avatars.githubusercontent.com/u/171789491?v=4" alt="Great Ola In Wealth">
  <h1>Hello, I'm Great Ola In Wealth</h1>
  <p>Professional full stack web developer specializing in building modern, responsive websites and web applications that combine clean design, seamless functionality, and an exceptional user experience.</p>
  <a href="https://wa.me/2348144466868?text=Hi,%20I'm%20[Your Name]%20from%20your%20portfolio.%20I%20have%20a%20deal%20for%20you" class="btn" target="_blank">Hire Me</a>
</section>

<!-- About -->
<section id="about">
  <img src="https://picsum.photos/300/300?random=10" alt="Sharp Profile Image">
  <div class="text">
    <h2>About Me</h2>
    <p>I build websites, landing pages, and web applications with clean design, intuitive UI, and responsive layouts.</p>
    <p>Email: <a href="mailto:assistancepromoter@gmail.com">assistancepromoter@gmail.com</a></p>
    <p>Address: Jbo Hotel and Suites, Osun State, Nigeria</p>
  </div>
</section>

<!-- Services -->
<section id="services">
  <h2>Services</h2>
  <div class="service-grid">
    <div class="service-card">
      <img src="https://cdn-icons-png.flaticon.com/512/919/919847.png" alt="">
      <h3>Web & Frontend Development</h3>
      <p>HTML, CSS, JavaScript, React, responsive design, and clean UI.</p>
    </div>
    <div class="service-card">
      <img src="https://cdn-icons-png.flaticon.com/512/919/919825.png" alt="">
      <h3>Backend & APIs</h3>
      <p>Node.js, Express, database integration, scalable backend solutions.</p>
    </div>
    <div class="service-card">
      <img src="https://cdn-icons-png.flaticon.com/512/919/919836.png" alt="">
      <h3>Full Stack Solutions</h3>
      <p>Complete web applications, deployable projects, end-to-end solutions.</p>
    </div>
  </div>
</section>

<!-- Work Experience -->
<section id="experience">
  <h2>Work Experience</h2>
  <div class="experience-grid">
    <div class="experience-card">
      <img src="https://picsum.photos/400/150?random=1" alt="Frontend work">
      <h3>Frontend Developer - ABC Web Solutions</h3>
      <p>Jan 2024 – Present</p>
      <p>Built responsive landing pages and web applications using HTML, CSS, and React.</p>
    </div>
    <div class="experience-card">
      <img src="https://picsum.photos/400/150?random=2" alt="Backend work">
      <h3>Backend Developer - XYZ Tech</h3>
      <p>Jun 2023 – Dec 2023</p>
      <p>Developed REST APIs with Node.js and integrated databases for client projects.</p>
    </div>
    <div class="experience-card">
      <img src="https://picsum.photos/400/150?random=3" alt="Full stack project">
      <h3>Full Stack Developer - Freelance</h3>
      <p>2021 – 2023</p>
      <p>Delivered end-to-end web solutions for multiple clients globally.</p>
    </div>
  </div>
</section>

<!-- Testimonials -->
<section id="comments">
  <h2>Client Satisfaction</h2>
  <div class="testimonials">
    <div class="comment-card">
      <img src="https://randomuser.me/api/portraits/men/11.jpg" alt="">
      <p>"Delivered our website professionally and on time!"</p>
      <strong>- John D.</strong>
    </div>
    <div class="comment-card">
      <img src="https://randomuser.me/api/portraits/women/21.jpg" alt="">
      <p>"Highly recommend for web development projects."</p>
      <strong>- Sarah K.</strong>
    </div>
    <div class="comment-card">
      <img src="https://randomuser.me/api/portraits/men/31.jpg" alt="">
      <p>"Full stack project handled flawlessly."</p>
      <strong>- Michael R.</strong>
    </div>
  </div>
</section>

<!-- Work Location -->
<section id="office">
  <h2>Work Environment</h2>
  <div class="map-container"><div class="pin"></div></div>
</section>

<!-- Contact -->
<section id="contact">
  <div class="form">
    <h2>Contact Me</h2>
    <form action="mailto:assistancepromoter@gmail.com" method="post" enctype="text/plain">
      <input type="text" name="name" placeholder="Your Name" required>
      <input type="email" name="email" placeholder="Your Email" required>
      <textarea name="message" placeholder="Your Message" rows="5" required></textarea>
      <button type="submit">Send Message</button>
    </form>
  </div>
  <div class="info">
    <h2>Get in Touch</h2>
    <p>Email: assistancepromoter@gmail.com</p>
    <p>Address: Jbo Hotel and Suites, Osun State, Nigeria</p>
    <p>Phone: +2348144466868</p>
  </div>
</section>

<!-- Footer -->
<footer>
  <p>⭐⭐⭐ 4.8/5 Client Rating • 120+ Daily Visits</p>
  <p>&copy; 2025 Great Ola In Wealth. All rights reserved.</p>
</footer>

<!-- Hamburger -->
<div id="menu-btn"><div></div><div></div><div></div></div>
<div id="top-menu">
  <a href="#hero">Home</a>
  <a href="#about">About</a>
  <a href="#services">Services</a>
  <a href="#experience">Experience</a>
  <a href="#comments">Clients</a>
  <a href="#office">Work</a>
  <a href="#contact">Contact</a>
</div>

<!-- WhatsApp -->
<div class="customer-service">
  <img src="https://cdn-icons-png.flaticon.com/512/733/733585.png" alt="WhatsApp" onclick="window.open('https://wa.me/2348144466868?text=Hi,%20I\'m%20[Your Name]%20from%20your%20portfolio.%20I%20have%20a%20deal%20for%20you','_blank')">
</div>

<script>
const menuBtn=document.getElementById('menu-btn');
const topMenu=document.getElementById('top-menu');
menuBtn.addEventListener('click',()=>{topMenu.style.display=topMenu.style.display==='flex'?'none':'flex';topMenu.style.flexDirection='column';});
</script>

</body>
</html>
