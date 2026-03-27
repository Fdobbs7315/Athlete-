
<!DOCTYPE html>

<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0">
<title>Zane Rowe — Athlete Mogul Playbook</title>
<link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=DM+Sans:ital,wght@0,300;0,400;0,500;0,600;1,300&family=Space+Mono:wght@400;700&display=swap" rel="stylesheet">
<style>
:root {
  --gold: #F5B800;
  --gold2: #e0a800;
  --black: #080808;
  --dark: #0f0f0f;
  --card: #161616;
  --card2: #1c1c1c;
  --border: #252525;
  --text: #e0e0e0;
  --muted: #555;
  --muted2: #888;
  --green: #22c55e;
  --red: #ef4444;
  --blue: #60a5fa;
  --purple: #a78bfa;
}

- { margin:0; padding:0; box-sizing:border-box; -webkit-tap-highlight-color:transparent; }

html { scroll-behavior: smooth; }

body {
background: var(–black);
color: var(–text);
font-family: ‘DM Sans’, sans-serif;
overflow-x: hidden;
}

/* ── NAV ── */
.nav {
position: fixed; top:0; left:0; right:0; z-index:200;
background: rgba(8,8,8,0.96);
backdrop-filter: blur(12px);
border-bottom: 1px solid var(–border);
display: flex; align-items: center;
padding: 0 16px;
height: 52px;
gap: 6px;
overflow-x: auto;
scrollbar-width: none;
}
.nav::-webkit-scrollbar { display:none; }
.nav-dot {
flex-shrink: 0;
font-family: ‘Bebas Neue’, sans-serif;
font-size: 11px;
letter-spacing: 1.5px;
color: var(–muted);
padding: 6px 10px;
border-radius: 20px;
cursor: pointer;
border: 1px solid transparent;
white-space: nowrap;
transition: all 0.2s;
}
.nav-dot.active { color: var(–black); background: var(–gold); border-color: var(–gold); }
.nav-logo {
font-family: ‘Bebas Neue’, sans-serif;
font-size: 16px;
letter-spacing: 2px;
color: var(–gold);
margin-right: 8px;
flex-shrink: 0;
}

/* ── SECTIONS ── */
section {
padding: 72px 20px 40px;
min-height: 100vh;
border-bottom: 1px solid var(–border);
}

/* ── HERO ── */
#s0 {
display: flex; flex-direction: column; justify-content: center;
background:
radial-gradient(ellipse 80% 60% at 50% 0%, rgba(245,184,0,0.08) 0%, transparent 70%),
var(–black);
text-align: center;
padding-top: 80px;
min-height: 100vh;
}
.hero-eyebrow {
font-size: 10px; letter-spacing: 4px; color: var(–gold);
text-transform: uppercase; font-weight: 600; margin-bottom: 16px;
}
.hero-name {
font-family: ‘Bebas Neue’, sans-serif;
font-size: clamp(64px, 18vw, 96px);
line-height: 0.9;
color: #fff;
letter-spacing: 2px;
margin-bottom: 8px;
}
.hero-name span { color: var(–gold); }
.hero-pos {
font-family: ‘Bebas Neue’, sans-serif;
font-size: 18px; letter-spacing: 4px; color: var(–muted2);
margin-bottom: 32px;
}
.hero-divider {
width: 48px; height: 2px; background: var(–gold);
margin: 0 auto 32px;
}
.hero-quote {
font-size: 13px; color: var(–muted2); font-style: italic;
line-height: 1.6; max-width: 320px; margin: 0 auto 40px;
}
.hero-quote strong { color: var(–gold); font-style: normal; }
.hero-stats {
display: grid; grid-template-columns: 1fr 1fr 1fr;
gap: 12px; max-width: 360px; margin: 0 auto 40px;
}
.hstat {
background: var(–card);
border: 1px solid var(–border);
border-radius: 8px; padding: 14px 8px;
}
.hstat-val {
font-family: ‘Bebas Neue’, sans-serif;
font-size: 22px; color: var(–gold); line-height: 1;
}
.hstat-label { font-size: 9px; color: var(–muted); letter-spacing: 2px; text-transform: uppercase; margin-top: 3px; }

.scroll-hint {
font-size: 11px; color: var(–muted); letter-spacing: 2px;
animation: bounce 2s infinite;
}
@keyframes bounce { 0%,100%{transform:translateY(0)} 50%{transform:translateY(6px)} }

/* ── SECTION HEADERS ── */
.sec-header { margin-bottom: 24px; }
.sec-step {
font-size: 10px; letter-spacing: 4px; color: var(–gold);
text-transform: uppercase; font-weight: 700; margin-bottom: 4px;
}
.sec-title {
font-family: ‘Bebas Neue’, sans-serif;
font-size: 32px; letter-spacing: 2px; color: #fff; line-height: 1;
}
.sec-sub { font-size: 12px; color: var(–muted2); margin-top: 6px; line-height: 1.5; }

/* ── MODULE 1: PIE ── */
#s1 { background: var(–dark); }
.pie-tabs {
display: grid; grid-template-columns: 1fr 1fr 1fr;
gap: 8px; margin-bottom: 20px;
}
.pie-tab {
padding: 12px 8px; border: 1.5px solid var(–border);
background: transparent; color: var(–muted);
font-family: ‘Bebas Neue’, sans-serif;
font-size: 15px; letter-spacing: 1.5px;
cursor: pointer; border-radius: 6px;
transition: all 0.2s; text-align: center;
}
.pie-tab.active { background: var(–gold); color: var(–black); border-color: var(–gold); }
.pie-card {
background: var(–card); border: 1px solid var(–border);
border-radius: 10px; padding: 20px; margin-bottom: 16px;
transition: all 0.3s;
}
.pie-card.active-card { border-color: var(–gold); }
.pie-card-header {
display: flex; align-items: center; gap: 12px; margin-bottom: 14px;
}
.pie-letter {
font-family: ‘Bebas Neue’, sans-serif; font-size: 36px;
width: 48px; height: 48px; display: flex; align-items: center; justify-content: center;
border-radius: 8px; flex-shrink: 0; line-height: 1;
}
.pie-card-title { font-family: ‘Bebas Neue’, sans-serif; font-size: 20px; letter-spacing: 1px; }
.pie-card-sub { font-size: 11px; color: var(–muted2); margin-top: 2px; }
.pie-tax {
display: flex; justify-content: space-between; align-items: center;
background: var(–card2); border-radius: 6px; padding: 10px 14px;
margin-bottom: 12px;
}
.pie-tax-label { font-size: 11px; color: var(–muted); letter-spacing: 1px; }
.pie-tax-val { font-family: ‘Space Mono’, monospace; font-size: 14px; font-weight: 700; }
.pie-examples { font-size: 11px; color: var(–muted2); line-height: 1.7; }
.pie-examples span { color: var(–gold); font-weight: 600; }
.pie-visual {
display: flex; gap: 4px; margin: 16px 0 8px; height: 10px; border-radius: 5px; overflow: hidden;
}
.pie-seg { height: 100%; transition: width 0.5s cubic-bezier(0.34,1.56,0.64,1); border-radius: 0; }
.pie-seg:first-child { border-radius: 5px 0 0 5px; }
.pie-seg:last-child { border-radius: 0 5px 5px 0; }
.pie-legend {
display: flex; gap: 12px; flex-wrap: wrap; margin-top: 4px;
}
.pie-legend-item {
display: flex; align-items: center; gap: 5px;
font-size: 10px; color: var(–muted2);
}
.legend-dot { width: 8px; height: 8px; border-radius: 50%; flex-shrink: 0; }

