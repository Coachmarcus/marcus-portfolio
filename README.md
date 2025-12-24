<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Makanaki Car Hire Services</title>
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
<style>
* { margin:0; padding:0; box-sizing:border-box; font-family: 'Roboto', sans-serif; }
body { scroll-behavior: smooth; }
a { text-decoration: none; }

/* Hero Section */
.hero {
    position: relative;
    height: 60vh;
    background: url('https://images.pexels.com/photos/110844/pexels-photo-110844.jpeg?auto=compress&cs=tinysrgb&h=750&w=1260') center/cover no-repeat;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    color: white;
    text-align: center;
    padding: 0 20px;
}
.hero h2 { font-size: 1.8rem; margin-bottom: 0.5rem; text-shadow: 2px 2px 6px rgba(0,0,0,0.6);}
.hero h1 { font-size: 2.2rem; margin-bottom: 1rem; text-shadow: 1px 1px 4px rgba(0,0,0,0.5);}
.hero p { font-size: 1rem; margin-bottom: 1.5rem; text-shadow: 1px 1px 4px rgba(0,0,0,0.5);}
.hero .cta { background-color: #007bff; color: white; padding: 12px 28px; border-radius: 30px; font-weight: bold; transition: all 0.3s ease; cursor: pointer;}
.hero .cta:hover { background-color: #0056b3; transform: scale(1.05); }

/* Fleet Section */
.fleet { padding: 50px 20px; background: #f5f5f5; text-align: center;}
.fleet h2 { font-size: 2rem; margin-bottom: 0.5rem; color: #333;}
.fleet p { font-size: 1rem; margin-bottom: 2rem; color: #555;}
.car-carousel { display: flex; overflow-x: auto; gap: 20px; scroll-behavior: smooth; padding-bottom: 20px; }
.car-carousel img { width: 300px; height: 200px; border-radius: 15px; object-fit: cover; flex-shrink: 0; }

.pricing-table { display: flex; justify-content: center; gap: 20px; margin: 30px 0; flex-wrap: wrap; }
.pricing { background: white; padding: 20px; border-radius: 15px; box-shadow: 0 4px 10px rgba(0,0,0,0.1); width: 200px; }
.pricing h3 { margin-bottom: 10px; color: #007bff;}
.pricing p { margin-bottom: 5px; color: #555; }

.services { display: flex; justify-content: center; gap: 40px; margin-top: 30px; flex-wrap: wrap; }
.service { text-align: center; }
.service img { width: 50px; margin-bottom: 10px; }

.fleet-buttons { display: flex; justify-content: center; gap: 20px; margin-top: 30px; flex-wrap: wrap;}
.fleet-buttons button { padding: 10px 25px; border: none; border-radius: 25px; font-weight: bold; color: white; cursor: pointer; box-shadow: 0 4px 8px rgba(0,0,0,0.2); transition: all 0.3s ease;}
.fleet-buttons button:hover { transform: scale(1.05);}
.view-fleet { background-color: #ff7f00;}
.get-quote { background-color: #28a745;}
.contact-us { background-color: #6f42c1;}

/* Features Section */
.features { padding: 50px 20px; background: #fff; text-align:center; }
.features h2 { font-size: 2rem; margin-bottom: 1rem; color: #333;}
.feature-cards { display: flex; justify-content: center; gap: 30px; flex-wrap: wrap; }
.feature { background: #f5f5f5; padding: 20px; border-radius: 15px; width: 200px; box-shadow: 0 4px 10px rgba(0,0,0,0.1);}
.feature img { width:50px; margin-bottom:10px; }
.feature p { color:#555; font-size:1rem; }

/* How It Works Section */
.how { padding:50px 20px; background:#f5f5f5; text-align:center; }
.how h2 { font-size:2rem; margin-bottom:20px; color:#333;}
.steps { display:flex; justify-content:center; gap:30px; flex-wrap:wrap;}
.step { background:white; padding:20px; border-radius:15px; width:200px; box-shadow:0 4px 10px rgba(0,0,0,0.1);}
.step img { width:50px; margin-bottom:10px;}
.step p { color:#555; font-size:1rem; }
.step a { text-decoration:none; color:#007bff; font-weight:bold; cursor:pointer; }

/* Testimonials Section */
.testimonials { padding:50px 20px; text-align:center; background:#fff;}
.testimonials h2 { font-size:2rem; margin-bottom:1.5rem; color:#333;}
.testimonial-card { max-width:400px; margin: 0 auto 20px; background:#f5f5f5; padding:20px; border-radius:15px; box-shadow:0 4px 10px rgba(0,0,0,0.1); display:flex; align-items:center; gap:15px;}
.testimonial-card img { width:50px; height:50px; border-radius:50%; object-fit:cover;}
.testimonial-card p { color:#555; font-size:1rem; margin:0;}
.testimonial-card span { font-weight:bold; color:#333; }

/* FAQ Section */
.faq { padding:50px 20px; text-align:center; background:#f5f5f5;}
.faq h2 { font-size:2rem; margin-bottom:1.5rem; color:#333;}
.faq-item { max-width:600px; margin:10px auto; background:white; padding:15px; border-radius:10px; box-shadow:0 4px 10px rgba(0,0,0,0.1);}
.faq-item p { font-size:1rem; color:#555; }

/* Contact Section */
.contact { padding:50px 20px; text-align:center; background:#fff; }
.contact h2 { font-size:2rem; margin-bottom:1rem; color:#333; }

/* First Box Image */
.contact-box {
    margin: 20px auto;
    text-align: center;
}
.contact-img {
    width: 200px;
    height: auto;
    border-radius: 15px;
}

.contact .map-contact { display:flex; flex-wrap:wrap; justify-content:center; gap:40px; margin-top:30px;}
.map { width:200px; height:200px; border-radius:15px; background: url('https://images.pexels.com/photos/383482/pexels-photo-383482.jpeg?auto=compress&cs=tinysrgb&h=300&w=400') center/cover no-repeat; }
.contact-info { max-width:300px; text-align:left;}
.contact-info img { width:50px; margin-right:10px; vertical-align:middle;}
.contact-info p { margin-bottom:10px; }

/* Sticky Footer Buttons */
.sticky-footer { position: fixed; bottom:0; left:0; width:100%; background: rgba(255,255,255,0.95); display:flex; justify-content:center; gap:20px; padding:10px 0; box-shadow:0 -2px 8px rgba(0,0,0,0.2); z-index:100; }
.sticky-footer button { padding:10px 20px; border-radius:20px; border:none; color:white; font-weight:bold; cursor:pointer; box-shadow:0 4px 8px rgba(0,0,0,0.2); transition: transform 0.3s ease;}
.sticky-footer .home { background-color:#007bff;}
.sticky-footer .fleet-btn { background-color:#ff7f00;}
.sticky-footer .contact { background-color:#28a745;}
.sticky-footer button:hover { transform: scale(1.05); }

@media(max-width:768px){
    .car-carousel img { width:250px; height:150px;}
    .pricing-table, .feature-cards, .steps { flex-direction: column; align-items:center; }
    .map-contact { flex-direction: column; align-items:center; }
    .hero h1 { font-size:1.8rem;}
    .hero h2 { font-size:1.2rem;}
    .hero p { font-size:0.9rem;}
}
</style>
</head>
<body>

<!-- Hero Section -->
<section class="hero">
    <h2>Makanaki Car Hire Services</h2>
    <h1>Reliable Car Hire & Rental Across Nigeria</h1>
    <p>Affordable, Easy, and Safe Car Rentals – Book Online or WhatsApp Today</p>
    <button class="cta" onclick="scrollToFleet()">Book Now</button>
</section>

<!-- Fleet Section -->
<section class="fleet" id="fleet">
    <h2>Our Fleet & Services</h2>
    <p>Choose from our selection of local Nigerian cars for your travel needs.</p>
    <div class="car-carousel">
        <img src="https://images.pexels.com/photos/358070/pexels-photo-358070.jpeg?auto=compress&cs=tinysrgb&h=300&w=400" alt="Toyota Corolla">
        <img src="https://images.pexels.com/photos/386145/pexels-photo-386145.jpeg?auto=compress&cs=tinysrgb&h=300&w=400" alt="Toyota Camry">
        <img src="https://images.pexels.com/photos/1149831/pexels-photo-1149831.jpeg?auto=compress&cs=tinysrgb&h=300&w=400" alt="Mercedes GLK">
        <img src="https://images.pexels.com/photos/210019/pexels-photo-210019.jpeg?auto=compress&cs=tinysrgb&h=300&w=400" alt="Mercedes GLE">
        <img src="https://images.pexels.com/photos/170811/pexels-photo-170811.jpeg?auto=compress&cs=tinysrgb&h=300&w=400" alt="Toyota Highlander">
    </div>

    <div class="pricing-table">
        <div class="pricing"><h3>Daily</h3><p>₦15,000/day</p></div>
        <div class="pricing"><h3>Weekly</h3><p>₦90,000/week</p></div>
        <div class="pricing"><h3>Airport Pickup</h3><p>₦20,000/ride</p></div>
    </div>

    <div class="services">
        <div class="service"><img src="https://img.icons8.com/ios-filled/50/000000/checked--v1.png"/><p>Easy Booking</p></div>
        <div class="service"><img src="https://img.icons8.com/ios-filled/50/000000/phone.png"/><p>24/7 Support</p></div>
        <div class="service"><img src="https://img.icons8.com/ios-filled/50/000000/car.png"/><p>Flexible Pickup & Drop</p></div>
    </div>

    <div class="fleet-buttons">
        <button class="view-fleet" onclick="scrollToFleet()">View Fleet</button>
        <button class="get-quote" onclick="openQuote()">Get a Quote</button>
        <button class="contact-us" onclick="scrollToContact()">Contact Us</button>
    </div>
</section>

<!-- Features Section -->
<section class="features">
    <h2>Why Choose Us</h2>
    <div class="feature-cards">
        <div class="feature"><img src="https://img.icons8.com/ios-filled/50/000000/rocket.png"/><p>Fast Booking</p></div>
        <div class="feature"><img src="https://img.icons8.com/ios-filled/50/000000/driver.png"/><p>Professional Drivers</p></div>
        <div class="feature"><img src="https://img.icons8.com/ios-filled/50/000000/wallet.png"/><p>Affordable Rates</p></div>
        <div class="feature"><img src="https://img.icons8.com/ios-filled/50/000000/clock.png"/><p>24/7 Support</p></div>
    </div>
</section>

<!-- How It Works Section -->
<section class="how">
    <h2>How It Works</h2>
    <div class="steps">
        <div class="step"><a onclick="openQuote()"><img src="https://img.icons8.com/ios-filled/50/000000/search.png"/><p>Choose Car</p></a></div>
        <div class="step"><img src="https://img.icons8.com/ios-filled/50/000000/form.png"/><p>Book Online</p></div>
        <div class="step"><img src="https://img.icons8.com/ios-filled/50/000000/handshake.png"/><p>Confirm & Pay</p></div>
        <div class="step"><img src="https://img.icons8.com/ios-filled/50/000000/car.png"/><p>Pickup Vehicle</p></div>
        <div class="step"><img src="https://images.pexels.com/photos/1005822/pexels-photo-1005822.jpeg?auto=compress&cs=tinysrgb&h=300&w=400"/><p>Enjoy Your Ride</p></div>
    </div>
</section>

<!-- Testimonials Section -->
<section class="testimonials">
    <h2>Customer Reviews</h2>
    <div class="testimonial-card">
        <img src="https://images.pexels.com/photos/220453/pexels-photo-220453.jpeg?auto=compress&cs=tinysrgb&h=100&w=100" alt="Tunde">
        <p><span>Tunde</span> Excellent service, the car was clean and the driver punctual.</p>
    </div>
    <div class="testimonial-card">
        <img src="https://images.pexels.com/photos/415829/pexels-photo-415829.jpeg?auto=compress&cs=tinysrgb&h=100&w=100" alt="Chiamaka">
        <p><span>Chiamaka</span> Booking was super easy and the customer support very responsive.</p>
    </div>
    <div class="testimonial-card">
        <img src="https://images.pexels.com/photos/2379005/pexels-photo-2379005.jpeg?auto=compress&cs=tinysrgb&h=100&w=100" alt="Emeka">
        <p><span>Emeka</span> Affordable cars, easy process, very satisfied with Makanaki Car Hire.</p>
    </div>
</section>

<!-- FAQ Section -->
<section class="faq">
    <h2>Frequently Asked Questions</h2>
    <div class="faq-item"><p>Q: How do I book a car? <br>A: Simply click Book Now or Get a Quote and follow instructions.</p></div>
    <div class="faq-item"><p>Q: What types of cars do you offer? <br>A: We have Corolla, Camry, GLK, GLE, SUVs and more.</p></div>
    <div class="faq-item"><p>Q: Can I book for airport pickup? <br>A: Yes, we provide airport pickup services at affordable rates.</p></div>
</section>

<!-- Contact Section -->
<section class="contact" id="contact">
    <h2>Contact Us</h2>

    <!-- First Box Image -->
    <div class="contact-box">
        <img src="https://images.pexels.com/photos/110844/pexels-photo-110844.jpeg" alt="First Box" class="contact-img">
    </div>
        <div class="contact-info">
            <p><img src="https://img.icons8.com/ios-filled/50/000000/phone.png"/> +234 801 234 5678</p>
            <p><img src="https://img.icons8.com/ios-filled/50/000000/whatsapp.png"/> +234 801 234 5678</p>
            <p><img src="https://img.icons8.com/ios-filled/50/000000/new-post.png"/> info@makanakicarhire.ng</p>
            <p><img src="https://img.icons8.com/ios-filled/50/000000/facebook-new.png"/> Follow us on social media</p>
        </div>
    </div>
</section>

<!-- Sticky Footer Buttons -->
<<!-- Sticky Footer Buttons -->
<div class="sticky-footer">
    <button class="footer-btn home" onclick="scrollToHome()">
        🏠 Home
    </button>
    <button class="footer-btn fleet-btn" onclick="scrollToFleet()">
        🚗 Fleet
    </button>
    <button class="footer-btn contact" onclick="scrollToContact()">
        📞 Contact
    </button>
</div>

<style>
/* Sticky Footer Container */
.sticky-footer {
    position: fixed;
    bottom: 15px;           /* slightly above bottom */
    left: 50%;
    transform: translateX(-50%);
    background: rgba(255, 255, 255, 0.95);
    display: flex;
    gap: 15px;
    padding: 10px 15px;
    border-radius: 50px;    /* pill shape */
    box-shadow: 0 4px 15px rgba(0,0,0,0.2);
    z-index: 1000;
}

/* Footer Buttons */
.footer-btn {
    background: linear-gradient(135deg, #ff7e5f, #feb47b);
    border: none;
    color: #fff;
    font-weight: bold;
    padding: 12px 20px;
    border-radius: 30px;
    cursor: pointer;
    transition: transform 0.2s, box-shadow 0.2s;
    display: flex;
    align-items: center;
    gap: 8px;
}

.footer-btn:hover {
    transform: scale(1.1);
    box-shadow: 0 6px 15px rgba(0,0,0,0.3);
}

/* Responsive */
@media screen and (max-width: 480px) {
    .sticky-footer {
        gap: 10px;
        padding: 8px 10px;
    }
    .footer-btn {
        padding: 10px 14px;
        font-size: 14px;
    }
}
</style>

<script>
function scrollToHome() {
    window.scrollTo({ top: 0, behavior: 'smooth' });
}

function scrollToFleet() {
    const fleetSection = document.getElementById('fleet');
    fleetSection.scrollIntoView({ behavior: 'smooth' });
}

function scrollToContact() {
    const contactSection = document.getElementById('contact');
    contactSection.scrollIntoView({ behavior: 'smooth' });
}
</script>
