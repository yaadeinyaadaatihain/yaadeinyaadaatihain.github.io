<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Yaadein Yaad Aati Hain</title>
  <style>
    /* Reset and base styles */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: linear-gradient(to bottom, #4c1d95, #000);
      color: #fff;
      scroll-behavior: smooth;
    }

    header {
      background-color: #6b21a8;
      padding: 2rem 1rem;
      text-align: center;
    }

    header h1 {
      font-size: 2.5rem;
      margin-bottom: 0.5rem;
    }

    header p {
      font-style: italic;
      font-size: 1.2rem;
    }

    nav {
      background-color: #5b21b6;
      display: flex;
      justify-content: center;
      gap: 2rem;
      padding: 1rem 0;
    }

    nav a {
      color: #fff;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s ease;
    }

    nav a:hover {
      color: #facc15;
    }

    .banner {
      position: relative;
      height: 300px;
      background: url('https://images.unsplash.com/photo-1527254059242-8e1f2d622b7e?auto=format&fit=crop&w=1400&q=80') no-repeat center center/cover;
    }

    .banner-text {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      background: rgba(0, 0, 0, 0.5);
      padding: 1.5rem 2rem;
      border-radius: 10px;
      font-size: 2rem;
      font-weight: bold;
    }

    section {
      padding: 3rem 1.5rem;
      text-align: center;
      animation: fadeIn 1s ease-in;
    }

    section img {
      max-width: 90%;
      border-radius: 10px;
      margin-bottom: 1rem;
      box-shadow: 0 4px 8px rgba(255, 255, 255, 0.1);
    }

    .gallery, .achievements {
      display: grid;
      gap: 1.5rem;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      padding-top: 1rem;
    }

    .achievement-card {
      background: rgba(255, 255, 255, 0.1);
      padding: 1rem;
      border-radius: 10px;
    }

    .achievement-card img {
      width: 100%;
      border-radius: 6px;
    }

    footer {
      background-color: #6b21a8;
      padding: 1rem;
      text-align: center;
      margin-top: 2rem;
    }

    @keyframes fadeIn {
      from {opacity: 0;}
      to {opacity: 1;}
    }
  </style>
</head>
<body>

  <header>
    <h1>Yaadein Yaad Aati Hain</h1>
    <p>A journey through memories and emotions</p>
  </header>

  <div class="banner">
    <div class="banner-text">Welcome to the World of Words</div>
  </div>

  <nav>
    <a href="#introduction">Introduction</a>
    <a href="#about">About Us</a>
    <a href="#gallery">Gallery</a>
    <a href="#achievements">Achievements</a>
    <a href="#contact">Contact</a>
  </nav>

  <section id="introduction">
    <h2>Introduction</h2>
    <img src="https://images.unsplash.com/photo-1531988042231-d39a9cc12a9a?auto=format&fit=crop&w=800&q=80" alt="Writing Introduction Image" />
    <p>Welcome to Yaadein Yaad Aati Hain — a sanctuary of emotions, stories, and the magic of words that bring back memories.</p>
  </section>

  <section id="about" style="background-color: #3c0d99;">
    <h2>About Us</h2>
    <img src="https://images.unsplash.com/photo-1485217988980-11786ced9454?auto=format&fit=crop&w=800&q=80" alt="About Us Image" />
    <p>We are a community of writers, poets, and dreamers who believe in the healing power of writing. Our stories are not just ink on paper—they are echoes of the heart.</p>
  </section>

  <section id="gallery">
    <h2>Gallery</h2>
    <div class="gallery">
      <img src="https://source.unsplash.com/random/400x300?sig=1&writing" alt="Gallery 1">
      <img src="https://source.unsplash.com/random/400x300?sig=2&writing" alt="Gallery 2">
      <img src="https://source.unsplash.com/random/400x300?sig=3&writing" alt="Gallery 3">
    </div>
  </section>

  <section id="achievements" style="background-color: #3c0d99;">
    <h2>Achievements</h2>
    <div class="achievements">
      <div class="achievement-card">
        <img src="https://images.unsplash.com/photo-1494173853739-c21f58b16055?auto=format&fit=crop&w=400&q=80" alt="Published Poet">
        <h3>Published Poet</h3>
        <p>Published in national poetry anthologies</p>
      </div>
      <div class="achievement-card">
        <img src="https://images.unsplash.com/photo-1520974735194-1bc3c46d84c5?auto=format&fit=crop&w=400&q=80" alt="Stage Performer">
        <h3>Stage Performer</h3>
        <p>Performed on major stages across India</p>
      </div>
      <div class="achievement-card">
        <img src="https://images.unsplash.com/photo-1601987077399-a4c2be9c4b4e?auto=format&fit=crop&w=400&q=80" alt="Featured on Radio">
        <h3>Featured on Radio</h3>
        <p>Invited on Red FM to share poetry journey</p>
      </div>
      <div class="achievement-card">
        <img src="https://images.unsplash.com/photo-1519681393784-d120267933ba?auto=format&fit=crop&w=400&q=80" alt="1st Prize - Swarn Abha">
        <h3>1st Prize - Swarn Abha</h3>
        <p>Winner in the Swarn Abha Writing Competition</p>
      </div>
    </div>
  </section>

  <section id="contact">
    <h2>Contact Us</h2>
    <p>For collaborations, queries, or submissions:</p>
    <p>Email: <a href="mailto:yaadeinyaadaatihain@example.com" style="color: #facc15;">yaadeinyaadaatihain@example.com</a></p>
  </section>

  <footer>
    <p>&copy; 2025 Yaadein Yaad Aati Hain. All rights reserved.</p>
  </footer>

</body>
</html>
