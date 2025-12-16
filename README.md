<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Great Ola In Wealth - Portfolio</title>
<style>
/* Reset */
* {margin:0;padding:0;box-sizing:border-box;font-family: Arial, sans-serif;}
body {line-height:1.6;color:#333;scroll-behavior:smooth;position:relative;}

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
  background: rgba(255,255,255,0.9);
  box-shadow: 0 5px 20px rgba(0,0,0,0.1);
  text-align:center;
  position:relative;
}

/* Hero */
#hero img {
  width:180px;
  height:180px;
  border-radius:50%;
  border:3px solid #1a1a2e;
  margin-bottom:1.5rem;
}
#hero h2 {font-size:2.5rem;margin-bottom:0.5rem;}
#hero p {margin-bottom:1.5rem;color:#444;}
.btn {
  display:inline-block;
  padding:0.8rem 2rem;
  background:#ff6f61;
  color:#fff;
  border-radius:8px;
  font-weight:bold;
  text-decoration:none;
  transition:0.3s;
  margin:0.5rem;
  animation: pulse 2s infinite;
}
.btn:hover {background:#ff4b3e;}
@keyframes pulse {0%,100%{transform: scale(1);}50%{transform: scale(1.1);}}

/* Services */
.service-card {
  background: rgba(240,240,240,0.95);
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
  width:60px;height:60px;border-radius:50%;margin-bottom:0.5rem;border:2px solid #1a1a2e;
}

/* Floating customer service icons */
.customer-service {
  position:fixed;
  bottom:20px;
  right:20px;
  display:flex;
  flex-direction:column;
  gap:1rem;
  z-index:50;
}
.customer-service img {
  width:50px;
  height:50px;
  border-radius:50%;
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

/* Footer */
footer {text-align:center;padding:2rem 0;background:#1a1a2e;color:#fff;margin-top:3rem;}

/* Hamburger Menu Top-Right */
#menu-btn {
  position: fixed;
  top:20px;
  right:20px;
  width:50px;
  height:50px;
  background:#1a1a2e;
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

#top-menu {
  position: fixed;
  top:80px;
  right:20px;
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
  color:#1a1a2e;
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
  <!-- YOUR PROFILE PICTURE -->
  <img src="YOUR_PICTURE.jpg" alt="Your Picture">
  <h2>Hello, I'm Great Ola In Wealth</h2>
  <p>A full stack web developer delivering clean, professional web solutions.</p>
  <!-- CALL TO ACTION BUTTONS -->
  <a href="https://wa.me/YOURNUMBER" class="btn" target="_blank">WhatsApp</a>
  <a href="https://t.me/YOURTELEGRAM" class="btn" target="_blank">Telegram</a>
</section>

<!-- About -->
<section id="about">
  <h2>About Me</h2>
  <p>I build websites, landing pages, and web apps. Clean design, responsive layouts, client satisfaction.</p>
</section>

<!-- Services -->
<section id="services">
  <h2>Services</h2>
  <div class="service-card">
    <img src="https://cdn-icons-png.flaticon.com/512/919/919847.png" alt="HTML">
    <h3>Frontend Development</h3>
    <p>HTML, CSS, JavaScript, React, and many more.</p>
  </div>
  <div class="service-card">
    <img src="https://cdn-icons-png.flaticon.com/512/919/919825.png" alt="Backend">
    <h3>Backend Development</h3>
    <p>Node.js, Express, MongoDB, and many more.</p>
  </div>
  <div class="service-card">
    <img src="https://cdn-icons-png.flaticon.com/512/919/919836.png" alt="Full Stack">
    <h3>Full Stack Projects</h3>
    <p>Complete web solutions, and many more.</p>
  </div>
</section>

<!-- Client Testimonials -->
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
  <img class="office-pic" src="OFFICE_PIC.jpg" alt="Office / Laptop">
</section>

<!-- Footer -->
<footer>
  <p>&copy; 2025 Great Ola In Wealth</p>
</footer>

<!-- Top-Right Hamburger -->
<div id="menu-btn">
  <div></div>
  <div></div>
  <div></div>
</div>
<div id="top-menu">
  <a href="#hero">Home</a>
  <a href="#about">About</a>
  <a href="#services">Services</a>
  <a href="#comments">Clients</a>
  <a href="#office">Work</a>
  <a href="#contact">Contact</a>
</div>

<!-- Floating Customer Service Icons -->
<div class="customer-service">
  <img src="https://cdn-icons-png.flaticon.com/512/2111/2111728.png" alt="Support 1" onclick="window.open('https://wa.me/YOURNUMBER','_blank')">


<script>
const menuBtn = document.getElementById('menu-btn');
const topMenu = document.getElementById('top-menu');
menuBtn.addEventListener('click', ()=>{
  if(topMenu.style.display==='flex'){topMenu.style.display='none';}
  else{topMenu.style.display='flex';topMenu.style.flexDirection='column';}
});
</script>
</body>
</html>
