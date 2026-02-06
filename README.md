<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Rose Day 🌹</title>
<style>
body{
  margin:0;
  min-height:100vh;
  font-family:Arial, Helvetica, sans-serif;
  background:linear-gradient(135deg,#ffd6e8,#ffeef5);
  display:flex;
  justify-content:center;
  align-items:center;
}
.card{
  width:92%;
  max-width:380px;
  background:#fff;
  border-radius:24px;
  padding:16px;
  box-shadow:0 12px 35px rgba(0,0,0,0.15);
  text-align:center;
}
.hidden{display:none;}
h2,h3{color:#d6336c;margin:8px 0;}
p{font-size:14px;color:#555;}
button{
  background:#ff4d6d;color:white;border:none;padding:10px 24px;border-radius:24px;font-size:14px;margin-top:12px;cursor:pointer;
}
/* GIF Box */
.gif-box{width:110px;height:110px;margin:0 auto 12px;border-radius:16px;overflow:hidden;}
.gif-box img{width:100%;height:100%;object-fit:cover;}
/* Rose Game */
.roses{display:flex;justify-content:center;gap:18px;font-size:40px;cursor:pointer;}
#roseMessage{margin-top:12px;min-height:44px;font-size:15px;color:#b0004e;font-weight:500;}
/* Photo Grid */
.photo-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:10px;}
.photo-grid img{width:100%;border-radius:14px;}
/* Videos */
video{width:100%;border-radius:14px;margin-bottom:10px;}
/* Letter */
.letter{background:#fff5fa;padding:14px;border-radius:16px;text-align:left;font-size:13px;color:#444;max-height:300px;overflow-y:auto;white-space:pre-wrap;}
/* Mini Games */
.game-box{background:#ffe4f0;padding:10px;border-radius:14px;margin:10px 0;}
.drag-item{width:50px;height:50px;margin:5px;display:inline-block;font-size:32px;cursor:pointer;}
</style>
</head>
<body>

<div class="card">

<!-- HOME -->
<div id="home">
  <div class="gif-box">
    <img src="https://files.catbox.moe/mw3f2q.mp4.gif" alt="GIF">
  </div>
  <h2>Happy Rose Day 🌹</h2>
  <p>For the one who makes my world softer</p>
  <button onclick="openPage('game')">Tap a Rose 🌹</button>
</div>

<!-- ROSE GAME -->
<div id="game" class="hidden">
  <h3>Pick a Rose 🌹</h3>
  <p>Tap any rose to see a cute message</p>
  <div class="roses">
    <span onclick="pickRose()">🌹</span>
    <span onclick="pickRose()">🌹</span>
    <span onclick="pickRose()">🌹</span>
  </div>
  <div id="roseMessage"></div>
  <div class="game-box">
    <h4>Mini Game 1: Tap the heart</h4>
    <div id="hearts">
      <span class="drag-item" onclick="heartClick(this)">❤️</span>
      <span class="drag-item" onclick="heartClick(this)">💖</span>
      <span class="drag-item" onclick="heartClick(this)">💗</span>
    </div>
    <p id="heartMsg"></p>
  </div>
  <button onclick="openPage('photos')">Our Memories 🎀🧿</button>
</div>

<!-- PHOTOS -->
<div id="photos" class="hidden">
  <h3>Our Memories 🎀🧿</h3>
  <div class="photo-grid">
    <img src="https://i.postimg.cc/yNqkyd81/IMG_20260206_190532.png">
    <img src="https://i.postimg.cc/s2Fv4Xg3/IMG_20260206_190558.png">
    <img src="https://i.postimg.cc/K831TLx4/IMG_20260206_190630.png">
    <img src="https://i.postimg.cc/rp6KNmw8/IMG_20260206_190726.png">
    <img src="https://i.postimg.cc/XNxB64s3/IMG_20260206_190744.png">
    <img src="https://i.postimg.cc/MGkvmTpR/IMG_20260206_190444.png">
    <img src="https://i.postimg.cc/k5rBv4gN/IMG_20260206_190512.png">
    <img src="https://i.postimg.cc/xdrc3C16/IMG_20260206_190418.png">
  </div>
  <div class="game-box">
    <h4>Mini Game 2: Find the sparkle ✨</h4>
    <div id="sparkleGame">
      <span class="drag-item" onclick="sparkleClick(this)">✨</span>
      <span class="drag-item" onclick="sparkleClick(this)">💫</span>
      <span class="drag-item" onclick="sparkleClick(this)">🌟</span>
    </div>
    <p id="sparkleMsg"></p>
  </div>
  <button onclick="openPage('videos')">For You 🫶🏻💗</button>
</div>

<!-- VIDEOS -->
<div id="videos" class="hidden">
  <h3>For You 🫶🏻💗</h3>
  <video controls playsinline src="https://files.catbox.moe/mw3f2q.mp4"></video>
  <video controls playsinline src="https://files.catbox.moe/ggbrik.mp4"></video>
  <video controls playsinline src="https://files.catbox.moe/sfk5b8.mp4"></video>
  <video controls playsinline src="https://files.catbox.moe/p150ss.mp4"></video>
  <video controls playsinline src="https://files.catbox.moe/3ju0zb.mp4"></video>
  <video controls playsinline src="https://files.catbox.moe/6kf2dd.mp4"></video>
  <div class="game-box">
    <h4>Mini Game 3: Click the smile 😊</h4>
    <span class="drag-item" onclick="smileClick(this)">😊</span>
    <span class="drag-item" onclick="smileClick(this)">😄</span>
    <span class="drag-item" onclick="smileClick(this)">😃</span>
    <p id="smileMsg"></p>
  </div>
  <button onclick="openPage('letter')">From My Heart 💌</button>
</div>

<!-- LETTER -->
<div id="letter" class="hidden">
  <h3>From My Heart 💌</h3>
  <div class="letter">
Happy Rose Day, meri zindagi ke sabse khoobsurat ehsaas 🌹  
Aaj Rose Day hai, aur jab bhi rose ka naam aata hai na, mujhe aap yaad aa jaate ho. Kyunki jaise ek rose simple hoke bhi special hota hai, waise hi aap meri life me aaye bina koi shor machaye… par dheere dheere sabse important ban gaye. Aapke saath hone ka ehsaas hi alag hai — bina zyada bole, bina zyada dikhaye, bas ek sukoon sa. Jaise kisi thake hue din ke baad achanak thandi hawa mil jaaye.  

Mujhe aapki woh chhoti chhoti baatein bohot pasand hain, jinhe shayad duniya notice bhi na kare, par mere liye wahi sabse important hoti hain. Aapka mood, aapki khamoshi, aapki hasi, aur kabhi kabhi aapka bina wajah gussa hona — sab kuch. Aap perfect isliye nahi ho kyunki aap kabhi galat nahi hote, balki isliye ho kyunki aap real ho. Aur mujhe real cheezein hi sabse zyada apni lagti hain.  

Rose ki tarah hi pyaar bhi hota hai — thoda soft, thoda strong, kabhi khushboo se bhara, kabhi thoda sa dard bhi deta hai. Par phir bhi koi rose ko chhodta nahi… bilkul waise hi, aap bhi.  

Aaj Rose Day pe bas itna kehna chahta hoon ki aap meri life ka woh rose ho jo main sambhaal ke rakhna chahta hoon — bina todhe, bina force kiye, bas respect aur care ke saath.  

“Aap meri life me ho, wahi mere liye sabse badi khushi hai.” 🌹  
Happy Rose Day 🤍
  </div>
  <button onclick="openPage('end')">One Last Thing 🤍</button>
</div>

<!-- END -->
<div id="end" class="hidden">
  <h3>Thank You 🤍</h3>
  <p>
Is chhoti si duniya ka hissa banne ke liye shukriya…  
Agar aap muskuraye ho, to mera purpose complete ho gaya 🌹  
Always stay the way you are. Someone out there cares — deeply.
  </p>
</div>

</div>

<script>
// Page Navigation
function openPage(id){
  document.querySelectorAll('.card > div').forEach(d=>d.classList.add('hidden'));
  document.getElementById(id).classList.remove('hidden');
}

// Rose Game
var roseMessages=[
"You are my calm in chaos ❤️",
"Life feels softer with you 🌸",
"I choose you, every single day 🫶🏻",
"You are my safe place 🤍"
];
function pickRose(){
  var msg=roseMessages[Math.floor(Math.random()*roseMessages.length)];
  document.getElementById("roseMessage").innerText=msg;
}

// Mini Games
function heartClick(el){
  document.getElementById("heartMsg").innerText="You tapped a heart! ❤️";
}
function sparkleClick(el){
  document.getElementById("sparkleMsg").innerText="You found the sparkle! ✨";
}
function smileClick(el){
  document.getElementById("smileMsg").innerText="You clicked the smile! 😊";
}
</script>

</body>
</html>
