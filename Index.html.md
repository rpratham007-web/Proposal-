<!DOCTYPE html>  
<html lang="en">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>Will You Marry Me?</title>  
    <style>  
        @import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400;700&family=Poppins:wght@300;400;600&display=swap');  
          
        * {  
            margin: 0;  
            padding: 0;  
            box-sizing: border-box;  
        }  
          
        body {  
            font-family: 'Poppins', sans-serif;  
            overflow: hidden;  
            background: linear-gradient(135deg, #ff9a9e 0%, #fecfef 50%, #fecfef 100%);  
            height: 100vh;  
            display: flex;  
            justify-content: center;  
            align-items: center;  
            position: relative;  
        }  
          
        .stars {  
            position: absolute;  
            top: 0;  
            left: 0;  
            width: 100%;  
            height: 100%;  
            pointer-events: none;  
        }  
          
        .star {  
            position: absolute;  
            background: white;  
            border-radius: 50%;  
            animation: twinkle 2s infinite alternate;  
        }  
          
        @keyframes twinkle {  
            0% { opacity: 0.3; transform: scale(1); }  
            100% { opacity: 1; transform: scale(1.2); }  
        }  
          
        .container {  
            text-align: center;  
            max-width: 800px;  
            padding: 20px;  
            animation: fadeInUp 1.5s ease-out;  
        }  
          
        @keyframes fadeInUp {  
            from { opacity: 0; transform: translateY(50px); }  
            to { opacity: 1; transform: translateY(0); }  
        }  
          
        h1 {  
            font-family: 'Dancing Script', cursive;  
            font-size: clamp(3rem, 8vw, 6rem);  
            color: #fff;  
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);  
            margin-bottom: 20px;  
            animation: heartbeat 1.5s infinite;  
        }  
          
        @keyframes heartbeat {  
            0%, 100% { transform: scale(1); }  
            50% { transform: scale(1.05); }  
        }  
          
        .message {  
            font-size: clamp(1.2rem, 4vw, 1.8rem);  
            color: #fff;  
            line-height: 1.6;  
            margin-bottom: 40px;  
            opacity: 0;  
            animation: fadeIn 2s ease-out 0.5s forwards;  
        }  
          
        @keyframes fadeIn {  
            to { opacity: 1; }  
        }  
          
        .photo {  
            width: 200px;  
            height: 200px;  
            border-radius: 50%;  
            object-fit: cover;  
            border: 8px solid rgba(255,255,255,0.8);  
            box-shadow: 0 10px 30px rgba(0,0,0,0.3);  
            margin: 20px auto;  
            animation: float 3s ease-in-out infinite;  
        }  
          
        @keyframes float {  
            0%, 100% { transform: translateY(0px); }  
            50% { transform: translateY(-10px); }  
        }  
          
        .proposal-btn {  
            font-family: 'Dancing Script', cursive;  
            font-size: clamp(1.5rem, 5vw, 2.5rem);  
            background: linear-gradient(45deg, #ff6b6b, #feca57);  
            color: white;  
            border: none;  
            padding: 20px 50px;  
            border-radius: 50px;  
            cursor: pointer;  
            box-shadow: 0 15px 35px rgba(0,0,0,0.2);  
            transition: all 0.3s ease;  
            text-transform: uppercase;  
            letter-spacing: 2px;  
        }  
          
        .proposal-btn:hover {  
            transform: translateY(-5px) scale(1.05);  
            box-shadow: 0 20px 45px rgba(0,0,0,0.3);  
        }  
          
        .celebration {  
            display: none;  
            position: fixed;  
            top: 0;  
            left: 0;  
            width: 100%;  
            height: 100%;  
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);  
            z-index: 1000;  
            flex-direction: column;  
            justify-content: center;  
            align-items: center;  
        }  
          
        .celebration h2 {  
            font-family: 'Dancing Script', cursive;  
            font-size: clamp(4rem, 10vw, 8rem);  
            color: #fff;  
            text-shadow: 3px 3px 6px rgba(0,0,0,0.5);  
            animation: bounce 1s infinite;  
        }  
          
        @keyframes bounce {  
            0%, 20%, 50%, 80%, 100% { transform: translateY(0); }  
            40% { transform: translateY(-20px); }  
            60% { transform: translateY(-10px); }  
        }  
          
        .confetti {  
            position: fixed;  
            width: 10px;  
            height: 10px;  
            background: #feca57;  
            animation: confetti-fall 3s linear infinite;  
        }  
          
        @keyframes confetti-fall {  
            0% {  
                transform: translateY(-100vh) rotate(0deg);  
                opacity: 1;  
            }  
            100% {  
                transform: translateY(100vh) rotate(720deg);  
                opacity: 0;  
            }  
        }  
          
        @media (max-width: 768px) {  
            .container { padding: 10px; }  
            .message { font-size: 1.1rem; }  
        }  
    </style>  
