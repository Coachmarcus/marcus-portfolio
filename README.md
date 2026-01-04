<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>FDI Platform - Intelligence & Deal Facilitation</title>
  <meta name="description" content="Curated FDI intelligence and deal facilitation for emerging markets.">
  
  <style>
    /* Embedded CSS - Mobile-first, clean, professional */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
      line-height: 1.6;
      color: #333;
      background-color: #fafafa;
    }

    .container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 1rem;
    }

    /* Header & Navigation */
    header {
      background: #ffffff;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.08);
      position: sticky;
      top: 0;
      z-index: 100;
    }

    .navbar {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1rem;
    }

    .logo {
      font-size: 1.5rem;
      font-weight: 700;
      color: #1a3d7c;
    }

    .nav-links {
      display: none;
      flex-direction: column;
      position: absolute;
      top: 100%;
      left: 0;
      right: 0;
      background: white;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
    }

    .nav-links.active {
      display: flex;
    }

    .nav-links a {
      padding: 1rem;
      text-align: center;
      color: #333;
      font-weight: 500;
      display: block;
    }

    .nav-links a:hover {
      background: #f0f7ff;
    }

    .menu-toggle {
      font-size: 1.8rem;
      cursor: pointer;
      color: #1a3d7c;
    }

    /* Hero with background image */
    .hero {
      background-image: linear-gradient(rgba(230, 240, 255, 0.8), rgba(248, 251, 255, 0.8)), url('https://www.pgim.com/content/dam/jennison/us/en/active/graphical-elements/tbd/EM-RisingTide-162819887.jpg');
      background-size: cover;
      background-position: center;
      text-align: center;
      padding: 6rem 1rem;
    }

    .hero h1 {
      font-size: 2.4rem;
      margin-bottom: 1rem;
      color: #1a3d7c;
    }

    .hero p {
      font-size: 1.1rem;
      max-width: 600px;
      margin: 0 auto 2rem;
      color: #444;
    }

    .cta-button {
      display: inline-block;
      background: #1a3d7c;
      color: white;
      padding: 0.9rem 2rem;
      border-radius: 6px;
      font-weight: 600;
      text-decoration: none;
      transition: background 0.3s;
    }

    .cta-button:hover {
      background: #0f2a5c;
    }

    /* Sections */
    section {
      padding: 4rem 0;
      display: none;
    }

    section.active {
      display: block;
    }

    h2 {
      text-align: center;
      font-size: 1.8rem;
      margin-bottom: 2rem;
      color: #1a3d7c;
    }

    h3 {
      margin-bottom: 0.8rem;
      color: #1a3d7c;
    }

    .deal-grid {
      display: grid;
      gap: 2rem;
      grid-template-columns: 1fr;
    }

    .deal-item, article {
      background: white;
      padding: 1.5rem;
      border-radius: 8px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.06);
      text-align: center;
    }

    .deal-item img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      border-radius: 8px;
      margin-bottom: 1rem;
    }

    ul {
      max-width: 600px;
      margin: 2rem auto;
      line-height: 2;
    }

    /* Form */
    form {
      max-width: 600px;
      margin: 0 auto;
      background: white;
      padding: 2rem;
      border-radius: 8px;
      box-shadow: 0 2px 12px rgba(0,0,0,0.08);
    }

    label {
      display: block;
      margin: 0.5rem 0 0.3rem;
      font-weight: 500;
    }

    input, textarea {
      width: 100%;
      padding: 0.75rem;
      border: 1px solid #ddd;
      border-radius: 6px;
      font-family: inherit;
    }

    textarea {
      min-height: 150px;
      resize: vertical;
    }

    .hidden {
      display: none;
    }

    /* Footer */
    footer {
      background: #1a3d7c;
      color: white;
      text-align: center;
      padding: 2rem 1rem;
    }

    footer a {
      color: #a8c7ff;
      margin: 0 0.8rem;
      text-decoration: none;
    }

    /* Desktop */
    @media (min-width: 768px) {
      .menu-toggle {
        display: none;
      }

      .nav-links {
        display: flex;
        flex-direction: row;
        position: static;
        box-shadow: none;
        background: transparent;
      }

      .nav-links a {
        padding: 0 1.2rem;
      }

      .hero h1 {
        font-size: 3.2rem;
      }

      .deal-grid {
        grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
      }

      .deal-item img {
        height: 240px;
      }
    }
  </style>
</head>
<body>

<header>
  <nav class="navbar container">
    <div class="logo">FDI Platform</div>
    <div class="menu-toggle">☰</div>
    <ul class="nav-links">
      <li><a href="#home" onclick="showPage('home')">Home</a></li>
      <li><a href="#about" onclick="showPage('about')">About</a></li>
      <li><a href="#insights" onclick="showPage('insights')">Insights</a></li>
      <li><a href="#deals" onclick="showPage('deals')">Deals</a></li>
      <li><a href="#contact" onclick="showPage('contact')">Contact</a></li>
    </ul>
  </nav>
</header>

