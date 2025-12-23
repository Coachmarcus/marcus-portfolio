<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Julytee Plumbing</title>
<style>
  * { box-sizing:border-box; margin:0; padding:0; font-family:Arial,sans-serif; scroll-behavior:smooth; }
  body { background:#1a202c; color:#f5f5f5; position:relative; }

  /* Hero/Home */
  .hero { position:relative; width:100%; min-height:500px; background:url('https://images.pexels.com/photos/6801643/pexels-photo-6801643.jpeg') center/cover no-repeat; display:flex; align-items:center; justify-content:center; flex-direction:column; text-align:center; padding:20px; }
  .hero::after { content:""; position:absolute; top:0; left:0; width:100%; height:100%; background:rgba(0,0,0,0.5); z-index:1; }
  .hero-content { position:relative; z-index:2; max-width:800px; }
  .hero-content img.logo { width:100px; height:100px; border-radius:50%; object-fit:cover; border:3px solid #f0a500; margin-bottom:15px; }
  .hero-content h1 { font-size:2.5rem; margin-bottom:10px; color:#f5f5f5; }
  .hero-content p { font-size:1.2rem; margin-bottom:20px; color:#ddd; }
  .hero-buttons { display:flex; gap:15px; justify-content:center; flex-wrap:wrap; }
  .hero-buttons a { text-decoration:none; padding:12px 22px; border-radius:6px; font-weight:bold; color:#222; background:#f0a500; transition:0.3s; }
  .hero-buttons a:hover { background:#e69500; }

  /* Section Styling */
  section { padding:40px 20px; }
  section h2 { text-align:center; font-size:2rem; margin-bottom:20px; color:#f5f5f5; }
  .services-grid { display:grid; grid-template-columns:repeat(auto-fit,minmax(250px,1fr)); gap:20px; }
  .service-card { background:#2a3653; border-radius:12px; padding:15px; text-align:center; position:relative; overflow:hidden; }
  .service-card img { width:100%; border-radius:8px; height:180px; object-fit:cover; transition:opacity 1s ease; }
  .service-card h3 { margin:10px 0 5px 0; font-size:1.2rem; }
  .service-card p { font-size:0.95rem; color:#ccc; }

  .about-section { background:#162447; border-radius:12px; padding:30px 20px; margin:40px 0; }
  .about-section p { margin:10px 0; line-height:1.5rem; text-align:center; color:#ddd; }

  .testimonials { background:#0f1626; padding:40px 20px; border-radius:12px; margin:40px 20px; }
  .testimonial { background:#1e2940; margin:15px auto; padding:12px 18px; border-radius:8px; max-width:800px; }
  .testimonial p { font-style:italic; }

  .contact-section { background:#162447; padding:30px 20px; border-radius:12px; max-width:700px; margin:40px auto; }
  .contact-section h2 { text-align:center; margin-bottom:20px; }
  .contact-details { text-align:center; margin-bottom:20px; }
  .contact-details p { margin:6px 0; font-size:1.1rem; }
  .contact-details a { color:#f0a500; text-decoration:none; font-weight:bold; }

  .contact-form { display:flex; flex-direction:column; gap:12px; }
  .contact-form input, .contact-form textarea { padding:10px; border-radius:6px; border:1px solid #555; background:#0d1626; color:#fff; }
  .contact-form button { padding:12px; border:none; background:#f0a500; color:#222; font-size:1rem; border-radius:6px; cursor:pointer; }
  .contact-form button:hover { background:#e69500; }

  footer { background:#0d3b66; text-align:center; padding:18px; font-size:0.9rem; color:#fff; margin-top:40px; }

  /* Left-side toggle button */
  .menu-toggle { position:fixed; top:50%; left:0; transform:translateY(-50%); width:40px; height:40px; background:#f0a500; color:#222; font-weight:bold; cursor:pointer; border-radius:0 8px 8px 0; display:flex; align-items:center; justify-content:center; z-index:1000; }
  .side-buttons { position:fixed; top:50%; left:0; transform:translateY(-50%) translateX(-100%); display:flex; flex-direction:column; gap:10px; transition:0.3s; z-index:999; }
  .side-buttons.show { transform:translateY(-50%) translateX(0); }
  .side-buttons button { padding:12px 18px; border:none; background:#0d3b66; color:#fff; border-radius:0 8px 8px 0; cursor:pointer; font-weight:bold; transition:0.3s; }
  .side-buttons button.active, .side-buttons button:hover { background:#f0a500; color:#222; }

  /* AI Chatbox */
  .ai-icon { position:fixed; bottom:20px; right:20px; width:50px; height:50px; background:#f0a500; color:#222; border-radius:50%; display:flex; align-items:center; justify-content:center; cursor:pointer; font-weight:bold; z-index:2000; }
  .ai-chat { position:fixed; bottom:80px; right:20px; background:#0d3b66; color:#fff; border-radius:12px; width:300px; max-height:400px; display:none; flex-direction:column; overflow:hidden; z-index:2000; }
  .ai-header { background:#f0a500; color:#222; padding:10px; font-weight:bold; cursor:pointer; }
  .ai-messages { flex:1; padding:10px; overflow-y:auto; font-size:0.95rem; }
  .ai-input { display:flex; border-top:1px solid #555; }
  .ai-input input { flex:1; padding:8px; border:none; outline:none; background:#162447; color:#fff; }
  .ai-input button { padding:8px 12px; background:#f0a500; border:none; color:#222; cursor:pointer; }

</style>
</head>
<body>

<!-- Home / Hero -->
<div id="home" class="hero">
  <div class="hero-content">
    <img class="logo" src="https://images.pexels.com/photos/6801643/pexels-photo-6801643.jpeg" alt="Company Logo">
    <h1>Julytee Plumbing</h1>
    <p>Reliable plumbing solutions for homes & businesses in Ogbomosho, Oyo State. Pipe repairs, water system installations, drainage cleaning & emergency services.</p>
    <div class="hero-buttons">
      <a href="tel:+2347061362802">Call Now</a>
      <a href="https://wa.me/2347061362802" target="_blank">WhatsApp</a>
      <a href="#contact">Get a Quote</a>
    </div>
  </div>
</div>

<!-- About Section -->
<section id="about" class="about-section">
  <h2>About Us</h2>
  <p>Julytee Plumbing has been providing top-quality plumbing solutions in Ogbomosho and Oyo State for years. Our team is skilled in both residential and commercial plumbing, ensuring your water systems are safe, efficient, and reliable.</p>
  <p>We pride ourselves on excellent customer service, transparent pricing, and timely project completion. Our mission is to make plumbing simple, stress-free, and reliable for every client.</p>
</section>

<!-- Services Section -->
<section id="services">
  <h2>Our Main Services</h2>
  <div class="services-grid">
    <div class="service-card">
      <img src="https://images.pexels.com/photos/4164050/pexels-photo-4164050.jpeg" alt="Pipe Repair">
      <h3>Pipe Repair & Replacement</h3>
      <p>Quickly fix or replace damaged pipes to prevent leaks.</p>
    </div>
    <div class="service-card">
      <img src="https://images.pexels.com/photos/5801132/pexels-photo-5801132.jpeg" alt="Water System Installation">
      <h3>Water System Installation</h3>
      <p>Install reliable water systems for homes & businesses.</p>
    </div>
    <div class="service-card">
      <img src="https://images.pexels.com/photos/5991752/pexels-photo-5991752.jpeg" alt="Drainage Cleaning">
      <h3>Drainage Cleaning</h3>
      <p>Clear clogged drains quickly and efficiently.</p>
    </div>
    <div class="service-card">
      <img src="https://images.pexels.com/photos/6595383/pexels-photo-6595383.jpeg" alt="Emergency Plumbing">
      <h3>Emergency Plumbing Support</h3>
      <p>24/7 emergency response for urgent plumbing issues.</p>
    </div>
    <div class="service-card">
      <img src="https://images.pexels.com/photos/6231621/pexels-photo-6231621.jpeg" alt="Consultation">
      <h3>Plumbing Consultation & Maintenance</h3>
      <p>Expert advice and maintenance solutions to avoid future problems.</p>
    </div>
  </div>
</section>

<!-- Testimonials -->
<section id="testimonials" class="testimonials">
  <h2>What Our Clients Say</h2>
  <div class="testimonial"><p>“Super reliable and fast service! Highly recommend Julytee Plumbing!”</p></div>
  <div class="testimonial"><p>“Installed our water system perfectly and on time. Very professional.”</p></div>
</section>

<!-- Contact -->
<section id="contact" class="contact-section">
  <h2>Contact Us</h2>
  <div class="contact-details">
    <p>Phone / WhatsApp: <a href="tel:+2347061362802">+234 706 136 2802</a></p>
    <p>Email: <a href="mailto:info@julyteeplumbing.com">info@julyteeplumbing.com</a></p>
    <p>Address: Olodude’s house, Off Lagos‑Ibadan Expressway, opposite Ogbomosho High School, Ogbomosho, Oyo State, Nigeria</p>
  </div>
  <div class="contact-form">
    <input type="text" placeholder="Your Name" required>
    <input type="email" placeholder="Your Email" required>
    <textarea placeholder="Your Message" rows="5" required></textarea>
    <button>Send Message</button>
  </div>
</section>

<footer>© 2025 Julytee Plumbing Services | Ogbomosho, Oyo State, Nigeria</footer>

<!-- top-Left-side toggle button -->
<div class="menu-toggle" id="menuToggle">⋮⋮⋮⋮</div>
<div class="side-buttons" id="sideButtons">
  <button data-target="#home" class="active">Home</button>
  <button data-target="#about">About</button>
  <button data-target="#services">Services</button>
  <button data-target="#testimonials">Testimonials</button>
  <button data-target="#contact">Contact</button>
</div>

<!-- AI Icon -->
<div class="ai-icon" id="aiIcon">AI</div>
<div class="ai-chat" id="aiChat">
  <div class="ai-header" onclick="toggleChat()">AI Assistant</div>
  <div class="ai-messages" id="aiMessages"></div>
  <div class="ai-input">
    <input type="text" id="aiInput" placeholder="Ask me anything...">
    <button onclick="sendAI()">Send</button>
  </div>
</div>

<script>
  // Toggle left menu
  const menuToggle = document.getElementById('menuToggle');
  const sideButtons = document.getElementById('sideButtons');
  menuToggle.addEventListener('click', () => { sideButtons.classList.toggle('show'); });

  // Side buttons scroll & active
  const buttons = document.querySelectorAll('.side-buttons button');
  buttons.forEach(btn => {
    btn.addEventListener('click', () => {
      buttons.forEach(b => b.classList.remove('active'));
      btn.classList.add('active');
      const target = document.querySelector(btn.getAttribute('data-target'));
      target.scrollIntoView({behavior:'smooth'});
    });
  });

  // AI Chat toggle
  const aiIcon = document.getElementById('aiIcon');
  const aiChat = document.getElementById('aiChat');
  aiIcon.addEventListener('click', () => { aiChat.style.display = aiChat.style.display==='flex'?'none':'flex'; });

  function toggleChat(){ /* Header click does nothing */ }

  // AI Chat functionality
  function sendAI(){
    const input = document.getElementById('aiInput');
    const msg = input.value.trim();
    if(!msg) return;
    const messages = document.getElementById('aiMessages');
    let botReply = 'This is just a preview.';

    messages.innerHTML += `<p><b>You:</b> ${msg}</p><p><b>AI:</b> ${botReply}</p>`;
    messages.scrollTop = messages.scrollHeight;
    input.value = '';
  }
</script>
</body>
</html>
