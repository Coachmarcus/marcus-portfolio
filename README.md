<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Portfolio Last Tab Revamp</title>
  <style>
    /* Reset & Basic Styles */
    * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Poppins', sans-serif; }
    body { min-height: 100vh; background: linear-gradient(135deg, #6a11cb, #2575fc); display: flex; justify-content: center; align-items: center; color: #fff; }
    a { text-decoration: none; color: inherit; }

    /* Container */
    .portfolio-tab {
      background: rgba(255,255,255,0.05);
      border-radius: 20px;
      padding: 40px;
      width: 90%;
      max-width: 1200px;
      backdrop-filter: blur(10px);
      box-shadow: 0 8px 20px rgba(0,0,0,0.3);
      animation: fadeIn 1s ease-in-out;
    }

    /* Header */
    .portfolio-tab h1 {
      text-align: center;
      margin-bottom: 30px;
      font-size: 2.5rem;
      color: #fff;
      text-shadow: 2px 2px 8px rgba(0,0,0,0.3);
    }

    /* Cards */
    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }

    .card {
      background: rgba(255,255,255,0.1);
      border-radius: 15px;
      padding: 20px;
      transition: transform 0.3s, box-shadow 0.3s;
      backdrop-filter: blur(5px);
      cursor: pointer;
    }

    .card:hover {
      transform: translateY(-10px);
      box-shadow: 0 10px 25px rgba(0,0,0,0.5);
    }

    .card img {
      width: 100%;
      border-radius: 15px;
      margin-bottom: 15px;
    }

    .card h3 {
      margin-bottom: 10px;
      font-size: 1.5rem;
      color: #fff;
    }

    .card p {
      font-size: 1rem;
      line-height: 1.4;
      color: #ddd;
    }

    /* Buttons */
    .card a {
      display: inline-block;
      margin-top: 10px;
      padding: 10px 20px;
      background: #2575fc;
      color: #fff;
      border-radius: 10px;
      transition: background 0.3s;
    }

    .card a:hover {
      background: #6a11cb;
    }

    /* Profile Image Highlight */
    .profile-img {
      display: flex;
      justify-content: center;
      margin-bottom: 30px;
    }

    .profile-img img {
      width: 150px;
      height: 150px;
      border-radius: 50%;
      border: 4px solid #fff;
      transition: transform 0.3s;
    }

    .profile-img img:hover {
      transform: scale(1.1);
    }

    /* Animations */
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    /* Responsive */
    @media(max-width: 768px){
      .portfolio-tab { padding: 30px; }
      .portfolio-tab h1 { font-size: 2rem; }
    }

  </style>
</head>
<body>
  <div class="portfolio-tab">
    <!-- Profile -->
    <div class="profile-img">
      <img src="https://avatars.githubusercontent.com/u/171789491?v=4" alt="Profile Picture">
    </div>

    <h1>My Projects</h1>

    <!-- Project Cards -->
    <div class="cards">
      <div class="card">
        <img src="https://via.placeholder.com/400x250.png?text=Project+1" alt="Project 1">
        <h3>Project One</h3>
        <p>A clean and modern web project showcasing interactive design and responsive layout.</p>
        <a href="#">View Project</a>
      </div>

      <div class="card">
        <img src="https://via.placeholder.com/400x250.png?text=Project+2" alt="Project 2">
        <h3>Project Two</h3>
        <p>Another creative design highlighting animation effects and modern UI patterns.</p>
        <a href="#">View Project</a>
      </div>

      <div class="card">
        <img src="https://via.placeholder.com/400x250.png?text=Project+3" alt="Project 3">
        <h3>Project Three</h3>
        <p>A responsive web section that adapts beautifully across all devices and screens.</p>
        <a href="#">View Project</a>
      </div>
    </div>
  </div>
</body>
</html>
