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
        .mobile-container { width: 100vw; max-width: 450px; min-height: 100vh; margin: auto; padding: 15px; position: relative; }
        
        .screen { display: none; text-align: center; animation: fadeIn 0.6s ease; }
        .active { display: block; }
        @keyframes fadeIn { from { opacity: 0; transform: scale(0.9); } to { opacity: 1; transform: scale(1); } }

        .card { background: white; border-radius: 20px; padding: 20px; box-shadow: 0 10px 25px rgba(255, 182, 193, 0.4); border: 2px solid #ffb6c1; margin-top: 10px; }
        h1 { font-family: 'Dancing Script', cursive; color: #d63384; font-size: 2.2rem; }
        
        /* Floating Photo Animation */
        .photo-grid { display: grid; grid-template-columns: repeat(2, 1fr); gap: 15px; padding: 10px; }
        .photo-grid img { 
            width: 100%; height: 160px; object-fit: cover; border-radius: 10px; 
            border: 5px solid white; box-shadow: 0 5px 15px rgba(0,0,0,0.2);
            animation: float 3s ease-in-out infinite alternate;
        }
        .photo-grid img:nth-child(even) { animation-delay: 1.5s; }
        @keyframes float { from { transform: translateY(0) rotate(-2deg); } to { transform: translateY(-10px) rotate(2deg); } }

        /* Vintage Letter */
        .vintage-paper {
            background: #f4e4bc;
            background-image: url('https://www.transparenttextures.com/patterns/paper-fibers.png');
            padding: 30px;
            position: relative;
            border: 2px solid #d2b48c;
            box-shadow: inset 0 0 50px rgba(139,69,19,0.3), 0 5px 15px rgba(0,0,0,0.2);
            font-family: 'Great Vibes', cursive;
            font-size: 1.5rem;
            line-height: 1.4;
            color: #3d2b1f;
            text-align: left;
            border-radius: 5px;
            overflow: hidden;
        }
        .vintage-paper::before {
            content: ''; position: absolute; top:0; left:0; width:100%; height:100%;
            box-shadow: inset 0 0 30px #00000033; pointer-events: none;
        }

        /* Video Box */
        .video-box { width: 100%; height: 500px; background: #000; border-radius: 15px; overflow: hidden; border: 3px solid #ffb6c1; }
        iframe { width: 100%; height: 100%; border: none; }
        .next-btn-hidden { display: none; } /* Initially Hidden */

        .btn { background: #ff69b4; color: white; border: none; padding: 16px; border-radius: 50px; font-size: 1.1rem; font-weight: bold; width: 100%; margin-top: 20px; cursor: pointer; }

        /* Games Section */
        .game-area { width: 100%; height: 300px; background: white; border-radius: 15px; position: relative; overflow: hidden; border: 2px dashed #ff69b4; margin: 15px 0; }
        .heart { position: absolute; font-size: 30px; cursor: pointer; user-select: none; }
        .prize-msg { display: none; background: #fff0f5; padding: 10px; border-radius: 10px; color: #d63384; font-weight: bold; margin-top: 10px; border: 1px solid #ffb6c1; }
    </style>
</head>
<body>

<div class="mobile-container">
    
    <div id="p1" class="screen active">
        <div class="card">
            <h1>Happy Rose Day Baby 🌹</h1>
            <img src="https://lh3.googleusercontent.com/d/1oA0_BlRwJSCSlu5ddegF1Pc8XFp5EI-6" class="media-img" style="width:100%; border-radius:15px;">
            <p>Ready for a small journey of us?</p>
            <button class="btn" onclick="show('p2')">Start 🎀</button>
        </div>
    </div>

    <div id="p2" class="screen">
        <div class="card">
            <h1>Chose a Rose 🌹</h1>
            <img src="https://lh3.googleusercontent.com/d/18jB_pnODqn1pbOB1XJCcVnP_QBYr6ouF" class="media-img" style="width:100%; border-radius:15px;">
            <div style="font-size: 50px; display: flex; justify-content: space-around; padding: 20px;">
                <span onclick="show('p3')">🌹</span><span onclick="show('p3')">🌹</span><span onclick="show('p3')">🌹</span>
            </div>
        </div>
    </div>

    <div id="p3" class="screen">
        <h1>Our Memories 🧿</h1>
        <div class="photo-grid">
            <img src="https://lh3.googleusercontent.com/d/1B4Bj9d15ClW3IoIHJDNuTVes3I8arDg-">
            <img src="https://lh3.googleusercontent.com/d/1MZBfHzLtyw7UORTQTxVQM2ZGCHzJ_Imt">
            <img src="https://lh3.googleusercontent.com/d/18enhwLyCvEYDL2Xo__YfZRFAUbjUKmET">
            <img src="https://lh3.googleusercontent.com/d/1d9aMJEtvlADsNWh0mBp2LiF7iR9fnV22">
            <img src="https://lh3.googleusercontent.com/d/1aFSL8ukbhy2tohjoAf03eotzja4J4Kik">
            <img src="https://lh3.googleusercontent.com/d/1YPtSs7ckY65qpKCOctQEKqTKmzFepByc">
            <img src="https://lh3.googleusercontent.com/d/17G2nGQuqMN9L78QCH39GcsfXHP-XY8SW">
            <img src="https://lh3.googleusercontent.com/d/1IfJckumLmzfKTpTVfDHV_SO10V_SO10">
        </div>
        <button class="btn" onclick="show('g1')">Let's Play A Game ✨</button>
    </div>

    <div id="g1" class="screen">
        <h1>Catch 5 Hearts ❤️</h1>
        <p>Aapki smile jitni pyaari hai, utne hi dil pakadne hain!</p>
        <div class="game-area" id="heart-game"></div>
        <div id="prize1" class="prize-msg">"Waah! Aapki speed to bilkul meri dhadkan tez karne jaisi hai. Pata hai aap bahut zyada beautiful ho?"</div>
        <button id="nextG1" class="btn next-btn-hidden" onclick="show('g2')">Agla Game 🎀</button>
    </div>

    <div id="g2" class="screen">
        <h1>Pop the Stars 🌟</h1>
        <div class="game-area" id="star-game"></div>
        <div id="prize2" class="prize-msg">"Aapke baare mein jitna likhu kam hai, aap kisi angel se kam nahi lagti!"</div>
        <button id="nextG2" class="btn next-btn-hidden" onclick="show('v1')">Ab Kuch Khaas... 🎥</button>
    </div>

    <div id="v1" class="screen">
        <h1>For You 🫶🏻</h1>
        <div class="video-box" data-src="https://drive.google.com/file/d/1KJUT3jNxH10EEdlHUZO-rQ_juQbfV-Ov/preview"></div>
        <p style="font-size: 12px; margin-top:10px;">(Please watch full video to continue...)</p>
        <button class="btn next-btn-hidden" onclick="show('v2')">Next Video ✨</button>
    </div>

    <div id="v6" class="screen">
        <h1>Last One 🫶🏻</h1>
        <div class="video-box" data-src="https://drive.google.com/file/d/1ompKdCqZo51LkXg_e-Y4ytFndp83v6sy/preview"></div>
        <button class="btn next-btn-hidden" onclick="show('pLetter')">Read My Letter 💌</button>
    </div>

    <div id="pLetter" class="screen">
        <h1 style="margin-bottom:15px;">From My Heart 💖</h1>
        <div class="vintage-paper">
            Happy Rose Day, meri zindagi ke sabse khoobsurat ehsaas 🌹<br><br>
            Aaj Rose Day hai, aur jab bhi rose ka naam aata hai na, mujhe aap yaad aa jaate ho. Kyunki jaise ek rose simple hoke bhi special hota hai, waise hi aap meri life me aaye bina koi shor machaye… par dheere dheere sabse important ban gaye. Aapke saath hone ka ehsaas hi alag hai — bina zyada bole, bina zyada dikhaye, bas ek sukoon sa. Jaise kisi thake hue din ke baad achanak thandi hawa mil jaaye.<br><br>
            Mujhe aapki woh chhoti chhoti baatein bohot pasand hain, jinhe shayad duniya notice bhi na kare, par mere liye wahi sabse important hoti hain. Aapka mood, aapki khamoshi, aapki hasi, aur kabhi kabhi aapka bina wajah gussa hona — sab kuch. Aap perfect isliye nahi ho kyunki aap kabhi galat nahi hote, balki isliye ho kyunki aap real ho.<br><br>
            Rose ki tarah hi pyaar bhi hota hai — thoda soft, thoda strong, kabhi khushboo se bhara, kabhi thoda sa dard bhi deta hai. Par phir bhi koi rose ko chhodta nahi, kyunki uski khoobsurti uske saath aane wale har ehsaas ke layak hoti hai. Bilkul waise hi, aap bhi.<br><br>
            Aapko shayad andaza bhi nahi hai ki aapki presence mere liye kya maayne rakhti hai. Jab aap theek hote ho, mujhe lagta hai sab theek hai. Jab aap thode low feel karte ho, to dil karta hai bas itna kar paun ki aapko thoda sa halka feel kara saku. <br><br>
            Aaj Rose Day pe main koi wada nahi kar raha, bas itna kehna chahta hoon ki aap meri life ka woh rose ho jo main sambhaal ke rakhna chahta hoon. Aap jaisa ho, jaise bhi ho, wahi mere liye kaafi hai.<br><br>
            “Aap meri life me ho, wahi mere liye sabse badi khushi hai.” 🌹<br><br>
            Happy Rose Day 🤍
        </div>
        <button class="btn" onclick="show('p6')">Ek Last Cheez... 🥺</button>
    </div>

    <div id="p6" class="screen">
        <div class="card">
            <h1>Thank You 💖</h1>
            <div style="font-family: 'Great Vibes'; font-size: 2rem; color: #d63384;">
                "Thank you for being my constant. Aap meri life ki woh smile ho jo main kabhi khona nahi chahta."
            </div>
            <button class="btn" onclick="location.reload()">Replay ❤️</button>
        </div>
    </div>

</div>

<script>
    function show(id) {
        // Stop current iframes
        document.querySelectorAll('.video-box').forEach(b => b.innerHTML = '');
        
        // Switch Screen
        document.querySelectorAll('.screen').forEach(s => s.classList.remove('active'));
        const next = document.getElementById(id);
        next.classList.add('active');

        // If Video Screen, Load it
        const vBox = next.querySelector('.video-box');
        if(vBox) {
            const src = vBox.getAttribute('data-src');
            vBox.innerHTML = `<iframe src="${src}" allow="autoplay"></iframe>`;
            
            // Simulation: Show button after 15 seconds (As we can't detect Drive end perfectly)
            setTimeout(() => {
                const btn = next.querySelector('.btn');
                if(btn) btn.style.display = 'block';
            }, 15000); 
        }

        // Init Games if needed
        if(id === 'g1') initHeartGame();
        if(id === 'g2') initStarGame();
        
        window.scrollTo(0,0);
    }

    // Heart Game Logic
    function initHeartGame() {
        const area = document.getElementById('heart-game');
        let count = 0;
        const interval = setInterval(() => {
            if(count >= 5) { clearInterval(interval); return; }
            const h = document.createElement('div');
            h.className = 'heart';
            h.innerHTML = '❤️';
            h.style.left = Math.random() * 80 + '%';
            h.style.top = Math.random() * 80 + '%';
            h.onclick = () => {
                h.remove();
                count++;
                if(count === 5) {
                    document.getElementById('prize1').style.display = 'block';
                    document.getElementById('nextG1').style.display = 'block';
                }
            };
            area.appendChild(h);
        }, 1000);
    }

    // Star Game Logic
    function initStarGame() {
        const area = document.getElementById('star-game');
        let count = 0;
        for(let i=0; i<8; i++) {
            const s = document.createElement('div');
            s.className = 'heart';
            s.innerHTML = '🌟';
            s.style.left = Math.random() * 80 + '%';
            s.style.top = Math.random() * 80 + '%';
            s.onclick = () => {
                s.style.transform = 'scale(0)';
                count++;
                if(count === 8) {
                    document.getElementById('prize2').style.display = 'block';
                    document.getElementById('nextG2').style.display = 'block';
                }
            };
            area.appendChild(s);
        }
    }
</script>
</body>
</html>
