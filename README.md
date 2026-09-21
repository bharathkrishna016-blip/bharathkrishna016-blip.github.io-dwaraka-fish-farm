<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>Dwaraka Fish Farm | Ornamental Fish & Aquariums</title>

  <meta name="description"
        content="Dwaraka Fish Farm - Ornamental fish, aquarium plants, aquariums and accessories in Kozhikode, Kerala.">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }

    body {
      font-family: Arial, Helvetica, sans-serif;
      background: #06141c;
      color: white;
      line-height: 1.6;
    }

    /* NAVBAR */

    header {
      position: fixed;
      top: 0;
      width: 100%;
      z-index: 1000;
      background: rgba(3, 15, 22, 0.88);
      backdrop-filter: blur(12px);
      border-bottom: 1px solid rgba(255,255,255,0.08);
    }

    nav {
      max-width: 1200px;
      margin: auto;
      padding: 18px 25px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .logo {
      font-size: 22px;
      font-weight: bold;
      color: #50e3c2;
    }

    .nav-links {
      display: flex;
      gap: 25px;
      list-style: none;
    }

    .nav-links a {
      color: white;
      text-decoration: none;
      font-size: 15px;
      transition: 0.3s;
    }

    .nav-links a:hover {
      color: #50e3c2;
    }

    /* HERO */

    .hero {
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 120px 20px 60px;

      background:
        linear-gradient(rgba(0,15,25,0.65), rgba(0,15,25,0.9)),
        url("images/hero.jpg");

      background-size: cover;
      background-position: center;
    }

    .hero-content {
      max-width: 850px;
    }

    .hero h1 {
      font-size: clamp(45px, 8vw, 85px);
      line-height: 1;
      margin-bottom: 20px;
    }

    .hero h1 span {
      color: #50e3c2;
    }

    .hero p {
      font-size: 20px;
      color: #d4e5e8;
      margin-bottom: 30px;
    }

    .button {
      display: inline-block;
      padding: 14px 25px;
      border-radius: 30px;
      background: #50e3c2;
      color: #031016;
      text-decoration: none;
      font-weight: bold;
      margin: 6px;
      transition: 0.3s;
    }

    .button:hover {
      transform: translateY(-3px);
      box-shadow: 0 10px 30px rgba(80,227,194,0.3);
    }

    .button-outline {
      background: transparent;
      color: white;
      border: 1px solid #50e3c2;
    }

    /* GENERAL */

    section {
      padding: 90px 20px;
    }

    .container {
      max-width: 1150px;
      margin: auto;
    }

    .section-title {
      text-align: center;
      margin-bottom: 50px;
    }

    .section-title h2 {
      font-size: 40px;
      margin-bottom: 10px;
    }

    .section-title p {
      color: #9db1b7;
    }

    /* ABOUT */

    .about {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 45px;
      align-items: center;
    }

    .about img {
      width: 100%;
      border-radius: 20px;
    }

    .about-text h2 {
      font-size: 40px;
      margin-bottom: 20px;
    }

    .about-text p {
      color: #b9c9cd;
      margin-bottom: 15px;
    }

    /* PRODUCTS */

    .products {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 22px;
    }

    .card {
      background: #0b222c;
      border: 1px solid rgba(255,255,255,0.07);
      border-radius: 18px;
      overflow: hidden;
      transition: 0.3s;
    }

    .card:hover {
      transform: translateY(-7px);
      border-color: #50e3c2;
    }

    .card img {
      width: 100%;
      height: 220px;
      object-fit: cover;
    }

    .card-content {
      padding: 22px;
    }

    .card h3 {
      margin-bottom: 8px;
    }

    .card p {
      color: #9db1b7;
      font-size: 14px;
    }

    /* SERVICES */

    .services {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 20px;
    }

    .service {
      text-align: center;
      padding: 30px 20px;
      background: #0b222c;
      border-radius: 18px;
    }

    .service .icon {
      font-size: 40px;
      margin-bottom: 15px;
    }

    .service p {
      color: #9db1b7;
      font-size: 14px;
      margin-top: 8px;
    }

    /* GALLERY */

    .gallery {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 12px;
    }

    .gallery img {
      width: 100%;
      height: 250px;
      object-fit: cover;
      border-radius: 14px;
      transition: 0.3s;
    }

    .gallery img:hover {
      transform: scale(1.03);
    }

    /* CONTACT */

    .contact-box {
      max-width: 800px;
      margin: auto;
      background: #0b222c;
      padding: 45px;
      border-radius: 25px;
      text-align: center;
    }

    .contact-box p {
      color: #b9c9cd;
      margin: 10px;
    }

    /* FOOTER */

    footer {
      text-align: center;
      padding: 35px 20px;
      background: #030b10;
      color: #80939a;
    }

    footer strong {
      color: #50e3c2;
    }

    /* MOBILE */

    @media(max-width: 800px) {

      .nav-links {
        display: none;
      }

      .about {
        grid-template-columns: 1fr;
      }

      .products {
        grid-template-columns: 1fr 1fr;
      }

      .services {
        grid-template-columns: 1fr 1fr;
      }

      .gallery {
        grid-template-columns: 1fr 1fr;
      }
    }

    @media(max-width: 500px) {

      .products,
      .services,
      .gallery {
        grid-template-columns: 1fr;
      }

      .gallery img {
        height: 230px;
      }

      section {
        padding: 70px 18px;
      }
    }
  </style>
</head>

<body>

<!-- NAVIGATION -->

<header>
  <nav>

    <div class="logo">
      🐟 DWARAKA FISH FARM
    </div>

    <ul class="nav-links">
      <li><a href="#home">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#products">Fish</a></li>
      <li><a href="#services">Services</a></li>
      <li><a href="#gallery">Gallery</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>

  </nav>
</header>


<!-- HERO -->

<section class="hero" id="home">

  <div class="hero-content">

    <h1>
      Dwaraka <span>Fish Farm</span>
    </h1>

    <p>
      Ornamental Fish • Aquariums • Aquarium Plants
    </p>

    <p>
      Bringing the beauty of underwater life to your home.
    </p>

    <a href="#products" class="button">
      Explore Our Fish
    </a>

    <a href="#contact" class="button button-outline">
      Contact Us
    </a>

  </div>

</section>


<!-- ABOUT -->

<section id="about">

  <div class="container">

    <div class="about">

      <img src="images/farm.jpg" alt="Dwaraka Fish Farm">

      <div class="about-text">

        <h2>About Our Farm</h2>

        <p>
          Welcome to Dwaraka Fish Farm, your destination for
          beautiful ornamental fish, aquarium plants and
          aquarium solutions.
        </p>

        <p>
          We provide healthy and carefully maintained fish
          for hobbyists, beginners and aquarium enthusiasts.
        </p>

        <p>
          From individual fish to complete aquarium setups,
          we aim to make aquarium keeping simple and enjoyable.
        </p>

      </div>

    </div>

  </div>

</section>


<!-- PRODUCTS -->

<section id="products">

  <div class="container">

    <div class="section-title">

      <h2>Our Collection</h2>

      <p>
        Explore some of the varieties available at our farm.
      </p>

    </div>


    <div class="products">

      <div class="card">

        <img src="images/guppy.jpg">

        <div class="card-content">

          <h3>Guppies</h3>

          <p>
            Colourful and active ornamental fish.
          </p>

        </div>

      </div>


      <div class="card">

        <img src="images/betta.jpg">

        <div class="card-content">

          <h3>Betta</h3>

          <p>
            Beautiful freshwater fish with stunning colours.
          </p>

        </div>

      </div>


      <div class="card">

        <img src="images/molly.jpg">

        <div class="card-content">

          <h3>Molly</h3>

          <p>
            Hardy and beginner-friendly ornamental fish.
          </p>

        </div>

      </div>


      <div class="card">

        <img src="images/goldfish.jpg">

        <div class="card-content">

          <h3>Goldfish</h3>

          <p>
            Classic aquarium favourite.
          </p>

        </div>

      </div>


      <div class="card">

        <img src="images/plants.jpg">

        <div class="card-content">

          <h3>Aquarium Plants</h3>

          <p>
            Natural plants for beautiful aquascapes.
          </p>

        </div>

      </div>


      <div class="card">

        <img src="images/aquarium.jpg">

        <div class="card-content">

          <h3>Custom Aquariums</h3>

          <p>
            Aquariums designed according to your requirements.
          </p>

        </div>

      </div>

    </div>

  </div>

</section>


<!-- SERVICES -->

<section id="services">

  <div class="container">

    <div class="section-title">

      <h2>What We Offer</h2>

      <p>
        Everything you need to create your own underwater world.
      </p>

    </div>


    <div class="services">

      <div class="service">

        <div class="icon">🐟</div>

        <h3>Ornamental Fish</h3>

        <p>
          Different varieties and colour strains.
        </p>

      </div>


      <div class="service">

        <div class="icon">🌿</div>

        <h3>Aquarium Plants</h3>

        <p>
          Plants for natural and planted aquariums.
        </p>

      </div>


      <div class="service">

        <div class="icon">🪟</div>

        <h3>Custom Aquariums</h3>

        <p>
          Aquarium construction and setup.
        </p>

      </div>


      <div class="service">

        <div class="icon">🚚</div>

        <h3>Delivery</h3>

        <p>
          Contact us for available delivery options.
        </p>

      </div>

    </div>

  </div>

</section>


<!-- GALLERY -->

<section id="gallery">

  <div class="container">

    <div class="section-title">

      <h2>Our Gallery</h2>

      <p>
        A glimpse into Dwaraka Fish Farm.
      </p>

    </div>


    <div class="gallery">

      <img src="images/gallery1.jpg">
      <img src="images/gallery2.jpg">
      <img src="images/gallery3.jpg">
      <img src="images/gallery4.jpg">
      <img src="images/gallery5.jpg">
      <img src="images/gallery6.jpg">

    </div>

  </div>

</section>


<!-- CONTACT -->

<section id="contact">

  <div class="container">

    <div class="contact-box">

      <h2>Visit Dwaraka Fish Farm</h2>

      <p>
        Have a question about fish, plants or aquariums?
      </p>

      <p>
        Contact us directly.
      </p>


      <!-- CHANGE THIS NUMBER -->

      <a
        href="https://wa.me/919387522912"
        class="button"
        target="_blank">

        WhatsApp Us

      </a>


      <!-- CHANGE PHONE NUMBER -->

      <a
        href="tel:+919387522912"
        class="button button-outline">

        Call Us

      </a>


      <p>
        📍 Kozhikode, Kerala, India
      </p>

    </div>

  </div>

</section>


<!-- FOOTER -->

<footer>

  <p>
    © 2026 <strong>Dwaraka Fish Farm</strong>
  </p>

  <p>
    Ornamental Fish • Aquariums • Aquarium Plants
  </p>

</footer>


</body>
</html>
