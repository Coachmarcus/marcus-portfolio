<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Earnest Model Private School, Ikirun</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">
    <!-- Custom CSS for enhanced school branding and visuals -->
    <style>
        :root {
            --primary-color: #004080; /* Deep blue for school primary */
            --secondary-color: #FFD700; /* Gold accent for highlights */
            --accent-color: #28a745; /* Green for calls to action */
            --text-color: #333;
            --bg-light: #f8f9fa;
            --bg-dark: #e9ecef;
        }
        body {
            font-family: 'Roboto', sans-serif;
            color: var(--text-color);
            background-color: var(--bg-light);
        }
        .header {
            background-color: var(--primary-color);
            color: white;
            padding: 60px 0;
            text-align: center;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }
        .logo {
            height: 180px;
            margin-bottom: 20px;
            animation: fadeIn 1s ease-in-out;
        }
        .navbar {
            background-color: var(--bg-dark);
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }
        .nav-link {
            color: var(--primary-color) !important;
            font-weight: bold;
        }
        .nav-link:hover {
            color: var(--secondary-color) !important;
        }
        .footer {
            background-color: var(--primary-color);
            color: white;
            padding: 40px 0;
            text-align: center;
            margin-top: 60px;
        }
        .hero-carousel .carousel-item img {
            height: 500px;
            object-fit: cover;
        }
        .hero-carousel .carousel-caption {
            background: rgba(0, 0, 0, 0.5);
            padding: 20px;
            border-radius: 10px;
        }
        .section-title {
            margin-bottom: 40px;
            color: var(--primary-color);
            position: relative;
            text-align: center;
        }
        .section-title::after {
            content: '';
            width: 50px;
            height: 3px;
            background: var(--secondary-color);
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
        }
        .card {
            transition: transform 0.3s, box-shadow 0.3s;
            border: none;
            border-radius: 15px;
            overflow: hidden;
        }
        .card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.15);
        }
        .card-icon {
            font-size: 3rem;
            color: var(--accent-color);
        }
        #gallery .img-fluid {
            border-radius: 10px;
            transition: transform 0.3s;
        }
        #gallery .img-fluid:hover {
            transform: scale(1.05);
        }
        .btn-primary {
            background-color: var(--accent-color);
            border-color: var(--accent-color);
        }
        .btn-primary:hover {
            background-color: darken(var(--accent-color), 10%);
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        .fade-in {
            animation: fadeIn 1.5s ease-in-out;
        }
        #map {
            height: 400px;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }
    </style>
    <!-- Google Fonts for better typography -->
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
</head>
<body>

<!-- Header with Animated Logo -->
<header class="header">
    <img src="https://emps.edu.mm/assets/uploads/4e150-logo.png" alt="Earnest Model Private School Logo" class="logo">
    <h1 class="fade-in">Earnest Model Private School, Ikirun</h1>
    <p class="fade-in">A Place Where Future Leaders Are Nurtured</p>
</header>

<!-- Navigation Bar with Hover Effects -->
<nav class="navbar navbar-expand-lg sticky-top">
    <div class="container">
        <a class="navbar-brand" href="#"><i class="bi bi-school me-2"></i>EMPS</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav ms-auto">
                <li class="nav-item"><a class="nav-link" href="#home">Home</a></li>
                <li class="nav-item"><a class="nav-link" href="#about">About Us</a></li>
                <li class="nav-item"><a class="nav-link" href="#academics">Academics</a></li>
                <li class="nav-item"><a class="nav-link" href="#admissions">Admissions</a></li>
                <li class="nav-item"><a class="nav-link" href="#gallery">Gallery</a></li>
                <li class="nav-item"><a class="nav-link" href="#contact">Contact</a></li>
                <li class="nav-item"><a class="nav-link btn btn-primary text-white ms-3" href="portal.html">Portal</a></li>
            </ul>
        </div>
    </div>
</nav>

