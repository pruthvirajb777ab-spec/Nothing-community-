# Nothing-community-
X
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Nothing Community</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Doto:wght@400;700;900&family=Inter:wght@400;500&family=Instrument+Serif&display=swap" rel="stylesheet">
<style>
:root{
  --bg:#f2f2f2; --card:#fdfdfd; --ink:#111; --mute:#8a8a8a; --line:#d9d9d9; --chip:#ececec; --dot:#111; --red:#d71921;
}
:root[data-theme="dark"]{
  --bg:#0c0c0c; --card:#161616; --ink:#f2f2f2; --mute:#8a8a8a; --line:#2e2e2e; --chip:#1f1f1f; --dot:#f2f2f2;
}
*{box-sizing:border-box;margin:0}
html{scroll-behavior:smooth}
body{
  font-family:Inter,system-ui,sans-serif;color:var(--ink);background:var(--bg);
  background-image:radial-gradient(circle,var(--dot) 1.2px,transparent 1.6px);
  background-size:134px 134px;background-position:26px 24px;
  -webkit-font-smoothing:antialiased;line-height:1.5;
}
.dm{font-family:Doto,monospace;font-weight:900;letter-spacing:.02em}
.serif{font-family:"Instrument Serif",Georgia,serif;font-weight:400}
.wrap{max-width:1040px;margin:0 auto;padding:0 20px}

/* nav */
nav{display:flex;align-items:center;justify-content:space-between;padding:22px 0}
.logo{display:flex;align-items:center;gap:10px;font-size:22px;text-decoration:none;color:var(--ink)}
.logo img{height:26px;width:auto;display:block}
.pill{display:inline-flex;align-items:center;justify-content:center;gap:8px;height:48px;padding:0 26px;border-radius:999px;border:0;font:500 16px Inter,sans-serif;text-decoration:none;cursor:pointer;transition:transform .15s}
.pill:active{transform:scale(.97)}
.pill.dark{background:var(--ink);color:var(--bg)}
.pill.soft{background:var(--chip);color:var(--ink)}
.pill.sm{height:40px;padding:0 20px;font-size:14px}
:focus-visible{outline:2px solid var(--red);outline-offset:3px}

/* hero */
.hero{padding:72px 0 56px;text-align:left}
.hero h1{font-size:clamp(46px,11vw,112px);line-height:.95;margin-bottom:28px}
.hero h1 span{display:block}
.hero p.lead{font-family:"Instrument Serif",serif;font-size:clamp(24px,4vw,34px);line-height:1.2;max-width:560px;color:var(--ink)}
.cta{display:flex;flex-wrap:wrap;gap:12px;margin-top:36px}
.live{display:inline-flex;align-items:center;gap:8px;font-size:13px;color:var(--mute);margin-top:22px}
.live i{width:8px;height:8px;border-radius:50%;background:var(--red);animation:blink 1.6s steps(2,start) infinite}
@keyframes blink{50%{opacity:.15}}