/* ── MODULE 2: PAIGE ── */
#s2 { background: var(–black); }
.nil-row {
display: flex; align-items: center; gap: 12px; margin-bottom: 6px;
}
.nil-label-sm { font-size: 10px; letter-spacing: 2px; color: var(–gold); text-transform: uppercase; font-weight: 600; }
.nil-val {
font-family: ‘Bebas Neue’, sans-serif; font-size: 32px; color: #fff; line-height: 1;
}
input[type=range] {
-webkit-appearance: none; width: 100%; height: 4px;
background: var(–border); border-radius: 2px; outline: none; margin: 8px 0 4px;
}
input[type=range]::-webkit-slider-thumb {
-webkit-appearance: none; width: 24px; height: 24px;
background: var(–gold); border-radius: 50%; cursor: pointer;
border: 3px solid var(–black); box-shadow: 0 0 0 2px var(–gold);
}
.range-labels { display: flex; justify-content: space-between; font-size: 10px; color: var(–muted); font-family: ‘Space Mono’, monospace; margin-bottom: 16px; }

.phase-tabs {
display: grid; grid-template-columns: 1fr 1fr 1fr;
gap: 8px; margin-bottom: 16px;
}
.phase-tab {
padding: 10px 4px; border: 1.5px solid var(–border);
background: transparent; color: var(–muted);
font-family: ‘Bebas Neue’, sans-serif;
font-size: 12px; letter-spacing: 1px;
cursor: pointer; border-radius: 6px 6px 0 0;
border-bottom: none; transition: all 0.2s; text-align: center;
position: relative; bottom: -1px; line-height: 1.3;
}
.phase-tab.active { background: var(–gold); color: var(–black); border-color: var(–gold); }

.phase-desc-box {
background: var(–card); border-left: 3px solid var(–gold);
border-radius: 0 8px 8px 0; padding: 12px 14px;
font-size: 12px; color: var(–muted2); line-height: 1.6;
margin-bottom: 16px;
}

