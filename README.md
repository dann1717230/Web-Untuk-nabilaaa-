# Web-Untuk-nabilaaa-
Web coba coba

<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>BUCIN LEVEL MAX 💗</title>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  min-height: 100vh;
  overflow-x: hidden;
  background: linear-gradient(135deg, #ffe1ec, #ffc6dc, #ffeaf2);
  font-family: 'Trebuchet MS', sans-serif;
  color: #7c3152;
}

.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 25px 15px;
}

.card {
  width: 100%;
  max-width: 380px;
  background: rgba(255,255,255,0.88);
  border: 3px solid white;
  border-radius: 30px;
  padding: 28px 20px;
  text-align: center;
  box-shadow: 0 12px 35px #d77da955;
  animation: muncul 1s ease;
  position: relative;
  z-index: 2;
}

@keyframes muncul {
  from {
    opacity: 0;
    transform: translateY(40px) scale(.9);
  }
  to {
    opacity: 1;
    transform: translateY(0) scale(1);
  }
}

h1 {
  font-size: 25px;
  margin: 15px 0;
  animation: goyang 2s infinite;
}

@keyframes goyang {
  0%, 100% { transform: rotate(-2deg); }
  50% { transform: rotate(2deg); }
}

.bunny {
  font-size: 90px;
  display: inline-block;
  animation: lompat 1.5s infinite;
}

@keyframes lompat {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(-13px); }
}

p {
  font-size: 14px;
  line-height: 1.8;
}

.name {
  margin: 18px 0;
  background: #fff0f6;
  border: 2px dashed #ff8eb8;
  border-radius: 15px;
  padding: 12px;
  font-weight: bold;
  color: #d64d87;
}

.buttons {
  margin-top: 25px;
  display: flex;
  justify-content: center;
  gap: 12px;
  flex-wrap: wrap;
}

button {
  border: none;
  padding: 13px 20px;
  border-radius: 30px;
  font-size: 14px;
  font-weight: bold;
  cursor: pointer;
  transition: transform .2s;
}

button:active {
  transform: scale(.92);
}

.yes {
  color: white;
  background: linear-gradient(135deg, #ff73a7, #ff4e91);
  box-shadow: 0 5px 0 #d83b79;
}

.no {
  color: #b34b76;
  background: #ffe1ed;
  border: 2px solid #ff9fc2;
}

#message {
  display: none;
  margin-top: 23px;
  padding: 15px;
  background: #fff0f6;
  border-radius: 20px;
  animation: muncul .5s ease;
}

#message h2 {
  margin-bottom: 10px;
  font-size: 21px;
}

.footer {
  margin-top: 22px;
  font-size: 11px;
  color: #c56a91;
}

.heart {
  position: fixed;
  top: -30px;
  z-index: 1;
  pointer-events: none;
  animation: jatuh linear forwards;
}

@keyframes jatuh {
  to {
    transform: translateY(110vh) rotate(360deg);
    opacity: 0;
  }
}

.sparkle {
  position: fixed;
  pointer-events: none;
  z-index: 5;
  animation: terbang 1s forwards;
}

@keyframes terbang {
  to {
    transform: translateY(-80px) scale(1.5);
    opacity: 0;
  }
}

.small {
  font-size: 12px;
  color: #b96b8b;
  margin-top: 10px;
}
</style>
</head>

<body>

<div class="container">
  <main class="card">

    <div class="bunny" id="bunny">🐰</div>

    <h1>HALOOO SAYANGGG! 💗</h1>

    <p>
      Ada pengumuman penting nihh... 📢<br>
      Harap dibaca dengan penuh cinta! 💕
    </p>

    <div class="name">
      ⚠️ PERINGATAN ⚠️<br>
      Kamu terlalu lucu & imutt  😭💘
    </div>

    <p>
      Aku punya satu pertanyaan serius...<br>
      <b>Serius banget</b> 
    </p>

    <h1 style="font-size:21px; animation:none;">
      KAMU MAU <br>
    SAYANGINN AKU GAA??💖
    </h1>

    <div class="buttons">
      <button class="yes" onclick="jawabYa()">
        MAUUU 💗
      </button>

      <button class="no" id="noBtn">
        NGGAK MAU 😝
      </button>
    </div>

    <div id="message">
      <h2>YEAYYYY!!! 😭💖</h2>

      <div style="font-size:55px; margin:10px;">
        🐰💗🐻
      </div>

      <p>
        Mulai hari ini kamu resmi jadi
        tersangka pencurian hati! 🚨💘
        <br><br>
        Hadaih nya adalah...
        <br>
        <b>DISAYANGG SETIAP HARI!!</b> 💕
        <br><br>
        Tidak ada banding, tidak ada remisi,
        pokoknya harus sayangiii akuuu! 🫶
      </p>

      <button class="yes" onclick="peluk()">
        KIRIM PELUKK HANGATT🫂
      </button>
    </div>

    <p class="small" id="hint">
    <b><b>jangan pilih tombol gamau!</b></b>
    </p>

    <div class="footer">
      MADE WITH 999999% LOVE 💗<br>
       SAYANGG NABILA
    </div>