<main>
  <!-- Home -->
  <section id="home" class="active">
    <div class="hero">
      <div class="container">
        <h1>FDI Intelligence for Emerging Markets</h1>
        <p>Curated insights, non-sensitive deal opportunities, and seamless facilitation for investors and project owners.</p>
        <a href="#contact" class="cta-button" onclick="showPage('contact')">Submit a Deal</a>
      </div>
    </div>
    <div class="container">
      <h2>Connecting Capital with Opportunity</h2>
      <p style="text-align:center;max-width:800px;margin:auto;">We provide trusted intelligence and facilitate high-quality investment deals in fast-growing emerging economies.</p>
    </div>
  </section>

  <!-- About -->
  <section id="about">
    <div class="container">
      <h2>About Us</h2>
      <p>We are a specialized platform dedicated to foreign direct investment (FDI) intelligence and deal facilitation in emerging markets.</p>
      <br>
      <h2>What We Do</h2>
      <ul>
        <li>Deliver curated market insights and analysis</li>
        <li>Publish vetted, non-sensitive investment opportunities</li>
        <li>Facilitate connections between investors and project sponsors</li>
        <li>Support deal origination and preliminary due diligence</li>
      </ul>
    </div>
  </section>

  <!-- Insights -->
  <section id="insights">
    <div class="container">
      <h2>Insights & News</h2>
      <article>
        <h3>Emerging Market FDI Trends – Q4 2025</h3>
        <p>Key sectors attracting capital include renewable energy, digital infrastructure, and agribusiness across Southeast Asia and Sub-Saharan Africa.</p>
      </article>
      <article>
        <h3>Policy Updates: New Incentives</h3>
        <p>Several emerging markets have introduced enhanced tax benefits and streamlined approvals for greenfield investments in 2026.</p>
      </article>
    </div>
  </section>

  <!-- Deals -->
  <section id="deals">
    <div class="container">
      <h2>Curated Deals</h2>
      <p style="text-align:center;max-width:800px;margin:auto 0 3rem;">Non-sensitive investment opportunities actively seeking capital or strategic partners.</p>
      
      <div class="deal-grid">
        <div class="deal-item">
          <img src="https://worldbank.scene7.com/is/image/worldbankprod/renewables-boost-sustainable-development-in-central-african-republic-and-the-gambia-4?wid=780&hei=439&qlt=85,0&resMode=sharp" alt="Solar farm renewable energy project in developing region">
          <h3>100 MW Solar Project – Southeast Asia</h3>
          <p>Development stage complete. Seeking equity partner for construction financing.</p>
        </div>
        <div class="deal-item">
          <img src="https://content.r9cdn.net/rimg/dimg/c6/b2/7e865843-city-26243-164a4a25d83.jpg?width=1366&height=768&xhint=3968&yhint=1450&crop=true" alt="Modern Nairobi city skyline representing emerging market growth">
          <h3>Agtech Processing Facility – East Africa</h3>
          <p>Expansion capital needed. Strong offtake agreements and proven operations.</p>
        </div>
        <div class="deal-item">
          <img src="https://images.stockcake.com/public/0/6/d/06d86394-ec36-422d-af6c-228f5d246baf_large/business-handshake-abstract-stockcake.jpg" alt="Professional business handshake symbolizing investment deal">
          <h3>Digital Infrastructure Rollout – South Asia</h3>
          <p>Fiber network expansion seeking joint venture partner.</p>
        </div>
      </div>
      
      <p style="text-align:center;margin-top:3rem;">
        <a href="#contact" class="cta-button" onclick="showPage('contact')">Submit Your Deal</a>
      </p>
    </div>
  </section>

  <!-- Contact / Deal Intake -->
  <section id="contact">
    <div class="container">
      <h2>Contact & Deal Submission</h2>
      <p style="text-align:center;max-width:600px;margin:auto 0 2rem;">Submit investment opportunities or get in touch securely.</p>
      
      <form name="deal-intake" method="POST" data-netlify="true" netlify-honeypot="bot-field">
        <input type="hidden" name="form-name" value="deal-intake" />
        <p class="hidden">
          <label>Don’t fill this out: <input name="bot-field" /></label>
        </p>

        <label for="name">Name *</label>
        <input type="text" id="name" name="name" required />

        <label for="email">Email *</label>
        <input type="email" id="email" name="email" required />

        <label for="company">Company / Organization</label>
        <input type="text" id="company" name="company" />

        <label for="message">Message / Deal Summary *</label>
        <textarea id="message" name="message" required></textarea>

        <button type="submit" class="cta-button" style="width:100%;padding:1rem;margin-top:1rem;">Submit</button>
      </form>
    </div>
  </section>

  <!-- Terms -->
  <section id="terms">
    <div class="container">
      <h2>Terms of Service</h2>
      <p>[Insert your full legal terms of service here.]</p>
      <p>Last updated: January 2026</p>
    </div>
  </section>

  <!-- Privacy -->
  <section id="privacy">
    <div class="container">
      <h2>Privacy Policy</h2>
      <p>[Insert your full privacy policy here.]</p>
      <p>Last updated: January 2026</p>
    </div>
  </section>
</main>

<footer>
  <div class="container">
    <p>&copy; 2026 FDI Platform. All rights reserved.</p>
    <div>
      <a href="#terms" onclick="showPage('terms')">Terms</a> • 
      <a href="#privacy" onclick="showPage('privacy')">Privacy</a>
    </div>
  </div>
</footer>

<script>
  // Mobile menu + page navigation
  document.addEventListener('DOMContentLoaded', () => {
    const menuToggle = document.querySelector('.menu-toggle');
    const navLinks = document.querySelector('.nav-links');

    menuToggle.addEventListener('click', () => {
      navLinks.classList.toggle('active');
    });

    document.querySelectorAll('.nav-links a').forEach(link => {
      link.addEventListener('click', () => {
        navLinks.classList.remove('active');
      });
    });
  });

  function showPage(pageId) {
    document.querySelectorAll('section').forEach(sec => {
      sec.classList.remove('active');
    });
    document.getElementById(pageId).classList.add('active');
    window.scrollTo({ top: 0, behavior: 'smooth' });
    history.pushState(null, '', '#' + pageId);
  }

  window.addEventListener('load', () => {
    const hash = window.location.hash.substring(1) || 'home';
    showPage(hash);
  });

  window.addEventListener('popstate', () => {
    const hash = window.location.hash.substring(1) || 'home';
    showPage(hash);
  });
</script>

</body>
</html>