/* cards */
.card{background:var(--card);border-radius:28px;padding:32px;position:relative;overflow:hidden}
.stage{display:grid;grid-template-columns:1.1fr .9fr;gap:16px}
.feed .row{display:flex;gap:12px;padding:16px 0;border-top:1px solid var(--line)}
.feed .row:first-of-type{border-top:0}
.av{flex:none;width:40px;height:40px;border-radius:50%;background:var(--ink);color:var(--bg);display:grid;place-items:center;font-family:Doto,monospace;font-weight:900;font-size:18px}
.av.r{background:var(--red);color:#fff}
.feed b{font-weight:500}.feed small{color:var(--mute);margin-left:6px}
.feed p{margin-top:2px;font-size:15px}
.meta{display:flex;gap:22px;margin-top:10px;color:var(--mute);font-size:13px}
.big{font-size:clamp(64px,12vw,120px);line-height:.9}
.card h3{font-family:"Instrument Serif",serif;font-weight:400;font-size:34px;line-height:1.05;margin-bottom:10px}
.card p.d{color:var(--mute);font-size:15px;max-width:34ch}
.logo-card{display:flex;flex-direction:column;justify-content:space-between;min-height:320px}
.applogo{width:96px;height:96px;border-radius:26px;background:var(--ink);display:grid;place-items:center;overflow:hidden;color:var(--bg);font-size:44px}
.applogo img{width:100%;height:100%;object-fit:cover}
.grid3{display:grid;grid-template-columns:repeat(3,1fr);gap:16px;margin-top:16px}
.grid3 .card{padding:28px;min-height:220px;display:flex;flex-direction:column;justify-content:space-between}
.glyph{font-size:46px;line-height:1}

/* join */
.join{margin:16px 0 0;text-align:center;padding:64px 24px}
.join h2{font-size:clamp(40px,8vw,72px);line-height:1;margin-bottom:12px}
.join .cta{justify-content:center}
footer{display:flex;flex-wrap:wrap;justify-content:space-between;gap:12px;padding:36px 0 96px;color:var(--mute);font-size:13px}
footer a{color:inherit}

/* theme toggle */
.theme{position:fixed;left:20px;bottom:calc(20px + env(safe-area-inset-bottom,0px));width:58px;height:58px;border-radius:50%;border:0;background:var(--card);color:var(--ink);font-size:20px;cursor:pointer;box-shadow:0 0 0 1px var(--line)}

html,body{overflow-x:hidden}
img{max-width:100%}
.wrap{padding-left:max(20px,env(safe-area-inset-left,0px));padding-right:max(20px,env(safe-area-inset-right,0px))}
nav{padding-top:max(22px,env(safe-area-inset-top,0px))}
.card,.feed p{overflow-wrap:anywhere}
@media(max-width:760px){
  body{background-size:90px 90px;background-position:20px 18px}
  .stage,.grid3{grid-template-columns:1fr}
  .hero{padding:36px 0 40px}
  .hero h1{font-size:clamp(44px,15vw,72px);margin-bottom:22px}
  .hero p.lead{font-size:24px}
  .cta{flex-direction:column;margin-top:28px}
  .cta .pill{width:100%;height:54px}
  .card{padding:22px;border-radius:24px}
  .card h3{font-size:30px}
  .feed .row{gap:10px;padding:14px 0}
  .meta{gap:16px;flex-wrap:wrap}
  .logo-card{min-height:0;gap:28px}
  .applogo{width:80px;height:80px;border-radius:22px}
  .big{font-size:72px}
  .grid3 .card{min-height:0;gap:36px}
  .join{padding:44px 20px}
  .join .lead{font-size:22px!important}
  footer{flex-direction:column;padding-bottom:110px}
  .theme{width:52px;height:52px}
}
@media(max-width:360px){
  .logo span{font-size:18px}
  .pill.sm{padding:0 16px}
}
@media(prefers-reduced-motion:reduce){.live i{animation:none}html{scroll-behavior:auto}}
</style>
</head>
<body>
<div class="wrap">
  <nav>
    <a class="logo" href="#">
      <!-- Replace with your file: nothingcommunity.png -->
      <img src="nothingcommunity.png" alt="Nothing Community" onerror="this.style.display='none';this.nextElementSibling.style.display='inline'">
      <span class="dm" style="display:none">NOTHING COMMUNITY</span>
    </a>
    <a class="pill dark sm" href="#join">Get the app</a>
  </nav>

  <header class="hero">
    <h1 class="dm"><span>Say it.</span><span>Share it.</span><span style="color:var(--red)">Nothing</span><span>else.</span></h1>
    <p class="lead">The home for everyone who loves Nothing. Post, follow and talk with the community, all in one place.</p>
    <div class="cta">
      <a class="pill dark" href="#join">Download the app</a>
      <a class="pill soft" href="#features">See what's inside</a>
    </div>
    <div class="live"><i></i>Community is live now</div>
  </header>

  <section class="stage" id="features">
    <div class="card feed" aria-label="Sample feed">
      <div class="row"><div class="av">N</div><div><b>Nothing Fan</b><small>@nothingfan · 2m</small><p>Glyph lights on the new setup look unreal. Anyone else building a Nothing desk?</p><div class="meta"><span>Reply 24</span><span>Repost 61</span><span>Like 412</span></div></div></div>
      <div class="row"><div class="av r">G</div><div><b>Glyph Lab</b><small>@glyphlab · 14m</small><p>Dropped a new widget pack for Nothing OS. Dot matrix everything.</p><div class="meta"><span>Reply 9</span><span>Repost 33</span><span>Like 208</span></div></div></div>
      <div class="row"><div class="av">D</div><div><b>Dot Daily</b><small>@dotdaily · 1h</small><p>Poll: best Nothing launcher wallpaper?</p><div class="meta"><span>Reply 112</span><span>Repost 18</span><span>Like 97</span></div></div></div>
    </div>

    <div class="card logo-card">
      <div class="applogo dm">
        <!-- Replace with your file: applogo.png -->
        <img src="applogo.png" alt="App logo" onerror="this.remove();">
      </div>
      <div>
        <div class="big dm">N</div>
        <h3 style="margin-top:18px">A feed made for Nothing.</h3>
        <p class="d">Same pace as the platforms you know. Built only for this community.</p>
      </div>
    </div>
  </section>

  <section class="grid3">
    <div class="card"><div class="glyph dm">Aa</div><div><h3>Post</h3><p class="d">Share thoughts, photos and setups with the community.</p></div></div>
    <div class="card"><div class="glyph dm">@</div><div><h3>Follow</h3><p class="d">Keep up with creators, designers and fellow owners.</p></div></div>
    <div class="card"><div class="glyph dm">&#9679;&#9679;&#9679;</div><div><h3>Talk</h3><p class="d">Reply, repost and start conversations in real time.</p></div></div>
  </section>

  <section class="card join" id="join">
    <h2 class="dm">Join in.</h2>
    <p class="lead serif" style="font-size:26px;color:var(--mute)">Create an account and post your first message.</p>
    <div class="cta">
      <a class="pill dark" href="#">Create an account</a>
      <a class="pill soft" href="#">Sign in</a>
    </div>
  </section>

  <footer>
    <span>Nothing Community is an independent fan project.</span>
    <span><a href="#">Privacy Policy</a> and <a href="#">User Agreement</a></span>
  </footer>
</div>

<button class="theme" id="t" aria-label="Toggle light and dark theme">&#9680;</button>
<script>
(function(){
  var r=document.documentElement,b=document.getElementById('t');
  if(window.matchMedia&&matchMedia('(prefers-color-scheme: dark)').matches)r.dataset.theme='dark';
  b.onclick=function(){r.dataset.theme=r.dataset.theme==='dark'?'light':'dark'};
})();
</script>
</body>
</html>
