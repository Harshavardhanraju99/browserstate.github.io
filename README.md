<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Hidden Hackers | Security Awareness</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@600;800&family=DM+Sans:wght@400;700&display=swap" rel="stylesheet">
<style>
    .harsha{
        display: flex;
    }
    
  :root{
    --bg:#070707;
    --fg:#f6f6f6;
    --red:#ff2b2b;
    --green:#16ff7a;
    --amber:#ffc300;
    --muted:#bbbbbb;
    --glow: 0 0 8px currentColor, 0 0 16px currentColor, 0 0 28px currentColor;
  }
  html,body{height:100%}
  body{
    margin:0;
    background:#000 radial-gradient(1500px 800px at 50% -10%, #111 0%, #000 60%);
    color:var(--fg);
    font-family:"DM Sans", system-ui, -apple-system, Segoe UI, Roboto, Arial, sans-serif;
    letter-spacing:.2px;
  }
  .wrap{
    max-width:1050px;
    margin:0 auto;
    padding:42px 18px 60px;
    text-align:center;
  }
  /* tricolor heading */
  .jai{
    font-family:"Orbitron", monospace;
    font-size: clamp(36px, 6vw, 84px);
    font-weight: 800;
    line-height:1.05;
    letter-spacing:1px;
    margin:6px 0 18px;
    text-shadow: 0 4px 30px rgba(0,0,0,.6);
  }
  .jai .saffron{ color:#ff7a00; text-shadow: var(--glow); }
  .jai .white{ color:#ffffff; text-shadow: var(--glow); }
  .jai .green{ color:#00c853; text-shadow: var(--glow); }

  .sep{
    margin:22px auto;
    width:min(900px, 92%);
    height:2px;
    background: repeating-linear-gradient(90deg, #d61d1d 0 18px, transparent 18px 30px);
    box-shadow: 0 0 12px #d61d1d;
  }

  .blink{ animation: blink 1.2s steps(1,end) infinite; }
  @keyframes blink{ 50%{ opacity:.35 } }

  .msg{
    font-size: clamp(16px, 2.4vw, 22px);
    margin:10px auto;
  }
  .msg .red{ color:var(--red); text-shadow: var(--glow); }
  .msg .amber{ color:var(--amber); text-shadow: var(--glow); }
  .msg .green{ color:var(--green); text-shadow: var(--glow); }

  .glow{
    text-shadow: var(--glow);
  }

  .scroll{
    margin: 6px 0 18px;
    font-weight:700;
  }

  .badge{
    display:inline-flex; gap:10px; align-items:center; justify-content:center;
    padding:12px 18px;
    border:1px solid #222; border-radius:999px;
    background:linear-gradient(180deg, #0b0b0b, #050505);
    box-shadow: inset 0 0 24px rgba(255,255,255,.04), 0 0 24px rgba(255,255,255,.05);
    font-size:14px; color:#ddd;
  }

  .crew{
    font-family:"Orbitron", monospace;
    margin-top:34px;
    font-size: clamp(16px, 2.2vw, 22px);
    color:#fff;
    text-shadow: 0 0 8px #f00, 0 0 16px #f00;
    letter-spacing:1px;
  }

  /* Company block */
  .brand{
    margin: 26px auto 6px;
    font-family:"Orbitron", monospace;
    font-size: clamp(26px, 4.5vw, 54px);
    font-weight:800;
    background: radial-gradient(120% 120% at 50% 0%, #ff4d4d, #d400ff 45%, #00e676 90%);
    -webkit-background-clip: text;
    background-clip: text;
    color: transparent;
    filter: drop-shadow(0 0 14px rgba(255,0,150,.45));
  }
  .tagline{
    color:#d9fdd3;
    font-size: clamp(12px, 1.8vw, 16px);
    letter-spacing: .5px;
    text-transform: uppercase;
    opacity:.9;
  }

  /* 3D Globe-style rotating logo */
.logo-container {
  margin: 20px auto;
  width: 220px;
  height: 220px;
  border-radius: 50%;
  border: 4px solid #ff0000;
  overflow: hidden;
  display: flex;
  align-items: center;
  justify-content: center;
  perspective: 1000px; /* adds depth */
  box-shadow: 0 0 25px #ff0000, 0 0 50px #ff0000;
}

.logo-container img {
  width: 95%;
  height: auto;
  border-radius: 50%;
  transform-style: preserve-3d;
  animation: globeSpin 8s linear infinite;
}

/* 3D globe spin animation */
@keyframes globeSpin {
  0%   { transform: rotateY(0deg) rotateX(10deg); }
  50%  { transform: rotateY(180deg) rotateX(-10deg); }
  100% { transform: rotateY(360deg) rotateX(10deg); }
}

  /* floating badge bottom-right */
  .floating{
    position:fixed; right:16px; bottom:16px;
    padding:10px 14px; border-radius:14px;
    background:#0c0c0c; border:1px solid #1d1d1d;
    box-shadow: 0 10px 30px rgba(0,0,0,.5);
    font-size:13px; color:#cfcfcf;
  }

  a{ color:#7cdfff; text-decoration:none }
  a:hover{ text-decoration:underline }
</style>
</head>
<body>
  <div class="wrap">
    <div class="jai">
      <span class="saffron">Say </span>
      <span class="white">Jai </span>
      <span class="green">Hind</span>
    </div>

    <div class="sep"></div>

    <div class="badge">
      🇮🇳 <strong>Hidden Hackers</strong> • Ethical Security Awareness Page
    </div>

    <!-- Rotating Logo -->
     <div class="harsha">
     <!-- <div class="flag-container"> -->
    <img class="pradeep" src="https://media3.giphy.com/media/v1.Y2lkPTc5MGI3NjExa3hlaTQzbmZvajF6c2lvdmhseDJyM3Fscnphd3U2a3cwaHo0c2d4YyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/9Gnbm29r7ftUA/giphy.gif" class="flag" alt="Indian Flag">

    <div class="logo-container">
      <img src="https://i.postimg.cc/76pkPFMp/hidden-hackers.jpg" alt="Hidden Hackers Logo">
    </div>

    <!-- <div class="flag-container"> -->
    <img  class="pradeep" src="https://media3.giphy.com/media/v1.Y2lkPTc5MGI3NjExa3hlaTQzbmZvajF6c2lvdmhseDJyM3Fscnphd3U2a3cwaHo0c2d4YyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/9Gnbm29r7ftUA/giphy.gif" class="flag" alt="Indian Flag">
   </div>

    <p class="msg">
      🖕 <span class="red glow">Don't blame me</span> 🖕 — <span class="amber">Blame your security!</span> 😄
    </p>
    <p class="msg">
      😎 You call it <span class="red glow">Hacking</span> — we call it <span class="green glow">Security Awareness</span> ⚠️✨
    </p>
    <p class="msg red">
      We did not damage any data. We are here only to convey our message.
    </p>
    <p class="msg green">
      ♡ ♻ Improve Your Security ♻ ♡
    </p>

    <div class="sep"></div>

    <!-- marquee effect (classic vibe) -->
    <p class="scroll">
      <marquee behavior="alternate" scrollamount="6" direction="right">🇮🇳  TELENGANA — CYBER — HEROS  🇮🇳</marquee>
    </p>

    <!-- Company branding -->
    <div class="brand">HIDDEN HACKERS</div>
    <div class="tagline">We Are Cyber Heroes • Security. Awareness. Resilience.</div>

    <!-- crew / aliases -->
    <div class="crew" style="margin-top:26px">
         <p class="scroll"></p>
      <marquee behavior="alternate" direction="right" scrollamount="6">
         NJ18-H4X04 | SPYDER | DIB0237 | ORVILL | All Indian Hackers
      </marquee>

    </p>
    </div>

    <div class="sep"></div>

    <!-- Optional footer / disclosure -->
    <p class="msg" style="color:var(--muted)">
      This is a <span class="glow">responsible security awareness</span> demo page.
      If you’re the website owner and received this on your domain, contact
      <a href="mailto:contact@hiddenhackers.example">contact@hiddenhackers.example</a> to coordinate remediation.
    </p>
  </div>

  <div class="floating">
    © <span class="blink">2025</span> Hidden Hackers — Stay Safe, Stay Aware
  </div>
</body>
</html>