.alloc-row {
display: flex; align-items: center; gap: 10px; margin-bottom: 12px;
}
.a-letter { font-family: ‘Bebas Neue’, sans-serif; font-size: 18px; color: var(–gold); width: 16px; flex-shrink: 0; }
.a-info { flex: 1; min-width: 0; }
.a-name { font-size: 9px; letter-spacing: 2px; text-transform: uppercase; color: var(–muted); font-weight: 600; margin-bottom: 4px; }
.a-bar-wrap { height: 7px; background: var(–border); border-radius: 4px; overflow: hidden; }
.a-bar { height: 100%; border-radius: 4px; transition: width 0.5s cubic-bezier(0.34,1.56,0.64,1); }
.bar-p { background: var(–blue); }
.bar-a { background: var(–purple); }
.bar-i { background: var(–green); }
.bar-g { background: var(–red); }
.bar-e { background: var(–gold); }
.a-amt { font-family: ‘Space Mono’, monospace; font-size: 12px; font-weight: 700; color: #fff; width: 76px; text-align: right; flex-shrink: 0; }
.a-pct { font-family: ‘Space Mono’, monospace; font-size: 10px; color: var(–muted); width: 30px; text-align: right; flex-shrink: 0; }

.result-box {
border-radius: 10px; padding: 16px; text-align: center;
margin: 16px 0; transition: all 0.4s;
}
.result-label { font-size: 9px; letter-spacing: 3px; text-transform: uppercase; font-weight: 700; margin-bottom: 6px; }
.result-amount { font-family: ‘Bebas Neue’, sans-serif; font-size: 42px; line-height: 1; }
.result-caption { font-size: 11px; color: var(–muted2); margin-top: 4px; }

.mini-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 10px; margin-top: 16px; }
.mini-card {
background: var(–card); border: 1px solid var(–border);
border-radius: 8px; padding: 12px;
}
.mini-card.hl { border-color: var(–gold); background: #161200; }
.mini-label { font-size: 9px; letter-spacing: 2px; text-transform: uppercase; color: var(–muted); font-weight: 600; margin-bottom: 5px; }
.mini-val { font-family: ‘Bebas Neue’, sans-serif; font-size: 24px; line-height: 1; }
.mini-sub { font-size: 10px; color: var(–muted); margin-top: 2px; }

/* ── MODULE 3: COMPOUNDING ── */
#s3 { background: var(–dark); }
.compound-input-row {
display: flex; align-items: center; gap: 10px; margin-bottom: 20px;
}
.c-input-group { flex: 1; }
.c-input-label { font-size: 9px; letter-spacing: 2px; color: var(–gold); text-transform: uppercase; font-weight: 600; margin-bottom: 6px; }
.c-input-val { font-family: ‘Bebas Neue’, sans-serif; font-size: 26px; color: #fff; line-height: 1; }

.chart-wrap { position: relative; margin: 0 0 16px; height: 180px; }
canvas { display: block; }

.compound-cards { display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 8px; margin-bottom: 16px; }
.cc {
background: var(–card); border: 1px solid var(–border);
border-radius: 8px; padding: 12px 8px; text-align: center;
}
.cc-year { font-size: 9px; letter-spacing: 2px; color: var(–muted); text-transform: uppercase; margin-bottom: 4px; }
.cc-val { font-family: ‘Bebas Neue’, sans-serif; font-size: 20px; color: var(–green); line-height: 1; }
.cc-invested { font-size: 9px; color: var(–muted); margin-top: 3px; font-family: ‘Space Mono’, monospace; }

.rate-row { display: flex; gap: 8px; margin-bottom: 16px; }
.rate-btn {
flex: 1; padding: 8px 4px; border: 1px solid var(–border);
background: transparent; color: var(–muted);
font-family: ‘Space Mono’, monospace; font-size: 11px;
border-radius: 6px; cursor: pointer; transition: all 0.2s;
}
.rate-btn.active { background: var(–green); color: var(–black); border-color: var(–green); font-weight: 700; }

.vs-box {
background: var(–card); border: 1px solid var(–border);
border-radius: 10px; padding: 16px;
}
.vs-title { font-size: 10px; letter-spacing: 3px; color: var(–muted2); text-transform: uppercase; margin-bottom: 12px; }
.vs-row { display: flex; justify-content: space-between; align-items: center; margin-bottom: 8px; padding-bottom: 8px; border-bottom: 1px solid var(–border); }
.vs-row:last-child { border-bottom: none; margin-bottom: 0; padding-bottom: 0; }
.vs-name { font-size: 12px; color: var(–muted2); }
.vs-val { font-family: ‘Space Mono’, monospace; font-size: 13px; font-weight: 700; }

/* ── MODULE 4: DRIVER ── */
#s4 { background: var(–black); }
.driver-grid { display: flex; flex-direction: column; gap: 10px; margin-bottom: 20px; }
.driver-card {
background: var(–card); border: 1px solid var(–border);
border-radius: 10px; overflow: hidden; cursor: pointer;
transition: border-color 0.2s;
}
.driver-card.open { border-color: var(–gold); }
.driver-card-header {
display: flex; align-items: center; gap: 14px; padding: 14px 16px;
}
.driver-initial {
font-family: ‘Bebas Neue’, sans-serif; font-size: 32px; line-height: 1;
width: 40px; flex-shrink: 0;
}
.driver-info { flex: 1; }
.driver-name { font-family: ‘Bebas Neue’, sans-serif; font-size: 18px; letter-spacing: 1px; }
.driver-tagline { font-size: 11px; color: var(–muted2); margin-top: 1px; }
.driver-impact { text-align: right; }
.driver-impact-val { font-family: ‘Space Mono’, monospace; font-size: 13px; font-weight: 700; }
.driver-impact-label { font-size: 9px; color: var(–muted); letter-spacing: 1px; text-transform: uppercase; }
.driver-chevron { color: var(–muted); font-size: 12px; transition: transform 0.3s; flex-shrink: 0; }
.driver-card.open .driver-chevron { transform: rotate(180deg); color: var(–gold); }
.driver-body {
max-height: 0; overflow: hidden;
transition: max-height 0.4s cubic-bezier(0.4,0,0.2,1);
}
.driver-card.open .driver-body { max-height: 300px; }
.driver-body-inner { padding: 0 16px 16px; }
.driver-desc { font-size: 12px; color: var(–muted2); line-height: 1.7; margin-bottom: 10px; }
.driver-tactics { display: flex; flex-direction: column; gap: 6px; }
.tactic {
display: flex; align-items: flex-start; gap: 8px;
font-size: 11px; color: var(–text); line-height: 1.5;
}
.tactic-bullet { color: var(–gold); font-size: 14px; flex-shrink: 0; margin-top: 1px; }

.driver-total {
background: var(–card); border: 1.5px solid var(–gold);
border-radius: 10px; padding: 16px; text-align: center;
}
.dt-label { font-size: 10px; letter-spacing: 3px; color: var(–gold); text-transform: uppercase; font-weight: 600; margin-bottom: 6px; }
.dt-val { font-family: ‘Bebas Neue’, sans-serif; font-size: 48px; color: var(–gold); line-height: 1; }
.dt-sub { font-size: 11px; color: var(–muted2); margin-top: 4px; }

/* ── MODULE 5: ROADMAP ── */
#s5 { background: var(–dark); }
.roadmap { display: flex; flex-direction: column; gap: 0; position: relative; }
.roadmap::before {
content: ‘’; position: absolute; left: 20px; top: 28px; bottom: 28px;
width: 2px; background: var(–border);
}
.rm-item {
display: flex; gap: 16px; position: relative; padding-bottom: 24px;
cursor: pointer;
}
.rm-item:last-child { padding-bottom: 0; }
.rm-dot-wrap {
display: flex; flex-direction: column; align-items: center; flex-shrink: 0; z-index: 1;
}
.rm-dot {
width: 40px; height: 40px; border-radius: 50%;
display: flex; align-items: center; justify-content: center;
font-family: ‘Bebas Neue’, sans-serif; font-size: 16px;
border: 2px solid var(–border); background: var(–card);
transition: all 0.3s; flex-shrink: 0;
}
.rm-item.active .rm-dot { border-color: var(–gold); background: var(–gold); color: var(–black); }
.rm-content { flex: 1; padding-top: 8px; }
.rm-stage { font-size: 9px; letter-spacing: 3px; color: var(–muted); text-transform: uppercase; font-weight: 600; margin-bottom: 4px; }
.rm-title { font-family: ‘Bebas Neue’, sans-serif; font-size: 22px; letter-spacing: 1px; margin-bottom: 6px; }
.rm-item.active .rm-title { color: var(–gold); }
.rm-etr {
display: inline-block; padding: 3px 10px; border-radius: 20px;
font-family: ‘Space Mono’, monospace; font-size: 12px; font-weight: 700;
margin-bottom: 8px;
}
.rm-desc { font-size: 12px; color: var(–muted2); line-height: 1.6; }
.rm-checklist { margin-top: 10px; display: flex; flex-direction: column; gap: 6px; }
.rm-check {
display: flex; gap: 8px; font-size: 11px; color: var(–text);
align-items: flex-start;
}
.rm-check-icon { font-size: 13px; flex-shrink: 0; margin-top: 1px; }
.rm-check.done { color: var(–muted); text-decoration: line-through; }

.rm-panel {
background: var(–card); border: 1px solid var(–border);
border-radius: 10px; padding: 16px; overflow: hidden;
max-height: 0; transition: max-height 0.5s cubic-bezier(0.4,0,0.2,1);
margin-top: 8px;
}
.rm-item.active .rm-panel { max-height: 400px; }

.jump-cta {
background: var(–gold); border-radius: 10px; padding: 20px;
text-align: center; margin-top: 24px;
}
.jump-cta-title { font-family: ‘Bebas Neue’, sans-serif; font-size: 24px; color: var(–black); letter-spacing: 2px; margin-bottom: 4px; }
.jump-cta-sub { font-size: 12px; color: rgba(0,0,0,0.6); }

/* ── CLOSING SECTION ── */
#s6 {
background: radial-gradient(ellipse 80% 60% at 50% 100%, rgba(245,184,0,0.1) 0%, transparent 70%), var(–black);
text-align: center; display: flex; flex-direction: column; justify-content: center; align-items: center;
min-height: 80vh;
}
.close-quote {
font-family: ‘Bebas Neue’, sans-serif; font-size: clamp(28px, 8vw, 48px);
letter-spacing: 2px; line-height: 1.1; color: #fff;
max-width: 340px; margin: 0 auto 8px;
}
.close-quote span { color: var(–gold); }
.close-attr { font-size: 11px; color: var(–muted); letter-spacing: 2px; margin-bottom: 32px; }
.team-grid { display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 10px; width: 100%; max-width: 360px; margin: 0 auto 32px; }
.team-card {
background: var(–card); border: 1px solid var(–border);
border-radius: 8px; padding: 14px 8px; text-align: center;
}
.team-role { font-size: 8px; letter-spacing: 2px; color: var(–gold); text-transform: uppercase; font-weight: 700; margin-bottom: 5px; }
.team-name { font-family: ‘Bebas Neue’, sans-serif; font-size: 14px; letter-spacing: 1px; line-height: 1.1; }
.team-org { font-size: 9px; color: var(–muted2); margin-top: 2px; }

.close-motto { font-family: ‘Bebas Neue’, sans-serif; font-size: 20px; letter-spacing: 4px; color: var(–muted); }
.close-motto span { color: var(–gold); }

/* ── UTILS ── */
.gold { color: var(–gold); }
.green { color: var(–green); }
.red { color: var(–red); }
.fade-up {
opacity: 0; transform: translateY(20px);
transition: opacity 0.5s, transform 0.5s;
}
.fade-up.visible { opacity: 1; transform: translateY(0); }
</style>

</head>
<body>

<!-- NAV -->

<nav class="nav">
  <div class="nav-logo">ZR</div>
  <div class="nav-dot active" onclick="scrollTo(0)">Intro</div>
  <div class="nav-dot" onclick="scrollTo(1)">P.I.E.</div>
  <div class="nav-dot" onclick="scrollTo(2)">PAIGE</div>
  <div class="nav-dot" onclick="scrollTo(3)">Compound</div>
  <div class="nav-dot" onclick="scrollTo(4)">D.R.I.V.E.R.</div>
  <div class="nav-dot" onclick="scrollTo(5)">Roadmap</div>
</nav>

<!-- ── SECTION 0: HERO ── -->

<section id="s0">
  <div class="hero-eyebrow">Athlete Mogul Playbook</div>
  <div class="hero-name">ZANE<br><span>ROWE</span></div>
  <div class="hero-pos">DL · University of Oregon · Denton, TX</div>
  <div class="hero-divider"></div>
  <div class="hero-quote">
    "If three amazing organizations come together with super high skills in complementary domains, the outcome isn't 3× as big — it's <strong>30× or 300×.</strong>"
    <br><br>— Alex Hormozi
  </div>
  <div class="hero-stats">
    <div class="hstat"><div class="hstat-val">$200K</div><div class="hstat-label">2026 NIL</div></div>
    <div class="hstat"><div class="hstat-val">NFL</div><div class="hstat-label">Target</div></div>
    <div class="hstat"><div class="hstat-val">$50M</div><div class="hstat-label">Goal</div></div>
  </div>
  <div class="scroll-hint">▼ SWIPE DOWN TO BEGIN</div>
</section>

<!-- ── SECTION 1: PIE ── -->

<section id="s1">
  <div class="sec-header">
    <div class="sec-step">Step 1</div>
    <div class="sec-title">SLICE THE P.I.E.</div>
    <div class="sec-sub">Three income streams. Three different tax treatments. The goal: shift more income to the right.</div>
  </div>

  <div class="pie-tabs">
    <button class="pie-tab active" onclick="setPie('P')">P<br><span style="font-size:9px;letter-spacing:1px">PERSONAL</span></button>
    <button class="pie-tab" onclick="setPie('I')">I<br><span style="font-size:9px;letter-spacing:1px">INVESTOR</span></button>
    <button class="pie-tab" onclick="setPie('E')">E<br><span style="font-size:9px;letter-spacing:1px">ENTREPRENEUR</span></button>
  </div>

  <div id="pieCard" class="pie-card active-card">
    <div class="pie-card-header">
      <div class="pie-letter" id="pieLetter" style="background:#1a2a3a;color:var(--blue)">P</div>
      <div>
        <div class="pie-card-title" id="pieTitle">Personal Income</div>
        <div class="pie-card-sub" id="pieSub">W2 / NIL — Trading time for money</div>
      </div>
    </div>
    <div class="pie-tax">
      <div class="pie-tax-label">TAX BURDEN</div>
      <div class="pie-tax-val" id="pieTax" style="color:var(--red)">Up to 37%</div>
    </div>
    <div class="pie-examples" id="pieExamples">
      <span>Current Focus:</span> $200,000 NIL earnings<br>
      Active income — highest tax burden<br>
      Every dollar earned is a dollar taxed
    </div>
  </div>

  <div style="margin-bottom:8px;">
    <div class="sec-sub" style="font-size:10px;letter-spacing:2px;text-transform:uppercase;color:var(--gold);margin-bottom:8px;">YOUR INCOME MIX TODAY vs. THE GOAL</div>
    <div class="pie-visual">
      <div class="pie-seg" id="pieSegP" style="width:100%;background:var(--blue)"></div>
      <div class="pie-seg" id="pieSegI" style="width:0%;background:var(--green)"></div>
      <div class="pie-seg" id="pieSegE" style="width:0%;background:var(--gold)"></div>
    </div>
    <div class="pie-legend">
      <div class="pie-legend-item"><div class="legend-dot" style="background:var(--blue)"></div>Personal <span id="pctP" style="color:var(--blue);margin-left:3px;font-family:'Space Mono',monospace;font-size:10px">100%</span></div>
      <div class="pie-legend-item"><div class="legend-dot" style="background:var(--green)"></div>Investor <span id="pctI" style="color:var(--green);margin-left:3px;font-family:'Space Mono',monospace;font-size:10px">0%</span></div>
      <div class="pie-legend-item"><div class="legend-dot" style="background:var(--gold)"></div>Entrepreneur <span id="pctE" style="color:var(--gold);margin-left:3px;font-family:'Space Mono',monospace;font-size:10px">0%</span></div>
    </div>
  </div>

  <div style="margin-top:16px;">
    <div class="sec-sub" style="font-size:10px;letter-spacing:2px;text-transform:uppercase;color:var(--muted);margin-bottom:10px;">DRAG TO SEE YOUR GOAL MIX</div>
    <div style="display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:8px;">
      <div>
        <div style="font-size:9px;color:var(--muted);letter-spacing:2px;text-transform:uppercase;margin-bottom:4px;">Investor %</div>
        <input type="range" min="0" max="50" value="0" id="pieSliderI" oninput="updatePie()">
        <div style="font-family:'Space Mono',monospace;font-size:12px;color:var(--green)" id="pieSliderIVal">0%</div>
      </div>
      <div>
        <div style="font-size:9px;color:var(--muted);letter-spacing:2px;text-transform:uppercase;margin-bottom:4px;">Entrepreneur %</div>
        <input type="range" min="0" max="50" value="0" id="pieSliderE" oninput="updatePie()">
        <div style="font-family:'Space Mono',monospace;font-size:12px;color:var(--gold)" id="pieSliderEVal">0%</div>
      </div>
    </div>
    <div class="pie-tax" id="pieTaxResult" style="border-radius:8px;">
      <div class="pie-tax-label">BLENDED TAX RATE</div>
      <div class="pie-tax-val" id="pieTaxBlended" style="color:var(--red)">37%</div>
    </div>
  </div>
</section>

<!-- ── SECTION 2: PAIGE ── -->

<section id="s2">
  <div class="sec-header">
    <div class="sec-step">Step 3</div>
    <div class="sec-title">THE PAIGE PLAYBOOK</div>
    <div class="sec-sub">Every dollar Zane earns gets a job. See exactly where it goes — and how it changes.</div>
  </div>

  <div class="nil-label-sm">Annual Income</div>
  <div class="nil-val">$<span id="nilDisplay2">200,000</span></div>
  <input type="range" min="50000" max="5000000" step="10000" value="200000" id="nilSlider2" oninput="updatePaige()">
  <div class="range-labels"><span>$50K NIL</span><span>$5M NFL</span></div>

  <div class="phase-tabs">
    <button class="phase-tab active" onclick="setPhase2('good')">PAG<br>GOOD</button>
    <button class="phase-tab" onclick="setPhase2('better')">PAIG<br>BETTER</button>
    <button class="phase-tab" onclick="setPhase2('best')">PAIGE<br>BEST ⭐</button>
  </div>

  <div class="phase-desc-box" id="phaseDesc2">Earning NIL, paying taxes. No entity, no investing. You're leaving serious money on the table every season.</div>

  <div class="alloc-row"><div class="a-letter">P</div><div class="a-info"><div class="a-name">Personal</div><div class="a-bar-wrap"><div class="a-bar bar-p" id="aBarP" style="width:50%"></div></div></div><div class="a-amt" id="aAmtP">$100,000</div><div class="a-pct" id="aPctP">50%</div></div>
  <div class="alloc-row"><div class="a-letter">A</div><div class="a-info"><div class="a-name">Agent</div><div class="a-bar-wrap"><div class="a-bar bar-a" id="aBarA" style="width:10%"></div></div></div><div class="a-amt" id="aAmtA">$20,000</div><div class="a-pct" id="aPctA">10%</div></div>
  <div class="alloc-row"><div class="a-letter">I</div><div class="a-info"><div class="a-name">Investing</div><div class="a-bar-wrap"><div class="a-bar bar-i" id="aBarI" style="width:0%"></div></div></div><div class="a-amt" id="aAmtI">$0</div><div class="a-pct" id="aPctI">0%</div></div>
  <div class="alloc-row"><div class="a-letter">G</div><div class="a-info"><div class="a-name">Government</div><div class="a-bar-wrap"><div class="a-bar bar-g" id="aBarG" style="width:40%"></div></div></div><div class="a-amt" id="aAmtG">$80,000</div><div class="a-pct" id="aPctG">40%</div></div>
  <div class="alloc-row"><div class="a-letter">E</div><div class="a-info"><div class="a-name">Entrepreneur</div><div class="a-bar-wrap"><div class="a-bar bar-e" id="aBarE" style="width:0%"></div></div></div><div class="a-amt" id="aAmtE">$0</div><div class="a-pct" id="aPctE">0%</div></div>

  <div class="result-box" id="resultBox2" style="background:#1a0a0a;border:1px solid var(--red)">
    <div class="result-label" id="resultLabel2" style="color:var(--red)">Left After Season</div>
    <div class="result-amount" id="resultAmt2" style="color:var(--red)">$0</div>
    <div class="result-caption" id="resultCaption2">None invested — money sitting still</div>
  </div>

  <div class="mini-grid">
    <div class="mini-card hl"><div class="mini-label">Tax Saved</div><div class="mini-val gold" id="mTaxSaved">$0</div><div class="mini-sub">vs. doing nothing</div></div>
    <div class="mini-card"><div class="mini-label">Eff. Tax Rate</div><div class="mini-val red" id="mETR">40%</div><div class="mini-sub">Target: ≤15%</div></div>
    <div class="mini-card"><div class="mini-label">Deployed</div><div class="mini-val" id="mDeployed" style="color:var(--muted)">$0</div><div class="mini-sub">Working for you</div></div>
    <div class="mini-card"><div class="mini-label">5-Yr NFL Proj.</div><div class="mini-val" id="mNFL" style="color:var(--muted)">$0</div><div class="mini-sub">invested + compounded</div></div>
  </div>
</section>

<!-- ── SECTION 3: COMPOUNDING ── -->

<section id="s3">
  <div class="sec-header">
    <div class="sec-step">The Power</div>
    <div class="sec-title">MONEY MAKES MONEY</div>
    <div class="sec-sub">This is the number that separates athletes from moguls. Set your annual investment and watch the math work.</div>
  </div>

  <div style="margin-bottom:16px;">
    <div class="c-input-label">Annual Investment Amount</div>
    <div class="c-input-val">$<span id="cInvestDisplay">66,667</span></div>
    <input type="range" min="0" max="2000000" step="5000" value="66667" id="cInvestSlider" oninput="updateCompound()">
    <div class="range-labels"><span>$0</span><span>$2M</span></div>
  </div>

  <div class="rate-row">
    <button class="rate-btn" onclick="setRate(0.06)">6% Conservative</button>
    <button class="rate-btn active" onclick="setRate(0.10)">10% Market Avg</button>
    <button class="rate-btn" onclick="setRate(0.15)">15% Aggressive</button>
  </div>

  <div class="chart-wrap">
    <canvas id="cChart"></canvas>
  </div>

  <div class="compound-cards">
    <div class="cc"><div class="cc-year">5 Years</div><div class="cc-val" id="cc5">$432K</div><div class="cc-invested" id="ci5">put in $333K</div></div>
    <div class="cc"><div class="cc-year">10 Years</div><div class="cc-val" id="cc10">$1.1M</div><div class="cc-invested" id="ci10">put in $667K</div></div>
    <div class="cc"><div class="cc-year">20 Years</div><div class="cc-val" id="cc20">$4.2M</div><div class="cc-invested" id="ci20">put in $1.3M</div></div>
  </div>

  <div class="vs-box">
    <div class="vs-title">WHAT IF YOU SPENT IT INSTEAD?</div>
    <div class="vs-row">
      <div class="vs-name">Spent on lifestyle</div>
      <div class="vs-val red" id="vsSpent">$333,333</div>
    </div>
    <div class="vs-row">
      <div class="vs-name">Invested (5 years)</div>
      <div class="vs-val green" id="vsInvested">$432,421</div>
    </div>
    <div class="vs-row">
      <div class="vs-name" style="font-weight:600;color:#fff">The difference</div>
      <div class="vs-val gold" id="vsDiff">$99,088</div>
    </div>
  </div>
</section>

<!-- ── SECTION 4: DRIVER ── -->

<section id="s4">
  <div class="sec-header">
    <div class="sec-step">Step 5</div>
    <div class="sec-title">D.R.I.V.E.R.</div>
    <div class="sec-sub">Six levers that turn income into lasting wealth. Tap each to see how it applies to Zane.</div>
  </div>

  <div class="driver-grid" id="driverGrid">
    <!-- Populated by JS -->
  </div>

  <div class="driver-total">
    <div class="dt-label">Total Annual Tax Optimization Potential</div>
    <div class="dt-val" id="driverTotal">$0</div>
    <div class="dt-sub">Based on $200K NIL — scales with NFL contract</div>
  </div>
</section>

<!-- ── SECTION 5: ROADMAP ── -->

<section id="s5">
  <div class="sec-header">
    <div class="sec-step">The Journey</div>
    <div class="sec-title">GOOD → BETTER → BEST</div>
    <div class="sec-sub">Where are you today? Tap each stage to see exactly what changes.</div>
  </div>

  <div class="roadmap" id="roadmap">
    <!-- Populated by JS -->
  </div>

  <div class="jump-cta">
    <div class="jump-cta-title">THE DIFFERENCE IS NOT HOW MUCH YOU EARN</div>
    <div class="jump-cta-sub">It's how intentionally you manage what you earn.</div>
  </div>
</section>

<!-- ── SECTION 6: CLOSE ── -->

<section id="s6">
  <div class="close-quote">"YOU ARE A <span>BUSINESS</span>, MAN."</div>
  <div class="close-attr">— The Athlete Mogul Mindset</div>

  <div class="team-grid">
    <div class="team-card">
      <div class="team-role">Make It</div>
      <div class="team-name">Donnell Bruce</div>
      <div class="team-org">Famo Sports</div>
    </div>
    <div class="team-card" style="border-color:var(--gold)">
      <div class="team-role" style="color:var(--gold)">Grow It</div>
      <div class="team-name">Frankie Dobbs</div>
      <div class="team-org">Bank of America</div>
    </div>
    <div class="team-card">
      <div class="team-role">Keep It</div>
      <div class="team-name">J.R. Tolver</div>
      <div class="team-org">Athlete Mogul</div>
    </div>
  </div>

  <div class="close-motto">ATHLETE PLAYS. <span>MOGUL OWNS.</span></div>
</section>

<script>
/* ─────────────────────────────────────────
   NAV / SCROLL
───────────────────────────────────────── */
const sections = ['s0','s1','s2','s3','s4','s5','s6'];
function scrollTo(i) {
  document.getElementById(sections[i]).scrollIntoView({behavior:'smooth'});
}
const navDots = document.querySelectorAll('.nav-dot');
const observer = new IntersectionObserver((entries) => {
  entries.forEach(e => {
    if (e.isIntersecting) {
      const i = sections.indexOf(e.target.id);
      if (i >= 0 && i < navDots.length) {
        navDots.forEach(d => d.classList.remove('active'));
        navDots[i].classList.add('active');
      }
    }
  });
}, {threshold: 0.3});
sections.forEach(id => { const el = document.getElementById(id); if (el) observer.observe(el); });

/* ─────────────────────────────────────────
   UTILS
───────────────────────────────────────── */
function fmt(n) {
  if (n >= 1000000) return '$' + (n/1000000).toFixed(1) + 'M';
  if (n >= 1000) return '$' + Math.round(n/1000) + 'K';
  return '$' + Math.round(n).toLocaleString();
}
function fmtFull(n) { return '$' + Math.round(n).toLocaleString(); }
function compound(annual, years, rate) {
  let t = 0;
  for (let y = 0; y < years; y++) t = (t + annual) * (1 + rate);
  return t;
}

/* ─────────────────────────────────────────
   MODULE 1: PIE
───────────────────────────────────────── */
const pieData = {
  P: {
    letter:'P', letterBg:'#1a2a3a', letterColor:'var(--blue)',
    title:'Personal Income', sub:'W2 / NIL — Trading time for money',
    tax:'Up to 37%', taxColor:'var(--red)',
    examples:'<span>Current Focus:</span> $200,000 NIL earnings<br>Active income — highest tax burden<br>Every dollar earned, a dollar taxed'
  },
  I: {
    letter:'I', letterBg:'#0a1a0a', letterColor:'var(--green)',
    title:'Investor Income', sub:'Market / Passive — Money working for you',
    tax:'15–20% Capital Gains', taxColor:'var(--gold)',
    examples:'<span>Goal:</span> Build the FIN # (Financial Independence Number)<br>Dividends, interest, long-term gains<br>Taxed at lower capital gains rates'
  },
  E: {
    letter:'E', letterBg:'#1a1200', letterColor:'var(--gold)',
    title:'Entrepreneur Income', sub:'Business / Real Estate — Systems working for you',
    tax:'Lowest — Deductions & Depreciation', taxColor:'var(--green)',
    examples:'<span>Goal:</span> LLC Formation (TBD)<br>Business expenses reduce taxable income<br>Real estate depreciation shields earnings'
  }
};
let currentPie = 'P';

function setPie(key) {
  currentPie = key;
  document.querySelectorAll('.pie-tab').forEach((t,i) => t.classList.toggle('active', ['P','I','E'][i] === key));
  const d = pieData[key];
  document.getElementById('pieLetter').textContent = d.letter;
  document.getElementById('pieLetter').style.background = d.letterBg;
  document.getElementById('pieLetter').style.color = d.letterColor;
  document.getElementById('pieTitle').textContent = d.title;
  document.getElementById('pieSub').textContent = d.sub;
  document.getElementById('pieTax').textContent = d.tax;
  document.getElementById('pieTax').style.color = d.taxColor;
  document.getElementById('pieExamples').innerHTML = d.examples;
}

function updatePie() {
  const iVal = parseInt(document.getElementById('pieSliderI').value);
  const eVal = parseInt(document.getElementById('pieSliderE').value);
  const total = Math.min(iVal + eVal, 90);
  const pVal = Math.max(100 - iVal - eVal, 10);
  document.getElementById('pieSliderIVal').textContent = iVal + '%';
  document.getElementById('pieSliderEVal').textContent = eVal + '%';
  document.getElementById('pieSegP').style.width = pVal + '%';
  document.getElementById('pieSegI').style.width = iVal + '%';
  document.getElementById('pieSegE').style.width = eVal + '%';
  document.getElementById('pctP').textContent = pVal + '%';
  document.getElementById('pctI').textContent = iVal + '%';
  document.getElementById('pctE').textContent = eVal + '%';
  // Blended tax
  const blended = Math.round(pVal * 0.37 + iVal * 0.20 + eVal * 0.10);
  const el = document.getElementById('pieTaxBlended');
  el.textContent = blended + '%';
  el.style.color = blended <= 20 ? 'var(--green)' : blended <= 28 ? 'var(--gold)' : 'var(--red)';
}

/* ─────────────────────────────────────────
   MODULE 2: PAIGE
───────────────────────────────────────── */
let nil2 = 200000, phase2 = 'good';
const phases2 = {
  good:   {p:0.50, a:0.10, i:0.00, g:0.40, e:0.00},
  better: {p:0.167, a:0.10, i:0.333, g:0.40, e:0.00},
  best:   {p:0.167, a:0.10, i:0.333, g:0.133, e:0.267},
};
const phaseDescs2 = {
  good: "Earning NIL, paying taxes. No entity, no investing. You're leaving serious money on the table every season.",
  better: "LLC forming, investing 33% of income. Tax burden unchanged — but capital is now compounding in the market.",
  best: "Full P.I.E. diversification. Entity deductions, active tax strategy — ETR drops to 13%. Wealth-building mode unlocked."
};

function setPhase2(p) {
  phase2 = p;
  document.querySelectorAll('.phase-tab').forEach((t,i) => t.classList.toggle('active', ['good','better','best'][i] === p));
  updatePaige();
}

function updatePaige() {
  nil2 = parseInt(document.getElementById('nilSlider2').value);
  document.getElementById('nilDisplay2').textContent = nil2.toLocaleString();
  const p = phases2[phase2];
  const v = {
    p: nil2*p.p, a: nil2*p.a, i: nil2*p.i,
    g: nil2*p.g, e: nil2*p.e
  };
  ['P','A','I','G','E'].forEach(k => {
    const key = {P:'p',A:'a',I:'i',G:'g',E:'e'}[k];
    const pct = p[key];
    document.getElementById('aBar'+k).style.width = (pct*100)+'%';
    document.getElementById('aAmt'+k).textContent = fmtFull(v[key]);
    document.getElementById('aPct'+k).textContent = Math.round(pct*100)+'%';
  });
  document.getElementById('phaseDesc2').textContent = phaseDescs2[phase2];
  const kept = nil2 - v.g - v.a;
  const rb = document.getElementById('resultBox2');
  const ra = document.getElementById('resultAmt2');
  const rl = document.getElementById('resultLabel2');
  const rc = document.getElementById('resultCaption2');
  ra.textContent = fmtFull(kept);
  if (phase2==='good') {
    rb.style.cssText = 'background:#1a0a0a;border:1px solid var(--red)';
    ra.style.color='var(--red)'; rl.style.color='var(--red)';
    rl.textContent='Left After Season';
    rc.textContent='None invested — money sitting still';
  } else if (phase2==='better') {
    rb.style.cssText = 'background:#0a1a0a;border:1px solid var(--green)';
    ra.style.color='var(--green)'; rl.style.color='var(--green)';
    rl.textContent='Kept & Deployed';
    rc.textContent='33% is actively compounding in the market';
  } else {
    rb.style.cssText = 'background:#1a1200;border:1px solid var(--gold)';
    ra.style.color='var(--gold)'; rl.style.color='var(--gold)';
    rl.textContent='Wealth Building Mode 🏆';
    rc.textContent='Entity deductions saved $'+Math.round((nil2*0.40-v.g)/1000)+'K in taxes';
  }
  const ts = Math.max(0, nil2*0.40 - v.g);
  const tsEl = document.getElementById('mTaxSaved');
  tsEl.textContent = fmtFull(ts);
  tsEl.className = 'mini-val ' + (ts>0?'gold':'');
  const etrEl = document.getElementById('mETR');
  const etr = Math.round(p.g*100);
  etrEl.textContent = etr+'%';
  etrEl.className = 'mini-val ' + (etr<=15?'green':etr<=25?'gold':'red');
  const dep = v.i + v.e;
  const depEl = document.getElementById('mDeployed');
  depEl.textContent = fmtFull(dep);
  depEl.style.color = dep>0?'var(--green)':'var(--muted)';
  const nfl = compound(v.i, 5, 0.10);
  const nflEl = document.getElementById('mNFL');
  nflEl.textContent = fmt(nfl);
  nflEl.style.color = nfl>0?'var(--green)':'var(--muted)';
}

/* ─────────────────────────────────────────
   MODULE 3: COMPOUNDING
───────────────────────────────────────── */
let cRate = 0.10;
function setRate(r) {
  cRate = r;
  document.querySelectorAll('.rate-btn').forEach(b => b.classList.toggle('active', parseFloat(b.textContent) === r*100 || b.textContent.includes(r===0.06?'6':r===0.10?'10':'15')));
  updateCompound();
}

function updateCompound() {
  const annual = parseInt(document.getElementById('cInvestSlider').value);
  document.getElementById('cInvestDisplay').textContent = annual.toLocaleString();
  const y5 = compound(annual, 5, cRate);
  const y10 = compound(annual, 10, cRate);
  const y20 = compound(annual, 20, cRate);
  document.getElementById('cc5').textContent = fmt(y5);
  document.getElementById('cc10').textContent = fmt(y10);
  document.getElementById('cc20').textContent = fmt(y20);
  document.getElementById('ci5').textContent = 'put in ' + fmt(annual*5);
  document.getElementById('ci10').textContent = 'put in ' + fmt(annual*10);
  document.getElementById('ci20').textContent = 'put in ' + fmt(annual*20);
  // vs spent
  document.getElementById('vsSpent').textContent = fmt(annual*5);
  document.getElementById('vsInvested').textContent = fmt(y5);
  document.getElementById('vsDiff').textContent = fmt(y5 - annual*5);
  drawCChart(annual);
}

function drawCChart(annual) {
  const canvas = document.getElementById('cChart');
  const dpr = window.devicePixelRatio || 1;
  const W = canvas.parentElement.offsetWidth;
  const H = 180;
  canvas.width = W * dpr; canvas.height = H * dpr;
  canvas.style.width = W + 'px'; canvas.style.height = H + 'px';
  const ctx = canvas.getContext('2d');
  ctx.scale(dpr, dpr);

  const years = 25;
  const data = [], contrib = [];
  for (let y=1; y<=years; y++) { data.push(compound(annual,y,cRate)); contrib.push(annual*y); }
  const max = Math.max(...data, 1);
  const pad = {top:10, bottom:28, left:4, right:4};
  const cW = W - pad.left - pad.right;
  const cH = H - pad.top - pad.bottom;

  ctx.clearRect(0,0,W,H);

  function xP(i) { return pad.left + (i/(years-1))*cW; }
  function yP(v) { return pad.top + cH - (v/max)*cH; }

  // Contributed fill
  ctx.beginPath(); ctx.moveTo(xP(0), yP(contrib[0]));
  for (let i=1;i<years;i++) ctx.lineTo(xP(i), yP(contrib[i]));
  ctx.lineTo(xP(years-1), yP(0)); ctx.lineTo(xP(0), yP(0)); ctx.closePath();
  ctx.fillStyle = 'rgba(255,255,255,0.05)'; ctx.fill();

  // Growth fill
  const gGrad = ctx.createLinearGradient(0,pad.top,0,H);
  gGrad.addColorStop(0,'rgba(34,197,94,0.5)'); gGrad.addColorStop(1,'rgba(34,197,94,0.02)');
  ctx.beginPath(); ctx.moveTo(xP(0), yP(data[0]));
  for (let i=1;i<years;i++) ctx.lineTo(xP(i), yP(data[i]));
  ctx.lineTo(xP(years-1), yP(0)); ctx.lineTo(xP(0), yP(0)); ctx.closePath();
  ctx.fillStyle = gGrad; ctx.fill();

  // Line
  ctx.beginPath(); ctx.moveTo(xP(0), yP(data[0]));
  for (let i=1;i<years;i++) ctx.lineTo(xP(i), yP(data[i]));
  ctx.strokeStyle = '#22c55e'; ctx.lineWidth = 2.5; ctx.stroke();

  // Year labels
  ctx.fillStyle='#444'; ctx.font='9px Space Mono,monospace'; ctx.textAlign='center';
  [4,9,14,19,24].forEach(i => ctx.fillText('Yr'+(i+1), xP(i), H-6));

  // Value callouts
  [4,9,24].forEach(i => {
    const x = xP(i); const y = yP(data[i]);
    ctx.beginPath(); ctx.arc(x,y,3,0,Math.PI*2);
    ctx.fillStyle='#22c55e'; ctx.fill();
    ctx.fillStyle='#22c55e'; ctx.font='bold 9px Space Mono,monospace'; ctx.textAlign='center';
    ctx.fillText(fmt(data[i]), x, y-8);
  });
}

/* ─────────────────────────────────────────
   MODULE 4: DRIVER
───────────────────────────────────────── */
const driverItems = [
  {
    letter:'D', color:'var(--blue)', label:'DONATE',
    tagline:'Charitable Giving — Values-aligned tax reduction',
    impact: 3400, impactLabel: 'Est. tax savings',
    desc: 'Strategic charitable giving reduces taxable income while building community reputation and personal brand. Sets the foundation for Zane\'s public legacy.',
    tactics: [
      'Donor Advised Fund (DAF) — contribute appreciated assets, deduct immediately',
      'Deduct up to 60% of AGI for cash donations',
      'Charitable remainder trust for larger amounts later in career'
    ]
  },
  {
    letter:'R', color:'var(--purple)', label:'RETIRE',
    tagline:'Retirement Accounts — Tax-deferred compounding',
    impact: 7400, impactLabel: 'Annual tax deferral',
    desc: 'Self-employed retirement accounts let Zane shelter significant income now and let it compound tax-deferred for decades.',
    tactics: [
      'Solo 401(k) — up to $69K/year contribution via LLC',
      'SEP-IRA — up to 25% of net self-employment income',
      'Roth conversions during low-income years'
    ]
  },
  {
    letter:'I', color:'var(--green)', label:'INVEST',
    tagline:'Deploy Capital — Money working 24/7',
    impact: 0, impactLabel: 'Compounding wealth',
    desc: 'This is the core engine. Capital deployed today compounds into generational wealth. The earlier Zane starts, the more time does the work.',
    tactics: [
      'Index funds for long-term market exposure (15–20% cap gains rate)',
      'Real estate for cash flow + depreciation shield',
      'Private equity co-investments alongside advisors'
    ]
  },
  {
    letter:'V', color:'var(--gold)', label:'AVOID',
    tagline:'Eliminate Waste — Unnecessary tax triggers',
    impact: 12000, impactLabel: 'Avoidable tax cost',
    desc: 'Not all income has to be recognized immediately. Structuring contracts and timing income recognition correctly can defer significant tax bills.',
    tactics: [
      'Avoid short-term capital gains (hold >12 months)',
      'Structure signing bonuses with installment timing',
      'Don\'t trigger state taxes by playing in high-tax states unnecessarily'
    ]
  },
  {
    letter:'E', color:'var(--gold2)', label:'MINIMIZE',
    tagline:'Entity Structure — Deductions & depreciation',
    impact: 53333, impactLabel: 'LLC deduction potential',
    desc: 'The LLC is the single most important tool in the Athlete Mogul toolkit. It converts personal spending into business deductions.',
    tactics: [
      'Deduct training, equipment, nutrition, travel as business expenses',
      'Home office deduction via LLC',
      'Vehicle depreciation if used for business purposes',
      'Professional development, coaching, and software'
    ]
  },
  {
    letter:'R', color:'var(--red)', label:'DEFER',
    tagline:'Timing — Push taxes into the future',
    impact: 8000, impactLabel: 'Deferred annually',
    desc: 'A dollar of tax paid in 10 years costs less than a dollar paid today. Strategic deferral is legal, simple, and powerful.',
    tactics: [
      'Max out tax-deferred retirement contributions each year',
      'Installment sales on business assets',
      'Like-kind (1031) exchanges in real estate'
    ]
  }
];

let openDriver = null;
let driverNil = 200000;

function buildDriverGrid() {
  const grid = document.getElementById('driverGrid');
  grid.innerHTML = '';
  let total = 0;
  driverItems.forEach((d, i) => {
    total += d.impact;
    const impact = d.impact > 0 ? fmtFull(Math.round(d.impact * (driverNil/200000))) : '∞';
    const card = document.createElement('div');
    card.className = 'driver-card' + (openDriver===i?' open':'');
    card.innerHTML = `
      <div class="driver-card-header" onclick="toggleDriver(${i})">
        <div class="driver-initial" style="color:${d.color}">${d.letter}</div>
        <div class="driver-info">
          <div class="driver-name">${d.label}</div>
          <div class="driver-tagline">${d.tagline}</div>
        </div>
        <div class="driver-impact">
          <div class="driver-impact-val" style="color:${d.color}">${impact}</div>
          <div class="driver-impact-label">${d.impactLabel}</div>
        </div>
        <div class="driver-chevron">▼</div>
      </div>
      <div class="driver-body">
        <div class="driver-body-inner">
          <div class="driver-desc">${d.desc}</div>
          <div class="driver-tactics">${d.tactics.map(t=>`<div class="tactic"><div class="tactic-bullet">▸</div><div>${t}</div></div>`).join('')}</div>
        </div>
      </div>`;
    grid.appendChild(card);
  });
  document.getElementById('driverTotal').textContent = fmtFull(Math.round(total * (driverNil/200000)));
}

function toggleDriver(i) {
  openDriver = openDriver === i ? null : i;
  buildDriverGrid();
}

/* ─────────────────────────────────────────
   MODULE 5: ROADMAP
───────────────────────────────────────── */
const rmData = [
  {
    stage:'Stage 1', title:'PAG — GOOD',
    etr:'40%', etrColor:'var(--red)',
    desc:'You\'re earning NIL income, paying taxes — no entity, no investing structure. This is the starting point, not the destination.',
    checks: [
      {text:'Earning NIL income', done:true},
      {text:'Paying W2/1099 taxes at 37-40%', done:true},
      {text:'No LLC or entity formed', done:false},
      {text:'No investing or deployment', done:false},
      {text:'No proactive tax strategy', done:false}
    ],
    detail: 'Most athletes stay here their entire career — and retire with a fraction of what they earned. The gap between Good and Best is not effort. It\'s structure.'
  },
  {
    stage:'Stage 2', title:'PAIG — BETTER',
    etr:'40% → dropping', etrColor:'var(--gold)',
    desc:'LLC formed. 33% of income deployed into the market. Tax burden is unchanged, but capital is now compounding.',
    checks: [
      {text:'LLC entity formed', done:true},
      {text:'Business banking separated', done:true},
      {text:'33% invested annually', done:true},
      {text:'Bookkeeping in place', done:true},
      {text:'ETR still ~40% (strategy coming)', done:false}
    ],
    detail: 'The critical unlock here: Zane starts the PAIGE allocation. Money is no longer idle. Compounding begins. The NFL contract will multiply this dramatically.'
  },
  {
    stage:'Stage 3 — TARGET', title:'PAIGE — BEST ⭐',
    etr:'≤ 15%', etrColor:'var(--green)',
    desc:'Full P.I.E. diversification. Active entity deductions. Entrepreneur income shields tax. ETR drops from 40% to 13%.',
    checks: [
      {text:'LLC actively generating deductions', done:true},
      {text:'Solo 401(k) or SEP-IRA maxed', done:true},
      {text:'33% Investing + 27% Entrepreneur split', done:true},
      {text:'Charitable giving strategy active', done:true},
      {text:'ETR at 13–15% — saving $53K+ annually', done:true}
    ],
    detail: 'At $200K, the difference between Good and Best is $53,333 in tax saved — every single year. On an NFL contract of $3M, that\'s $795,000 back in Zane\'s pocket annually.'
  }
];

let activeRm = 2;

function buildRoadmap() {
  const rm = document.getElementById('roadmap');
  rm.innerHTML = '';
  rmData.forEach((d, i) => {
    const item = document.createElement('div');
    item.className = 'rm-item' + (activeRm===i?' active':'');
    item.onclick = () => { activeRm = activeRm===i?-1:i; buildRoadmap(); };
    item.innerHTML = `
      <div class="rm-dot-wrap">
        <div class="rm-dot">${i+1}</div>
      </div>
      <div class="rm-content">
        <div class="rm-stage">${d.stage}</div>
        <div class="rm-title">${d.title}</div>
        <div class="rm-etr" style="background:${d.etrColor}22;color:${d.etrColor};border:1px solid ${d.etrColor}44">ETR ${d.etr}</div>
        <div class="rm-desc">${d.desc}</div>
        <div class="rm-panel">
          <div class="rm-checklist">
            ${d.checks.map(c=>`<div class="rm-check${c.done?' done':''}"><div class="rm-check-icon">${c.done?'✓':'○'}</div><div>${c.text}</div></div>`).join('')}
          </div>
          <div style="margin-top:12px;padding-top:12px;border-top:1px solid var(--border);font-size:12px;color:var(--muted2);line-height:1.6;font-style:italic">"${d.detail}"</div>
        </div>
      </div>`;
    rm.appendChild(item);
  });
}

/* ─────────────────────────────────────────
   INIT
───────────────────────────────────────── */
updatePie();
updatePaige();
updateCompound();
buildDriverGrid();
buildRoadmap();

window.addEventListener('resize', () => {
  updateCompound();
});
</script>

</body>
</html>