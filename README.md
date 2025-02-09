# Amrit-lal
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Apology & Friend Request</title>
    <style>
        body {
            text-align: center;
            background-color: #fce4ec; /* Light pink background */
            font-family: 'Comic Sans MS', cursive, sans-serif;
            overflow: hidden;
        }

        h1 {
            color: #ff4081;
            font-size: 26px;
            margin-top: 50px;
            text-shadow: 2px 2px #ff80ab;
        }

        .sticker {
            width: 150px;
            height: auto;
            margin: 20px;
        }

        .button {
            background: #ff4081;
            color: white;
            padding: 15px 25px;
            font-size: 20px;
            border-radius: 50px;
            text-decoration: none;
            display: inline-block;
            transition: transform 0.3s ease-in-out;
            box-shadow: 3px 3px 8px rgba(0, 0, 0, 0.2);
        }

        .button:hover {
            background: #e91e63;
            transform: scale(1.1);
        }

        /* Floating Hearts Animation */
        .heart {
            position: absolute;
            color: #ff1744;
            font-size: 20px;
            animation: floatUp 4s linear infinite;
            opacity: 0.8;
        }

        @keyframes floatUp {
            0% {
                transform: translateY(0) scale(1);
                opacity: 1;
            }
            100% {
                transform: translateY(-500px) scale(0);
                opacity: 0;
            }
        }
    </style>
</head>
<body>

    <h1>I'm really sorry for my rude behavior! 🥺</h1>
    <p>Will you forgive me and be my friend again?</p>

    <!-- Cute GIF -->
    <img class="sticker" src="https://media.giphy.com/media/jUwpNzg9IcyrK/giphy.gif" alt="Cute Apology">

    <!-- Friend Request Button -->
    <br>
    <a class="button" href="#">Let's Be Friends Again 💖</a>

    <script>
        // Function to create floating hearts
        function createHeart() {
            const heart = document.createElement("div");
            heart.classList.add("heart");
            heart.innerHTML = "💖";
            document.body.appendChild(heart);

            // Random position
            heart.style.left = Math.random() * window.innerWidth + "px";
            heart.style.top = window.innerHeight + "px";

            // Animation
            setTimeout(() => {
                heart.remove();
            }, 4000);
        }

        // Generate hearts every 500ms
        setInterval(createHeart, 500);
    </script>

</body>
</html>
