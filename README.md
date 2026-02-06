<!DOCTYPE html>
<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Rose Day Special 🌹</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&family=Poppins:wght@300;400;600&family=Great+Vibes&display=swap');
        
        * { box-sizing: border-box; margin: 0; padding: 0; }
        body { background: #fff0f5; font-family: 'Poppins', sans-serif; overflow-x: hidden; }
        .mobile-container { width: 100vw; max-width: 450px; min-height: 100vh; margin: auto; padding: 15px; }
        
        .screen { display: none; text-align: center; animation: fadeIn 0.5s ease; }
        .active { display: block; }
        @keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }

        .card { background: white; border-radius: 20px; padding: 20px; box-shadow: 0 10px 25px rgba(255, 182, 193, 0.4); border: 2px solid #ffb6c1; margin-top: 10px; }
        h1 { font-family: 'Dancing Script', cursive; color: #d63384; font-size: 2rem; margin-bottom: 15px; }
        
        /* Floating Photos */
        .photo-grid { display: grid; grid-template-columns: repeat(2, 1fr); gap: 12px; padding: 5px; }
        .photo-grid img { 
            width: 100%; height: 150px; object-fit: cover; border-radius: 10px; 
            border: 4px solid white; box-shadow: 0 4px 10px rgba(0,0,0,0.1);
            animation: float 3s ease-in-out infinite alternate;
        }
        @keyframes float { from { transform: translateY(0px) rotate(-1deg); } to { transform: translateY(-8px) rotate(1deg); } }

        /* Vintage Letter */
        .vintage-paper {
            background: #f4e4bc;
            background-image: url('https://www.transparenttextures.com/patterns/paper-fibers.png');
            padding: 25px; border: 1px solid #d2b48c; border-radius: 5px;
            box-shadow: inset 0 0 40px rgba(139,69,19,0.2);
            font-family: 'Great Vibes', cursive; font-size: 1.4rem;
            color: #3d2b1f; text-align: left; line-height: 1.3;
        }

        .video-box { width: 100%; height: 480px; background: #000; border-radius: 15px; overflow: hidden; border: 2px solid #ffb6c1; }
        iframe { width: 100%; height: 100%; border: none; }
        
        .btn { background: #ff69b4; color: white; border: none; padding: 16px; border-radius: 50px; font-size: 1.1rem; font-weight: bold; width: 100%; margin-top: 20px; cursor: pointer; }
        .next-btn-hidden { display: none; }

        /* Games */
        .game-area { width: 100%; height: 280px; background: white; border-radius: 15px; position: relative; overflow: hidden; border: 2px dashed #ffb6c1; margin-top: 10px; }
        .obj { position: absolute; font-size: 30px; cursor: pointer; transition: transform 0.2s; }
        .prize-msg { display: none; background: #fffafb; padding: 12px; border-radius: 10px; color: #d63384; font-weight: 600; margin-top: 10px; border: 1px solid #ffb6c1; font-size: 0.9rem; }
    </style>
</head>
<body>

<div class="mobile-container">
    
    <div id="p1" class="screen active">
        <div class="card">
            <h1>Happy Rose Day Baby 🌹</h1>
            <img src="https://lh3.googleusercontent.com/d/1X-u9W6mU-x2_fX_U9-YJ6g2D5p8E6vXU" class="media-img" style="width:100%; border-radius:15px;">
            <p>Ready for a small journey of us?</p>
            <button class="btn" onclick="show('p2')">Start 🎀</button>
        </div>
    </div>

    <div id="p2" class="screen">
        <div class="card">
            <h1>Choose a Rose 🌹</h1>
            <img src="https://lh3.googleusercontent.com/d/1_T0e5T4M8e7kXn9_F_U9-YJ6g2D5p8E6v" class="media-img" style="width:100%; border-radius:15px;">
            <div style="font-size: 50px; display: flex; justify-content: space-around; padding: 20px;">
                <span onclick="show('p3')">🌹</span><span onclick="show('p3')">🌹</span><span onclick="show('p3')">🌹</span>
            </div>
        </div>
    </div>

    <div id="p3" class="screen">
        <h1>Our Memories 🧿</h1>
        <div class="photo-grid">
            <img src="https://lh3.googleusercontent.com/d/1KJUT3jNxH10EEdlHUZO-rQ_juQbfV-Ov">
            <img src="https://lh3.googleusercontent.com/d/1rHikV2ia4Dh8sddrcn8u54Z18HsGDfAo">
            <img src="https://lh3.googleusercontent.com/d/1a-7kXpd6EMq7zGIIgX7GlC6gMIQNcztM">
            <img src="https://lh3.googleusercontent.com/d/1q_xc4axTytBExwOpwlYU4gpra6WHTMt6">
            <img src="https://lh3.googleusercontent.com/d/133glT6xC8dVyjcCNrLBTvCr5rSy8aAtv">
            <img src="https://lh3.googleusercontent.com/d/1ompKdCqZo51LkXg_e-Y4ytFndp83v6sy">
            <img src="https://lh3.googleusercontent.com/d/1_T0e5T4M8e7kXn9_F_U9-YJ6g2D5p8E6v">
            <img src="https://lh3.googleusercontent.com/d/1X-u9W6mU-x2_fX_U9-YJ6g2D5p8E6vXU">
        </div>
        <button class="btn" onclick="show('g1')">Let's Play Games ✨</button>
    </div>

    <div id="g1" class="screen">
        <h1>Catch 5 Hearts ❤️</h1>
        <div class="game-area" id="heart-game"></div>
        <div id="prize1" class="prize-msg">"Waah! Aapki speed meri dhadkan tez karne jaisi hai. Pata hai aap bahut beautiful ho?"</div>
        <button id="nextG1" class="btn next-btn-hidden" onclick="show('g2')">Next Game 🎀</button>
    </div>

    <div id="g2" class="screen">
        <h1>Pop 8 Stars 🌟</h1>
        <div class="game-area" id="star-game"></div>
        <div id="prize2" class="prize-msg">"Aap kisi angel se kam nahi lagti, aapki aankhein sab kuch bol deti hain!"</div>
        <button id="nextG2" class="btn next-btn-hidden" onclick="show('v1')">Watch Videos 🎥</button>
    </div>

    <div id="v1" class="screen"><h1>For You 🫶🏻</h1><div class="video-box" data-src="https://drive.google.com/file/d/1KJUT3jNxH10EEdlHUZO-rQ_juQbfV-Ov/preview"></div><button class="btn next-btn-hidden" onclick="show('v2')">Next Video ✨</button></div>
    <div id="v2" class="screen"><h1>For You 🫶🏻</h1><div class="video-box" data-src="https://drive.google.com/file/d/1rHikV2ia4Dh8sddrcn8u54Z18HsGDfAo/preview"></div><button class="btn next-btn-hidden" onclick="show('v3')">Next Video ✨</button></div>
    <div id="v3" class="screen"><h1>For You 🫶🏻</h1><div class="video-box" data-src="https://drive.google.com/file/d/1a-7kXpd6EMq7zGIIgX7GlC6gMIQNcztM/preview"></div><button class="btn next-btn-hidden" onclick="show('v4')">Next Video ✨</button></div>
    <div id="v4" class="screen"><h1>For You 🫶🏻</h1><div class="video-box" data-src="https://drive.google.com/file/d/1q_xc4axTytBExwOpwlYU4gpra6WHTMt6/preview"></div><button class="btn next-btn-hidden" onclick="show('v5')">Next Video ✨</button></div>
    <div id="v5" class="screen"><h1>For You 🫶🏻</h1><div class="video-box" data-src="https://drive.google.com/file/d/133glT6xC8dVyjcCNrLBTvCr5rSy8aAtv/preview"></div><button class="btn next-btn-hidden" onclick="show('v6')">Last Video ✨</button></div>
    <div id="v6" class="screen"><h1>For You 🫶🏻</h1><div class="video-box" data-src="https://drive.google.com/file/d/1ompKdCqZo51LkXg_e-Y4ytFndp83v6sy/preview"></div><button class="btn next-btn-hidden" onclick="show('pLetter')">Read My Letter 💌</button></div>

    <div id="pLetter" class="screen">
        <h1>From My Heart 💖</h1>
        <div class="vintage-paper">
            Happy Rose Day, meri zindagi ke sabse khoobsurat ehsaas 🌹<br><br>
            Aaj Rose Day hai, aur jab bhi rose ka naam aata hai na, mujhe aap yaad aa jaate ho. Kyunki jaise ek rose simple hoke bhi special hota hai, waise hi aap meri life me aaye bina koi shor machaye… par dheere dheere sabse important ban gaye. Aapke saath hone ka ehsaas hi alag hai — bina zyada bole, bina zyada dikhaye, bas ek sukoon sa. Jaise kisi thake hue din ke baad achanak thandi hawa mil jaaye.<br><br>
            Mujhe aapki woh chhoti chhoti baatein bohot pasand hain, jinhe shayad duniya notice bhi na kare, par mere liye wahi sabse important hoti hain. Aapka mood, aapki khamoshi, aapki hasi, aur kabhi kabhi aapka bina wajah gussa hona — sab kuch. Aap perfect isliye nahi ho kyunki aap kabhi galat nahi hote, balki isliye ho kyunki aap real ho. Aur mujhe real cheezein hi sabse zyada apni lagti hain.<br><br>
            Rose ki tarah hi pyaar bhi hota hai — thoda soft, thoda strong, kabhi khushboo se bhara, kabhi thoda sa dard bhi deta hai. Par phir bhi koi rose ko chhodta nahi, kyunki uski khoobsurti uske saath aane wale har ehsaas ke layak hoti hai. Bilkul waise hi, aap bhi. Aapke saath har moment easy nahi hota, par har moment worth it hota hai.<br><br>
            Aapko shayad andaza bhi nahi hai ki aapki presence mere liye kya maayne rakhti hai. Jab aap theek hote ho, mujhe lagta hai sab theek hai. Aur jab aap thode low feel karte ho, to dil karta hai bas itna kar paun ki aapko thoda sa halka feel kara saku. Kyunki pyaar ka matlab sirf saath rehna nahi hota, balki ek dusre ki care bina shart ke karna hota hai.<br><br>
            Aaj Rose Day pe main koi wada nahi kar raha, koi badi baat nahi keh raha. Bas itna kehna chahta hoon ki aap meri life ka woh rose ho jo main sambhaal ke rakhna chahta hoon — bina todhe, bina force kiye, bas respect aur care ke saath. Aap jaisa ho, jaise bhi ho, wahi mere liye kaafi hai.<br><br>
            Is Rose Day pe agar main aapko ek rose deta, to uske saath sirf ek hi baat likhta — “Aap meri life me ho, wahi mere liye sabse badi khushi hai.” 🌹<br><br>
            Happy Rose Day 🤍<br>
            Hamesha muskurate rahiye…
        </div>
        <button class="btn" onclick="show('p6')">Ek Last Cheez... 🥺</button>
    </div>

    <div id="p6" class="screen">
        <div class="card">
            <h1>Thank You 💖</h1>
            <div style="font-family: 'Great Vibes'; font-size: 1.8rem; color: #d63384; padding: 10px;">
                "Thank you meri har chhoti baat samajhne ke liye, mere pagalpan ko jhelne ke liye aur mujhe itna special feel karane ke liye. Aap meri life ki woh smile ho jo main kabhi khona nahi chahta. 🧿🫶🏻"
            </div>
            <button class="btn" onclick="location.reload()">Replay ❤️</button>
        </div>
    </div>

</div>

<script>
    function show(id) {
        // Stop sound: Clear all video boxes
        document.querySelectorAll('.video-box').forEach(b => b.innerHTML = '');
        
        // Switch screens
        document.querySelectorAll('.screen').forEach(s => s.classList.remove('active'));
        const next = document.getElementById(id);
        next.classList.add('active');

        // Load Video and Timer
        const vBox = next.querySelector('.video-box');
        if(vBox) {
            vBox.innerHTML = `<iframe src="${vBox.getAttribute('data-src')}" allow="autoplay"></iframe>`;
            // Button appears after 12 seconds
            setTimeout(() => {
                const b = next.querySelector('.btn');
                if(b) b.style.display = 'block';
            }, 12000);
        }

        if(id === 'g1') initHearts();
        if(id === 'g2') initStars();
        window.scrollTo(0,0);
    }

    function initHearts() {
        const a = document.getElementById('heart-game'); a.innerHTML = ''; let c = 0;
        const i = setInterval(() => {
            if(c >= 5) { clearInterval(i); return; }
            const h = document.createElement('div'); h.className = 'obj'; h.innerHTML = '❤️';
            h.style.left = Math.random()*80+'%'; h.style.top = Math.random()*80+'%';
            h.onclick = () => { h.remove(); c++; if(c==5){ document.getElementById('prize1').style.display='block'; document.getElementById('nextG1').style.display='block'; } };
            a.appendChild(h);
        }, 800);
    }

    function initStars() {
        const a = document.getElementById('star-game'); a.innerHTML = ''; let c = 0;
        for(let i=0; i<8; i++) {
            const s = document.createElement('div'); s.className = 'obj'; s.innerHTML = '🌟';
            s.style.left = Math.random()*80+'%'; s.style.top = Math.random()*80+'%';
            s.onclick = () => { s.style.transform='scale(0)'; c++; if(c==8){ document.getElementById('prize2').style.display='block'; document.getElementById('nextG2').style.display='block'; } };
            a.appendChild(s);
        }
    }
</script>
</body>
</html>
