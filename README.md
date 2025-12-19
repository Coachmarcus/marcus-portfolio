<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Marcus D. Portfolio</title>
<style>
/* Reset & Base */
* { margin:0; padding:0; box-sizing:border-box; font-family: 'Arial', sans-serif; }
body { line-height:1.6; color:#111; background:#f5f5f5; scroll-behavior:smooth; }
a { text-decoration:none; color:inherit; }
img { max-width:100%; display:block; }

/* Container */
.container { max-width:1200px; margin:0 auto; padding:0 20px; }

/* Navigation */
nav { position:fixed; top:0; width:100%; background:rgba(30,30,47,0.85); color:#fff; display:flex; justify-content:center; gap:30px; padding:15px 0; z-index:999; backdrop-filter:blur(8px);}
nav a { color:#fff; font-weight:600; transition:0.3s; }
nav a:hover { color:#ff5c5c; }

/* Header */
header { height:100vh; display:flex; flex-direction:column; justify-content:center; align-items:center; background:#1e1e2f; color:#fff; text-align:center; padding:0 20px; }
header h1 { font-size:3rem; margin-bottom:10px; }
header p { font-size:1.2rem; color:#ccc; margin-bottom:20px; max-width:600px; }
header a.btn { padding:12px 30px; background:#ff5c5c; color:#fff; border-radius:30px; transition:0.3s; margin:5px; display:inline-block; }
header a.btn:hover { background:#ff3333; }

/* Sections */
section { padding:80px 0; }
section h2 { text-align:center; font-size:2.5rem; margin-bottom:40px; color:#1e1e2f; }
section p { text-align:center; max-width:700px; margin:0 auto 20px; color:#555; }

/* About */
#about { background:#fff; }
#about img { border-radius:50%; width:180px; margin-bottom:20px; display:block; margin-left:auto; margin-right:auto; }
#about p { font-size:1.1rem; margin-top:15px; }

/* Skills */
.skills { display:flex; flex-wrap:wrap; justify-content:center; gap:20px; }
.skill { background:#fff; padding:20px; border-radius:10px; width:200px; text-align:center; box-shadow:0 5px 15px rgba(0,0,0,0.1);}
.skill h3 { margin-bottom:10px; color:#1e1e2f; }
.skill p { color:#777; }

/* Portfolio */
.portfolio-grid { display:grid; grid-template-columns:repeat(auto-fit, minmax(280px, 1fr)); gap:20px; }
.portfolio-item { background:#fff; border-radius:10px; overflow:hidden; box-shadow:0 5px 15px rgba(0,0,0,0.1); transition:transform 0.3s; }
.portfolio-item:hover { transform:translateY(-5px);}
.portfolio-item img { width:100%; height:200px; object-fit:cover; }
.portfolio-item .info { padding:15px; }
.portfolio-item h3 { margin-bottom:10px; color:#1e1e2f; }
.portfolio-item p { color:#555; font-size:0.95rem; }

/* Testimonials */
.testimonials { display:flex; flex-wrap:wrap; justify-content:center; gap:20px; }
.testimonial { background:#fff; padding:20px; border-radius:10px; width:300px; box-shadow:0 5px 15px rgba(0,0,0,0.1);}
.testimonial p { font-style:italic; margin-bottom:10px; color:#555; }
.testimonial h4 { color:#1e1e2f; font-weight:600; }

/* Services */
.services { display:flex; flex-wrap:wrap; justify-content:center; gap:20px; }
.service { background:#fff; padding:20px; border-radius:10px; width:250px; text-align:center; box-shadow:0 5px 15px rgba(0,0,0,0.1);}
.service h3 { margin-bottom:10px; color:#1e1e2f; }
.service p { color:#555; font-size:0.95rem; }

/* Contact */
#contact form { max-width:600px; margin:0 auto; display:flex; flex-direction:column; gap:15px; }
#contact input, #contact textarea { padding:12px; border-radius:5px; border:1px solid #ccc; font-size:1rem; width:100%; }
#contact button { padding:12px; border:none; border-radius:30px; background:#ff5c5c; color:#fff; font-size:1rem; cursor:pointer; transition:0.3s; }
#contact button:hover { background:#ff3333; }

/* Footer */
footer { background:#1e1e2f; color:#fff; text-align:center; padding:20px; }

/* Responsive */
@media(max-width:768px){ 
    header h1{ font-size:2.2rem; } 
    section h2{ font-size:2rem; } 
    nav { gap:15px;}
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
    <a href="#contact" class="btn">Hire Me</a>
    <a href="mailto:assistancepromoter@gmail.com" class="btn">Email Me</a>
    <a href="https://www.behance.net/olamilemarcus" target="_blank" class="btn">My Behance</a>
    <a href="tel:+2348144466868" class="btn">Call Me</a>
</header>

<!-- About -->
<section id="about">
    <div class="container">
        <img src="https://avatars.githubusercontent.com/u/171789491?v=4" alt="Marcus D.">
        <h2>About Me</h2>
        <p>Hello! I’m Marcus D., a passionate web designer creating visually appealing and user-friendly websites. I specialize in UI/UX design, responsive layouts, and building digital experiences that delight users. I love turning ideas into functional, beautiful websites that clients and users enjoy.</p>
    </div>
</section>

<!-- Skills -->
<section id="skills">
    <div class="container">
        <h2>My Skills</h2>
        <div class="skills">
            <div class="skill"><h3>HTML & CSS</h3><p>Responsive & semantic coding</p></div>
            <div class="skill"><h3>JavaScript</h3><p>Interactive web experiences</p></div>
            <div class="skill"><h3>UI/UX Design</h3><p>Wireframing & prototyping</p></div>
            <div class="skill"><h3>WordPress & Webflow</h3><p>Custom website builds</p></div>
            <div class="skill"><h3>Figma & Adobe XD</h3><p>Modern design tools</p></div>
            <div class="skill"><h3>SEO & Performance</h3><p>Optimized for speed & search</p></div>
        </div>
    </div>
</section>

<!-- Portfolio -->
<section id="portfolio">
    <div class="container">
        <h2>Portfolio</h2>
        <div class="portfolio-grid">
            <div class="portfolio-item"><img src="https://via.placeholder.com/400x250?text=Project+1" alt="Project 1"><div class="info"><h3>Landing Page</h3><p>Designed responsive landing page for a startup using Figma & HTML/CSS.</p></div></div>
            <div class="portfolio-item"><img src="https://via.placeholder.com/400x250?text=Project+2" alt="Project 2"><div class="info"><h3>E-commerce Website</h3><p>Built an online store on WordPress with custom theme and UX optimization.</p></div></div>
            <div class="portfolio-item"><img src="https://via.placeholder.com/400x250?text=Project+3" alt="Project 3"><div class="info"><h3>Portfolio Redesign</h3><p>Redesigned a creative portfolio website to enhance visuals and UX.</p></div></div>
            <div class="portfolio-item"><img src="https://via.placeholder.com/400x250?text=Project+4" alt="Project 4"><div class="info"><h3>Blog Website</h3><p>Developed a modern, responsive blog platform with clean UI.</p></div></div>
            <div class="portfolio-item"><img src="https://via.placeholder.com/400x250?text=Project+5" alt="Project 5"><div class="info"><h3>Business Website</h3><p>Created a professional business website with interactive sections.</p></div></div>
            <div class="portfolio-item"><img src="https://via.placeholder.com/400x250?text=Project+6" alt="Project 6"><div class="info"><h3>Web App UI</h3><p>Designed interface for a productivity web application.</p></div></div>
        </div>
    </div>
</section>

<!-- Testimonials -->
<section id="testimonials">
    <div class="container">
        <h2>Testimonials</h2>
        <div class="testimonials">
            <div class="testimonial"><p>"Marcus delivered an amazing website with exceptional attention to detail. Highly recommended!"</p><h4>Jane Doe, CEO TechStartup</h4></div>
            <div class="testimonial"><p>"Professional, creative, and fast. Marcus truly understands modern web design."</p><h4>John Smith, Freelancer</h4></div>
        </div>
    </div>
</section>

<!-- Services -->
<section id="services">
    <div class="container">
        <h2>Services</h2>
        <div class="services">
            <div class="service"><h3>Web Design</h3><p>Modern, responsive websites with creative UI.</p></div>
            <div class="service"><h3>UI/UX Design</h3><p>User-friendly interfaces and seamless experiences.</p></div>
            <div class="service"><h3>Website Maintenance</h3><p>Ongoing support to keep websites secure and updated.</p></div>
            <div class="service"><h3>Branding & Graphics</h3><p>Visual identity, logos, and graphics for your brand.</p></div>
        </div>
    </div>
</section>

<!-- Contact -->
<section id="contact">
    <div class="container">
        <h2>Contact Me</h2>
        <form>
            <input type="text" placeholder="Your Name" required>
            <input type="email" placeholder="Your Email" required>
            <textarea rows="5" placeholder="Your Message" required></textarea>
            <button type="submit">Send Message</button>
        </form>
        <p style="text-align:center; margin-top:20px;">Phone: <a href="tel:+2348144466868">+234 814 446 6868</a> | Email: <a href="mailto:assistancepromoter@gmail.com">assistancepromoter@gmail.com</a> | Behance: <a href="https://www.behance.net/olamilemarcus" target="_blank">behance.net/olamilemarcus</a></p>
    </div>
</section>

<!-- Footer -->
<footer>
    <p>&copy; 2025 Marcus D. All rights reserved.</p>
</footer>

</body>
</html>
