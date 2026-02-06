<!DOCTYPE html>
<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Rose Day Special 🌹</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&family=Poppins:wght@300;400;600&display=swap');

        * { box-sizing: border-box; margin: 0; padding: 0; touch-action: manipulation; }
        
        body {
            background-color: #fff0f5;
            font-family: 'Poppins', sans-serif;
            color: #333;
            display: flex;
            justify-content: center;
        }

        .container {
            width: 100%;
            max-width: 400px;
            min-height: 100vh;
            padding: 15px;
            position: relative;
        }

        .page { display: none; text-align: center; animation: fadeIn 0.4s ease-in; }
        .active { display: block; }

        @keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }

        .card {
            background: #ffffff;
            border-radius: 20px;
            padding: 20px;
            box-shadow: 0 10px 20px rgba(255,105,180,0.15);
            margin-bottom: 20px;
            border: 1px solid #ffdae9;
        }

        h1 { font-family: 'Dancing Script', cursive; color: #d63384; font-size: 2rem; margin-bottom: 15px; }

        img, video {
            width: 100%;
            border-radius: 12px;
            background: #f0f0f0;
            display: block;
            margin-bottom: 15px;
        }

        .btn {
            background: #ff69b4;
            color: white;
            border: none;
            padding: 15px;
            border-radius: 30px;
            font-size: 1rem;
            font-weight: bold;
            width: 100%;
            cursor: pointer;
            box-shadow: 0 4px 10px rgba(255, 105, 180, 0.3);
        }

        .photo-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 10px;
        }

        .photo-grid img { height: 120px; object-fit: cover; margin: 0; }

        .letter-box {
            text-align: left;
            font-size: 0.9rem;
            line-height: 1.6;
            background: #fffafa;
            padding: 15px;
            border-radius: 12px;
            max-height: 350px;
            overflow-y: auto;
            white-space: pre-line;
            border-left: 4px solid #ff69b4;
        }

        /* Video Container Fix */
        .video-wrapper {
            position: relative;
            background: #000;
            border-radius: 12px;
            margin-bottom: 20px;
            min-height: 200px;
        }
    </style>
</head>
<body>

<div class="container">
    
    <div id="p1" class="page active">
        <div class="card">
            <h1>Happy Rose Day 🌹</h1>
            <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExZ3R6bm5pM3R4bmV4bmV4bmV4bmV4bmV4bmV4bmV4bmV4bmV4JmVwPXYxX2ludGVybmFsX2dpZl9ieV9pZCZjdD1n/iS7XvYF6X0EWCXvL0o/giphy.gif" alt="Cute Rose">
            <p>A rose for the person who makes my world more beautiful ✨</p>
            <button class="btn" onclick="nav('p2')">Memories Dekho 🎀</button>
        </div>
    </div>

    <div id="p2" class="page">
        <h1>Our Memories 🎀 🧿</h1>
        <div class="photo-grid">
            <img src="https://i.postimg.cc/yNqkyd81/IMG_20260206_190532.png" loading="lazy">
            <img src="https://i.postimg.cc/s2Fv4Xg3/IMG_20260206_190558.png" loading="lazy">
            <img src="https://i.postimg.cc/K831TLx4/IMG_20260206_190630.png" loading="lazy">
            <img src="https://i.postimg.cc/rp6KNmw8/IMG_20260206_190726.png" loading="lazy">
            <img src="https://i.postimg.cc/XNxB64s3/IMG_20260206_190744.png" loading="lazy">
            <img src="https://i.postimg.cc/MGkvmTpR/IMG_20260206_190444.png" loading="lazy">
            <img src="https://i.postimg.cc/k5rBv4gN/IMG_20260206_190512.png" loading="lazy">
            <img src="https://i.postimg.cc/xdrc3C16/IMG_20260206_190418.png" loading="lazy">
        </div>
        <button class="btn" onclick="nav('p3')" style="margin-top:20px;">For You 🫶🏻💗</button>
    </div>

    <div id="p3" class="page">
        <h1>For You 🫶🏻💗</h1>
        <p style="font-size: 0.8rem; margin-bottom: 15px;">Video par tap karo agar load na ho ✨</p>
        
        <div class="video-wrapper">
            <video controls playsinline poster="https://i.postimg.cc/yNqkyd81/IMG_20260206_190532.png">
                <source src="https://files.catbox.moe/mw3f2q.mp4" type="video/mp4">
            </video>
        </div>
        
        <div class="video-wrapper">
            <video controls playsinline>
                <source src="https://files.catbox.moe/ggbrik.mp4" type="video/mp4">
            </video>
        </div>

        <div class="video-wrapper">
            <video controls playsinline>
                <source src="https://files.catbox.moe/sfk5b8.mp4" type="video/mp4">
            </video>
        </div>

        <button class="btn" onclick="nav('p4')">Final Message 💌</button>
    </div>

    <div id="p4" class="page">
        <div class="card">
            <h1>From My Heart 💖</h1>
            <div class="letter-box">
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
            <button class="btn" onclick="location.reload()" style="margin-top:15px;">Pura Phir Se Dekho ❤️</button>
        </div>
    </div>

</div>

<script>
    function nav(id) {
        // Pause all videos
        const vids = document.querySelectorAll('video');
        vids.forEach(v => v.pause());

        // Change page
        document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
        const next = document.getElementById(id);
        next.classList.add('active');

        // Scroll top
        window.scrollTo(0,0);

        // Force Video Load when entering Video page
        if(id === 'p3') {
            vids.forEach(v => {
                v.load();
                v.play().catch(() => {
                    console.log("Auto-play blocked, waiting for user tap.");
                });
            });
        }
    }
</script>

</body>
</html>