<!-- Hero Carousel for Visual Engagement -->
<section id="home" class="hero-carousel">
    <div id="heroCarousel" class="carousel slide" data-bs-ride="carousel">
        <div class="carousel-inner">
            <div class="carousel-item active">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR4zan8j9jVHvZ8wtDvS4XQCIHlzMxpBswXWuc66XlbWgV9FbI0oY3e5Z28&s=10" class="d-block w-100" alt="Campus 1">
                <div class="carousel-caption d-none d-md-block">
                    <h2>Welcome to EMPS</h2>
                    <p>Quality Education in a Nurturing Environment</p>
                    <a href="#admissions" class="btn btn-light">Apply Now</a>
                </div>
            </div>
            <div class="carousel-item">
                <img src="https://cdn.businessday.ng/wp-content/uploads/2024/08/Untitled-design-2024-08-15T155047.340-1.png" class="d-block w-100" alt="Learning">
                <div class="carousel-caption d-none d-md-block">
                    <h2>Empowering Future Leaders</h2>
                    <p>Holistic Development for Every Child</p>
                    <a href="#academics" class="btn btn-light">Learn More</a>
                </div>
            </div>
            <div class="carousel-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcST4uMDdfWGXQ2CMYeNzS4WX26JEdU2m7rcSlwfcWy7OSaKiuZKtk1-FC8&s=10" class="d-block w-100" alt="Events">
                <div class="carousel-caption d-none d-md-block">
                    <h2>Join Our Community</h2>
                    <p>Exciting Events and Activities</p>
                    <a href="#gallery" class="btn btn-light">View Gallery</a>
                </div>
            </div>
        </div>
        <button class="carousel-control-prev" type="button" data-bs-target="#heroCarousel" data-bs-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Previous</span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#heroCarousel" data-bs-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Next</span>
        </button>
    </div>
</section>

