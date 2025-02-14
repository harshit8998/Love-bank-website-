# Love-bank-website-<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>A Special Surprise for You ❤️</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <div class="container">
        <h1 id="message">I have something special for you... 💖</h1>
        <button class="btn" onclick="showSurprise()">Click to Unlock</button>
        <p id="finalMessage" style="display: none;">You are the reason my world is so beautiful! 💞 Will you forgive me and be my Valentine? ❤️</p>
    </div>

    <audio id="loveSong" src="valentine-song.mp3"></audio>

    <script src="script.js"></script>

</body>
</html>body {
    text-align: center;
    background-color: black;
    color: white;
    font-family: Arial, sans-serif;
    transition: background 2s, color 2s;
}

.container {
    margin-top: 100px;
}

.btn {
    padding: 10px 20px;
    font-size: 18px;
    background: red;
    color: white;
    border: none;
    cursor: pointer;
    margin-top: 20px;
}

.heart {
    font-size: 50px;
    color: red;
    animation: heartbeat 1s infinite;
}

@keyframes heartbeat {
    0% { transform: scale(1); }
    50% { transform: scale(1.2); }
    100% { transform: scale(1); }
}function showSurprise() {
    document.body.style.backgroundColor = "pink";
    document.body.style.color = "black";
    document.getElementById("message").innerHTML = "Surprise Unlocked! 💖";
    document.getElementById("finalMessage").style.display = "block";
    document.getElementById("loveSong").play();
}