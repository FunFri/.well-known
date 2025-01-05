<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Home Page</title>
    <link rel="stylesheet" href="styles.css">
    <link href="https://fonts.googleapis.com/css2?family=Unbounded:wght@900&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Unbounded', sans-serif;
            font-weight: 900;
            margin: 0;
            padding: 0;
            background: #000000;  /* Updated to true black */
            color: #fff;
        }

        header {
            background-color: #000;
            color: #fff;
            padding: 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.3);
        }

        .logo a {
            display: flex;
            align-items: center;
            text-decoration: none;
            color: white;
            font-size: 24px;
        }

        .logo a span {
            color: white;
        }

        .logo img {
            width: 40px;
            height: 40px;
            margin-right: 10px;
        }

        nav a {
            margin: 0 15px;
            text-decoration: none;
            color: white;
            font-size: 18px;
            transition: color 0.3s;
        }

        nav a:hover {
            color: #87CEEB;
        }

        .game-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            gap: 20px;
            padding: 40px;
        }

        .game-widget {
            display: block;
            background-color: #000;
            border-radius: 15%;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.3);
            overflow: hidden;
            text-align: center;
            transition: transform 0.3s ease, box-shadow 0.3s ease, background-color 0.3s ease;
        }

        .game-widget img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            transition: transform 0.3s ease;
            border-radius: 15%;
        }

        .game-widget p {
            font-size: 18px;
            padding: 10px;
            background-color: #000;
            color: #fff;
            margin: 0;
            font-weight: bold;
        }

        .game-widget:hover {
            transform: scale(1.05);
            background-color: #000;
            box-shadow: 0 10px 15px rgba(0, 0, 0, 0.5);
        }

        .game-widget:hover img {
            transform: scale(1.1);
        }

        .alert-message {
            background-color: #000;
            color: #fff;
            padding: 10px;
            font-size: 18px;
            text-align: center;
            margin: 20px 0;
            font-weight: bold;
            border-radius: 8px;
        }

        .alert-message p {
            margin: 10px 0;
        }

        .alert-message p:first-of-type {
            font-size: 96px;
            font-weight: bold; 
            margin-bottom: 0;
        }

        .alert-message p:nth-of-type(2) {
            margin-top: 0;
        }

        .alert-message strong {
            color: red;
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .game-widget {
            animation: fadeInUp 0.5s ease-out;
        }

        .game-widget:nth-child(even) {
            animation-delay: 0.2s;
        }

        .game-widget:nth-child(odd) {
            animation-delay: 0.4s;
        }

        footer {
            background: #000;
            color: #fff;
            padding: 10px 20px;
            display: flex;
            justify-content: space-between; /* Align items to the left and right */
            align-items: center;
            font-size: 16px;
            position: fixed;
            bottom: 0;
            width: 100%;
            box-shadow: 0px -4px 6px rgba(0, 0, 0, 0.3);
        }

        .support-email {
            margin-right: 20px; /* Adds some space between the email and social icons */
        }

        .button-container {
            display: flex;
            align-items: center;
        }

        .image-button {
            background: none;
            border: none;
            margin-left: 10px;
            cursor: pointer;
        }

        .image-button img {
            width: 30px;
            height: 30px;
            transition: transform 0.3s ease;
        }

        .image-button img:hover {
            transform: scale(1.2);
        }

        /* Style for the email link */
        .email-link {
            color: white;  /* Set the text color to white */
            text-decoration: underline;  /* Underline the email */
        }

        /* Style for the TinyURL link */
        .tinyurl-link {
            color: white; /* Set the text color to white */
            text-decoration: underline; /* Make the link underlined */
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">
            <a href="HomePage.html">
                <span>Fun-Fri</span>
            </a>
        </div>
        <nav>
            <a href="Activities.html">Games</a>
            <a href="Apps.html">Apps</a>
            <a href="Extra.html">Extras</a>
        </nav>
    </header>

    <div class="alert-message">
        <p>Fun-Fri</p>
        <p>Happy New Year!</p>
        <p>↓</p>
        <p><strong>PLEASE NOTE:</strong> This platform is not to be used during instructional teaching time, and violating this rule will cause this website to have limited access!</p>
        <p>Questions or Suggestions? Email me at <a href="mailto:funfribusiness@gmail.com" class="email-link">funfribusiness@gmail.com</a></p>
        <p>Share with friends! URL: <a href="https://tinyurl.com/funfri25" class="tinyurl-link">tinyurl.com/funfri25</a></p>
        <p>Want to search games? Just press "ctrl f" on your keyboard!</p>
    </div>

    <main>
        <div class="game-grid">
            <a href="Baldi.html" class="game-widget">
                <img src="Assets/Images/Baldi.jpg" alt="Baldi">
                <p>Baldi Basics</p>
            </a>
            <a href="GeforceNow.html" class="game-widget">
                <img src="Assets/Images/Fortnite.png" alt="Fortnite">
                <p>Fortnite</p>
            </a>
            <a href="CarKingArena.html" class="game-widget">
                <img src="Assets/Images/CarKingArena.jpg" alt="Car King Arena">
                <p>Car King Arena</p>
            </a>
            <a href="Roblox.html" class="game-widget">
                <img src="Assets/Images/Roblox.png" alt="Roblox">
                <p>Roblox</p>
            </a>
            <a href="FInalearth.html" class="game-widget">
                <img src="Assets/Images/TheFinalEarth2.jpg" alt="The Final Earth 2">
                <p>The Final Earth 2</p>
            </a>
            <a href="Granny.html" class="game-widget">
                <img src="Assets/Images/Granny.jpg" alt="Granny">
                <p>Granny</p>
            </a>
            <a href="PolyTrack.html" class="game-widget">
                <img src="Assets/Images/PolyTrack.jpg" alt="Poly Track">
                <p>Poly Track</p>
            </a>
            <a href="PixelSpeedrun.html" class="game-widget">
                <img src="Assets/Images/PixelSpeedrun.jpg" alt="Pixel Speedrun">
                <p>Pixel Speedrun</p>
            </a>
        </div>
    </main>
    
    </script>
</body>
</html>
