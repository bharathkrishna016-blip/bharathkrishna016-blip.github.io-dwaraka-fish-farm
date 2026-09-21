<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Dwaraka Fish Farm | Ornamental Fish & Aquariums</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            background: #f5fbff;
            color: #123;
        }

        /* HEADER */
        header {
            background: #0077b6;
            color: white;
            padding: 18px 7%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .logo {
            font-size: 24px;
            font-weight: bold;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin-left: 20px;
            font-weight: bold;
        }

        /* HERO */
        .hero {
            min-height: 75vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding: 40px 20px;

            background:
                linear-gradient(rgba(0,80,120,0.65), rgba(0,40,80,0.75)),
                url("images/farm.jpg");

            background-size: cover;
            background-position: center;
            color: white;
        }

        .hero h1 {
            font-size: 48px;
            margin-bottom: 15px;
        }

        .hero p {
            font-size: 20px;
            margin-bottom: 25px;
        }

        .button {
            display: inline-block;
            padding: 13px 25px;
            background: #00b4d8;
            color: white;
            text-decoration: none;
            border-radius: 30px;
            margin: 5px;
            font-weight: bold;
        }

        .button:hover {
            background: #0096c7;
        }

        /* SECTIONS */
        section {
            padding: 60px 7%;
            text-align: center;
        }

        section h2 {
            font-size: 32px;
            margin-bottom: 30px;
            color: #0077b6;
        }

        /* PRODUCTS */
        .products {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 25px;
        }

        .card {
            background: white;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 5px 20px rgba(0,0,0,0.1);
            transition: 0.3s;
        }

        .card:hover {
            transform: translateY(-5px);
        }

        .card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .card-content {
            padding: 20px;
        }

        .card h3 {
            margin-bottom: 10px;
        }

        /* ABOUT */
        .about {
            max-width: 800px;
            margin: auto;
            font-size: 18px;
            line-height: 1.7;
        }

        /* CONTACT */
        .contact {
            background: #023e8a;
            color: white;
        }

        .contact h2 {
            color: white;
        }

        /* FOOTER */
        footer {
            background: #001d3d;
            color: white;
            text-align: center;
            padding: 20px;
        }

        /* MOBILE */
        @media(max-width: 700px) {

            header {
                flex-direction: column;
                gap: 10px;
            }

            nav a {
                margin: 5px;
                font-size: 14px;
            }

            .hero h1 {
                font-size: 34px;
            }

            .hero p {
                font-size: 17px;
            }
        }
    </style>
</head>

<body>

<!-- HEADER -->

<header>

    <div class="logo">
        🐟 Dwaraka Fish Farm
    </div>

    <nav>
        <a href="#home">Home</a>
        <a href="#fish">Fish</a>
        <a href="#aquariums">Aquariums</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
    </nav>

</header>


<!-- HERO -->

<section class="hero" id="home">

    <div>

        <h1>Dwaraka Fish Farm</h1>

        <p>
            Ornamental Fish • Aquariums • Aquatic Plants
        </p>

        <a class="button" href="#fish">
            View Our Fish
        </a>

        <a class="button"
           href="https://wa.me/91XXXXXXXXXX">
            WhatsApp Us
        </a>

    </div>

</section>


<!-- FISH -->

<section id="fish">

    <h2>Our Ornamental Fish</h2>

    <div class="products">

        <div class="card">

            <img src="images/guppy.jpg" alt="Guppy Fish">

            <div class="card-content">

                <h3>Guppy</h3>

                <p>Beautiful colourful guppies.</p>

            </div>

        </div>


        <div class="card">

            <img src="images/betta.jpg" alt="Betta Fish">

            <div class="card-content">

                <h3>Betta</h3>

                <p>Colourful and unique betta varieties.</p>

            </div>

        </div>


        <div class="card">

            <img src="images/goldfish.jpg" alt="Goldfish">

            <div class="card-content">

                <h3>Goldfish</h3>

                <p>Healthy ornamental goldfish.</p>

            </div>

        </div>


        <div class="card">

            <img src="images/flowerhorn.jpg" alt="Flowerhorn">

            <div class="card-content">

                <h3>Flowerhorn</h3>

                <p>Premium ornamental varieties.</p>

            </div>

        </div>

    </div>

</section>


<!-- AQUARIUMS -->

<section id="aquariums">

    <h2>Custom Aquariums</h2>

    <div class="products">

        <div class="card">

            <img src="images/aquarium1.jpg" alt="Aquarium">

            <div class="card-content">

                <h3>Custom Aquariums</h3>

                <p>
                    Aquariums made according to your requirements.
                </p>

            </div>

        </div>


        <div class="card">

            <img src="images/aquarium2.jpg" alt="Planted Aquarium">

            <div class="card-content">

                <h3>Planted Aquariums</h3>

                <p>
                    Beautiful planted aquarium setups.
                </p>

            </div>

        </div>

    </div>

</section>


<!-- PLANTS -->

<section>

    <h2>Aquatic Plants</h2>

    <div class="products">

        <div class="card">

            <img src="images/plants.jpg" alt="Aquatic Plants">

            <div class="card-content">

                <h3>Aquatic Plants</h3>

                <p>
                    Healthy aquatic plants for your aquarium.
                </p>

            </div>

        </div>

    </div>

</section>


<!-- ABOUT -->

<section id="about">

    <h2>About Dwaraka Fish Farm</h2>

    <div class="about">

        <p>
            Welcome to Dwaraka Fish Farm. We specialize in
            ornamental fish, aquariums and aquatic plants.
            Our goal is to provide healthy fish and quality
            aquarium products for hobbyists.
        </p>

    </div>

</section>


<!-- CONTACT -->

<section class="contact" id="contact">

    <h2>Contact Us</h2>

    <p>📍 Kozhikode, Kerala</p>

    <br>

    <p>📞 +91 9387522912</p>

    <br>

    <a class="button"
       href="https://wa.me/919387522912">
        💬 WhatsApp
    </a>

</section>


<!-- FOOTER -->

<footer>

    <p>
        © 2026 Dwaraka Fish Farm. All Rights Reserved.
    </p>

</footer>

</body>
</html>
