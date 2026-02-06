<!DOCTYPE html>
<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Happy Rose Day 🌹</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&family=Poppins:wght@300;400;600&display=swap');

        * { box-sizing: border-box; margin: 0; padding: 0; }
        
        body {
            background: #fff0f5;
            font-family: 'Poppins', sans-serif;
            color: #4a4a4a;
            overflow-x: hidden;
            display: flex;
            justify-content: center;
        }

        .mobile-container {
            width: 100vw;
            max-width: 450px;
            min-height: 100vh;
            background: #fff0f5;
            padding: 15px;
            display: flex;
            flex-direction: column;
        }

        .screen {
            display: none;
            text-align: center;
            animation: fadeIn 0.5s ease-in-out;
        }

        .active { display: block; }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .card {
            background: white;
            border-radius: 20px;
            padding: 20px;
            box-shadow: 0 10px 25px rgba(255, 182, 193, 0.4);
            margin-top: 10px;
            border: 2px solid #ffb6c1;
        }

        h1 { font-family: 'Dancing Script', cursive; color: #d63384; font-size: 2.2rem; margin-bottom: 10px; }

        .media-img { width: 100%; border-radius: 15px; margin-bottom: 15px; display: block; box-shadow: 0 4px 10px rgba(0,0,0,0.1); }

        .btn {
            background: #ff69b4;
            color: white;
            border: none;
            padding: 16px;
            border-radius: 50px;
            font-size: 1.1rem;
            font-weight: bold;
            width: 100%;
            margin-top: 15px;
            box-shadow: 0 5px 15px rgba(255, 105, 180, 0.3);
            cursor: pointer;
        }

        .photo-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 12px;
            margin: 15px 0;
        }
        .photo-grid img { 
            width: 100%; height: 160px; object-fit: cover; 
            border-radius: 10px; border: 4px solid #fff;
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
        }

        .video-box { 
            margin-bottom: 25px; 
            background: #000; 
            border-radius: 15px; 
            overflow: hidden; 
            border: 2px solid #ffb6c1;
        }
        video { width: 100%; display: block; }

        .letter-content {
            text-align: left;
            font-size: 0.95rem;
            line-height: 1.7;
            padding: 15px;
            background: #fffafb;
            border-radius: 15px;
            max-height: 400px;
            overflow-y: auto;
            white-space: pre-line;
            border-left: 5px solid #ff69b4;
            color: #444;
        }

        .thanks-note {
            margin-top: 20px;
            padding: 15px;
            background: #ffe4e1;
            border-radius: 15px;
            font-style: italic;
            color: #d63384;
            font-weight: 600;
        }

        .rose-picker { font-size: 50px; display: flex; justify-content: space-around; padding: 20px 0; }
    </style>
</head>
<body>

