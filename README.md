<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>For My Favorite Person 🌹</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&family=Poppins:wght@300;400;600&display=swap');

        * { box-sizing: border-box; -webkit-tap-highlight-color: transparent; }
        
        body {
            margin: 0;
            padding: 0;
            background: #ffe4e1;
            font-family: 'Poppins', sans-serif;
            overflow-x: hidden;
            display: flex;
            justify-content: center;
        }

        .mobile-container {
            width: 100vw;
            max-width: 450px;
            min-height: 100vh;
            background: #fff0f5;
            position: relative;
            padding: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .screen {
            display: none;
            width: 100%;
            animation: slideIn 0.4s ease-out;
            text-align: center;
        }

        .active { display: block; }

        @keyframes slideIn {
            from { opacity: 0; transform: translateX(20px); }
            to { opacity: 1; transform: translateX(0); }
        }

        /* Elements Styling */
        .glass-card {
            background: rgba(255, 255, 255, 0.8);
            border-radius: 25px;
            padding: 20px;
            box-shadow: 0 8px 32px rgba(255, 182, 193, 0.3);
            border: 1px solid rgba(255, 255, 255, 0.4);
            margin-bottom: 20px;
        }

        h1 { font-family: 'Dancing Script', cursive; color: #d63384; font-size: 2rem; }
        
        .gif-img { width: 100%; border-radius: 15px; margin-bottom: 15px; max-height: 250px; object-fit: contain; }

        .btn {
            background: #ff69b4;
            color: white;
            border: none;
            padding: 15px 30px;
            border-radius: 50px;
            font-weight: 600;
            font-size: 1rem;
            width: 80%;
            margin-top: 10px;
            box-shadow: 0 5px 15px rgba(255, 105, 180, 0.4);
        }

        /* Memories Grid */
        .memories-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 10px;
            margin: 15px 0;
        }
        .mem-img { width: 100%; height: 140px; object-fit: cover; border-radius: 12px; border: 3px solid white; }

        /* Video Styling */
        .video-container { width: 100%; margin-bottom: 20px; }
        video { width: 100%; border-radius: 15px; background: #000; height: 220px; }

        /* Letter Box - Full Message */
        .letter-text {
            text-align: left;
            font-size: 0.95rem;
            line-height: 1.6;
            color: #444;
            white-space: pre-line; /* Isse paragraphs sahi dikhenge */
            padding: 10px;
            max-height: 60vh;
            overflow-y: auto;
        }

        .rose-box { font-size: 50px; display: flex; justify-content: center; gap: 20px; cursor: pointer; }
    </style>
</head>
<body>

<div class="mobile-container">
    
    <div id="p1" class="screen active">
        <div class="glass-card">
            <h1>Happy Rose Day Baby 🌹</h1>
            <img src="http://tmpfiles.org/dl/22876715/fromklickpincftkthao219bubududugif-tkthao219bubududupanda-discoversharegifs_cutecartoonquotescuteanimecatcutebeardrawings1.gif" class="gif-img" alt="Rose Gif">
            <p>A rose for the person who makes my world more beautiful just by being in it ✨</p>
            <button class="btn" onclick="showPage('p2')">Open Memories 🎀</button>
        </div>
    </div>

    <div id="p2" class="screen">
        <div class="glass-card">
            <h1>Pick a Rose</h1>
            <img src="http://tmpfiles.org/dl/22876666/fromklickpincfpinvonelizavetapauesovaaufenrgy_gifbilderlustigniedlicheliebeszeichentrickliebegifthealeni.gif" class="gif-img">
            <p>One of these holds a secret message...</p>
            <div class="rose-box">
                <span onclick="alert('Try another one! 💖')">🌹</span>
                <span onclick="showPage('p3')">🌹</span>
                <span onclick="alert('So close! Try the middle one! 🥰')">🌹</span>
            </div>
        </div>
    </div>

    <div id="p3" class="screen">
        <h1>Our Memories 🎀 🧿</h1>
        <img src="http://tmpfiles.org/dl/22876616/fromklickpincfpinbyceciliadelpantaongif_cutegifcutelovecartoonscutelovepictures.gif" class="gif-img" style="height: 100px;">
        <div class="memories-grid">
            <img src="https://i.postimg.cc/yNqkyd81/IMG_20260206_190532.png" class="mem-img">
            <img src="https://i.postimg.cc/s2Fv4Xg3/IMG_20260206_190558.png" class="mem-img">
            <img src="https://i.postimg.cc/K831TLx4/IMG_20260206_190630.png" class="mem-img">
            <img src="https://i.postimg.cc/rp6KNmw8/IMG_20260206_190726.png" class="mem-img">
            <img src="https://i.postimg.cc/XNxB64s3/IMG_20260206_190744.png" class="mem-img">
            <img src="https://i.postimg.cc/MGkvmTpR/IMG_20260206_190444.png" class="mem-img">
        </div>
        <button class="btn" onclick="showPage('p4')">Next Page 🫶🏻</button>
    </div>

    <div id="p4" class="screen">
        <h1>For You 🫶🏻💗</h1>
        <div class="video-container"><video controls preload="none"><source src="https://files.catbox.moe/mw3f2q.mp4" type="video/mp4"></video></div>
        <div class="video-container"><video controls preload="none"><source src="https://files.catbox.moe/ggbrik.mp4" type="video/mp4"></video></div>
        <div class="video-container"><video controls preload="none"><source src="https://files.catbox.moe/sfk5b8.mp4" type="video/mp4"></video></div>
        <button class="btn" onclick="showPage('p5')">Read My Heart 💖</button>
    </div>

    <div id="p5" class="screen">
        <div class="glass-card">
            <h1>From My Heart 🌹</h1>
            <img src="http://tmpfiles.org/dl/22876413/fromklickpincfbunnysticker-bunny-discoversharegifs_cutelovegifcutegifloveyougif.gif" class="gif-img" style="height:80px">
            <div class="letter-text">
Happy Rose Day, meri zindagi ke sabse khoobsurat ehsaas 🌹

Aaj Rose Day hai, aur jab bhi rose ka naam aata hai na, mujhe aap yaad aa jaate ho. Kyunki jaise ek rose simple hoke bhi special hota hai, waise hi aap meri life me aaye bina koi shor machaye… par dheere dheere sabse important ban gaye. Aapke saath hone ka ehsaas hi alag hai — bina zyada bole, bina zyada dikhaye, bas ek sukoon sa. Jaise kisi thake hue din ke baad achanak thandi hawa mil jaaye.

Mujhe aapki woh chhoti chhoti baatein bohot pasand hain, jinhe shayad duniya notice bhi na kare, par mere liye wahi sabse important hoti hain. Aapka mood, aapki khamoshi, aapki hasi, aur kabhi kabhi aapka bina wajah gussa hona — sab kuch. Aap perfect isliye nahi ho kyunki aap kabhi galat nahi hote, balki isliye ho kyunki aap real ho. Aur mujhe real cheezein hi sabse zyada apni lagti hain.

Rose ki tarah hi pyaar bhi hota hai — thoda soft, thoda strong, kabhi khushboo se bhara, kabhi thoda sa dard bhi deta hai. Par phir bhi koi rose ko chhodta nahi, kyunki uski khoobsurti uske saath aane wale har ehsaas ke layak hoti hai. Bilkul waise hi, aap bhi. Aapke saath har moment easy nahi hota, par har moment worth it hota hai.

Aapko shayad andaza bhi nahi hai ki aapki presence mere liye kya maayne rakhti hai. Jab aap theek hote ho, mujhe lagta hai sab theek hai. Aur jab aap thode low feel karte ho, to dil karta hai bas itna kar paun ki aapko thoda sa halka feel kara saku. Kyunki pyaar ka matlab sirf saath rehna nahi hota, balki ek dusre ki care bina shart ke karna hota hai.

Aaj Rose Day pe main koi wada nahi kar raha, koi badi baat nahi keh raha. Bas itna kehna chahta hoon ki aap meri life ka woh rose ho jo main sambhaal ke rakhna chahta hoon — bina todhe, bina force kiye, bas respect aur care ke saath. Aap jaisa ho, jaise bhi ho, wahi mere liye kaafi hai.

Is Rose Day pe agar main aapko ek rose deta, to uske saath sirf ek hi baat likhta —
“Aap meri life me ho, wahi mere liye sabse badi khushi hai.” 🌹

Happy Rose Day 🤍
Hamesha muskurate rahiye… kyunki aapki muskurahat kisi ke liye bohot special hai.
            </div>
            <button class="btn" onclick="location.reload()">Replay ❤️</button>
        </div>
    </div>

</div>

<script>
    function showPage(pageId) {
        // Sabhi screens hide karo
        document.querySelectorAll('.screen').forEach(s => s.classList.remove('active'));
        // Puraane videos pause karo taaki background mein sound na chale
        document.querySelectorAll('video').forEach(v => v.pause());
        // Naya screen dikhao
        document.getElementById(pageId).classList.add('active');
        window.scrollTo(0,0);
    }
</script>

</body>
</html>
