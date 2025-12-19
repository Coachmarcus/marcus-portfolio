<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Marcus Portfolio</title>
<style>
    /* Reset & Base */
    * { margin:0; padding:0; box-sizing:border-box; font-family: 'Arial', sans-serif; }
    body { line-height:1.6; color:#111; background:#f5f5f5; }
    a { text-decoration:none; color:inherit; }
    img { max-width:100%; display:block; }

    /* Container */
    .container { max-width:1200px; margin:0 auto; padding:0 20px; }

    /* Header */
    header { background:#1e1e2f; color:#fff; padding:60px 0; text-align:center; }
    header h1 { font-size:3rem; margin-bottom:10px; }
    header p { font-size:1.2rem; color:#ccc; margin-bottom:20px; }
    header a.btn { padding:12px 30px; background:#ff5c5c; color:#fff; border-radius:30px; transition:0.3s; }
    header a.btn:hover { background:#ff3333; }

    /* Sections */
    section { padding:80px 0; }
    section h2 { text-align:center; font-size:2.5rem; margin-bottom:40px; color:#1e1e2f; }
    section p { text-align:center; max-width:700px; margin:0 auto 20px; color:#555; }

    /* About */
    #about img { border-radius:50%; width:150px; margin-bottom:20px; }
    #about p { font-size:1.1rem; }

    /* Skills */
    .skills { display:flex; flex-wrap:wrap; justify-content:center; gap:20px; }
    .skill { background:#fff; padding:20px; border-radius:10px; width:200px; text-align:center; box-shadow:0 5px 15px rgba(0,0,0,0.1);}
    .skill h3 { margin-bottom:10px; color:#1e1e2f; }
    .skill p { color:#777; }

    /* Portfolio */
    .portfolio-grid { display:grid; grid-template-columns:repeat(auto-fit, minmax(250px, 1fr)); gap:20px; }
    .portfolio-item { background:#fff; border-radius:10px; overflow:hidden; box-shadow:0 5px 15px rgba(0,0,0,0.1); }
    .portfolio-item img { width:100%; }
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
    @media(max-width:768px){ header h1{ font-size:2.2rem; } section h2{ font-size:2rem; } }
</style>
</head>
<body>

<!-- Header -->
<header>
    <h1>Marcus Olamile</h1>
    <p>Professional Web Designer | UI/UX Enthusiast | Building Creative Digital Experiences</p>
    <a href="#contact" class="btn">Hire Me</a>
</header>

<!-- About -->
<section id="about">
    <div class="container" style="text-align:center;">
        <img src="https://avatars.githubusercontent.com/u/171789491?v=4" alt="Marcus Olamile">
        <h2>About Me</h2>
        <p>Hello! I’m Marcus, a passionate web designer creating visually appealing and user-friendly websites. I specialize in UI/UX design, responsive layouts, and building digital experiences that delight users.</p>
    </div>
</section>

<!-- Skills -->
<section id="skills">
    <div class="container">
        <h2>My Skills</h2>
        <div class="skills">
            <div class="skill">
                <h3>HTML & CSS</h3>
                <p>Responsive & semantic coding</p>
            </div>
            <div class="skill">
                <h3>JavaScript</h3>
                <p>Interactive web experiences</p>
            </div>
            <div class="skill">
                <h3>UI/UX Design</h3>
                <p>Wireframing & prototyping</p>
            </div>
            <div class="skill">
                <h3>WordPress & Webflow</h3>
                <p>Custom website builds</p>
            </div>
        </div>
    </div>
</section>

<!-- Portfolio -->
<section id="portfolio">
    <div class="container">
        <h2>Portfolio</h2>
        <div class="portfolio-grid">
            <div class="portfolio-item">
                <img src="https://via.placeholder.com/400x250" alt="Project 1">
                <div class="info">
                    <h3>Landing Page Design</h3>
                    <p>Designed a responsive landing page for a tech startup using Figma & HTML/CSS.</p>
                </div>
            </div>
            <div class="portfolio-item">
                <img src="https://via.placeholder.com/400x250" alt="Project 2">
                <div class="info">
                    <h3>E-commerce Website</h3>
                    <p>Built an online store on WordPress with custom theme design and UX optimization.</p>
                </div>
            </div>
            <div class="portfolio-item">
                <img src="https://via.placeholder.com/400x250" alt="Project 3">
                <div class="info">
                    <h3>Portfolio Redesign</h3>
                    <p>Redesigned a creative portfolio website to enhance user engagement and visuals.</p>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- Testimonials -->
<section id="testimonials">
    <div class="container">
        <h2>Testimonials</h2>
        <div class="testimonials">
            <div class="testimonial">
                <p>"Marcus delivered an amazing website with exceptional attention to detail. Highly recommended!"</p>
                <h4>Jane Doe, CEO TechStartup</h4>
            </div>
            <div class="testimonial">
                <p>"Professional, creative, and fast. Marcus truly understands modern web design."</p>
                <h4>John Smith, Freelancer</h4>
            </div>
        </div>
    </div>
</section>

<!-- Services -->
<section id="services">
    <div class="container">
        <h2>Services</h2>
        <div class="services">
            <div class="service">
                <h3>Web Design</h3>
                <p>Modern, responsive websites with creative UI.</p>
            </div>
            <div class="service">
                <h3>UI/UX Design</h3>
                <p>User-friendly interfaces and seamless experiences.</p>
            </div>
            <div class="service">
                <h3>Website Maintenance</h3>
                <p>Ongoing support to keep websites secure and updated.</p>
            </div>
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
    </div>
</section>

<!-- Footer -->
<footer>
    <p>&copy; 2025 Marcus Olamile. All rights reserved.</p>
</footer>

</body>
</html>