<!-- PEMUTAR LAGU BUCIN -->
<div class="music-player">
  <div class="music-icon" id="musicIcon">🎵</div>

  <div class="music-info">
    <strong>Lagu buat kamu 💗</strong>
    <span>Special song for you</span>
  </div>

  <button id="musicButton" onclick="toggleMusic()">
    ▶ PUTAR
  </button>

  <audio id="bgMusic" loop preload="metadata">
    <source src="/Images/untuk perempuan.mp3" type="audio/mpeg">
  </audio>
</div>

<style>
.music-player {
  display: flex;
  align-items: center;
  gap: 10px;
  background: #fff8fc;
  border: 2px solid white;
  border-radius: 20px;
  padding: 12px;
  margin-bottom: 20px;
  box-shadow: 0 5px 15px #d77da933;
}

.music-icon {
  font-size: 28px;
  animation: musicSpin 3s linear infinite;
  animation-play-state: paused;
}

.music-icon.playing {
  animation-play-state: running;
}

@keyframes musicSpin {
  to { transform: rotate(360deg); }
}

.music-info {
  flex: 1;
  min-width: 0;
  text-align: left;
}

.music-info strong,
.music-info span {
  display: block;
}

.music-info strong {
  font-size: 12px;
}

.music-info span {
  font-size: 10px;
  margin-top: 4px;
  color: #b96b8b;
}

#musicButton {
  padding: 10px 12px;
  background: #ff73a7;
  color: white;
  border: none;
  border-radius: 20px;
  font-size: 11px;
  font-weight: bold;
}
</style>

<script>
const bgMusic = document.getElementById("bgMusic");
const musicButton = document.getElementById("musicButton");
const musicIcon = document.getElementById("musicIcon");

async function toggleMusic() {
  if (bgMusic.paused) {
    try {
      await bgMusic.play();
      musicButton.textContent = "❚❚ JEDA";
      musicIcon.classList.add("playing");
    } catch (error) {
      musicButton.textContent = "GAGAL MEMUTAR";
      console.error("Audio error:", error);
    }
  } else {
    bgMusic.pause();
    musicButton.textContent = "▶ PUTAR";
    musicIcon.classList.remove("playing");
  }
}

bgMusic.addEventListener("ended", () => {
  musicButton.textContent = "▶ PUTAR";
  musicIcon.classList.remove("playing");
});
</script>

  </main>
</div>

<script>
const noBtn = document.getElementById("noBtn");
const hint = document.getElementById("hint");
const bunny = document.getElementById("bunny");

let kabur = 0;

function pindahTombol() {
  kabur++;

  const maxX = Math.max(0, window.innerWidth - noBtn.offsetWidth - 20);
  const maxY = Math.max(0, window.innerHeight - noBtn.offsetHeight - 20);

  noBtn.style.position = "fixed";
  noBtn.style.left = Math.random() * maxX + "px";
  noBtn.style.top = Math.random() * maxY + "px";
  noBtn.style.zIndex = "10";

  const jokes = [
    "MUAHHH MUAHHH😚",
    "LOVE YOUUU NABILAA",
    "NABILA KESAYANGANKUU 💗",
    "AKU CINTA NABILA",
    "AKU SAYANGG NABILA"
  ];

  hint.textContent = jokes[Math.min(kabur - 1, jokes.length - 1)];
}

noBtn.addEventListener("mouseenter", pindahTombol);

noBtn.addEventListener("touchstart", function(e) {
  e.preventDefault();
  pindahTombol();
}, { passive: false });

noBtn.addEventListener("click", pindahTombol);

function jawabYa() {
  document.getElementById("message").style.display = "block";
  hint.textContent = "PILIHAN KAMU SANGAT BERKELAS 😭🏆";
  bunny.textContent = "🥰";
  buatHati(35);

  document.getElementById("message").scrollIntoView({
    behavior: "smooth",
    block: "nearest"
  });
}

function peluk() {
  bunny.textContent = "🫂";
  hint.textContent = "PELUK VIRTUAL TERKIRIMMMM 💗";

  buatHati(45);

  for (let i = 0; i < 15; i++) {
    setTimeout(buatSparkle, i * 80);
  }
}

function buatHati(jumlah = 1) {
  for (let i = 0; i < jumlah; i++) {
    setTimeout(() => {
      const heart = document.createElement("div");
      heart.className = "heart";

      const emoji = ["🫂💞🩷", "✨"];
      heart.textContent = emoji[Math.floor(Math.random() * emoji.length)];

      heart.style.left = Math.random() * 100 + "vw";
      heart.style.fontSize = (15 + Math.random() * 22) + "px";
      heart.style.animationDuration = (3 + Math.random() * 4) + "s";

      document.body.appendChild(heart);

      setTimeout(() => heart.remove(), 7500);
    }, i * 45);
  }
}

function buatSparkle() {
  const sparkle = document.createElement("div");
  sparkle.className = "sparkle";
  sparkle.textContent = ["✨", "💗", "⭐", "💕"][Math.floor(Math.random() * 4)];

  sparkle.style.left = Math.random() * 100 + "vw";
  sparkle.style.top = (40 + Math.random() * 50) + "vh";
  sparkle.style.fontSize = "25px";

  document.body.appendChild(sparkle);
  setTimeout(() => sparkle.remove(), 1000);
}

/* Hati turun terus-menerus */
setInterval(() => {
  buatHati(1);
}, 650);
</script>

</body>
</html>
