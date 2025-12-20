<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Crystalline Montessori Academy</title>
  <style>
    /* Reset and base */
    * { margin:0; padding:0; box-sizing:border-box; font-family: Arial, sans-serif; }
    body { line-height: 1.6; color: #333; }
    a { text-decoration: none; color: inherit; }

    /* Header */
    header { background: #4CAF50; color: white; padding: 20px 0; text-align: center; }
    header h1 { font-size: 2rem; margin-bottom: 10px; }
    nav a { margin: 0 15px; color: white; font-weight: bold; }

    /* Hero */
    .hero { background: url('https://www.greenspringsschool.com/wp-content/uploads/2018/10/IMG_7290.jpg') center/cover no-repeat; height: 80vh; display: flex; flex-direction: column; justify-content: center; align-items: center; text-align: center; color: white; padding: 0 20px; }
    .hero h2 { font-size: 2.5rem; margin-bottom: 20px; text-shadow: 2px 2px 4px rgba(0,0,0,0.5); }
    .hero .btn { background: #FFC107; color: #333; padding: 15px 25px; margin: 5px; border-radius: 5px; font-weight: bold; transition: 0.3s; }
    .hero .btn:hover { background: #FFB300; }

    /* Sections */
    section { padding: 60px 20px; max-width: 1200px; margin: auto; }
    section h2 { text-align: center; font-size: 2rem; margin-bottom: 40px; color: #4CAF50; }

    /* About */
    .about { display: flex; flex-wrap: wrap; gap: 30px; align-items: center; }
    .about img { flex: 1; max-width: 500px; border-radius: 10px; }
    .about .content { flex: 2; }

    /* Programs */
    .programs { display: flex; flex-wrap: wrap; gap: 30px; justify-content: center; }
    .program { flex: 1 1 250px; background: #f4f4f4; padding: 20px; border-radius: 10px; text-align: center; transition: 0.3s; }
    .program:hover { transform: translateY(-5px); box-shadow: 0 5px 15px rgba(0,0,0,0.2); }

    /* Facilities */
    .facilities { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; }
    .facilities img { width: 100%; border-radius: 10px; }

    /* Testimonials */
    .testimonials { background: #f4f4f4; padding: 60px 20px; }
    .testimonial { text-align: center; margin-bottom: 30px; }
    .testimonial p { font-style: italic; margin-bottom: 10px; }
    .testimonial span { font-weight: bold; color: #4CAF50; }

    /* Contact */
    .contact form { display: flex; flex-direction: column; gap: 15px; max-width: 500px; margin: auto; }
    .contact input, .contact textarea { padding: 10px; border-radius: 5px; border: 1px solid #ccc; width: 100%; }
    .contact button { background: #4CAF50; color: white; padding: 15px; border: none; border-radius: 5px; font-weight: bold; cursor: pointer; transition: 0.3s; }
    .contact button:hover { background: #45a049; }

    /* Footer */
    footer { background: #333; color: white; text-align: center; padding: 20px; }
    
    /* Responsive */
    @media(max-width: 768px){
      .about { flex-direction: column; }
      .hero h2 { font-size: 2rem; }
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <h1>Crystalline Montessori Academy</h1>
    <nav>
      <a href="#about">About</a>
      <a href="#programs">Programs</a>
      <a href="#facilities">Facilities</a>
      <a href="#testimonials">Testimonials</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <!-- Hero Section -->
  <section class="hero">
    <h2>Nurturing Young Minds for a Bright Future</h2>
    <div>
      <a href="#contact" class="btn">Apply Now</a>
      <a href="#about" class="btn">Learn More</a>
    </div>
  </section>

  <!-- About Section -->
  <section id="about">
    <h2>About Us</h2>
    <div class="about">
      <img src="https://www.superprof.ng/blog/wp-content/uploads/2022/09/primary-school-students-980x649.jpg" alt="Classroom">
      <div class="content">
        <p><strong>Crystalline Montessori Academy</strong> is dedicated to providing top-quality Montessori education. We focus on academic excellence, moral development, and holistic learning to nurture future leaders.</p>
        <p><strong>Mission:</strong> To offer an enriching Montessori experience that develops the whole child – academically, morally, and socially.</p>
        <p><strong>Vision:</strong> To be a leading Montessori school recognized for excellence, integrity, and innovation.</p>
      </div>
    </div>
  </section>

  <!-- Programs Section -->
  <section id="programs">
    <h2>Our Programs</h2>
    <div class="programs">
      <div class="program">
        <h3>Early Childhood Education</h3>
        <p>Engaging Montessori lessons for foundational growth and curiosity-driven learning.</p>
      </div>
      <div class="program">
        <h3>Montessori Learning</h3>
        <p>Hands-on approach, independence, and personalized learning pace.</p>
      </div>
      <div class="program">
        <h3>Co-Curricular Activities</h3>
        <p>Sports, music, art, robotics, environmental and debate clubs.</p>
      </div>
    </div>
  </section>

  <!-- Facilities Section -->
  <section id="facilities">
    <h2>Our Facilities</h2>
    <div class="facilities">
      <img src="https://kidsusamontessori.org/wp-content/uploads/2024/11/build-safe-environment.jpg" alt="Playground">
      <img src="https://msbethhughes.org/wp-content/uploads/2015/11/class-library-e1448501343366.jpg?crop=1&h=1800&w=2400" alt="Library">
      <img src="https://www.thoughtco.com/thmb/OpPBudhFYkJ0JdCmkZUNZpNjhC8%3D/1500x0/filters%3Ano_upscale%28%29%3Amax_bytes%28150000%29%3Astrip_icc%28%29/Getty_girl_raising_hand_classroom_LARGE_Tetra-Images-Jamie-Grill-56a13e8b5f9b58b7d0bd5f12.jpg" alt="Classroom">
      <img src="https://www.kidzlet.com/images/products/kids-playground-flooring.jpg" alt="Play Area">
    </div>
  </section>

  <!-- Testimonials Section -->
  <section id="testimonials" class="testimonials">
    <h2>What Parents Say</h2>
    <div class="testimonial">
      <p>“Crystalline Montessori helped my child grow in confidence, discipline, and academics.”</p>
      <span>- Parent</span>
    </div>
    <div class="testimonial">
      <p>“The environment is calm, enriching, and focused on positive growth.”</p>
      <span>- Parent</span>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact">
    <h2>Contact Us</h2>
    <form>
      <input type="text" placeholder="Full Name" required>
      <input type="email" placeholder="Email Address" required>
      <input type="tel" placeholder="Phone Number" required>
      <textarea rows="5" placeholder="Message" required></textarea>
      <button type="submit">Send Message</button>
    </form>
    <p style="text-align:center; margin-top:20px;">📍 10 Mafowurosere Street, Jaleyemi Area, Osogbo, Osun State, Nigeria<br>📞 +234 704 443 3328</p>
  </section>

  <!-- Footer -->
  <footer>
    &copy; 2025 Crystalline Montessori Academy. All Rights Reserved.
  </footer>

</body>
</html>
