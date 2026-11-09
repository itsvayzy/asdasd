<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Hollow Woods — Survival Horror</title>
<link rel="icon" href="data:image/svg+xml,<svg xmlns=%22http://www.w3.org/2000/svg%22 viewBox=%220 0 100 100%22><text y=%22.9em%22 font-size=%2290%22>💀</text></svg>">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@500;700;900&family=Inter:wght@400;500;600&display=swap" rel="stylesheet">
<style>
  :root{
    --void:#060504; --dark:#110d0c; --card:#171212;
    --ash:#8a8178; --bone:#ece5d9;
    --blood:#6b0a0a; --blood-bright:#e2231f;
    --glow:0 0 24px rgba(226,35,31,.65), 0 0 70px rgba(107,10,10,.45);
    color-scheme: dark;
    box-sizing:border-box;
    padding-top: env(safe-area-inset-top,0px);
    padding-bottom: env(safe-area-inset-bottom,0px);
  }
  *,*::before,*::after{box-sizing:inherit; margin:0; padding:0;}
  html{scroll-behavior:smooth; scroll-padding-top:env(safe-area-inset-top,0px);}
  body{
    background:var(--void); color:var(--bone);
    font-family:'Inter',system-ui,-apple-system,sans-serif;
    line-height:1.65; overflow-x:hidden;
  }
  h1,h2,h3,.logo{font-family:'Cinzel',Georgia,serif;}
  a{color:inherit; text-decoration:none;}
  img{max-width:100%; display:block;}
  .wrap{max-width:1120px; margin:0 auto; padding:0 24px;}
  ::selection{background:var(--blood); color:var(--bone);}
  :focus-visible{outline:2px solid var(--blood-bright); outline-offset:3px;}
  .grain{position:fixed; inset:0; z-index:9; pointer-events:none; opacity:.05; mix-blend-mode:overlay;
    background-image:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='120' height='120'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='2' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)'/%3E%3C/svg%3E");
    animation:grainShift .4s steps(2) infinite;}
  @keyframes grainShift{0%{transform:translate(0,0);}100%{transform:translate(-2%,2%);}}
  .ambient{position:fixed; inset:0; z-index:8; pointer-events:none;
    background:radial-gradient(ellipse at 50% 0%, rgba(107,10,10,.10), transparent 55%);
    animation:ambientPulse 9s ease-in-out infinite;}
  @keyframes ambientPulse{0%,100%{opacity:.6;}50%{opacity:1;}}

  /* ---------- NAV ---------- */
  body::before{content:"";position:fixed;inset:0 0 auto;height:env(safe-area-inset-top,0px);z-index:11;background:var(--void);}
  header{
    position:fixed; top:env(safe-area-inset-top,0px); left:0; right:0; z-index:10;
    display:flex; align-items:center; justify-content:space-between;
    padding:20px 32px; transition:background .4s, padding .4s, border-color .4s;
    border-bottom:1px solid transparent;
  }
  header.scrolled{background:rgba(6,5,4,.94); backdrop-filter:blur(12px); padding:14px 32px; border-color:rgba(226,35,31,.4); box-shadow:0 1px 24px rgba(107,10,10,.35);}
  .logo{font-size:1.25rem; font-weight:700; letter-spacing:.08em; color:var(--bone);}
  .logo span{color:var(--blood-bright);}
  nav ul{display:flex; gap:36px; list-style:none;}
  nav a{font-size:.95rem; color:var(--ash); position:relative; padding:4px 0;}
  nav a:hover{color:var(--bone);}
  nav a::after{content:"";position:absolute; left:0; bottom:0; width:0; height:1px; background:var(--blood-bright); transition:width .3s;}
  nav a:hover::after{width:100%;}
  .nav-toggle{display:none; background:none; border:0; color:var(--bone); font-size:1.6rem; cursor:pointer; line-height:1;}

  /* ---------- HERO ---------- */
  .hero{
    position:relative; height:100vh; min-height:560px;
    display:flex; align-items:center; justify-content:center; text-align:center;
    overflow:hidden; background:
      radial-gradient(ellipse at 50% 15%, #2b0f0f 0%, #0d0707 55%, var(--void) 85%);
  }
  .drip{position:absolute; top:0; width:2px; background:linear-gradient(var(--blood-bright),transparent); opacity:.55; filter:blur(.3px); animation:dripfall 6s ease-in infinite;}
  .drip::after{content:"";position:absolute; left:50%; bottom:0; width:5px; height:5px; margin-left:-2.5px; background:var(--blood-bright); border-radius:50%; box-shadow:0 0 6px var(--blood-bright);}
  @keyframes dripfall{0%{height:0; top:0; opacity:.7;}70%{opacity:.5;}100%{height:38vh; top:0; opacity:0;}}
  .fog{position:absolute; bottom:-10%; width:160%; height:55%; left:-30%;
    background:radial-gradient(ellipse at center, rgba(170,165,160,.13) 0%, transparent 70%);
    filter:blur(10px); animation:drift 36s linear infinite;}
  .fog.f2{animation-duration:52s; animation-direction:reverse; bottom:-16%; opacity:.75;}
  .fog.f3{animation-duration:70s; bottom:0; opacity:.6; background:radial-gradient(ellipse at center, rgba(90,15,15,.16) 0%, transparent 70%);}
  @keyframes drift{0%{transform:translateX(0);}50%{transform:translateX(6%);}100%{transform:translateX(0);}}
  .treeline{position:absolute; bottom:0; left:0; width:100%; height:26vh; background:#050404;
    clip-path:polygon(0% 100%,0% 55%,3% 70%,6% 40%,9% 68%,13% 48%,16% 75%,20% 50%,24% 72%,28% 42%,32% 66%,36% 52%,40% 78%,45% 46%,49% 70%,53% 50%,57% 74%,61% 44%,65% 68%,69% 54%,73% 76%,77% 48%,81% 70%,85% 50%,89% 73%,93% 46%,97% 69%,100% 55%,100% 100%);}
  .vignette{position:absolute; inset:0; box-shadow:inset 0 0 16vw 5vw rgba(0,0,0,.92), inset 0 0 3vw 1vw rgba(0,0,0,.6); pointer-events:none;}
  .flicker{position:absolute; inset:0; background:radial-gradient(ellipse at 50% 35%, rgba(120,10,10,.16), transparent 60%); animation:flicker 5.5s ease-in-out infinite;}
  @keyframes flicker{0%,17%,19%,55%,100%{opacity:1;}18%{opacity:.25;}56%,59%{opacity:.6;}80%{opacity:.85;}}
  .hero-inner{position:relative; z-index:2; padding:0 20px; opacity:0; animation:rise 1.4s .3s ease forwards;}
  @keyframes rise{from{opacity:0; transform:translateY(22px);}to{opacity:1; transform:translateY(0);}}
  .hero h1{font-size:clamp(2.8rem,8vw,6rem); font-weight:900; letter-spacing:.03em;
    color:var(--bone); text-shadow:var(--glow); animation:titleglow 5.5s ease-in-out infinite;}
  @keyframes titleglow{0%,100%{text-shadow:var(--glow);}50%{text-shadow:0 0 34px rgba(226,35,31,.9), 0 0 90px rgba(107,10,10,.6);}}
  .hero .tagline{margin-top:18px; font-size:clamp(1rem,2vw,1.25rem); color:var(--ash); letter-spacing:.02em; max-width:36em; margin-left:auto; margin-right:auto;}
  .btn{display:inline-block; margin-top:40px; padding:17px 42px; font-family:'Cinzel',serif; font-weight:700; font-size:1.02rem; letter-spacing:.06em;
    background:linear-gradient(160deg,var(--blood-bright),var(--blood)); color:#fff; border-radius:3px;
    box-shadow:0 0 0 1px rgba(255,255,255,.08), 0 8px 30px rgba(140,10,10,.45); transition:transform .25s, box-shadow .25s;
    animation:btnpulse 3.4s ease-in-out infinite;}
  @keyframes btnpulse{0%,100%{box-shadow:0 0 0 1px rgba(255,255,255,.08), 0 8px 30px rgba(140,10,10,.45);}50%{box-shadow:0 0 0 1px rgba(255,255,255,.1), 0 10px 42px rgba(226,35,31,.7);}}
  .btn:hover{transform:translateY(-3px); box-shadow:0 0 0 1px rgba(255,255,255,.12), 0 14px 38px rgba(200,20,20,.6); animation-play-state:paused;}
  .scroll-cue{position:absolute; bottom:34px; left:50%; transform:translateX(-50%); z-index:2; color:var(--ash); font-size:1.6rem; animation:bob 2.2s ease-in-out infinite;}
  @keyframes bob{0%,100%{transform:translate(-50%,0);}50%{transform:translate(-50%,10px);}}

  /* ---------- SECTIONS ---------- */
  section{padding:120px 0;}
  .section-head{max-width:640px; margin-bottom:56px;}
  .section-head h2{font-size:clamp(1.9rem,3.6vw,2.6rem); font-weight:700;}
  .section-head p.lede{margin-top:14px; color:var(--ash); font-size:1.05rem;}
  .rule{width:64px; height:2px; background:var(--blood-bright); margin-bottom:22px;}

  .about{background:radial-gradient(ellipse at 15% 20%, rgba(107,10,10,.12), transparent 55%), var(--dark); position:relative; border-top:1px solid rgba(122,12,12,.25); border-bottom:1px solid rgba(122,12,12,.25);}
  .about .wrap{max-width:760px;}
  .about p{font-size:1.15rem; color:#cfc7bc; margin-top:18px; max-width:58ch;}
  .about p:first-of-type{margin-top:0;}
  .about .whisper{margin-top:30px; font-family:'Cinzel',serif; font-style:normal; color:var(--blood-bright); font-size:1.15rem; letter-spacing:.02em; text-shadow:0 0 18px rgba(226,35,31,.45);}

  .features{position:relative; background:radial-gradient(ellipse at 85% 10%, rgba(107,10,10,.09), transparent 55%);}
  .features .grid{display:grid; grid-template-columns:repeat(2,1fr); gap:28px;}
  .card{background:var(--card); border:1px solid rgba(122,12,12,.22); border-radius:6px; padding:34px 30px; transition:transform .3s, border-color .3s, background .3s, box-shadow .3s;}
  .card:hover{transform:translateY(-6px); border-color:var(--blood-bright); background:#201a19; box-shadow:0 18px 44px rgba(0,0,0,.6), 0 0 0 1px rgba(226,35,31,.25), inset 0 0 40px rgba(107,10,10,.18);}
  .card .icon{font-size:1.8rem; filter:drop-shadow(0 0 10px rgba(200,30,30,.6)); margin-bottom:16px;}
  .card h3{font-size:1.25rem; font-weight:700; margin-bottom:10px;}
  .card p{color:var(--ash); font-size:.98rem;}

  .download{position:relative; text-align:center; background:radial-gradient(ellipse at 50% 30%, rgba(107,10,10,.18), transparent 60%), linear-gradient(180deg,var(--void),#1a0d0d 55%,var(--void));}
  .download .wrap{max-width:620px;}
  .download h2{font-size:clamp(1.9rem,4vw,2.8rem); font-weight:700;}
  .download p.lede{margin-top:16px; color:var(--ash); font-size:1.05rem;}
  .badge{display:inline-block; margin-top:28px; font-size:.78rem; letter-spacing:.12em; color:var(--blood-bright); border:1px solid rgba(200,30,30,.5); padding:6px 14px; border-radius:20px;}
  .download .btn{margin-top:22px;}
  .download .fineprint{margin-top:18px; font-size:.85rem; color:#6b6460;}

  footer{padding:46px 0; text-align:center; color:#5c5550; font-size:.88rem; border-top:1px solid rgba(122,12,12,.2);}
  footer .logo{display:block; margin-bottom:10px; font-size:1.05rem;}

  .reveal{opacity:0; transform:translateY(24px); transition:opacity .7s ease, transform .7s ease;}
  .reveal.visible{opacity:1; transform:translateY(0);}

  @media (max-width:760px){
    nav ul{position:fixed; top:0; right:0; height:100vh; width:72%; max-width:300px; background:rgba(10,9,8,.97);
      flex-direction:column; justify-content:center; align-items:flex-start; gap:30px; padding:40px; transform:translateX(100%); transition:transform .35s ease;}
    nav ul.open{transform:translateX(0);}
    .nav-toggle{display:block;}
    .features .grid{grid-template-columns:1fr;}
    section{padding:80px 0;}
  }
  @media (prefers-reduced-motion:reduce){
    *{animation-duration:.001s !important; animation-iteration-count:1 !important; transition-duration:.001s !important;}
  }
</style>
</head>
<body>
<div class="grain"></div>
<div class="ambient"></div>

<header id="siteHeader">
  <a href="#" class="logo">HOLLOW<span>WOODS</span></a>
  <nav>
    <ul id="navList">
      <li><a href="#top">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#features">Features</a></li>
      <li><a href="#download">Download</a></li>
    </ul>
  </nav>
  <button class="nav-toggle" id="navToggle" aria-label="Toggle menu" aria-expanded="false">☰</button>
</header>

<section class="hero" id="top">
  <div class="fog f1"></div>
  <div class="fog f2"></div>
  <div class="fog f3"></div>
  <div class="treeline"></div>
  <div class="drip" style="left:18%; animation-delay:.2s"></div>
  <div class="drip" style="left:47%; animation-delay:2.1s"></div>
  <div class="drip" style="left:76%; animation-delay:3.6s"></div>
  <div class="flicker"></div>
  <div class="vignette"></div>
  <div class="hero-inner">
    <h1>HOLLOW WOODS</h1>
    <p class="tagline">No map. No rescue. You are not alone.</p>
    <a href="#download" class="btn">Download the Game</a>
  </div>
  <a href="#about" class="scroll-cue" aria-label="Scroll down">⌄</a>
</section>

<section class="about" id="about">
  <div class="wrap reveal">
    <div class="section-head">
      <div class="rule"></div>
      <h2>About the Nightmare</h2>
    </div>
    <p>You and your friends are flying to Russia in a small private jet you rented for the trip. Mid-air, the engine suddenly gives out — the only option is to land in the forest below.</p>
    <p>You survive the landing, but the jet is wrecked and the crew is gone. With no map and no signal, you'll have to find a way to call for help before you die!</p>
    <p class="whisper">But you should know — you are not alone out here.</p>
  </div>
</section>

<section class="features" id="features">
  <div class="wrap">
    <div class="section-head reveal">
      <div class="rule"></div>
      <h2>Survive the Forest</h2>
      <p class="lede">Four reasons you won't sleep tonight.</p>
    </div>
    <div class="grid">
      <div class="card reveal"><div class="icon">🤝</div><h3>Survive Together</h3><p>Band together with your friends. In the dark, you're only as strong as the group around you.</p></div>
      <div class="card reveal"><div class="icon">🌲</div><h3>Lost in the Forest</h3><p>Explore a massive, shifting forest with no map and no markers. Every path looks the same... until it doesn't.</p></div>
      <div class="card reveal"><div class="icon">👁</div><h3>Unknown Dangers</h3><p>Something moves between the trees. You won't always see it. You'll always feel it.</p></div>
      <div class="card reveal"><div class="icon">🔦</div><h3>Find a Way Out</h3><p>Search for clues, tools, and allies. Escape is possible — but it will cost you.</p></div>
    </div>
  </div>
</section>

<section class="download" id="download">
  <div class="wrap reveal">
    <span class="badge">IN DEVELOPMENT</span>
    <h2>Enter the Woods — If You Dare</h2>
    <p class="lede">The full download goes live soon. Check back, or follow along for the release.</p>
    <!-- Replace href="#" with your real public download URL when it's ready -->
    <a href="#" class="btn" id="downloadBtn">Download the Game</a>
    <p class="fineprint">Download link placeholder — swap the href on this button once your game is live.</p>
  </div>
</section>

<footer>
  <span class="logo">HOLLOW<span style="color:var(--blood-bright)">WOODS</span></span>
  <p>&copy; <span id="year"></span> Hollow Woods. All rights reserved.</p>
</footer>

<script>
  document.getElementById('year').textContent = new Date().getFullYear();

  const header = document.getElementById('siteHeader');
  window.addEventListener('scroll', () => {
    header.classList.toggle('scrolled', window.scrollY > 40);
  }, {passive:true});

  const navList = document.getElementById('navList');
  const navToggle = document.getElementById('navToggle');
  navToggle.addEventListener('click', () => {
    const open = navList.classList.toggle('open');
    navToggle.setAttribute('aria-expanded', open);
    navToggle.textContent = open ? '✕' : '☰';
  });
  navList.querySelectorAll('a').forEach(a => a.addEventListener('click', () => {
    navList.classList.remove('open'); navToggle.textContent = '☰'; navToggle.setAttribute('aria-expanded', false);
  }));

  const io = new IntersectionObserver((entries) => {
    entries.forEach(e => { if (e.isIntersecting) e.target.classList.add('visible'); });
  }, {threshold:0.15});
  document.querySelectorAll('.reveal').forEach(el => io.observe(el));

  document.getElementById('downloadBtn').addEventListener('click', function(e){
    if (this.getAttribute('href') === '#') e.preventDefault();
  });
</script>
</body>
</html>
