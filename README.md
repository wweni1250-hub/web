<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Portfolio</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: "Poppins", sans-serif;
    }

    body {
      background: #f4f4f9;
      color: #333;
      line-height: 1.6;
    }

    /* Navbar */
    .navbar {
      display: flex;
      justify-content: space-between;
      align-items: center;
      background: #222;
      padding: 1rem 2rem;
      position: sticky;
      top: 0;
      z-index: 1000;
    }

    .navbar .logo {
      color: #fff;
      font-size: 1.5rem;
      font-weight: bold;
    }

    .navbar .nav-links {
      list-style: none;
      display: flex;
    }

    .navbar .nav-links li {
      margin-left: 20px;
    }

    .navbar .nav-links a {
      color: #fff;
      text-decoration: none;
      transition: color 0.3s;
    }

    .navbar .nav-links a:hover {
      color: #ff9800;
    }

    /* Hamburger */
    .hamburger {
      display: none;
      font-size: 2rem;
      color: #fff;
      cursor: pointer;
    }

    @media(max-width: 768px) {
      .nav-links {
        display: none;
        flex-direction: column;
        background: #222;
        position: absolute;
        top: 60px;
        right: 0;
        width: 200px;
      }

      .nav-links li {
        margin: 15px 0;
        text-align: center;
      }

      .hamburger {
        display: block;
      }

      .nav-links.show {
        display: flex;
      }
    }

    /* Hero */
    .hero {
      height: 90vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      background: linear-gradient(to right, #222, #444);
      color: #fff;
      text-align: center;
    }

    .hero h1 {
      font-size: 3rem;
    }

    .hero .highlight {
      color: #ff9800;
    }

    .hero .btn {
      display: inline-block;
      margin-top: 20px;
      padding: 10px 20px;
      background: #ff9800;
      color: #fff;
      text-decoration: none;
      border-radius: 5px;
    }

    .hero .btn:hover {
      background: #e68900;
    }

    /* Section */
    .section {
      padding: 60px 20px;
      text-align: center;
    }

    .section h2 {
      font-size: 2rem;
      margin-bottom: 20px;
    }

    /* Skills */
    .skills-container {
      display: flex;
      justify-content: center;
      gap: 20px;
      flex-wrap: wrap;
    }

    .skill-card {
      background: #fff;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 5px 15px rgba(0,0,0,0.1);
      transition: transform 0.3s;
    }

    .skill-card:hover {
      transform: scale(1.1);
    }

    /* Contact */
    form {
      max-width: 400px;
      margin: auto;
      display: flex;
      flex-direction: column;
      gap: 15px;
    }

    form input, form textarea {
      padding: 10px;
      border: 1px solid #ddd;
      border-radius: 5px;
    }

    form button {
      padding: 10px;
      border: none;
      background: #222;
      color: #fff;
      border-radius: 5px;
      cursor: pointer;
    }

    form button:hover {
      background: #ff9800;
    }

    /* Footer */
    footer {
      text-align: center;
      padding: 20px;
      background: #222;
      color: #fff;
      margin-top: 20px;
    }
  </style>
</head>
<body>
  <!-- Navbar -->
  <header>
    <nav class="navbar">
      <div class="logo">MyPortofolio</div>
      <ul class="nav-links" id="nav-links">
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#portfolio">Portofolio</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
      <div class="hamburger" id="hamburger">☰</div>
    </nav>
  </header>

  <!-- Hero Section -->
  <section id="home" class="hero">
    <h1>Hi, I'm <span class="highlight">Dewi</span></h1>
    <p>Student | Photographer | Creative</p>
    <a href="#portfolio" class="btn">View My Work</a>
  </section>

  <!-- About -->
  <section id="about" class="section">
    <h2>About Me</h2>
    <p>
      Saya seorang pelajar di SMK Negeri 7 Batam.saat ini saya barada di kelas x rpl 1 saya memilih sekolah ini karena saya ingin belajar keterampilan yang bisa langsung diterapkan di dunia kerja khususnya dibidang Rpl saya juga ingin mengembangkan skil teknis dan soft skil sejak dini agar siap menghadapi tantangn di masa depan  dengan belajar disini saya berharap bisa menjadi pribadai yang mandiri ,terampil dan berprestasi
    </p>
  </section>

  <!-- Skills -->
  <section id="skills" class="section">
    <h2>Skills</h2>
    <div class="skills-container">
      <div class="skill-card">📸 Photography</div>
      <div class="skill-card">🖼 menggambar</div>
      <div class="skill-card">kerja sama tim </div>
      <div class="skill-card">menejemen waktu </div>
    </div>
  </section>

  <!-- Portfolio -->
  <section id="portfolio" class="section">
    <h2>Portfolio</h2>
    <div class="portfolio-container">
      <div class="portfolio-card">
        <img src="img1.jpg" alt
        
      
      "badminton">
        <img src="img2.jpg" alt="Event Photography">
        <p>pramuka </p>
      </div>
      <div class="portfolio-card">
        <img src="img3.jpg" alt="Street Photography">
        <p>Life in nongsa </p>
      </div>
    </div>
  </section>

  <!-- Contact -->
  <section id="contact" class="section">
    <h2>Contact</h2>
    <form>
      <input type="text" placeholder="Your Name" required>
      <input type="email" placeholder="Your Email" required>
      <textarea placeholder="Your Message" required></textarea>
      <button type="submit">Send</button>
    </form>
  </section>

  <!-- Footer -->
  <footer>
    <p>&copy; 2025 My Portfolio | All Rights Reserved</p>
  </footer>

  <script>
    // Responsive Hamburger Menu
    const hamburger = document.getElementById("hamburger");
    const navLinks = document.getElementById("nav-links");

    hamburger.addEventListener("click", () => {
      navLinks.classList.toggle("show");
    });

    document.querySelectorAll(".nav-links a").forEach(link => {
      link.addEventListener("click", () => {
        navLinks.classList.remove("show");
      });
    });
  </script>
</body>
</html>
