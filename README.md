<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Marcus D. Portfolio</title>
<style>
/* Reset & Base */
* { margin:0; padding:0; box-sizing:border-box; font-family:'Arial',sans-serif; }
body { background:#f0f2f5; color:#111; line-height:1.5; scroll-behavior:smooth; }
a { text-decoration:none; color:inherit; }
img { width:100%; display:block; }

/* Navigation */
nav { position:fixed; top:0; width:100%; background:rgba(30,30,47,0.9); color:#fff; display:flex; justify-content:space-around; padding:12px 0; z-index:1000; backdrop-filter:blur(8px); font-size:0.95rem;}
nav a:hover { color:#ff5c5c; }

/* Header */
header { height:65vh; display:flex; flex-direction:column; justify-content:center; align-items:center; background:#1e1e2f; color:#fff; text-align:center; padding:0 20px; }
header h1 { font-size:2.8rem; margin-bottom:10px; }
header p { font-size:1rem; color:#ccc; max-width:300px; margin-bottom:20px; }
.header-links { display:flex; flex-direction:column; gap:12px; }
.header-links a { padding:10px 25px; background:#ff5c5c; color:#fff; border-radius:30px; font-size:0.95rem; text-align:center; transition:0.3s; }
.header-links a:hover { background:#ff3333; }

/* Sections */
section { padding:60px 20px; }
section h2 { font-size:1.8rem; margin-bottom:30px; text-align:center; color:#1e1e2f; }
section p { text-align:center; max-width:300px; margin:0 auto 20px; color:#555; font-size:0.95rem; }

/* About */
#about img { border-radius:50%; width:130px; margin:15px auto; display:block; border:3px solid #ff5c5c; }

/* Skills */
.skills { display:flex; flex-direction:column; gap:12px; margin-bottom:20px; }
.skill { background:#fff; padding:15px; border-radius:12px; box-shadow:0 4px 12px rgba(0,0,0,0.1); text-align:center; }
.skill h3 { margin-bottom:6px; color:#1e1e2f; font-size:1rem; }
.skill p { font-size:0.85rem; color:#777; }

/* Portfolio */
.portfolio { display:flex; flex-direction:column; gap:20px; }
.portfolio-item { background:#fff; border-radius:12px; box-shadow:0 4px 12px rgba(0,0,0,0.1); overflow:hidden; transition:transform 0.3s; }
.portfolio-item:hover { transform:translateY(-3px); }
.portfolio-item img { width:100%; height:200px; object-fit:cover; }
.portfolio-item .info { padding:12px; }
.portfolio-item h3 { margin-bottom:6px; font-size:1rem; color:#1e1e2f; }
.portfolio-item p { font-size:0.85rem; color:#555; }

/* Testimonials */
.testimonials { display:flex; flex-direction:column; gap:15px; }
.testimonial { background:#fff; padding:15px; border-radius:12px; box-shadow:0 4px 12px rgba(0,0,0,0.1); display:flex; gap:12px; align-items:center; }
.testimonial img { width:50px; height:50px; border-radius:50%; object-fit:cover; }
.testimonial div { flex:1; }
.testimonial p { font-size:0.85rem; font-style:italic; color:#555; margin-bottom:6px; }
.testimonial h4 { font-size:0.9rem; color:#1e1e2f; font-weight:600; }

/* Services */
.services { display:flex; flex-direction:column; gap:12px; margin-bottom:20px; }
.service { background:#fff; padding:15px; border-radius:12px; box-shadow:0 4px 12px rgba(0,0,0,0.1); text-align:center; }
.service h3 { margin-bottom:6px; font-size:1rem; color:#1e1e2f; }
.service p { font-size:0.85rem; color:#555; }

/* Contact */
#contact .contact-methods { display:flex; flex-direction:column; gap:12px; margin-bottom:15px; text-align:center; }
.contact-methods a { display:flex; align-items:center; justify-content:center; gap:8px; background:#fff; padding:10px; border-radius:12px; box-shadow:0 4px 12px rgba(0,0,0,0.1); font-size:0.9rem; color:#111; transition:0.3s; }
.contact-methods a:hover { background:#ff5c5c; color:#fff; }
#contact form { display:flex; flex-direction:column; gap:10px; }
#contact input, #contact textarea { padding:10px; border-radius:8px; border:1px solid #ccc; font-size:0.9rem; width:100%; }
#contact button { padding:10px; border:none; border-radius:30px; background:#ff5c5c; color:#fff; font-size:0.95rem; cursor:pointer; transition:0.3s; }
#contact button:hover { background:#ff3333; }

/* Footer */
footer { text-align:center; padding:15px; font-size:0.85rem; background:#1e1e2f; color:#fff; }

/* Mobile adjustments */
@media(min-width:500px){ 
    header h1 { font-size:3rem; }
    header p { font-size:1.1rem; max-width:400px; }
}
</style>
</head>
<body>

<!-- Navigation -->
<nav>
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#portfolio">Portfolio</a>
    <a href="#services">Services</a>
    <a href="#contact">Contact</a>
</nav>

<!-- Header -->
<header id="home">
    <h1>Marcus D.</h1>
    <p>Professional Web Designer | UI/UX Enthusiast | Crafting Creative Digital Experiences</p>
    <div class="header-links">
        <a href="mailto:assistancepromoter@gmail.com">✉️ Email Me</a>
        <a href="https://www.behance.net/olamilemarcus" target="_blank">🎨 My Behance</a>
        <a href="tel:+2348144466868">📞 Call Me</a>
    </div>
</header>

<!-- About -->
<section id="about">
    <h2>About Me</h2>
    <img src="https://avatars.githubusercontent.com/u/171789491?v=4" alt="Marcus D.">
    <p>Hello! I’m Marcus D., a passionate web designer creating visually appealing and user-friendly websites. I specialize in UI/UX design, responsive layouts, and building digital experiences that delight users.</p>
</section>

<!-- Skills -->
<section id="skills">
    <h2>My Skills</h2>
    <div class="skills">
        <div class="skill"><h3>HTML & CSS</h3><p>Responsive & semantic coding</p></div>
        <div class="skill"><h3>JavaScript</h3><p>Interactive web experiences</p></div>
        <div class="skill"><h3>UI/UX Design</h3><p>Wireframing & prototyping</p></div>
        <div class="skill"><h3>WordPress & Webflow</h3><p>Custom website builds</p></div>
        <div class="skill"><h3>Figma & Adobe XD</h3><p>Modern design tools</p></div>
    </div>
</section>

<!-- Portfolio -->
<section id="portfolio">
    <h2>Portfolio</h2>
    <div class="portfolio">
        <div class="portfolio-item"><img src="https://via.placeholder.com/350x200?text=Project+1"><div class="info"><h3>Landing Page</h3><p>Responsive landing page for startup using Figma & HTML/CSS.</p></div></div>
        <div class="portfolio-item"><img src="https://via.placeholder.com/350x200?text=Project+2"><div class="info"><h3>E-commerce Website</h3><p>Online store built on WordPress with custom theme.</p></div></div>
        <div class="portfolio-item"><img src="https://via.placeholder.com/350x200?text=Project+3"><div class="info"><h3>Portfolio Redesign</h3><p>Redesigned portfolio website to enhance UX & visuals.</p></div></div>
        <div class="portfolio-item"><img src="https://via.placeholder.com/350x200?text=Project+4"><div class="info"><h3>Blog Website</h3><p>Developed modern, responsive blog platform.</p></div></div>
    </div>
</section>

<!-- Testimonials -->
<section id="testimonials">
    <h2>Testimonials</h2>
    <div class="testimonials">
        <div class="testimonial"><img src="https://via.placeholder.com/50" alt="Client"><div><p>"Marcus delivered an amazing website with exceptional attention to detail."</p><h4>Jane Doe, CEO TechStartup</h4></div></div>
        <div class="testimonial"><img src="https://via.placeholder.com/50" alt="Client"><div><p>"Professional, creative, and fast. Marcus truly understands modern web design."</p><h4>John Smith, Freelancer</h4></div></div>
    </div>
</section>

<!-- Services -->
<section id="services">
    <h2>Services</h2>
    <div class="services">
        <div class="service"><h3>Web Design</h3><p>Modern, responsive websites with creative UI.</p></div>
        <div class="service"><h3>UI/UX Design</h3><p>User-friendly interfaces and seamless experiences.</p></div>
        <div class="service"><h3>Website Maintenance</h3><p>Ongoing support to keep websites secure and updated.</p></div>
        <div class="service"><h3>Branding & Graphics</h3><p>Visual identity, logos, and graphics for your brand.</p></div>
    </div>
</section>

<!-- Contact -->
<section id="contact">
    <h2>Contact Me</h2>
    <div class="contact-methods">
        <a href="tel:+2348144466868">📞 +234 814 446 6868</a>
        <a href="mailto:assistancepromoter@gmail.com">✉️ assistancepromoter@gmail.com</a>
        <a href="https://www.behance.net/olamilemarcus" target="_blank">🎨 My Behance</a>
    </div>
    <form>
        <input type="text" placeholder="Your Name" required>
        <input type="email" placeholder="Your Email" required>
        <textarea rows="4" placeholder="Your Message" required></textarea>
        <button type="submit">Send Message</button>
    </form>
</section>

<!-- Footer -->
<footer>
    &copy; 2025 Marcus D. All rights reserved.
</footer>

</body>
</html>
