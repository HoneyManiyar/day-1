<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Day 1 - Visual Reaction Converter</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Poppins', sans-serif; }

        /* --- THE DYNAMIC BACKGROUND LAYER --- */
        body {
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            overflow: hidden;
            position: relative;
            /* Smooth background color transitions */
            transition: background 0.8s ease-in-out;
        }

        /* 1. Default State: Moving Blue/Navy Gradient */
        .bg-overlay {
            position: absolute;
            top: 0; left: 0; width: 100%; height: 100%;
            z-index: 1;
            background: linear-gradient(-45deg, #0f172a, #1e40af, #7e22ce, #1e1b4b);
            background-size: 400% 400%;
            animation: gradientBG 15s ease infinite;
            transition: opacity 0.8s ease-in-out, background 0.8s ease-in-out;
            opacity: 1;
        }

        /* 2. Focused Input State (Pink beautiful) */
        body.input-focus-active .bg-overlay {
            background: linear-gradient(-45deg, #ff9a9e, #fad0c4, #fad0c4, #ff9a9e);
            animation: gradientBG 10s ease infinite; /* Faster pink motion */
        }

        /* 3. Hovering the Card State (Unique Blue/Cyan) */
        body.card-hover-active .bg-overlay {
            background: linear-gradient(-45deg, #00c6ff, #0072ff, #38bdf8, #0ea5e9);
            animation: gradientBG 5s ease infinite; /* Fast radiant blue */
        }

        @keyframes gradientBG {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        /* --- THE APP CARD (UI) --- */
        .converter-card {
            background: rgba(255, 255, 255, 0.05); /* Very glassy */
            backdrop-filter: blur(20px);
            padding: 35px;
            border-radius: 30px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            width: 100%;
            max-width: 400px;
            color: white;
            box-shadow: 0 20px 50px rgba(0,0,0,0.5);
            transition: all 0.4s ease;
            position: relative;
            z-index: 10;
        }

        /* Card lifts slightly on hover */
        .converter-card:hover {
            transform: translateY(-5px);
            border-color: rgba(255, 255, 255, 0.3);
            box-shadow: 0 30px 60px rgba(0,0,0,0.6);
        }

        h2 { text-align: center; margin-bottom: 25px; color: white; letter-spacing: 1px; font-weight: 300;}

        .group { margin-bottom: 1.5rem; text-align: left; }
        label { display: block; margin-bottom: 8px; font-size: 0.8rem; color: rgba(255, 255, 255, 0.7); }

        input, select {
            width: 100%;
            padding: 14px;
            border-radius: 12px;
            border: 1px solid rgba(255,255,255,0.1);
            background: rgba(0,0,0,0.3);
            color: white;
            font-size: 1.1rem;
            outline: none;
            transition: 0.3s;
        }

        input:focus { 
            border-color: #ff9a9e; /* Pink accent on focus */
            background: rgba(255, 255, 255, 0.1);
        }

        .result-box {
            background: rgba(255, 255, 255, 0.03);
            padding: 20px;
            border-radius: 16px;
            text-align: center;
            border: 1px dashed rgba(255, 255, 255, 0.2);
            margin-top: 10px;
            transition: all 0.3s ease;
        }

        /* Result box lights up on focus */
        body.input-focus-active .result-box {
            border-color: #ff9a9e;
            background: rgba(255, 154, 158, 0.05);
        }

        /* Result box lights up on card hover */
        body.card-hover-active .result-box {
            border-color: #00c6ff;
            background: rgba(0, 198, 255, 0.05);
        }

        #resultValue { font-size: 3rem; font-weight: bold; display: block; color: white; }
        #resultUnit { color: rgba(255, 255, 255, 0.8); font-size: 1rem; }

        /* --- EMOJI BURST ANIMATION --- */
        .emoji {
            position: absolute;
            font-size: 2rem;
            pointer-events: none;
            animation: explode 0.8s forwards ease-out;
            opacity: 0;
            z-index: 100;
        }

        @keyframes explode {
            0% { transform: translate(0, 0) scale(1); opacity: 1; }
            100% { transform: translate(var(--x), var(--y)) scale(0.5); opacity: 0; }
        }
    </style>
</head>
<body>

    <div class="bg-overlay"></div>

    <div class="converter-card" id="mainCard">
        <h2>Smart Converter ✨</h2>
        
        <div class="group">
            <label>You Enter</label>
            <input type="number" id="inputValue" value="1">
        </div>

        <div class="group">
            <label>Convert From</label>
            <select id="fromUnit">
                <option value="km">Kilometers (km)</option>
                <option value="mi">Miles (mi)</option>
                <option value="kg">Kilograms (kg)</option>
                <option value="lb">Pounds (lb)</option>
            </select>
        </div>

        <div class="result-box">
            <span id="resultValue">0.62</span>
            <span id="resultUnit">Miles</span>
        </div>
    </div>

    <script>
        const input = document.getElementById('inputValue');
        const fromUnit = document.getElementById('fromUnit');
        const resValue = document.getElementById('resultValue');
        const resUnit = document.getElementById('resultUnit');
        const card = document.getElementById('mainCard');
        const body = document.body;

        // --- CONVERSION LOGIC ---
        function convert() {
            const val = parseFloat(input.value);
            const type = fromUnit.value;

            if (isNaN(val)) {
                resValue.innerText = "0";
                return;
            }

            switch(type) {
                case 'km':
                    resValue.innerText = (val * 0.621371).toFixed(2);
                    resUnit.innerText = "Miles";
                    break;
                case 'mi':
                    resValue.innerText = (val / 0.621371).toFixed(2);
                    resUnit.innerText = "Kilometers";
                    break;
                case 'kg':
                    resValue.innerText = (val * 2.20462).toFixed(2);
                    resUnit.innerText = "Pounds";
                    break;
                case 'lb':
                    resValue.innerText = (val / 2.20462).toFixed(2);
                    resUnit.innerText = "Kilograms";
                    break;
            }
        }

        // --- DYNAMIC BACKGROUND STATES (CSS CLASS TOGGLING) ---

        // 1. When Input is focused (Enter Number) -> Transition to beautiful pink
        input.addEventListener('focus', () => {
            body.classList.add('input-focus-active');
        });

        // 2. When focus leaves input -> Back to default
        input.addEventListener('blur', () => {
            body.classList.remove('input-focus-active');
        });

        // 3. When Card is Hovered -> Transition to radiant blue
        card.addEventListener('mouseenter', () => {
            body.classList.add('card-hover-active');
        });

        // 4. When Mouse leaves card -> Back to default
        card.addEventListener('mouseleave', () => {
            body.classList.remove('card-hover-active');
        });


        // --- EMOJI BURST LOGIC ---
        function createBurst(event) {
            const emojis = ['⚡', '✨', '📏', '⚖️', '🌈'];
            let centerX, centerY;

            // If triggered by click, explode from click point. Otherwise, explode from center.
            if (event && event.clientX) {
                centerX = event.clientX;
                centerY = event.clientY;
            } else {
                const rect = card.getBoundingClientRect();
                centerX = rect.left + rect.width / 2;
                centerY = rect.top + rect.height / 2;
            }

            for (let i = 0; i < 8; i++) {
                const span = document.createElement('span');
                span.classList.add('emoji');
                span.innerText = emojis[Math.floor(Math.random() * emojis.length)];
                
                const x = (Math.random() - 0.5) * 300; 
                const y = (Math.random() - 0.5) * 300; 
                
                span.style.setProperty('--x', `${x}px`);
                span.style.setProperty('--y', `${y}px`);
                span.style.left = `${centerX}px`;
                span.style.top = `${centerY}px`;

                document.body.appendChild(span);
                setTimeout(() => span.remove(), 800);
            }
        }

        // LISTENERS
        input.addEventListener('input', convert);
        fromUnit.addEventListener('change', convert);
        card.addEventListener('click', createBurst); // Click burst for fun interaction
        
        // Initial setup on load
        window.onload = () => {
            convert();
            createBurst(); // Explode once when it opens
        };
    </script>
</body>
</html>