<div class="mobile-container">
    
    <div id="p1" class="screen active">
        <div class="card">
            <h1>Happy Rose Day Baby 🌹</h1>
            <img src="https://lh3.googleusercontent.com/d/1oA0_BlRwJSCSlu5ddegF1Pc8XFp5EI-6" class="media-img">
            <p>A rose for the person who makes my world more beautiful just by being in it ✨</p>
            <button class="btn" onclick="show('p2')">Agge Dekho 🎀</button>
        </div>
    </div>

    <div id="p2" class="screen">
        <div class="card">
            <h1>Pick a Rose</h1>
            <img src="https://lh3.googleusercontent.com/d/18jB_pnODqn1pbOB1XJCcVnP_QBYr6ouF" class="media-img">
            <div class="rose-picker">
                <span onclick="alert('Try another one! ❤️')">🌹</span>
                <span onclick="show('p3')">🌹</span>
                <span onclick="alert('Middle wala try karo! ✨')">🌹</span>
            </div>
            <p>Sahi wala rose chuno mere message ke liye...</p>
        </div>
    </div>

    <div id="p3" class="screen">
        <h1>Our Memories 🎀 🧿</h1>
        <img src="https://lh3.googleusercontent.com/d/1zm_5MtzSdPwIItyl39vvteBJcjAU1oUV" class="media-img" style="max-height: 120px; object-fit: contain;">
        <div class="photo-grid">
            <img src="https://lh3.googleusercontent.com/d/1B4Bj9d15ClW3IoIHJDNuTVes3I8arDg-">
            <img src="https://lh3.googleusercontent.com/d/1MZBfHzLtyw7UORTQTxVQM2ZGCHzJ_Imt">
            <img src="https://lh3.googleusercontent.com/d/18enhwLyCvEYDL2Xo__YfZRFAUbjUKmET">
            <img src="https://lh3.googleusercontent.com/d/1d9aMJEtvlADsNWh0mBp2LiF7iR9fnV22">
            <img src="https://lh3.googleusercontent.com/d/1aFSL8ukbhy2tohjoAf03eotzja4J4Kik">
            <img src="https://lh3.googleusercontent.com/d/1YPtSs7ckY65qpKCOctQEKqTKmzFepByc">
            <img src="https://lh3.googleusercontent.com/d/17G2nGQuqMN9L78QCH39GcsfXHP-XY8SW">
            <img src="https://lh3.googleusercontent.com/d/1IfJckumLmzfKTpTVfDHV_SO10L6tFMyL">
        </div>
        <button class="btn" onclick="show('p4')">For You 🫶🏻💗</button>
    </div>

    <div id="p4" class="screen">
        <h1>For You 🫶🏻💗</h1>
        <div class="video-box"><video controls playsinline><source src="https://lh3.googleusercontent.com/d/1KJUT3jNxH10EEdlHUZO-rQ_juQbfV-Ov" type="video/mp4"></video></div>
        <div class="video-box"><video controls playsinline><source src="https://lh3.googleusercontent.com/d/1rHikV2ia4Dh8sddrcn8u54Z18HsGDfAo" type="video/mp4"></video></div>
        <div class="video-box"><video controls playsinline><source src="https://lh3.googleusercontent.com/d/1a-7kXpd6EMq7zGIIgX7GlC6gMIQNcztM" type="video/mp4"></video></div>
        <div class="video-box"><video controls playsinline><source src="https://lh3.googleusercontent.com/d/1q_xc4axTytBExwOpwlYU4gpra6WHTMt6" type="video/mp4"></video></div>
        <div class="video-box"><video controls playsinline><source src="https://lh3.googleusercontent.com/d/133glT6xC8dVyjcCNrLBTvCr5rSy8aAtv" type="video/mp4"></video></div>
        <div class="video-box"><video controls playsinline><source src="https://lh3.googleusercontent.com/d/1ompKdCqZo51LkXg_e-Y4ytFndp83v6sy" type="video/mp4"></video></div>
        <button class="btn" onclick="show('p5')">Read Final Note 💌</button>
    </div>

    <div id="p5" class="screen">
        <div class="card">
            <h1>From My Heart 💖</h1>
            <img src="https://lh3.googleusercontent.com/d/1dXkHhPJa_HTStp0XiXsYivngmY_ufFry" class="media-img" style="max-height: 100px; object-fit: contain;">
            <div class="letter-content">
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

            <div class="thanks-note">
                "And finally, a big Thank You for everything... 💖
                
                Thank you meri har chhoti baat samajhne ke liye, mere pagalpan ko jhelne ke liye aur mujhe itna special feel karane ke liye. Aap meri life ki woh smile ho jo main kabhi khona nahi chahta. 
                
                I am so lucky to have you! 🧿🫶🏻"
            </div>

            <button class="btn" onclick="location.reload()">Replay ❤️</button>
        </div>
    </div>

</div>

<script>
    function show(id) {
        document.querySelectorAll('video').forEach(v => v.pause());
        document.querySelectorAll('.screen').forEach(s => s.classList.remove('active'));
        document.getElementById(id).classList.add('active');
        window.scrollTo({top: 0, behavior: 'smooth'});
    }
</script>

</body>
</html>
