<!DOCTYPE html>
<html lang="bn">
<head>
<meta charset="UTF-8">
<title>অগ্রিম ভালোবাসা দিবসের শুভেচ্ছা 💌</title>

<!-- Cute Bangla-friendly font -->
<link href="https://fonts.googleapis.com/css2?family=Hind+Siliguri:wght@600&display=swap" rel="stylesheet">

<style>
    body {
        margin: 0;
        overflow: hidden;
        background: url("IMGjoyami.webp") no-repeat center center/cover;
        height: 100vh;
    }

    .falling-text {
        position: absolute;
        top: -50px;
        font-family: 'Hind Siliguri', sans-serif;
        font-size: 28px;
        color: #722F37; /* Wine red */
        animation: fall linear infinite;
        user-select: none;
        white-space: nowrap;
        text-shadow: 2px 2px 10px rgba(0,0,0,0.3);
    }

    @keyframes fall {
        to {
            transform: translateY(110vh);
        }
    }
</style>
</head>

<body>

<!-- Background Music -->
<audio id="bgMusic" autoplay loop>
    <source src="dui Prithibi.mp3" type="audio/mpeg">
</audio>

<script>
function createText() {
    const text = document.createElement("div");
    text.classList.add("falling-text");
    text.innerText = "অগ্রিম ভালোবাসা দিবসের শুভেচ্ছা 💖";

    text.style.left = Math.random() * window.innerWidth + "px";
    text.style.animationDuration = (4 + Math.random() * 4) + "s";
    text.style.fontSize = (22 + Math.random() * 18) + "px";

    document.body.appendChild(text);

    setTimeout(() => {
        text.remove();
    }, 8000);
}

setInterval(createText, 600);


/* Some browsers block autoplay.
   This ensures music plays when user taps anywhere */
document.addEventListener("click", function() {
    document.getElementById("bgMusic").play();
});
</script>

</body>
</html>
