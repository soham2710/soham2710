<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Soham Sharma — GitHub Profile README</title>
<link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@300;400;500;600;700;800&family=Space+Grotesk:wght@300;400;500;600;700&family=Outfit:wght@300;400;500;600;700;800;900&family=Syne:wght@400;500;600;700;800&display=swap" rel="stylesheet">
<style>
*,*::before,*::after{margin:0;padding:0;box-sizing:border-box}
:root{
  --bg:#020817;--bg2:#0a1628;--bg3:#0f1d32;
  --cyan:#06b6d4;--cyan2:#22d3ee;--cyan-dim:#0e7490;
  --purple:#8b5cf6;--purple2:#a78bfa;--purple-dim:#6d28d9;
  --gold:#fbbf24;--gold2:#fde68a;
  --green:#10b981;--green2:#34d399;
  --pink:#ec4899;--pink2:#f472b6;
  --text:#e2e8f0;--text-dim:#94a3b8;--text-muted:#64748b;
  --border:#1e293b;
}
html{scroll-behavior:smooth;background:var(--bg)}
body{font-family:'JetBrains Mono',monospace;background:var(--bg);color:var(--text);overflow-x:hidden;min-height:100vh}

/* ===== GLOBAL ANIMATED BG ===== */
body::before{
  content:'';position:fixed;inset:0;z-index:0;
  background:
    radial-gradient(ellipse 800px 600px at 20% 20%,rgba(6,182,212,.07),transparent),
    radial-gradient(ellipse 600px 800px at 80% 80%,rgba(139,92,246,.06),transparent),
    radial-gradient(ellipse 400px 400px at 50% 50%,rgba(251,191,36,.03),transparent);
  animation:bgShift 20s ease-in-out infinite;
  pointer-events:none;
}
@keyframes bgShift{
  0%,100%{background-position:0% 0%,100% 100%,50% 50%}
  33%{background-position:30% 20%,70% 80%,60% 40%}
  66%{background-position:10% 80%,90% 20%,40% 60%}
}

/* ===== GRID OVERLAY ===== */
.grid-overlay{
  position:fixed;inset:0;z-index:0;pointer-events:none;
  background-image:
    linear-gradient(rgba(6,182,212,.03) 1px,transparent 1px),
    linear-gradient(90deg,rgba(6,182,212,.03) 1px,transparent 1px);
  background-size:60px 60px;
}

/* ===== FLOATING PARTICLES ===== */
.particles{position:fixed;inset:0;z-index:0;pointer-events:none;overflow:hidden}
.particle{
  position:absolute;border-radius:50%;
  animation:particleFloat linear infinite;
  opacity:0;
}
@keyframes particleFloat{
  0%{transform:translateY(100vh) scale(0);opacity:0}
  10%{opacity:1}
  90%{opacity:1}
  100%{transform:translateY(-100px) scale(1);opacity:0}
}

/* ===== SCANLINE ===== */
.scanline{
  position:fixed;top:0;left:0;right:0;height:2px;z-index:1;pointer-events:none;
  background:linear-gradient(90deg,transparent,var(--cyan),var(--purple),transparent);
  animation:scanDown 8s linear infinite;
  opacity:.15;
}
@keyframes scanDown{0%{top:-2px}100%{top:100vh}}

/* ===== MAIN CONTAINER ===== */
.container{
  position:relative;z-index:2;
  max-width:920px;margin:0 auto;padding:40px 20px 80px;
}

/* ===== HERO SECTION ===== */
.hero{
  position:relative;
  border:1px solid var(--border);
  border-radius:20px;
  padding:60px 40px 50px;
  background:linear-gradient(135deg,rgba(6,182,212,.04),rgba(139,92,246,.04));
  overflow:hidden;
  animation:fadeInUp .8s ease-out;
}
.hero::before{
  content:'';position:absolute;top:0;left:0;right:0;height:2px;
  background:linear-gradient(90deg,var(--cyan),var(--purple),var(--cyan));
  animation:borderGlow 3s ease-in-out infinite;
}
@keyframes borderGlow{
  0%,100%{opacity:.6}50%{opacity:1}
}
.hero::after{
  content:'';position:absolute;top:-50%;right:-30%;width:500px;height:500px;
  background:radial-gradient(circle,rgba(139,92,246,.08),transparent 60%);
  animation:heroOrb 10s ease-in-out infinite;
  pointer-events:none;
}
@keyframes heroOrb{
  0%,100%{transform:translate(0,0)}
  50%{transform:translate(-60px,60px)}
}

/* Corner brackets */
.hero-corners{position:absolute;inset:8px;pointer-events:none}
.hero-corners span{
  position:absolute;width:20px;height:20px;
  border-color:var(--cyan);border-style:solid;border-width:0;
  animation:cornerPulse 2s ease-in-out infinite;
}
.hero-corners span:nth-child(1){top:0;left:0;border-top-width:2px;border-left-width:2px}
.hero-corners span:nth-child(2){top:0;right:0;border-top-width:2px;border-right-width:2px;animation-delay:.5s}
.hero-corners span:nth-child(3){bottom:0;left:0;border-bottom-width:2px;border-left-width:2px;animation-delay:1s}
.hero-corners span:nth-child(4){bottom:0;right:0;border-bottom-width:2px;border-right-width:2px;animation-delay:1.5s}
@keyframes cornerPulse{0%,100%{opacity:.5}50%{opacity:1}}

