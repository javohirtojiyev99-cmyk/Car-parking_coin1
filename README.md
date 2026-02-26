<!DOCTYPE html>
<html lang="uz">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Telegram Stars va Premium Tanlash</title>
<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@700&display=swap" rel="stylesheet">
<style>
    body {
        font-family: 'Orbitron', sans-serif;
        background: linear-gradient(270deg, #1a1a1a, #222222, #333333, #222222);
        background-size: 800% 800%;
        color: white;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        height: 100vh;
        text-align: center;
        animation: gradientBG 15s ease infinite;
    }

    @keyframes gradientBG {
        0%{background-position:0% 50%}
        50%{background-position:100% 50%}
        100%{background-position:0% 50%}
    }

    h1 {
        font-size: 2.5em;
        margin-bottom: 30px;
        animation: glowTitle 1.5s infinite alternate;
    }

    @keyframes glowTitle {
        from { text-shadow: 0 0 5px #ff9800, 0 0 10px #ff9800; }
        to { text-shadow: 0 0 20px #ffcc00, 0 0 30px #ffcc00; }
    }

    .button-container {
        display: flex;
        gap: 30px;
        margin-bottom: 30px;
    }

    button {
        padding: 15px 30px;
        font-size: 18px;
        border: none;
        border-radius: 10px;
        cursor: pointer;
        font-weight: bold;
        width: 180px;
        transition: 0.3s;
    }

    #stars { background-color:#ffcc00; color:black; }
    #premium { background-color:#ff99cc; color:white; }

    button:hover { opacity: 0.8; }

</style>
</head>
<body>

<h1>Telegram Tanlash</h1>

<div class="button-container">
    <button id="stars">TELEGRAM STARS</button>
    <button id="premium">TELEGRAM PREMIUM</button>
</div>

<script>
const telegramUsername = "TOJIYEV_722";

document.getElementById("stars").addEventListener("click", () => {
    const message = encodeURIComponent("Salom, men TELEGRAM STARS olmoqchiman");
    const link = `https://t.me/${telegramUsername}?text=${message}`;
    window.open(link, "_blank");
});

document.getElementById("premium").addEventListener("click", () => {
    const message = encodeURIComponent("Salom, men TELEGRAM PREMIUM olmoqchiman");
    const link = `https://t.me/${telegramUsername}?text=${message}`;
    window.open(link, "_blank");
});
</script>

</body>
</html>