<!-- Main Content with Fade-in Animations -->
<main class="container my-5">

    <!-- About Section -->
    <section id="about" class="fade-in">
        <h2 class="section-title">About Us</h2>
        <div class="row align-items-center">
            <div class="col-md-6">
                <img src="https://houseplanng.com/wp-content/uploads/wp-realestate-uploads/_property_gallery/2025/01/modern-school-plan1.jpg" alt="School Building" class="img-fluid rounded shadow">
            </div>
            <div class="col-md-6">
                <p>Earnest Model Private School is a premier educational institution in Ikirun, Osun State, Nigeria, committed to holistic education fostering academic excellence, moral integrity, and leadership.</p>
                <div class="row mt-4">
                    <div class="col-6">
                        <h4>Mission</h4>
                        <p>Empower students to become responsible global citizens.</p>
                    </div>
                    <div class="col-6">
                        <h4>Vision</h4>
                        <p>Leading in excellence and innovation in Nigeria.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Academics Section with Cards -->
    <section id="academics" class="mt-5 fade-in">
        <h2 class="section-title">Academics</h2>
        <p class="text-center mb-4">Our curriculum meets international standards across all levels.</p>
        <div class="row">
            <div class="col-md-4 mb-4">
                <div class="card text-center bg-white">
                    <div class="card-body">
                        <i class="bi bi-book card-icon d-block mb-3"></i>
                        <h5 class="card-title">Nursery</h5>
                        <p>Play-based learning for strong foundations.</p>
                    </div>
                </div>
            </div>
            <div class="col-md-4 mb-4">
                <div class="card text-center bg-white">
                    <div class="card-body">
                        <i class="bi bi-pencil-square card-icon d-block mb-3"></i>
                        <h5 class="card-title">Primary</h5>
                        <p>Focus on literacy, numeracy, and core skills.</p>
                    </div>
                </div>
            </div>
            <div class="col-md-4 mb-4">
                <div class="card text-center bg-white">
                    <div class="card-body">
                        <i class="bi bi-graduation card-icon d-block mb-3"></i>
                        <h5 class="card-title">Secondary</h5>
                        <p>Advanced preparation for higher education.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Admissions Section with Form -->
    <section id="admissions" class="mt-5 fade-in bg-light py-5">
        <h2 class="section-title">Admissions</h2>
        <p class="text-center">Join us! Apply online or download our form.</p>
        <div class="text-center">
            <a href="portal.html" class="btn btn-primary btn-lg">Online Admission</a>
            <a href="#" class="btn btn-outline-secondary btn-lg ms-3" data-bs-toggle="modal" data-bs-target="#newsletterModal">Subscribe to Newsletter</a>
        </div>
        <!-- Newsletter Modal -->
        <div class="modal fade" id="newsletterModal" tabindex="-1" aria-labelledby="newsletterLabel" aria-hidden="true">
            <div class="modal-dialog">
                <div class="modal-content">
                    <div class="modal-header">
                        <h5 class="modal-title" id="newsletterLabel">Subscribe to Our Newsletter</h5>
                        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                    </div>
                    <div class="modal-body">
                        <form>
                            <div class="mb-3">
                                <label for="email" class="form-label">Email Address</label>
                                <input type="email" class="form-control" id="email" required>
                            </div>
                            <button type="submit" class="btn btn-primary">Subscribe</button>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Gallery Section with Grid and Hover Effects -->
    <section id="gallery" class="mt-5 fade-in">
        <h2 class="section-title">Gallery</h2>
        <div class="row">
            <div class="col-md-4 mb-4">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcST4uMDdfWGXQ2CMYeNzS4WX26JEdU2m7rcSlwfcWy7OSaKiuZKtk1-FC8&s=10" alt="School Event 1" class="img-fluid shadow">
            </div>
            <div class="col-md-4 mb-4">
                <img src="https://cdn.businessday.ng/wp-content/uploads/2024/08/Untitled-design-2024-08-15T155047.340-1.png" alt="Classroom Activity" class="img-fluid shadow">
            </div>
            <div class="col-md-4 mb-4">
                <img src="https://tribuneonlineng.com/wp-content/uploads/2016/07/osun-public-secondary-school.jpg" alt="Sports Day" class="img-fluid shadow">
            </div>
            <div class="col-md-4 mb-4">
                <img src="https://tribuneonlineng.com/wp-content/uploads/2016/07/osun-public-secondary-school.jpg" alt="Graduation Ceremony" class="img-fluid shadow">
            </div>
            <div class="col-md-4 mb-4">
                <img src="https://www.shutterstock.com/image-photo/onitsha-anambra-statenigeria-october-6-260nw-2686747695.jpg" alt="Science Lab" class="img-fluid shadow">
            </div>
            <div class="col-md-4 mb-4">
                <img src="https://houseplanng.com/wp-content/uploads/wp-realestate-uploads/_property_gallery/2025/01/modern-school-plan1.jpg" alt="School Trip" class="img-fluid shadow">
            </div>
        </div>
    </section>

    <!-- Contact Section with Form and Map -->
    <section id="contact" class="mt-5 fade-in">
        <h2 class="section-title">Contact Us</h2>
        <div class="row">
            <div class="col-md-6">
                <p><i class="bi bi-geo-alt-fill me-2"></i>Location: Ikirun, Osun State, Nigeria</p>
                <p><i class="bi bi-telephone-fill me-2"></i>Phone: +234-123-456-7890</p>
                <p><i class="bi bi-envelope-fill me-2"></i>Email: info@earnestmodel.sch.ng</p>
                <form class="mt-4">
                    <div class="mb-3">
                        <label for="name" class="form-label">Name</label>
                        <input type="text" class="form-control" id="name" required>
                    </div>
                    <div class="mb-3">
                        <label for="email" class="form-label">Email</label>
                        <input type="email" class="form-control" id="email" required>
                    </div>
                    <div class="mb-3">
                        <label for="message" class="form-label">Message</label>
                        <textarea class="form-control" id="message" rows="5" required></textarea>
                    </div>
                    <button type="submit" class="btn btn-primary">Send Message</button>
                </form>
            </div>
            <div class="col-md-6">
                <div id="map">
                    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d15778.328849060964!2d4.655327!3d7.916666!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x103bb9a0a0000001%3A0x1000000000000000!2sIkirun%2C%20Osun%20State%2C%20Nigeria!5e0!3m2!1sen!2sus!4v1700000000000" width="100%" height="400" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
                </div>
            </div>
        </div>
    </section>

</main>

<!-- Footer with Social Links -->
<footer class="footer">
    <p>&copy; 2026 Earnest Model Private School, Ikirun. All rights reserved.</p>
    <p>Follow us: <a href="https://www.facebook.com/groups/me" class="text-white"><i class="bi bi-facebook me-2"></i>Facebook</a> | <a href="#" class="text-white"><i class="bi bi-twitter-x me-2"></i>X</a> | <a href="#" class="text-white"><i class="bi bi-instagram"></i>Instagram</a></p>
</footer>

<!-- Bootstrap JS -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script>

<!-- Custom JS for Smooth Scrolling -->
<script>
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
        anchor.addEventListener('click', function (e) {
            e.preventDefault();
            document.querySelector(this.getAttribute('href')).scrollIntoView({
                behavior: 'smooth'
            });
        });
    });
</script>

</body>
</html>
