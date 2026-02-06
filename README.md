<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Rose Day My Love</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&family=Poppins:wght@300;400;600&display=swap');

        body {
            margin: 0;
            padding: 0;
            background-color: #ffe4e1;
            font-family: 'Poppins', sans-serif;
            overflow-x: hidden;
            color: #4a4a4a;
        }

        .container {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            min-height: 100vh;
            padding: 20px;
            text-align: center;
        }

        .card {
            background: rgba(255, 255, 255, 0.9);
            padding: 25px;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            max-width: 400px;
            width: 90%;
            border: 2px solid #ffb6c1;
            animation: fadeIn 0.8s ease-in-out;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        h1 { font-family: 'Dancing Script', cursive; color: #d63384; font-size: 2.2rem; margin-bottom: 10px; }
        h2 { font-size: 1.2rem; color: #ff69b4; margin-bottom: 20px; }

        .main-gif { width: 100%; border-radius: 15px; margin-bottom: 15px; }

        .btn {
            background: #ff69b4;
            color: white;
            border: none;
            padding: 12px 25px;
            border-radius: 25px;
            font-size: 1rem;
            cursor: pointer;
            transition: 0.3s;
            box-shadow: 0 4px 15px rgba(255, 105, 180, 0.4);
            margin-top: 10px;
        }

        .btn:hover { background: #d63384; transform: scale(1.05); }

        /* Rose Pick Section */
        .rose-container { display: flex; justify-content: space-around; margin: 20px 0; }
        .rose { font-size: 40px; cursor: pointer; transition: 0.3s; }
        .rose:hover { transform: scale(1.2); }

        /* Memories Grid */
        .memory-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 10px;
            margin-top: 15px;
        }
        .mem-img { width: 100%; height: 100px; object-fit: cover; border-radius: 10px; border: 2px solid #ffb6c1; }

        /* Video Section */
        video { width: 100%; border-radius: 15px; margin-bottom: 10px; border: 2px solid #ff69b4; }

        /* Letter Section */
        .letter-box {
            text-align: left;
            font-size: 0.9rem;
            line-height: 1.6;
            background: #fffafa;
            padding: 15px;
            border-radius: 10px;
            height: 300px;
            overflow-y: auto;
            border-left: 5px solid #ff69b4;
        }

        .hidden { display: none; }
        
        /* Floating Hearts Background */
        .heart {
            position: fixed;
            top: -10%;
            font-size: 20px;
            color: #ffb6c1;
            z-index: -1;
            animation: move 5s linear infinite;
        }
        @keyframes move {
            to { transform: translateY(110vh) rotate(360deg); }
        }
    </style>
</head>
<body>

<div class="container">
    <div id="page1" class="card">
        <h1>Happy Rose Day Baby 🌹</h1>
        <img src="http://tmpfiles.org/dl/22876715/fromklickpincftkthao219bubududugif-tkthao219bubududupanda-discoversharegifs_cutecartoonquotescuteanimecatcutebeardrawings1.gif" class="main-gif">
        <p>A rose for the person who makes my world more beautiful just by being in it ✨</p>
        <button class="btn" onclick="nextPage('page2')">Open Memories</button>
    </div>

    <div id="page2" class="card hidden">
        <h1>Pick a Rose</h1>
        <h2>One of these holds a secret message...</h2>
        <img src="http://tmpfiles.org/dl/22876666/fromklickpincfpinvonelizavetapauesovaaufenrgy_gifbilderlustigniedlicheliebeszeichentrickliebegifthealeni.gif" class="main-gif">
        <div class="rose-container">
            <span class="rose" onclick="alert('This one is pretty, but try another!')">🌹</span>
            <span class="rose" onclick="nextPage('page3')">🌹</span>
            <span class="rose" onclick="alert('So close! Try the middle one!')">🌹</span>
        </div>
    </div>

    <div id="page3" class="card hidden">
        <h1>Our Memories 🎀 🧿</h1>
        <img src="http://tmpfiles.org/dl/22876616/fromklickpincfpinbyceciliadelpantaongif_cutegifcutelovecartoonscutelovepictures.gif" class="main-gif">
        <div class="memory-grid">
            <img src="https://i.postimg.cc/yNqkyd81/IMG_20260206_190532.png" class="mem-img">
            <img src="https://i.postimg.cc/s2Fv4Xg3/IMG_20260206_190558.png" class="mem-img">
            <img src="https://i.postimg.cc/K831TLx4/IMG_20260206_190630.png" class="mem-img">
            <img src="https://i.postimg.cc/rp6KNmw8/IMG_20260206_190726.png" class="mem-img">
            <img src="https://i.postimg.cc/XNxB64s3/IMG_20260206_190744.png" class="mem-img">
            <img src="https://i.postimg.cc/MGkvmTpR/IMG_20260206_190444.png" class="mem-img">
        </div>
        <button class="btn" onclick="nextPage('page4')">See More</button>
    </div>

    <div id="page4" class="card hidden">
        <h1>For You 🫶🏻💗</h1>
        <video controls> <source src="https://files.catbox.moe/mw3f2q.mp4" type="video/mp4"> </video>
        <video controls> <source src="https://files.catbox.moe/ggbrik.mp4" type="video/mp4"> </video>
        <video controls> <source src="https://files.catbox.moe/sfk5b8.mp4" type="video/mp4"> </video>
        <p style="font-size: 0.8rem;">Scroll down for more videos</p>
        <button class="btn" onclick="nextPage('page5')">Final Surprise</button>
    </div>

    <div id="page5" class="card hidden">
        <h1>From My Heart 💖</h1>
        <img src="http://tmpfiles.org/dl/22876413/fromklickpincfbunnysticker-bunny-discoversharegifs_cutelovegifcutegifloveyougif.gif" class="main-gif">
        <div class="letter-box">
            <strong>My Dearest,</strong><br><br>
            Happy Rose Day, meri zindagi ke sabse khoobsurat ehsaas 🌹<br>
            Aaj Rose Day hai, aur jab bhi rose ka naam aata hai na, mujhe aap yaad aa jaate ho...<br><br>
            Aap meri life me aaye bina koi shor machaye… par dheere dheere sabse important ban gaye. Aapke saath hone ka ehsaas hi alag hai — bina zyada bole, bina zyada dikhaye, bas ek sukoon sa. Jaise kisi thake hue din ke baad achanak thandi hawa mil jaaye.<br><br>
            Mujhe aapki woh chhoti chhoti baatein bohot pasand hain... Aapka mood, aapki khamoshi, aapki hasi, aur kabhi kabhi aapka bina wajah gussa hona — sab kuch. Aap perfect isliye nahi ho kyunki aap kabhi galat nahi hote, balki isliye ho kyunki aap real ho.<br><br>
            Rose ki tarah hi pyaar bhi hota hai — thoda soft, thoda strong. Aapke saath har moment easy nahi hota, par har moment worth it hota hai.<br><br>
            Aaj Rose Day pe main koi wada nahi kar raha, bas itna kehna chahta hoon ki aap meri life ka woh rose ho jo main sambhaal ke rakhna chahta hoon. Aap jaisa ho, jaise bhi ho, wahi mere liye kaafi hai.<br><br>
            “Aap meri life me ho, wahi mere liye sabse badi khushi hai.” 🌹<br><br>
            <strong>Always Yours 🤍</strong>
        </div>
        <button class="btn" onclick="location.reload()">Back to Start</button>
    </div>
</div>

<script>
    function nextPage(id) {
        document.querySelectorAll('.card').forEach(card => card.classList.add('hidden'));
        document.getElementById(id).classList.remove('hidden');
        window.scrollTo(0,0);
    }

    // Floating Hearts Logic
    function createHeart() {
        const heart = document.createElement('div');
        heart.classList.add('heart');
        heart.innerHTML = '❤️';
        heart.style.left = Math.random() * 100 + 'vw';
        heart.style.animationDuration = Math.random() * 2 + 3 + 's';
        document.body.appendChild(heart);
        setTimeout(() => { heart.remove(); }, 5000);
    }
    setInterval(createHeart, 400);
</script>

</body>
</html>