.hero-label{
  display:inline-flex;align-items:center;gap:8px;
  font-size:11px;letter-spacing:3px;text-transform:uppercase;
  color:var(--cyan);margin-bottom:20px;
  padding:6px 14px;border:1px solid rgba(6,182,212,.3);border-radius:20px;
  background:rgba(6,182,212,.06);
  animation:fadeInUp .8s ease-out .2s both;
}
.hero-label .dot{
  width:6px;height:6px;border-radius:50%;background:var(--cyan);
  animation:blink 1.5s ease-in-out infinite;
}
@keyframes blink{0%,100%{opacity:1}50%{opacity:.3}}

.hero-name{
  font-family:'Syne',sans-serif;
  font-size:clamp(42px,7vw,72px);
  font-weight:800;
  letter-spacing:-1px;
  line-height:1;
  margin-bottom:16px;
  animation:fadeInUp .8s ease-out .3s both;
  background:linear-gradient(135deg,#67e8f9 0%,#ffffff 40%,#a78bfa 100%);
  -webkit-background-clip:text;-webkit-text-fill-color:transparent;
  background-clip:text;
}

.hero-title{
  font-size:14px;letter-spacing:2px;
  background:linear-gradient(90deg,var(--cyan),var(--purple));
  -webkit-background-clip:text;-webkit-text-fill-color:transparent;
  background-clip:text;
  margin-bottom:12px;
  animation:fadeInUp .8s ease-out .4s both;
}

.hero-tagline{
  font-size:12px;color:var(--text-muted);letter-spacing:1px;
  animation:fadeInUp .8s ease-out .5s both;
}

/* Typing effect for tagline */
.typed-text{
  display:inline;
  border-right:2px solid var(--cyan);
  animation:cursorBlink .8s step-end infinite;
}
@keyframes cursorBlink{0%,100%{border-color:var(--cyan)}50%{border-color:transparent}}

/* Stats row */
.hero-stats{
  display:grid;grid-template-columns:repeat(auto-fit,minmax(140px,1fr));
  gap:12px;margin-top:32px;
  animation:fadeInUp .8s ease-out .6s both;
}
.stat-card{
  padding:14px 16px;border-radius:10px;
  border:1px solid var(--border);
  background:rgba(2,8,23,.6);
  transition:all .3s ease;
  position:relative;overflow:hidden;
}
.stat-card::before{
  content:'';position:absolute;top:0;left:0;right:0;height:1px;
  background:linear-gradient(90deg,transparent,var(--cyan),transparent);
  opacity:0;transition:opacity .3s;
}
.stat-card:hover::before{opacity:1}
.stat-card:hover{border-color:rgba(6,182,212,.3);transform:translateY(-2px)}
.stat-label{font-size:9px;letter-spacing:2px;color:var(--text-muted);text-transform:uppercase;margin-bottom:4px}
.stat-value{font-size:18px;font-weight:800}
.stat-value.cyan{color:var(--cyan)}
.stat-value.purple{color:var(--purple2)}
.stat-value.green{color:var(--green2)}
.stat-value.gold{color:var(--gold)}
.stat-value.pink{color:var(--pink2)}

/* ===== SECTION STYLING ===== */
.section{
  margin-top:48px;
  animation:fadeInUp .8s ease-out;
}
.section-header{
  display:flex;align-items:center;gap:12px;margin-bottom:24px;
}
.section-tag{
  font-size:11px;letter-spacing:2px;text-transform:uppercase;
  color:var(--text-muted);
  padding:4px 10px;border-radius:4px;
  border:1px solid var(--border);
  background:rgba(15,29,50,.6);
}
.section-line{flex:1;height:1px;background:linear-gradient(90deg,var(--border),transparent)}
.section-title{
  font-family:'Syne',sans-serif;font-size:28px;font-weight:700;
  margin-bottom:8px;
}

/* ===== ABOUT / WHOAMI ===== */
.whoami-block{
  border:1px solid var(--border);border-radius:16px;
  background:rgba(10,22,40,.5);
  overflow:hidden;
}
.whoami-top{
  padding:12px 20px;border-bottom:1px solid var(--border);
  display:flex;align-items:center;gap:8px;
  background:rgba(2,8,23,.8);
}
.whoami-dot{width:10px;height:10px;border-radius:50%}
.whoami-dot.r{background:#ef4444}.whoami-dot.y{background:#eab308}.whoami-dot.g{background:#22c55e}
.whoami-file{font-size:11px;color:var(--text-muted);margin-left:8px}
.whoami-body{padding:24px;font-size:13px;line-height:2}
.whoami-body .kw{color:var(--purple2)}
.whoami-body .str{color:var(--green2)}
.whoami-body .fn{color:var(--cyan2)}
.whoami-body .cm{color:var(--text-muted)}
.whoami-body .var{color:var(--gold2)}

/* ===== SKILLS GRID ===== */
.skills-grid{display:grid;grid-template-columns:1fr 1fr;gap:16px}
@media(max-width:700px){.skills-grid{grid-template-columns:1fr}}
.skill-card{
  border:1px solid var(--border);border-radius:14px;
  padding:24px;position:relative;overflow:hidden;
  background:rgba(10,22,40,.4);
  transition:all .4s ease;
}
.skill-card:hover{transform:translateY(-3px);border-color:rgba(6,182,212,.3)}
.skill-card::before{
  content:'';position:absolute;top:0;left:0;width:3px;height:100%;
  border-radius:3px 0 0 3px;
}
.skill-card.cyan-accent::before{background:linear-gradient(180deg,var(--cyan),var(--cyan-dim))}
.skill-card.purple-accent::before{background:linear-gradient(180deg,var(--purple),var(--purple-dim))}
.skill-card.green-accent::before{background:linear-gradient(180deg,var(--green),#047857)}
.skill-card.gold-accent::before{background:linear-gradient(180deg,var(--gold),#b45309)}
.skill-card-title{font-size:12px;letter-spacing:2px;font-weight:700;margin-bottom:16px;text-transform:uppercase}
.skill-card.cyan-accent .skill-card-title{color:var(--cyan)}
.skill-card.purple-accent .skill-card-title{color:var(--purple2)}
.skill-card.green-accent .skill-card-title{color:var(--green2)}
.skill-card.gold-accent .skill-card-title{color:var(--gold)}
.tags{display:flex;flex-wrap:wrap;gap:6px}
.tag{
  font-size:10px;padding:5px 10px;border-radius:20px;
  letter-spacing:.5px;
  transition:all .25s ease;
  cursor:default;
}
.tag:hover{transform:scale(1.08)}
.tag.t1{background:rgba(6,182,212,.1);border:1px solid rgba(6,182,212,.25);color:var(--cyan2)}
.tag.t2{background:rgba(139,92,246,.1);border:1px solid rgba(139,92,246,.25);color:var(--purple2)}
.tag.t3{background:rgba(16,185,129,.1);border:1px solid rgba(16,185,129,.25);color:var(--green2)}
.tag.t4{background:rgba(251,191,36,.1);border:1px solid rgba(251,191,36,.25);color:var(--gold2)}
.skill-footer{font-size:9px;color:var(--text-muted);letter-spacing:1.5px;margin-top:14px;text-transform:uppercase}

/* ===== TIMELINE ===== */
.timeline{position:relative;padding-left:40px}
.timeline::before{
  content:'';position:absolute;left:14px;top:0;bottom:0;width:2px;
  background:linear-gradient(180deg,var(--cyan),var(--purple),var(--gold));
  animation:timelinePulse 4s ease-in-out infinite;
}
@keyframes timelinePulse{0%,100%{opacity:.5}50%{opacity:1}}
.tl-item{position:relative;margin-bottom:32px;animation:fadeInUp .6s ease-out both}
.tl-item:nth-child(1){animation-delay:.1s}
.tl-item:nth-child(2){animation-delay:.2s}
.tl-item:nth-child(3){animation-delay:.3s}
.tl-item:nth-child(4){animation-delay:.4s}
.tl-item:nth-child(5){animation-delay:.5s}
.tl-item:nth-child(6){animation-delay:.6s}
.tl-dot{
  position:absolute;left:-33px;top:6px;
  width:16px;height:16px;border-radius:50%;
  border:2px solid var(--cyan);background:var(--bg);
  display:flex;align-items:center;justify-content:center;
  font-size:8px;
  z-index:1;
}
.tl-item.current .tl-dot{
  border-color:var(--gold);
  box-shadow:0 0 12px rgba(251,191,36,.4);
  animation:dotGlow 2s ease-in-out infinite;
}
@keyframes dotGlow{0%,100%{box-shadow:0 0 12px rgba(251,191,36,.3)}50%{box-shadow:0 0 20px rgba(251,191,36,.6)}}
.tl-date{font-size:10px;color:var(--text-muted);letter-spacing:2px;margin-bottom:4px}
.tl-role{font-size:15px;font-weight:700;color:var(--text);margin-bottom:2px}
.tl-company{font-size:12px;color:var(--cyan);margin-bottom:8px}
.tl-desc{font-size:11px;color:var(--text-dim);line-height:1.7;max-width:600px}
.tl-item.current .tl-role{color:var(--gold)}
.tl-item.current .tl-company{color:var(--gold)}
.tl-item.current .tl-date{color:var(--gold)}

/* ===== IMPACT METRICS ===== */
.metrics-row{display:grid;grid-template-columns:repeat(auto-fit,minmax(150px,1fr));gap:12px}
.metric{
  text-align:center;padding:24px 16px;
  border:1px solid var(--border);border-radius:14px;
  background:rgba(10,22,40,.4);
  position:relative;overflow:hidden;
  transition:all .3s ease;
}
.metric:hover{transform:translateY(-4px);border-color:rgba(6,182,212,.3)}
.metric::after{
  content:'';position:absolute;bottom:0;left:0;right:0;height:2px;
  opacity:0;transition:opacity .3s;
}
.metric:nth-child(1)::after{background:var(--cyan)}.metric:nth-child(1):hover::after{opacity:1}
.metric:nth-child(2)::after{background:var(--purple)}.metric:nth-child(2):hover::after{opacity:1}
.metric:nth-child(3)::after{background:var(--green)}.metric:nth-child(3):hover::after{opacity:1}
.metric:nth-child(4)::after{background:var(--gold)}.metric:nth-child(4):hover::after{opacity:1}
.metric:nth-child(5)::after{background:var(--pink)}.metric:nth-child(5):hover::after{opacity:1}
.metric-icon{font-size:24px;margin-bottom:8px}
.metric-num{font-family:'Syne',sans-serif;font-size:32px;font-weight:800;margin-bottom:4px}
.metric-label{font-size:9px;letter-spacing:2px;color:var(--text-muted);text-transform:uppercase}

/* ===== STATUS / NOW ===== */
.status-block{
  border:1px solid var(--border);border-radius:14px;
  background:rgba(10,22,40,.5);padding:24px;
}
.status-row{
  display:flex;align-items:center;gap:12px;
  padding:10px 0;
  border-bottom:1px solid rgba(30,41,59,.5);
  font-size:12px;
}
.status-row:last-child{border-bottom:none}
.status-emoji{font-size:18px;width:28px;text-align:center;flex-shrink:0}
.status-label{color:var(--cyan);font-weight:600;width:90px;font-size:10px;letter-spacing:1.5px;flex-shrink:0}
.status-text{color:var(--text-dim)}

/* ===== CONNECT / CTA ===== */
.cta{
  text-align:center;padding:48px 32px;
  border:1px solid var(--border);border-radius:20px;
  position:relative;overflow:hidden;
  background:linear-gradient(135deg,rgba(6,182,212,.03),rgba(139,92,246,.03));
}
.cta::before{
  content:'';position:absolute;inset:-1px;border-radius:20px;
  background:linear-gradient(135deg,rgba(6,182,212,.3),rgba(139,92,246,.3),rgba(6,182,212,.3));
  z-index:-1;
  animation:ctaBorder 4s ease-in-out infinite;
  -webkit-mask:linear-gradient(#fff 0 0) content-box,linear-gradient(#fff 0 0);
  -webkit-mask-composite:xor;mask-composite:exclude;
  padding:1px;
}
@keyframes ctaBorder{0%,100%{opacity:.4}50%{opacity:.8}}
.cta-quote{
  font-family:'Syne',sans-serif;font-size:22px;font-weight:700;
  background:linear-gradient(135deg,#67e8f9,#fff,#a78bfa);
  -webkit-background-clip:text;-webkit-text-fill-color:transparent;
  background-clip:text;
  margin-bottom:8px;line-height:1.4;
}
.cta-author{font-size:12px;color:var(--text-muted);margin-bottom:28px}
.cta-links{display:flex;flex-wrap:wrap;justify-content:center;gap:10px}
.cta-btn{
  display:inline-flex;align-items:center;gap:8px;
  padding:10px 20px;border-radius:8px;
  font-family:'JetBrains Mono',monospace;
  font-size:11px;letter-spacing:1px;font-weight:600;
  text-decoration:none;
  border:1px solid var(--border);
  background:rgba(2,8,23,.8);
  color:var(--text);
  transition:all .3s ease;
}
.cta-btn:hover{transform:translateY(-2px);border-color:var(--cyan);color:var(--cyan)}
.cta-btn svg{width:14px;height:14px}

/* ===== FOOTER WAVE ===== */
.footer{text-align:center;margin-top:48px;font-size:11px;color:var(--text-muted);letter-spacing:2px}
.footer-bar{
  height:3px;border-radius:2px;margin:0 auto 16px;width:200px;
  background:linear-gradient(90deg,var(--cyan),var(--purple),var(--cyan));
  animation:barGlow 3s ease-in-out infinite;
}
@keyframes barGlow{0%,100%{opacity:.5;width:200px}50%{opacity:1;width:260px}}

/* ===== ANIMATIONS ===== */
@keyframes fadeInUp{
  from{opacity:0;transform:translateY(24px)}
  to{opacity:1;transform:translateY(0)}
}

/* ===== SCROLL ANIMATIONS ===== */
.reveal{opacity:0;transform:translateY(30px);transition:all .7s cubic-bezier(.16,1,.3,1)}
.reveal.visible{opacity:1;transform:translateY(0)}

/* ===== CERTS BADGES ===== */
.certs{display:flex;flex-wrap:wrap;gap:8px;margin-top:12px}
.cert-badge{
  font-size:10px;padding:6px 12px;border-radius:6px;
  background:rgba(251,191,36,.06);
  border:1px solid rgba(251,191,36,.2);
  color:var(--gold2);
  transition:all .25s;
}
.cert-badge:hover{background:rgba(251,191,36,.12);transform:translateY(-1px)}

/* Mobile tweaks */
@media(max-width:600px){
  .hero{padding:40px 20px 32px}
  .hero-name{font-size:36px}
  .hero-stats{grid-template-columns:1fr 1fr}
  .metrics-row{grid-template-columns:1fr 1fr}
  .container{padding:20px 12px 60px}
}
</style>
</head>
<body>

<!-- Ambient layers -->
<div class="grid-overlay"></div>
<div class="particles" id="particles"></div>
<div class="scanline"></div>

<div class="container">

  <!-- ===== HERO ===== -->
  <div class="hero reveal">
    <div class="hero-corners"><span></span><span></span><span></span><span></span></div>
    <div class="hero-label"><span class="dot"></span> AVAILABLE FOR COLLABORATION</div>
    <div class="hero-name">SOHAM SHARMA</div>
    <div class="hero-title">GenAI Architect · AI/ML Engineer · AWS Solutions Architect</div>
    <div class="hero-tagline">
      ✈️ Aircraft Engineer → 🤖 GenAI Architect &nbsp;|&nbsp; 11+ Years &nbsp;|&nbsp; Indore, India
    </div>
    <div class="hero-stats">
      <div class="stat-card">
        <div class="stat-label">Corporate Clients</div>
        <div class="stat-value cyan" data-count="20">0+</div>
      </div>
      <div class="stat-card">
        <div class="stat-label">Satisfaction Rate</div>
        <div class="stat-value purple" data-count="95">0%</div>
      </div>
      <div class="stat-card">
        <div class="stat-label">Monthly Readers</div>
        <div class="stat-value green" data-count="10">0K+</div>
      </div>
      <div class="stat-card">
        <div class="stat-label">Institutions</div>
        <div class="stat-value gold" data-count="15">0+</div>
      </div>
      <div class="stat-card">
        <div class="stat-label">Years Experience</div>
        <div class="stat-value pink" data-count="11">0+</div>
      </div>
    </div>
  </div>

  <!-- ===== WHOAMI ===== -->
  <div class="section reveal">
    <div class="section-header">
      <span class="section-tag">> whoami</span>
      <span class="section-line"></span>
    </div>
    <div class="whoami-block">
      <div class="whoami-top">
        <span class="whoami-dot r"></span>
        <span class="whoami-dot y"></span>
        <span class="whoami-dot g"></span>
        <span class="whoami-file">soham_sharma.py</span>
      </div>
      <div class="whoami-body">
        <span class="kw">class</span> <span class="fn">SohamSharma</span>:<br>
        &nbsp;&nbsp;&nbsp;&nbsp;<span class="var">name</span> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;= <span class="str">"Soham Sharma"</span><br>
        &nbsp;&nbsp;&nbsp;&nbsp;<span class="var">based_in</span> &nbsp;&nbsp;&nbsp;&nbsp;= <span class="str">"Indore, India 🇮🇳"</span><br>
        &nbsp;&nbsp;&nbsp;&nbsp;<span class="var">experience</span> &nbsp;&nbsp;= <span class="str">"11+ years across IT, AI/ML &amp; Enterprise"</span><br>
        &nbsp;&nbsp;&nbsp;&nbsp;<span class="var">current</span> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;= <span class="str">"AI Product Manager &amp; Architect @ IntelliPaaS"</span><br>
        &nbsp;&nbsp;&nbsp;&nbsp;<span class="var">background</span> &nbsp;&nbsp;= <span class="str">"B.E. Aircraft Maintenance → PG Applied Stats"</span><br>
        &nbsp;&nbsp;&nbsp;&nbsp;<span class="var">languages</span> &nbsp;&nbsp;&nbsp;= [<span class="str">"English"</span>, <span class="str">"Hindi"</span>, <span class="str">"Gujarati"</span>, <span class="str">"French"</span>]<br>
        &nbsp;&nbsp;&nbsp;&nbsp;<span class="var">superpower</span> &nbsp;&nbsp;= <span class="str">"Inspecting aircraft engines ✈️ → building AI engines 🤖"</span><br><br>
        &nbsp;&nbsp;&nbsp;&nbsp;<span class="var">focus</span> = [<br>
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="str">"🧠 LLM Ecosystems &amp; Foundation Models"</span>,<br>
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="str">"🕸️ Agentic AI &amp; Multi-Agent Orchestration"</span>,<br>
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="str">"🔍 RAG Architectures &amp; Retrieval Systems"</span>,<br>
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="str">"☁️ Cloud-Native AI (AWS · Azure · GCP)"</span>,<br>
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="str">"⚙️ MLOps / LLMOps &amp; AI Lifecycle"</span>,<br>
        &nbsp;&nbsp;&nbsp;&nbsp;]<br><br>
        &nbsp;&nbsp;&nbsp;&nbsp;<span class="kw">def</span> <span class="fn">quote</span>(<span class="var">self</span>):<br>
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="kw">return</span> <span class="str">"Don't just use AI. Architect it. Ship it. Scale it."</span>
      </div>
    </div>
  </div>

  <!-- ===== SKILLS ===== -->
  <div class="section reveal">
    <div class="section-header">
      <span class="section-tag">> skills --all</span>
      <span class="section-line"></span>
    </div>
    <div class="skills-grid">
      <!-- GenAI & LLMs -->
      <div class="skill-card cyan-accent">
        <div class="skill-card-title">🤖 Generative AI & LLMs</div>
        <div class="tags">
          <span class="tag t1">GPT-4o</span><span class="tag t1">Claude 3</span><span class="tag t1">Gemini Pro</span><span class="tag t1">LLaMA</span><span class="tag t1">Mistral</span><span class="tag t1">Mixtral</span>
          <span class="tag t2">LangChain</span><span class="tag t2">LangGraph</span><span class="tag t2">AutoGen</span><span class="tag t2">CrewAI</span><span class="tag t2">ReAct</span>
          <span class="tag t3">LlamaIndex</span><span class="tag t3">FAISS</span><span class="tag t3">Pinecone</span><span class="tag t3">Chroma</span><span class="tag t3">Haystack</span>
          <span class="tag t4">LoRA</span><span class="tag t4">QLoRA</span><span class="tag t4">PEFT</span><span class="tag t4">HuggingFace</span><span class="tag t4">Prompt Eng.</span>
        </div>
        <div class="skill-footer">RAG · Agentic AI · Fine-Tuning · Multimodal · Vector Search</div>
      </div>
      <!-- Cloud & MLOps -->
      <div class="skill-card purple-accent">
        <div class="skill-card-title">☁️ Cloud & MLOps</div>
        <div class="tags">
          <span class="tag t2">AWS</span><span class="tag t2">SageMaker</span><span class="tag t2">Bedrock</span><span class="tag t2">Azure ML</span><span class="tag t2">Vertex AI</span>
          <span class="tag t1">Docker</span><span class="tag t1">Kubernetes</span><span class="tag t1">Terraform</span><span class="tag t1">GitHub Actions</span>
          <span class="tag t3">MLflow</span><span class="tag t3">W&B</span><span class="tag t3">LangSmith</span><span class="tag t3">PromptLayer</span>
          <span class="tag t4">CloudWatch</span><span class="tag t4">Prometheus</span><span class="tag t4">Grafana</span>
        </div>
        <div class="skill-footer">AWS · Azure · GCP · CI/CD · MLOps · LLMOps · Observability</div>
      </div>
      <!-- Full Stack -->
      <div class="skill-card green-accent">
        <div class="skill-card-title">🛠️ Full Stack Development</div>
        <div class="tags">
          <span class="tag t3">Python</span><span class="tag t3">Django</span><span class="tag t3">FastAPI</span><span class="tag t3">Flask</span><span class="tag t3">Node.js</span>
          <span class="tag t1">React</span><span class="tag t1">Next.js</span><span class="tag t1">TailwindCSS</span><span class="tag t1">AngularJS</span>
          <span class="tag t2">PostgreSQL</span><span class="tag t2">MongoDB</span><span class="tag t2">Redis</span><span class="tag t2">Firebase</span><span class="tag t2">MySQL</span>
          <span class="tag t4">PyTorch</span><span class="tag t4">TensorFlow</span><span class="tag t4">Keras</span><span class="tag t4">Scikit-learn</span>
        </div>
        <div class="skill-footer">Backend · Frontend · Databases · ML Frameworks</div>
      </div>
      <!-- Data, BI & Certs -->
      <div class="skill-card gold-accent">
        <div class="skill-card-title">📊 Data, BI & Certifications</div>
        <div class="tags">
          <span class="tag t4">Tableau</span><span class="tag t4">Power BI</span><span class="tag t4">R Lang</span><span class="tag t4">Jupyter</span><span class="tag t4">QGIS</span>
          <span class="tag t3">Git</span><span class="tag t3">Figma</span><span class="tag t3">Postman</span><span class="tag t3">NGINX</span>
        </div>
        <div class="certs">
          <span class="cert-badge">🏅 AWS Solutions Architect</span>
          <span class="cert-badge">🏅 Six Sigma Green Belt</span>
          <span class="cert-badge">🏅 MongoDB Python Dev</span>
          <span class="cert-badge">🏅 Python DS/ML</span>
          <span class="cert-badge">🏅 PostgreSQL</span>
          <span class="cert-badge">🏅 PowerBI + Tableau</span>
          <span class="cert-badge">🏅 Product Management</span>
        </div>
      </div>
    </div>
  </div>

  <!-- ===== CAREER TIMELINE ===== -->
  <div class="section reveal">
    <div class="section-header">
      <span class="section-tag">> history --career</span>
      <span class="section-line"></span>
    </div>
    <div class="timeline">
      <div class="tl-item current">
        <div class="tl-dot">🏗</div>
        <div class="tl-date">AUG 2025 — PRESENT</div>
        <div class="tl-role">AI Product Manager & Architect</div>
        <div class="tl-company">IntelliPaaS Inc. · Full-time · Remote</div>
        <div class="tl-desc">Owning end-to-end AI product lifecycle. Architecting scalable GenAI systems — LLM solutions, RAG architectures, agent-driven workflows. Driving cloud-native deployment across AWS, Azure, GCP.</div>
      </div>
      <div class="tl-item">
        <div class="tl-dot">🤖</div>
        <div class="tl-date">JAN 2024 — PRESENT</div>
        <div class="tl-role">AI/ML & GenAI Corporate Trainer</div>
        <div class="tl-company">Botmartz IT Solutions · Founder</div>
        <div class="tl-desc">20+ corporate trainings for MNCs (India & US). 95% satisfaction rate. Built real-world solutions — chatbots, LLM tools, RAG pipelines. 10K+ monthly blog readers.</div>
      </div>
      <div class="tl-item">
        <div class="tl-dot">📣</div>
        <div class="tl-date">JUN 2021 — MAR 2024</div>
        <div class="tl-role">GTM / Marketing / Training Lead</div>
        <div class="tl-company">Ziplyne Inc.</div>
        <div class="tl-desc">Led product strategy driving 25% higher retention & 40% new customer growth. Integrated AI/ML capabilities. Achieved 30% increase in CSAT and NPS up by 34 points.</div>
      </div>
      <div class="tl-item">
        <div class="tl-dot">🛠</div>
        <div class="tl-date">JAN 2020 — JUL 2021</div>
        <div class="tl-role">Technical Support Specialist</div>
        <div class="tl-company">Powerweave Software Pvt. Ltd.</div>
        <div class="tl-desc">Led customer onboarding. Reduced ticket resolution time by 35%. Built knowledge base and led cross-functional teams to cut critical bugs by 50%.</div>
      </div>
      <div class="tl-item">
        <div class="tl-dot">🌍</div>
        <div class="tl-date">DEC 2017 — DEC 2019</div>
        <div class="tl-role">GIS Trainer / QC / Production Associate</div>
        <div class="tl-company">Genesys International Corporation Ltd.</div>
        <div class="tl-desc">Built comprehensive GIS training programs. Improved team productivity by 25%. Reduced data errors by 40% through automated QC processes.</div>
      </div>
      <div class="tl-item">
        <div class="tl-dot">✈️</div>
        <div class="tl-date">2012 — 2016</div>
        <div class="tl-role">Aircraft Maintenance Engineering</div>
        <div class="tl-company">Singhania University · Wingsss College, Pune</div>
        <div class="tl-desc">B.E. in Aircraft Maintenance Engineering. The foundation that taught precision, systems thinking, and the discipline to build things that can't afford to fail.</div>
      </div>
    </div>
  </div>

  <!-- ===== IMPACT METRICS ===== -->
  <div class="section reveal">
    <div class="section-header">
      <span class="section-tag">> impact --metrics</span>
      <span class="section-line"></span>
    </div>
    <div class="metrics-row">
      <div class="metric">
        <div class="metric-icon">🏢</div>
        <div class="metric-num" style="color:var(--cyan)" data-count-metric="20">0+</div>
        <div class="metric-label">Corporate Clients</div>
      </div>
      <div class="metric">
        <div class="metric-icon">🎓</div>
        <div class="metric-num" style="color:var(--purple2)" data-count-metric="15">0+</div>
        <div class="metric-label">Institutions</div>
      </div>
      <div class="metric">
        <div class="metric-icon">⭐</div>
        <div class="metric-num" style="color:var(--green2)" data-count-metric="95">0%</div>
        <div class="metric-label">Satisfaction Rate</div>
      </div>
      <div class="metric">
        <div class="metric-icon">📖</div>
        <div class="metric-num" style="color:var(--gold)" data-count-metric="10">0K+</div>
        <div class="metric-label">Monthly Readers</div>
      </div>
      <div class="metric">
        <div class="metric-icon">🔥</div>
        <div class="metric-num" style="color:var(--pink2)" data-count-metric="11">0+</div>
        <div class="metric-label">Years Experience</div>
      </div>
    </div>
  </div>

  <!-- ===== STATUS ===== -->
  <div class="section reveal">
    <div class="section-header">
      <span class="section-tag">> status --now</span>
      <span class="section-line"></span>
    </div>
    <div class="status-block">
      <div class="status-row">
        <span class="status-emoji">🏗️</span>
        <span class="status-label">BUILDING</span>
        <span class="status-text">Production-grade GenAI SaaS @ IntelliPaaS Inc.</span>
      </div>
      <div class="status-row">
        <span class="status-emoji">🎓</span>
        <span class="status-label">TEACHING</span>
        <span class="status-text">AI/ML Corporate Training for MNCs (India & US)</span>
      </div>
      <div class="status-row">
        <span class="status-emoji">📚</span>
        <span class="status-label">MASTERING</span>
        <span class="status-text">Multi-Agent Systems · LLM Fine-Tuning · AI Safety</span>
      </div>
      <div class="status-row">
        <span class="status-emoji">✍️</span>
        <span class="status-label">WRITING</span>
        <span class="status-text">Technical blogs on Prompt Engineering, AI Agents & LLMs</span>
      </div>
      <div class="status-row">
        <span class="status-emoji">🤝</span>
        <span class="status-label">OPEN FOR</span>
        <span class="status-text">AI Consulting · GenAI Architecture · Collaboration</span>
      </div>
    </div>
  </div>

  <!-- ===== CONNECT ===== -->
  <div class="section reveal">
    <div class="cta">
      <div class="cta-quote">"Don't just use AI.<br>Architect it. Ship it. Scale it."</div>
      <div class="cta-author">— Soham Sharma, GenAI Architect · IntelliPaaS Inc.</div>
      <div class="cta-links">
        <a href="https://www.linkedin.com/in/soham-sharma/" class="cta-btn" target="_blank">
          <svg viewBox="0 0 24 24" fill="currentColor"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433a2.062 2.062 0 01-2.063-2.065 2.064 2.064 0 112.063 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/></svg>
          LinkedIn
        </a>
        <a href="mailto:sohamnsharma@gmail.com" class="cta-btn" target="_blank">
          <svg viewBox="0 0 24 24" fill="currentColor"><path d="M24 5.457v13.909c0 .904-.732 1.636-1.636 1.636h-3.819V11.73L12 16.64l-6.545-4.91v9.273H1.636A1.636 1.636 0 010 19.366V5.457c0-2.023 2.309-3.178 3.927-1.964L5.455 4.64 12 9.548l6.545-4.91 1.528-1.145C21.69 2.28 24 3.434 24 5.457z"/></svg>
          Email
        </a>
        <a href="http://www.medium.com/@sohamnsharma" class="cta-btn" target="_blank">
          <svg viewBox="0 0 24 24" fill="currentColor"><path d="M13.54 12a6.8 6.8 0 01-6.77 6.82A6.8 6.8 0 010 12a6.8 6.8 0 016.77-6.82A6.8 6.8 0 0113.54 12zm7.42 0c0 3.54-1.51 6.42-3.38 6.42-1.87 0-3.39-2.88-3.39-6.42s1.52-6.42 3.39-6.42 3.38 2.88 3.38 6.42M24 12c0 3.17-.53 5.75-1.19 5.75-.66 0-1.19-2.58-1.19-5.75s.53-5.75 1.19-5.75C23.47 6.25 24 8.83 24 12z"/></svg>
          Blog
        </a>
        <a href="https://www.twitter.com/sohamnsharma" class="cta-btn" target="_blank">
          <svg viewBox="0 0 24 24" fill="currentColor"><path d="M18.244 2.25h3.308l-7.227 8.26 8.502 11.24H16.17l-5.214-6.817L4.99 21.75H1.68l7.73-8.835L1.254 2.25H8.08l4.713 6.231zm-1.161 17.52h1.833L7.084 4.126H5.117z"/></svg>
          Twitter
        </a>
        <a href="https://www.youtube.com/c/UC9i2PROUgpxGIaDu-Argdjw" class="cta-btn" target="_blank">
          <svg viewBox="0 0 24 24" fill="currentColor"><path d="M23.498 6.186a3.016 3.016 0 00-2.122-2.136C19.505 3.545 12 3.545 12 3.545s-7.505 0-9.377.505A3.017 3.017 0 00.502 6.186C0 8.07 0 12 0 12s0 3.93.502 5.814a3.016 3.016 0 002.122 2.136c1.871.505 9.376.505 9.376.505s7.505 0 9.377-.505a3.015 3.015 0 002.122-2.136C24 15.93 24 12 24 12s0-3.93-.502-5.814zM9.545 15.568V8.432L15.818 12l-6.273 3.568z"/></svg>
          YouTube
        </a>
        <a href="https://www.buymeacoffee.com/sohamnsharma" class="cta-btn" target="_blank">
          ☕ Support
        </a>
      </div>
    </div>
  </div>

  <!-- ===== FOOTER ===== -->
  <div class="footer reveal">
    <div class="footer-bar"></div>
    ✨ Building tomorrow's AI infrastructure, today ✨
  </div>

</div>

<script>
// ===== FLOATING PARTICLES =====
(function(){
  const container = document.getElementById('particles');
  const colors = ['#06b6d4','#8b5cf6','#a78bfa','#67e8f9','#fbbf24','#34d399'];
  for(let i=0;i<30;i++){
    const p = document.createElement('div');
    p.className='particle';
    const size = Math.random()*3+1;
    p.style.cssText=`
      width:${size}px;height:${size}px;
      left:${Math.random()*100}%;
      background:${colors[Math.floor(Math.random()*colors.length)]};
      animation-duration:${Math.random()*15+10}s;
      animation-delay:${Math.random()*10}s;
    `;
    container.appendChild(p);
  }
})();

// ===== SCROLL REVEAL =====
const reveals = document.querySelectorAll('.reveal');
const observer = new IntersectionObserver((entries)=>{
  entries.forEach(e=>{
    if(e.isIntersecting){e.target.classList.add('visible');observer.unobserve(e.target)}
  });
},{threshold:0.1});
reveals.forEach(el=>observer.observe(el));

// ===== COUNT-UP ANIMATION =====
function animateCountUp(el, target, suffix){
  let current=0;
  const duration=2000;
  const step=Math.ceil(target/(duration/16));
  const timer=setInterval(()=>{
    current+=step;
    if(current>=target){current=target;clearInterval(timer)}
    el.textContent=current+suffix;
  },16);
}

// Hero stats
const heroObserver = new IntersectionObserver((entries)=>{
  entries.forEach(e=>{
    if(e.isIntersecting){
      document.querySelectorAll('.stat-value[data-count]').forEach(el=>{
        const t=parseInt(el.dataset.count);
        const text=el.textContent;
        const suffix=text.includes('%')?'%':text.includes('K')?'K+':'+';
        animateCountUp(el,t,suffix);
      });
      heroObserver.unobserve(e.target);
    }
  });
},{threshold:.3});
const heroEl=document.querySelector('.hero');
if(heroEl) heroObserver.observe(heroEl);

// Metric stats
const metricObserver = new IntersectionObserver((entries)=>{
  entries.forEach(e=>{
    if(e.isIntersecting){
      document.querySelectorAll('[data-count-metric]').forEach(el=>{
        const t=parseInt(el.dataset.countMetric);
        const text=el.textContent;
        const suffix=text.includes('%')?'%':text.includes('K')?'K+':'+';
        animateCountUp(el,t,suffix);
      });
      metricObserver.unobserve(e.target);
    }
  });
},{threshold:.3});
const metricsEl=document.querySelector('.metrics-row');
if(metricsEl) metricObserver.observe(metricsEl);

// ===== STAGGER TAGS ON SCROLL =====
document.querySelectorAll('.skill-card').forEach(card=>{
  const tagObs = new IntersectionObserver((entries)=>{
    entries.forEach(e=>{
      if(e.isIntersecting){
        const tags=e.target.querySelectorAll('.tag, .cert-badge');
        tags.forEach((t,i)=>{
          t.style.opacity='0';t.style.transform='translateY(8px)';
          setTimeout(()=>{
            t.style.transition='all .35s cubic-bezier(.16,1,.3,1)';
            t.style.opacity='1';t.style.transform='translateY(0)';
          },i*40);
        });
        tagObs.unobserve(e.target);
      }
    });
  },{threshold:.2});
  tagObs.observe(card);
});
</script>
</body>
</html>