</head>  
<body>  
    <div class="stars" id="stars"></div>  
      
    <div class="container">  
        <img src="[https://drive.google.com/file/d/1hL0Q6Zq80MREbYMeKlQadQjr-EIptmYE/view?usp=drivesdk ](https://drive.google.com/file/d/1hL0Q6Zq80MREbYMeKlQadQjr-EIptmYE/view?usp=drivesdk)/200x200/ff6b6b/fff?text=💕+YOU" alt="Our Photo" class="photo">  
      
          
        <h1>[Priya]!</h1>  
         
          
        <p class="message">  
            From the moment we met, you've made every day brighter.   
            You've been my best friend, my adventure partner, and my everything.  
            <br><br>  
            I can't imagine my life without you.   
            Will you make me the happiest person alive?  
        </p>  
         
          
        <button class="proposal-btn" onclick="propose()">  
            💍 Will You Marry Me? 💍  
        </button>  
    </div>  
      
    <div class="celebration" id="celebration">  
        <h2>She Said YES! 🎉</h2>  
        <p style="color: white; font-size: 2rem; margin-top: 20px;">Our forever starts now! ❤️</p>  
    </div>  
  
    <script>  
        // Create twinkling stars  
        function createStars() {  
            const starsContainer = document.getElementById('stars');  
            for (let i = 0; i < 100; i++) {  
                const star = document.createElement('div');  
                star.className = 'star';  
                star.style.left = Math.random() * 100 + '%';  
                star.style.top = Math.random() * 100 + '%';  
                star.style.width = star.style.height = (Math.random() * 3 + 1) + 'px';  
                star.style.animationDelay = Math.random() * 2 + 's';  
                starsContainer.appendChild(star);  
            }  
        }  
        createStars();  
  
        // Proposal function  
        function propose() {  
            document.querySelector('.container').style.display = 'none';  
            const celebration = document.getElementById('celebration');  
            celebration.style.display = 'flex';  
              
            // Confetti explosion  
            for (let i = 0; i < 100; i++) {  
                const confetti = document.createElement('div');  
                confetti.className = 'confetti';  
                confetti.style.left = Math.random() * 100 + '%';  
                confetti.style.background = ['#feca57', '#ff6b6b', '#48dbfb', '#fff', '#ff9ff3'][Math.floor(Math.random() * 5)];  
                confetti.style.animationDelay = Math.random() * 0.5 + 's';  
                confetti.style.animationDuration = (Math.random() * 1 + 2) + 's';  
                document.body.appendChild(confetti);  
                  
                setTimeout(() => confetti.remove(), 4000);  
            }  
              
            // Optional: Play celebration sound (uncomment and add audio file)  
            // const audio = new Audio('celebration.mp3');  
            // audio.play();  
        }  
  
        // Optional: Auto-play soft background music (add your MP3 URL)  
        // window.onload = () => {  
        //     const audio = new Audio('romantic-music.mp3');  
        //     audio.loop = true;  
        //     audio.volume = 0.3;  
        //     audio.play().catch(() => {}); // Ignore autoplay errors  
        // };  
    </script>  
</body>  
</html>  
