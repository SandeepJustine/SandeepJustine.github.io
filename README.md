<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Joseph Sandeep Justine | Full Stack Developer, Cyber Security Analyst, DevOps & AI Consultant</title>
<meta name="description" content="Portfolio of Joseph Sandeep Justine: Information Systems graduate, full stack developer, cyber security analyst, DevOps engineer and AI consultant based in Malawi.">
<meta name="theme-color" content="#0a0f1d">
<meta property="og:title" content="Joseph Sandeep Justine | Portfolio">
<meta property="og:description" content="Robust software engineering, ironclad security, scalable DevOps and intelligent AI solutions.">
<meta property="og:type" content="website">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&family=JetBrains+Mono:wght@400;500;700&display=swap" rel="stylesheet">
<link rel="icon" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 64 64'%3E%3Crect width='64' height='64' rx='12' fill='%230a0f1d'/%3E%3Ctext x='8' y='42' font-family='monospace' font-size='30' font-weight='700' fill='%2300f0ff'%3E%3E_J%3C/text%3E%3C/svg%3E">

<style>
:root{
  --bg:#0a0f1d; --bg2:#0e1528; --cyan:#00f0ff; --green:#00ff66; --white:#f4f8ff;
  --muted:#9aa7c2; --glass:rgba(255,255,255,.04); --border:rgba(0,240,255,.16);
  --mono:'JetBrains Mono',ui-monospace,SFMono-Regular,Menlo,Consolas,monospace;
  --sans:'Inter',system-ui,-apple-system,Segoe UI,Roboto,sans-serif;
}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth;scroll-padding-top:80px}
body{background:var(--bg);color:var(--white);font-family:var(--sans);line-height:1.65;overflow-x:hidden;-webkit-font-smoothing:antialiased}
::selection{background:var(--cyan);color:#001018}
::-webkit-scrollbar{width:10px}
::-webkit-scrollbar-track{background:var(--bg)}
::-webkit-scrollbar-thumb{background:linear-gradient(var(--cyan),var(--green));border-radius:8px;border:2px solid var(--bg)}
a{color:inherit;text-decoration:none}
img,svg{max-width:100%}
.container{width:min(1180px,100% - 40px);margin-inline:auto}
section{position:relative;padding:100px 0;z-index:2}

/* backgrounds */
#matrix,#mesh{position:fixed;inset:0;width:100%;height:100%;z-index:0;pointer-events:none}
#mesh{z-index:1}
.vignette{position:fixed;inset:0;z-index:1;pointer-events:none;background:radial-gradient(ellipse at center,transparent 35%,rgba(10,15,29,.85) 100%)}
.cursor-glow{position:fixed;width:420px;height:420px;border-radius:50%;pointer-events:none;z-index:1;transform:translate(-50%,-50%);
  background:radial-gradient(circle,rgba(0,240,255,.13),transparent 65%);left:50%;top:40%;transition:opacity .3s}

/* nav */
header{position:fixed;top:0;left:0;right:0;z-index:100;transition:.3s}
header.scrolled{background:rgba(10,15,29,.78);backdrop-filter:blur(14px);-webkit-backdrop-filter:blur(14px);border-bottom:1px solid var(--border)}
.nav{display:flex;align-items:center;justify-content:space-between;height:70px}
.logo{font-family:var(--mono);font-weight:700;font-size:1.05rem;color:var(--green);display:flex;align-items:center;gap:6px}
.logo .p{color:var(--cyan)}
.logo .caret{display:inline-block;width:9px;height:1.1em;background:var(--green);animation:blink 1s steps(1) infinite}
.logo:hover{text-shadow:0 0 12px var(--green)}
nav ul{display:flex;gap:30px;list-style:none}
nav a{font-family:var(--mono);font-size:.84rem;color:var(--muted);position:relative;padding:4px 0;transition:.25s}
nav a::after{content:"";position:absolute;left:0;bottom:-2px;height:2px;width:0;background:var(--cyan);box-shadow:0 0 8px var(--cyan);transition:.3s}
nav a:hover,nav a.active{color:var(--cyan)}
nav a:hover::after,nav a.active::after{width:100%}
.burger{display:none;background:none;border:1px solid var(--border);color:var(--cyan);width:42px;height:42px;border-radius:8px;font-size:1.3rem;cursor:pointer}

/* hero */
.hero{min-height:100vh;display:flex;align-items:center;padding-top:110px}
.hero-grid{display:grid;grid-template-columns:1.25fr .75fr;gap:50px;align-items:center}
.tag{display:inline-flex;align-items:center;gap:8px;font-family:var(--mono);font-size:.8rem;color:var(--green);border:1px solid rgba(0,255,102,.3);background:rgba(0,255,102,.06);padding:6px 14px;border-radius:50px;margin-bottom:22px}
.tag i{width:8px;height:8px;border-radius:50%;background:var(--green);box-shadow:0 0 10px var(--green);animation:pulse 2s infinite}
h1{font-size:clamp(2.3rem,5.4vw,4.1rem);line-height:1.1;font-weight:800;letter-spacing:-.02em}
h1 .name{background:linear-gradient(90deg,var(--cyan),var(--green));-webkit-background-clip:text;background-clip:text;color:transparent}
.typing{font-family:var(--mono);font-size:clamp(1.1rem,2.4vw,1.6rem);margin:18px 0;color:var(--cyan);min-height:2.2em}
.typing .cursor{display:inline-block;width:10px;height:1.1em;background:var(--cyan);vertical-align:-3px;margin-left:3px;animation:blink 1s steps(1) infinite}
.bio{color:var(--muted);max-width:600px;font-size:1.08rem}
.actions{display:flex;flex-wrap:wrap;gap:16px;margin:34px 0 26px;align-items:center}
.btn{font-family:var(--mono);font-weight:500;font-size:.92rem;padding:14px 26px;border-radius:8px;cursor:pointer;border:1px solid var(--cyan);transition:.3s;display:inline-flex;align-items:center;gap:8px}
.btn.primary{background:var(--cyan);color:#001018;box-shadow:0 0 22px rgba(0,240,255,.45);font-weight:700}
.btn.primary:hover{transform:translateY(-3px);box-shadow:0 0 38px rgba(0,240,255,.8)}
.btn.outline{background:transparent;color:var(--cyan)}
.btn.outline:hover{background:rgba(0,240,255,.1);transform:translateY(-3px);box-shadow:0 0 22px rgba(0,240,255,.3)}
.socials{display:flex;gap:12px}
.socials a{width:46px;height:46px;display:grid;place-items:center;border:1px solid var(--border);border-radius:10px;background:var(--glass);color:var(--muted);transition:.3s}
.socials a:hover{color:var(--cyan);border-color:var(--cyan);box-shadow:0 0 18px rgba(0,240,255,.4);transform:translateY(-3px)}
.socials svg{width:22px;height:22px;fill:currentColor}

.hero-card{border:1px solid var(--border);background:var(--glass);backdrop-filter:blur(16px);-webkit-backdrop-filter:blur(16px);border-radius:16px;overflow:hidden;box-shadow:0 20px 60px rgba(0,0,0,.4),0 0 40px rgba(0,240,255,.06)}
.bar{display:flex;gap:7px;padding:12px 16px;background:rgba(255,255,255,.04);border-bottom:1px solid var(--border);align-items:center}
.bar span{width:11px;height:11px;border-radius:50%;background:#ff5f56}
.bar span:nth-child(2){background:#ffbd2e}.bar span:nth-child(3){background:#27c93f}
.bar em{margin-left:auto;font-style:normal;font-family:var(--mono);font-size:.72rem;color:var(--muted)}
.code{padding:20px;font-family:var(--mono);font-size:.82rem;line-height:1.9;color:var(--muted)}
.code .k{color:var(--cyan)}.code .s{color:var(--green)}.code .c{color:#5c6a88}

/* headings */
.sec-head{margin-bottom:54px}
.sec-head .eyebrow{font-family:var(--mono);color:var(--green);font-size:.85rem}
.sec-head h2{font-size:clamp(1.9rem,4vw,2.7rem);font-weight:800;letter-spacing:-.01em;margin-top:6px;display:flex;align-items:center;gap:18px}
.sec-head h2::after{content:"";flex:1;height:1px;background:linear-gradient(90deg,var(--border),transparent)}

/* glass */
.glass{background:var(--glass);border:1px solid var(--border);border-radius:16px;backdrop-filter:blur(14px);-webkit-backdrop-filter:blur(14px);transition:.35s;position:relative}
.glass:hover{border-color:rgba(0,240,255,.6);box-shadow:0 0 30px rgba(0,240,255,.16),inset 0 0 30px rgba(0,240,255,.03);transform:translateY(-6px)}

/* about */
.about-grid{display:grid;grid-template-columns:1fr 1.2fr;gap:40px}
.about-text p{color:var(--muted);margin-bottom:18px;font-size:1.04rem}
.about-text strong{color:var(--white)}
.stats{display:grid;grid-template-columns:repeat(3,1fr);gap:14px;margin-top:28px}
.stat{padding:18px 12px;text-align:center}
.stat b{display:block;font-family:var(--mono);font-size:1.7rem;color:var(--cyan)}
.stat span{font-size:.78rem;color:var(--muted)}
.skills{display:grid;grid-template-columns:repeat(2,1fr);gap:18px}
.skill-box{padding:24px}
.skill-box h3{font-size:1rem;display:flex;align-items:center;gap:10px;margin-bottom:16px;font-family:var(--mono)}
.ico{width:34px;height:34px;border-radius:8px;display:grid;place-items:center;background:rgba(0,240,255,.1);color:var(--cyan);font-family:var(--mono);font-size:.85rem;font-weight:700;border:1px solid var(--border)}
.badges{display:flex;flex-wrap:wrap;gap:8px}
.badge{font-size:.78rem;padding:6px 12px;border-radius:50px;border:1px solid var(--border);background:rgba(0,240,255,.05);color:#cfe9ee;transition:.25s}
.badge:hover{border-color:var(--green);color:var(--green);background:rgba(0,255,102,.07)}

/* tabs / projects */
.tabs{display:flex;flex-wrap:wrap;gap:10px;margin-bottom:34px}
.tab{font-family:var(--mono);font-size:.82rem;padding:10px 18px;border-radius:50px;border:1px solid var(--border);background:var(--glass);color:var(--muted);cursor:pointer;transition:.3s}
.tab:hover{color:var(--cyan);border-color:var(--cyan)}
.tab.active{background:var(--cyan);color:#001018;border-color:var(--cyan);font-weight:700;box-shadow:0 0 20px rgba(0,240,255,.5)}
.projects{display:grid;grid-template-columns:repeat(auto-fill,minmax(340px,1fr));gap:24px}
.card{padding:28px;display:flex;flex-direction:column;animation:rise .5s both}
.card.hide{display:none}
.card .cat{font-family:var(--mono);font-size:.72rem;color:var(--green);text-transform:uppercase;letter-spacing:.08em}
.card h3{font-size:1.25rem;margin:8px 0 10px}
.card p{color:var(--muted);font-size:.95rem;margin-bottom:16px}
.tech{display:flex;flex-wrap:wrap;gap:7px;margin-bottom:16px}
.tech span{font-family:var(--mono);font-size:.72rem;padding:4px 10px;border-radius:6px;background:rgba(0,240,255,.08);color:var(--cyan);border:1px solid rgba(0,240,255,.2)}
.metrics{list-style:none;margin-bottom:22px;border-top:1px dashed var(--border);padding-top:14px}
.metrics li{font-size:.86rem;color:#cdd8ee;padding-left:20px;position:relative;margin-bottom:4px}
.metrics li::before{content:">";position:absolute;left:0;color:var(--green);font-family:var(--mono)}
.card .btn{margin-top:auto;align-self:flex-start;padding:10px 18px;font-size:.82rem}

/* experience */
.timeline{position:relative;padding-left:34px}
.timeline::before{content:"";position:absolute;left:7px;top:6px;bottom:6px;width:2px;background:linear-gradient(var(--cyan),var(--green),transparent)}
.job{padding:26px;margin-bottom:24px;position:relative}
.job::before{content:"";position:absolute;left:-34px;top:32px;width:16px;height:16px;border-radius:50%;background:var(--bg);border:2px solid var(--cyan);box-shadow:0 0 14px var(--cyan)}
.job .when{font-family:var(--mono);font-size:.78rem;color:var(--green)}
.job h3{font-size:1.2rem;margin:4px 0 2px}
.job .org{color:var(--cyan);font-size:.95rem;margin-bottom:10px}
.job ul{color:var(--muted);padding-left:18px;font-size:.95rem}
.job li{margin-bottom:5px}

/* certs */
.certs{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:20px}
.cert{padding:26px;text-align:center}
.cert .seal{width:64px;height:64px;margin:0 auto 16px;border-radius:50%;display:grid;place-items:center;font-family:var(--mono);font-weight:700;color:var(--cyan);border:2px solid var(--cyan);box-shadow:0 0 20px rgba(0,240,255,.3),inset 0 0 14px rgba(0,240,255,.15)}
.cert h3{font-size:1rem;margin-bottom:6px}
.cert p{font-size:.82rem;color:var(--muted);font-family:var(--mono)}

/* terminal */
.term{max-width:860px;margin-inline:auto;border:1px solid var(--border);border-radius:14px;overflow:hidden;background:rgba(5,8,16,.88);box-shadow:0 20px 60px rgba(0,0,0,.5),0 0 40px rgba(0,255,102,.07)}
.term-body{height:300px;overflow-y:auto;padding:18px;font-family:var(--mono);font-size:.85rem;color:#c8f7d8}
.term-body .out{white-space:pre-wrap;margin-bottom:8px}
.term-body .cmd{color:var(--cyan)}
.term-body a{color:var(--cyan);text-decoration:underline}
.term-input{display:flex;gap:10px;border-top:1px solid var(--border);padding:12px 18px;font-family:var(--mono);font-size:.85rem;align-items:center}
.term-input span{color:var(--green)}
.term-input input{flex:1;background:none;border:0;outline:0;color:var(--white);font-family:inherit;font-size:inherit}

/* contact */
.contact-grid{display:grid;grid-template-columns:.9fr 1.1fr;gap:34px}
.info{padding:30px}
.info h3{margin-bottom:8px;font-size:1.3rem}
.info > p{color:var(--muted);margin-bottom:24px}
.info a.row{display:flex;gap:14px;align-items:center;padding:14px;border:1px solid var(--border);border-radius:10px;margin-bottom:12px;transition:.3s;word-break:break-all}
.info a.row:hover{border-color:var(--cyan);background:rgba(0,240,255,.06);transform:translateX(5px)}
.info a.row small{display:block;font-family:var(--mono);color:var(--green);font-size:.7rem}
form.glass{padding:30px}
form.glass:hover{transform:none}
.field{margin-bottom:18px}
.field label{display:block;font-family:var(--mono);font-size:.76rem;color:var(--green);margin-bottom:6px}
.field input,.field textarea{width:100%;background:rgba(5,8,16,.7);border:1px solid var(--border);border-radius:8px;padding:13px 14px;color:var(--white);font-family:var(--sans);font-size:.95rem;transition:.25s;outline:0}
.field input:focus,.field textarea:focus{border-color:var(--cyan);box-shadow:0 0 0 3px rgba(0,240,255,.14)}
.field textarea{min-height:130px;resize:vertical}
.row2{display:grid;grid-template-columns:1fr 1fr;gap:16px}
.hp{position:absolute;left:-9999px}
.status{margin-top:16px;font-family:var(--mono);font-size:.84rem;display:none;padding:12px 14px;border-radius:8px}
.status.ok{display:block;color:var(--green);border:1px solid rgba(0,255,102,.35);background:rgba(0,255,102,.07)}
.status.err{display:block;color:#ff7b7b;border:1px solid rgba(255,90,90,.35);background:rgba(255,90,90,.07)}

footer{position:relative;z-index:2;border-top:1px solid var(--border);padding:34px 0;text-align:center;font-family:var(--mono);font-size:.82rem;color:var(--muted);background:rgba(10,15,29,.8)}
footer .g{color:var(--green)}

/* bg control */
.bgctl{position:fixed;right:18px;bottom:18px;z-index:90;display:flex;gap:10px;align-items:center;padding:9px 14px;border-radius:50px;background:rgba(10,15,29,.85);border:1px solid var(--border);font-family:var(--mono);font-size:.72rem;color:var(--muted);backdrop-filter:blur(10px)}
.bgctl input{width:80px;accent-color:var(--cyan)}

/* reveal */
.reveal{opacity:0;transform:translateY(28px);transition:opacity .8s ease,transform .8s ease;transition-delay:var(--d,0s)}
.reveal.in{opacity:1;transform:none}

@keyframes blink{50%{opacity:0}}
@keyframes pulse{50%{opacity:.35;transform:scale(.8)}}
@keyframes rise{from{opacity:0;transform:translateY(20px)}to{opacity:1;transform:none}}

@media(max-width:900px){
  .hero-grid,.about-grid,.contact-grid{grid-template-columns:1fr}
  .hero-card{display:none}
  .burger{display:block}
  nav ul{position:absolute;top:70px;left:0;right:0;flex-direction:column;gap:0;background:rgba(10,15,29,.97);border-bottom:1px solid var(--border);max-height:0;overflow:hidden;transition:max-height .4s}
  nav ul.open{max-height:420px}
  nav li a{display:block;padding:14px 24px}
  section{padding:76px 0}
}
@media(max-width:600px){
  .skills,.row2,.stats{grid-template-columns:1fr}
  .projects{grid-template-columns:1fr}
  .bgctl{display:none}
}
@media(prefers-reduced-motion:reduce){
  *{animation:none!important;transition:none!important;scroll-behavior:auto!important}
  .reveal{opacity:1;transform:none}
}
</style>
</head>
<body>

<canvas id="matrix" aria-hidden="true"></canvas>
<canvas id="mesh" aria-hidden="true"></canvas>
<div class="vignette"></div>
<div class="cursor-glow" id="glow"></div>

<header id="top">
  <div class="container nav">
    <a href="#home" class="logo" aria-label="Home"><span class="p">&gt;</span> Joseph_Justine.sh<span class="caret"></span></a>
    <button class="burger" id="burger" aria-label="Toggle menu">&#9776;</button>
    <nav>
      <ul id="menu">
        <li><a href="#about">About</a></li>
        <li><a href="#expertise">Expertise</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#experience">Experience</a></li>
        <li><a href="#certifications">Certifications</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </div>
</header>

<main id="home">
<!-- HERO -->
<section class="hero">
  <div class="container hero-grid">
    <div>
      <div class="tag reveal"><i></i> Available for new projects</div>
      <h1 class="reveal" style="--d:.1s">Hi, I'm <span class="name">Joseph Sandeep Justine</span></h1>
      <div class="typing reveal" style="--d:.2s">&gt; <span id="typed"></span><span class="cursor"></span></div>
      <p class="bio reveal" style="--d:.3s">Bridging the gap between robust software engineering, ironclad cloud security, scalable DevOps infrastructure, and intelligent AI solutions.</p>
      <div class="actions reveal" style="--d:.4s">
        <a href="#projects" class="btn primary">Explore Projects &rarr;</a>
        <a href="resume.pdf" class="btn outline" download>Download Resume &darr;</a>
      </div>
      <div class="socials reveal" style="--d:.5s">
        <a href="https://mw.linkedin.com/in/josephjustine" target="_blank" rel="noopener" aria-label="LinkedIn"><svg viewBox="0 0 24 24"><path d="M4.98 3.5a2.5 2.5 0 1 1 0 5 2.5 2.5 0 0 1 0-5zM3 9.75h4V21H3zM9.5 9.75h3.8v1.6h.06c.53-1 1.82-2.05 3.75-2.05 4 0 4.74 2.63 4.74 6.05V21h-4v-4.9c0-1.17-.02-2.67-1.63-2.67-1.63 0-1.88 1.27-1.88 2.58V21h-4z"/></svg></a>
        <a href="https://github.com/SandeepJustine" target="_blank" rel="noopener" aria-label="GitHub"><svg viewBox="0 0 24 24"><path d="M12 .5a11.5 11.5 0 0 0-3.64 22.41c.58.1.79-.25.79-.56v-2c-3.2.7-3.88-1.37-3.88-1.37-.52-1.33-1.28-1.69-1.28-1.69-1.04-.71.08-.7.08-.7 1.15.08 1.76 1.19 1.76 1.19 1.03 1.76 2.7 1.25 3.36.96.1-.75.4-1.25.73-1.54-2.55-.29-5.24-1.28-5.24-5.69 0-1.26.45-2.28 1.19-3.09-.12-.29-.52-1.46.11-3.05 0 0 .97-.31 3.17 1.18a11 11 0 0 1 5.77 0c2.2-1.49 3.16-1.18 3.16-1.18.63 1.59.23 2.76.11 3.05.74.81 1.19 1.83 1.19 3.09 0 4.42-2.69 5.39-5.25 5.68.41.36.78 1.06.78 2.14v3.17c0 .31.21.67.8.56A11.5 11.5 0 0 0 12 .5z"/></svg></a>
        <a href="mailto:josephjustne284@gmail.com" aria-label="Email"><svg viewBox="0 0 24 24"><path d="M2 5h20v14H2zm2 2v.5l8 5 8-5V7zm16 3-8 5-8-5V17h16z"/></svg></a>
      </div>
    </div>
    <div class="hero-card reveal" style="--d:.4s">
      <div class="bar"><span></span><span></span><span></span><em>whoami.json</em></div>
      <div class="code">
<span class="c">// system profile</span><br>
<span class="k">const</span> joseph = {<br>
&nbsp;&nbsp;role: <span class="s">"Full Stack Developer"</span>,<br>
&nbsp;&nbsp;focus: [<span class="s">"Security"</span>, <span class="s">"DevOps"</span>, <span class="s">"AI"</span>],<br>
&nbsp;&nbsp;degree: <span class="s">"Information Systems"</span>,<br>
&nbsp;&nbsp;certified: <span class="s">"ISO 27001"</span>,<br>
&nbsp;&nbsp;base: <span class="s">"Malawi"</span>,<br>
&nbsp;&nbsp;status: <span class="s">"building"</span><br>
};
      </div>
    </div>
  </div>
</section>

<!-- ABOUT -->
<section id="about">
  <div class="container">
    <div class="sec-head reveal"><div class="eyebrow">// 01. about</div><h2>About Me</h2></div>
    <div class="about-grid">
      <div class="about-text reveal">
        <p>I'm an <strong>Information Systems graduate</strong> and a versatile technical leader who designs, builds, secures and runs the systems businesses depend on.</p>
        <p>My work spans <strong>full stack development</strong>, <strong>cyber security and compliance</strong>, <strong>DevOps and server management</strong>, and <strong>AI consulting</strong>. I like turning messy manual processes into reliable, automated and well-protected platforms.</p>
        <p>I focus on practical, high-impact technology for organisations and entrepreneurs, with a strong interest in building digital solutions that work for the Malawian and wider African market.</p>
        <div class="stats">
          <div class="glass stat"><b data-count="4">0</b><span>Core disciplines</span></div>
          <div class="glass stat"><b data-count="5">0</b><span>Credentials</span></div>
          <div class="glass stat"><b data-count="24">0</b><span>/7 uptime mindset</span></div>
        </div>
      </div>
      <div class="skills" id="expertise">
        <div class="glass skill-box reveal" style="--d:.05s">
          <h3><span class="ico">&lt;/&gt;</span>Development</h3>
          <div class="badges"><span class="badge">Mobile Apps</span><span class="badge">Websites</span><span class="badge">Enterprise Systems</span><span class="badge">Full Stack Architecture</span></div>
        </div>
        <div class="glass skill-box reveal" style="--d:.15s">
          <h3><span class="ico">&#9919;</span>Security &amp; Compliance</h3>
          <div class="badges"><span class="badge">Cyber Security Analysis</span><span class="badge">IBM Cybersecurity Analyst</span><span class="badge">ISO 27001</span><span class="badge">Acronis Cloud Cyber Security</span></div>
        </div>
        <div class="glass skill-box reveal" style="--d:.25s">
          <h3><span class="ico">#</span>Infrastructure &amp; Data</h3>
          <div class="badges"><span class="badge">Server Management</span><span class="badge">Database Management</span><span class="badge">DevOps</span><span class="badge">CI/CD Pipelines</span></div>
        </div>
        <div class="glass skill-box reveal" style="--d:.35s">
          <h3><span class="ico">AI</span>AI &amp; Operations</h3>
          <div class="badges"><span class="badge">AI Consulting</span><span class="badge">Workflow Automation</span><span class="badge">Certified Virtual Assistance</span></div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- PROJECTS -->
<section id="projects">
  <div class="container">
    <div class="sec-head reveal"><div class="eyebrow">// 02. projects</div><h2>Featured Work</h2></div>
    <div class="tabs reveal" role="tablist">
      <button class="tab active" data-f="all">All</button>
      <button class="tab" data-f="fullstack">Full Stack</button>
      <button class="tab" data-f="security">Cyber Security</button>
      <button class="tab" data-f="devops">DevOps</button>
      <button class="tab" data-f="database">Database</button>
      <button class="tab" data-f="ai">AI Consultant</button>
    </div>
    <div class="projects" id="grid">

      <article class="glass card" data-c="fullstack">
        <div class="cat">Full Stack Development</div>
        <h3>Nexus Enterprise Suite</h3>
        <p>A modular enterprise platform covering inventory, billing, HR and reporting, with role-based access and a responsive web dashboard for day-to-day operations.</p>
        <div class="tech"><span>Laravel</span><span>Node.js</span><span>TypeScript</span><span>MySQL</span><span>REST API</span></div>
        <ul class="metrics"><li>Consolidated multiple manual workflows into one system</li><li>Role-based access across departments</li><li>Real-time dashboards and exportable reports</li></ul>
        <a class="btn outline" href="https://github.com/SandeepJustine" target="_blank" rel="noopener">View Repository &#8599;</a>
      </article>

      <article class="glass card" data-c="fullstack">
        <div class="cat">Full Stack Development</div>
        <h3>Nexus Mobile App</h3>
        <p>Cross-platform companion app that gives staff and customers secure, on-the-go access to the Nexus platform, including push notifications and offline-friendly screens.</p>
        <div class="tech"><span>Flutter</span><span>React Native</span><span>REST API</span><span>JWT</span></div>
        <ul class="metrics"><li>Single codebase for Android and iOS</li><li>Token-based secure authentication</li><li>Optimised for low-bandwidth networks</li></ul>
        <a class="btn outline" href="https://github.com/SandeepJustine" target="_blank" rel="noopener">View Repository &#8599;</a>
      </article>

      <article class="glass card" data-c="security">
        <div class="cat">Cyber Security &amp; Compliance</div>
        <h3>ISO 27001 &amp; IBM Security Framework</h3>
        <p>Security programme blending ISO/IEC 27001 controls with IBM cybersecurity practices: risk assessment, policy development, gap analysis, vulnerability review and incident response planning.</p>
        <div class="tech"><span>ISO 27001</span><span>Risk Assessment</span><span>SIEM Concepts</span><span>Policy &amp; Audit</span></div>
        <ul class="metrics"><li>Documented risk register and treatment plan</li><li>Control mapping to Annex A</li><li>Staff awareness and incident playbooks</li></ul>
        <a class="btn outline" href="https://github.com/SandeepJustine" target="_blank" rel="noopener">View Repository &#8599;</a>
      </article>

      <article class="glass card" data-c="devops">
        <div class="cat">DevOps &amp; Server Management</div>
        <h3>CI/CD Pipelines</h3>
        <p>Automated build, test and deploy pipelines using containers and self-hosted platforms, with zero-downtime releases, environment separation and one-click rollbacks.</p>
        <div class="tech"><span>Docker</span><span>Coolify</span><span>GitHub Actions</span><span>Linux</span><span>Nginx</span></div>
        <ul class="metrics"><li>Push-to-deploy workflow for web apps</li><li>Automatic SSL and reverse proxying</li><li>Repeatable, version-controlled environments</li></ul>
        <a class="btn outline" href="https://github.com/SandeepJustine" target="_blank" rel="noopener">View Repository &#8599;</a>
      </article>

      <article class="glass card" data-c="devops security">
        <div class="cat">DevOps &amp; Server Management</div>
        <h3>Acronis Backup Automation</h3>
        <p>Scheduled, monitored cloud backup and recovery for servers and endpoints using Acronis Cloud Cyber Protect, with retention policies and tested restore procedures.</p>
        <div class="tech"><span>Acronis</span><span>Backup Policies</span><span>Disaster Recovery</span><span>Monitoring</span></div>
        <ul class="metrics"><li>Automated daily backup schedules</li><li>Regular restore testing and reporting</li><li>Reduced recovery time for critical systems</li></ul>
        <a class="btn outline" href="https://github.com/SandeepJustine" target="_blank" rel="noopener">View Repository &#8599;</a>
      </article>

      <article class="glass card" data-c="database">
        <div class="cat">Database Management</div>
        <h3>High-Performance Relational DB Optimization</h3>
        <p>Schema redesign, indexing strategy, query tuning and backup planning for busy relational databases, improving response times and data integrity.</p>
        <div class="tech"><span>MySQL</span><span>PostgreSQL</span><span>Indexing</span><span>Query Tuning</span><span>Replication</span></div>
        <ul class="metrics"><li>Slow queries profiled and rewritten</li><li>Normalised schemas with integrity constraints</li><li>Automated backups with point-in-time recovery</li></ul>
        <a class="btn outline" href="https://github.com/SandeepJustine" target="_blank" rel="noopener">View Repository &#8599;</a>
      </article>

      <article class="glass card" data-c="ai">
        <div class="cat">AI Consultant</div>
        <h3>Intelligent Workflow Automation</h3>
        <p>Automations that remove repetitive admin work: intake, triage, reporting and follow-ups, connecting business tools through APIs and AI-assisted decision steps.</p>
        <div class="tech"><span>Python</span><span>n8n / Zapier</span><span>Webhooks</span><span>WhatsApp API</span></div>
        <ul class="metrics"><li>Hours of manual work saved each week</li><li>Human-in-the-loop approval steps</li><li>Audit trail for every automated action</li></ul>
        <a class="btn outline" href="https://github.com/SandeepJustine" target="_blank" rel="noopener">View Repository &#8599;</a>
      </article>

      <article class="glass card" data-c="ai">
        <div class="cat">AI Consultant</div>
        <h3>LLM Integration Suite</h3>
        <p>Reusable toolkit to embed large language models into business apps: chat assistants, document Q&amp;A with retrieval, summarisation and guardrails for safe use.</p>
        <div class="tech"><span>LLM APIs</span><span>RAG</span><span>Python</span><span>TypeScript</span><span>Vector DB</span></div>
        <ul class="metrics"><li>Retrieval over private company documents</li><li>Prompt and output safety guardrails</li><li>Plug-in connectors for existing systems</li></ul>
        <a class="btn outline" href="https://github.com/SandeepJustine" target="_blank" rel="noopener">View Repository &#8599;</a>
      </article>

    </div>
  </div>
</section>

<!-- EXPERIENCE -->
<section id="experience">
  <div class="container">
    <div class="sec-head reveal"><div class="eyebrow">// 03. experience</div><h2>Experience</h2></div>
    <div class="timeline">
      <div class="glass job reveal">
        <div class="when">PRESENT</div>
        <h3>Technical Lead</h3>
        <div class="org">Cool Enterprises Limited &middot; Digital Assurance &amp; Compliance Practice</div>
        <ul><li>Lead technical delivery of enterprise systems, compliance and digital assurance engagements</li><li>Oversee infrastructure, deployments and software development teams</li></ul>
      </div>
      <div class="glass job reveal" style="--d:.1s">
        <div class="when">PRESENT</div>
        <h3>Tech &amp; Enterprise Systems Lead</h3>
        <div class="org">Tech265 Limited</div>
        <ul><li>Manage platform infrastructure and enterprise systems for Malawi-focused clients</li><li>Drive product development across web, mobile and messaging platforms</li></ul>
      </div>
      <div class="glass job reveal" style="--d:.2s">
        <div class="when">EDUCATION</div>
        <h3>BSc Management Information Systems</h3>
        <div class="org">Malawi University of Business and Applied Sciences (MUBAS)</div>
        <ul><li>Foundation in systems analysis, databases, software engineering and IT management</li></ul>
      </div>
    </div>
  </div>
</section>

<!-- CERTS -->
<section id="certifications">
  <div class="container">
    <div class="sec-head reveal"><div class="eyebrow">// 04. credentials</div><h2>Certifications</h2></div>
    <div class="certs">
      <div class="glass cert reveal"><div class="seal">IBM</div><h3>IBM Cybersecurity Analyst Certificate</h3><p>verified_credential</p></div>
      <div class="glass cert reveal" style="--d:.08s"><div class="seal">ISO</div><h3>ISO 27001 Certified Professional</h3><p>information_security</p></div>
      <div class="glass cert reveal" style="--d:.16s"><div class="seal">ACR</div><h3>Acronis Cloud Cyber Security Certified</h3><p>cloud_protection</p></div>
      <div class="glass cert reveal" style="--d:.24s"><div class="seal">CVA</div><h3>Certified Virtual Assistant</h3><p>remote_operations</p></div>
      <div class="glass cert reveal" style="--d:.32s"><div class="seal">BSc</div><h3>Information Systems Degree Graduate</h3><p>MUBAS</p></div>
    </div>
  </div>
</section>

<!-- TERMINAL -->
<section id="terminal">
  <div class="container">
    <div class="sec-head reveal"><div class="eyebrow">// 05. easter_egg</div><h2>Interactive Terminal</h2></div>
    <div class="term reveal">
      <div class="bar"><span></span><span></span><span></span><em>guest@joseph:~</em></div>
      <div class="term-body" id="tbody"></div>
      <div class="term-input"><span>guest@joseph:~$</span><input id="tin" type="text" autocomplete="off" spellcheck="false" aria-label="Terminal input" placeholder="type 'help'"></div>
    </div>
  </div>
</section>

<!-- CONTACT -->
<section id="contact">
  <div class="container">
    <div class="sec-head reveal"><div class="eyebrow">// 06. contact</div><h2>Get In Touch</h2></div>
    <div class="contact-grid">
      <div class="glass info reveal">
        <h3>Let's build something secure &amp; smart.</h3>
        <p>Have a project, a security review or an automation idea? Send a transmission and I'll get back to you.</p>
        <a class="row" href="mailto:josephjustne284@gmail.com"><div><small>EMAIL</small>josephjustne284@gmail.com</div></a>
        <a class="row" href="https://mw.linkedin.com/in/josephjustine" target="_blank" rel="noopener"><div><small>LINKEDIN</small>mw.linkedin.com/in/josephjustine</div></a>
        <a class="row" href="https://github.com/SandeepJustine" target="_blank" rel="noopener"><div><small>GITHUB</small>github.com/SandeepJustine</div></a>
      </div>
      <form class="glass reveal" id="form" style="--d:.1s" novalidate>
        <div class="row2">
          <div class="field"><label for="n">&gt; NAME</label><input id="n" name="name" required placeholder="Your name"></div>
          <div class="field"><label for="e">&gt; EMAIL</label><input id="e" name="email" type="email" required placeholder="you@example.com"></div>
        </div>
        <div class="field"><label for="s">&gt; SUBJECT</label><input id="s" name="subject" required placeholder="Project inquiry"></div>
        <div class="field"><label for="m">&gt; MESSAGE</label><textarea id="m" name="message" required placeholder="Tell me about your project..."></textarea></div>
        <input class="hp" type="text" name="_gotcha" tabindex="-1" autocomplete="off" aria-hidden="true">
        <button type="submit" class="btn primary" id="send">Send Transmission &rarr;</button>
        <div class="status" id="status" role="status"></div>
      </form>
    </div>
  </div>
</section>
</main>

<footer>
  <div class="container"><span class="g">&copy; 2026 Joseph Sandeep Justine.</span> Compiled successfully.</div>
</footer>

<div class="bgctl"><label for="op">data stream</label><input type="range" id="op" min="0" max="100" value="35"></div>

<script>
/* ============ CONFIG (edit these) ============ */
const CONFIG = {
  email: "josephjustne284@gmail.com",
  // Optional: paste a Formspree / Web3Forms / Getform endpoint to send form messages directly.
  // e.g. "https://formspree.io/f/xxxxxxx". If empty, the form opens the visitor's email app instead.
  formEndpoint: "",
  titles: ["Full Stack Developer","Cyber Security Analyst","DevOps & Server Manager","AI Consultant"]
};

const reduce = matchMedia('(prefers-reduced-motion: reduce)').matches;
const $ = s => document.querySelector(s);

/* ---------- header / menu ---------- */
const header = $('#top'), menu = $('#menu');
addEventListener('scroll', () => header.classList.toggle('scrolled', scrollY > 30), {passive:true});
$('#burger').onclick = () => menu.classList.toggle('open');
menu.querySelectorAll('a').forEach(a => a.onclick = () => menu.classList.remove('open'));
const links = [...menu.querySelectorAll('a')];
const secs = links.map(a => document.querySelector(a.getAttribute('href')));
addEventListener('scroll', () => {
  let cur = -1; secs.forEach((s,i) => { if (s && s.getBoundingClientRect().top < 160) cur = i; });
  links.forEach((a,i) => a.classList.toggle('active', i === cur));
}, {passive:true});

/* ---------- typewriter ---------- */
(function(){
  const el = $('#typed'); let t = 0, c = 0, del = false;
  if (reduce) { el.textContent = CONFIG.titles[0]; return; }
  (function tick(){
    const w = CONFIG.titles[t];
    el.textContent = w.slice(0, c);
    if (!del && c === w.length) { del = true; return setTimeout(tick, 1600); }
    if (del && c === 0) { del = false; t = (t+1) % CONFIG.titles.length; }
    c += del ? -1 : 1;
    setTimeout(tick, del ? 35 : 75);
  })();
})();

/* ---------- matrix binary rain ---------- */
const mc = $('#matrix'), mx = mc.getContext('2d');
let mOpacity = .35, drops = [], fs = 16;
function sizeMatrix(){
  mc.width = innerWidth; mc.height = innerHeight;
  drops = Array.from({length: Math.ceil(mc.width / fs)}, () => Math.random() * -50);
}
sizeMatrix(); addEventListener('resize', sizeMatrix);
$('#op').oninput = e => { mOpacity = e.target.value / 100; mc.style.opacity = mOpacity; };
mc.style.opacity = mOpacity;
let last = 0;
function rain(ts){
  if (ts - last > 60) {
    last = ts;
    mx.fillStyle = 'rgba(10,15,29,.14)'; mx.fillRect(0,0,mc.width,mc.height);
    mx.font = fs + 'px "JetBrains Mono",monospace';
    drops.forEach((y,i) => {
      const ch = Math.random() > .5 ? '1' : '0';
      mx.fillStyle = Math.random() > .93 ? '#00f0ff' : '#00ff66';
      mx.fillText(ch, i * fs, y * fs);
      drops[i] = (y * fs > mc.height && Math.random() > .975) ? 0 : y + 1;
    });
  }
  requestAnimationFrame(rain);
}
if (!reduce) requestAnimationFrame(rain);

/* ---------- particle mesh + cursor glow ---------- */
const pc = $('#mesh'), px = pc.getContext('2d'), glow = $('#glow');
let pts = [], mouse = {x:-999,y:-999};
function sizeMesh(){
  pc.width = innerWidth; pc.height = innerHeight;
  const n = Math.min(90, Math.floor(innerWidth * innerHeight / 18000));
  pts = Array.from({length:n}, () => ({x:Math.random()*pc.width,y:Math.random()*pc.height,vx:(Math.random()-.5)*.4,vy:(Math.random()-.5)*.4}));
}
sizeMesh(); addEventListener('resize', sizeMesh);
addEventListener('pointermove', e => { mouse.x = e.clientX; mouse.y = e.clientY; glow.style.left = e.clientX + 'px'; glow.style.top = e.clientY + 'px'; }, {passive:true});
function mesh(){
  px.clearRect(0,0,pc.width,pc.height);
  for (let i = 0; i < pts.length; i++){
    const p = pts[i];
    p.x += p.vx; p.y += p.vy;
    if (p.x < 0 || p.x > pc.width) p.vx *= -1;
    if (p.y < 0 || p.y > pc.height) p.vy *= -1;
    px.beginPath(); px.arc(p.x,p.y,1.6,0,6.283); px.fillStyle = 'rgba(0,240,255,.7)'; px.fill();
    for (let j = i + 1; j < pts.length; j++){
      const q = pts[j], d = Math.hypot(p.x-q.x, p.y-q.y);
      if (d < 130){ px.strokeStyle = `rgba(0,240,255,${(1-d/130)*.22})`; px.lineWidth = 1; px.beginPath(); px.moveTo(p.x,p.y); px.lineTo(q.x,q.y); px.stroke(); }
    }
    const dm = Math.hypot(p.x-mouse.x, p.y-mouse.y);
    if (dm < 170){ px.strokeStyle = `rgba(0,255,102,${(1-dm/170)*.5})`; px.beginPath(); px.moveTo(p.x,p.y); px.lineTo(mouse.x,mouse.y); px.stroke(); }
  }
  requestAnimationFrame(mesh);
}
if (!reduce) requestAnimationFrame(mesh);

/* ---------- reveal on scroll + counters ---------- */
const io = new IntersectionObserver(es => es.forEach(e => {
  if (e.isIntersecting){
    e.target.classList.add('in');
    e.target.querySelectorAll('[data-count]').forEach(count);
    io.unobserve(e.target);
  }
}), {threshold:.12});
document.querySelectorAll('.reveal').forEach(el => io.observe(el));
function count(el){
  const to = +el.dataset.count; let n = 0;
  const step = () => { n += Math.max(1, to/30); if (n >= to){ el.textContent = to; return; } el.textContent = Math.floor(n); requestAnimationFrame(step); };
  step();
}

/* ---------- project tabs ---------- */
const tabs = document.querySelectorAll('.tab'), cards = document.querySelectorAll('.card');
tabs.forEach(t => t.onclick = () => {
  tabs.forEach(x => x.classList.remove('active')); t.classList.add('active');
  const f = t.dataset.f; let i = 0;
  cards.forEach(c => {
    const show = f === 'all' || c.dataset.c.split(' ').includes(f);
    c.classList.toggle('hide', !show);
    if (show){ c.style.animation = 'none'; void c.offsetWidth; c.style.animation = `rise .5s ${(i++)*.07}s both`; }
  });
});

/* ---------- terminal ---------- */
const tb = $('#tbody'), ti = $('#tin'), hist = []; let hi = 0;
function out(html, cls=''){ const d = document.createElement('div'); d.className = 'out ' + cls; d.innerHTML = html; tb.appendChild(d); tb.scrollTop = tb.scrollHeight; }
const cmds = {
  help: () => 'Available commands:\n  bio        who I am\n  skills     what I do\n  projects   what I build\n  certs      credentials\n  contact    reach me\n  theme      toggle data stream\n  clear      clear the screen',
  bio: () => 'Joseph Sandeep Justine\nInformation Systems graduate, full stack developer, cyber security analyst,\nDevOps engineer and AI consultant. Based in Malawi.',
  skills: () => '[Development]  Mobile Apps | Websites | Enterprise Systems | Full Stack\n[Security]     Cyber Security | IBM Analyst | ISO 27001 | Acronis\n[Infra/Data]   Servers | Databases | DevOps | CI/CD\n[AI/Ops]       AI Consulting | Automation | Virtual Assistance',
  projects: () => '1. Nexus Enterprise Suite & Mobile App\n2. ISO 27001 & IBM Security Framework\n3. CI/CD Pipelines & Acronis Backup Automation\n4. Relational DB Optimization\n5. Workflow Automation & LLM Integration Suite',
  certs: () => '- IBM Cybersecurity Analyst Certificate\n- ISO 27001 Certified Professional\n- Acronis Cloud Cyber Security Certified\n- Certified Virtual Assistant\n- Information Systems Degree',
  contact: () => `Email:    <a href="mailto:${CONFIG.email}">${CONFIG.email}</a>\nLinkedIn: <a href="https://mw.linkedin.com/in/josephjustine" target="_blank" rel="noopener">mw.linkedin.com/in/josephjustine</a>\nGitHub:   <a href="https://github.com/SandeepJustine" target="_blank" rel="noopener">github.com/SandeepJustine</a>`,
  theme: () => { const r = $('#op'); r.value = +r.value > 0 ? 0 : 35; r.dispatchEvent(new Event('input')); return 'data stream ' + (+r.value ? 'on' : 'off'); },
  whoami: () => 'guest', sudo: () => 'Nice try. Permission denied.', ls: () => 'about  projects  experience  certifications  contact',
  clear: () => { tb.innerHTML = ''; return null; }
};
out('Welcome. Type <span class="cmd">help</span> to see commands.');
ti.addEventListener('keydown', e => {
  if (e.key === 'Enter'){
    const v = ti.value.trim(); ti.value = ''; if (!v) return;
    hist.push(v); hi = hist.length;
    const esc = v.replace(/</g,'&lt;');
    out(`<span class="cmd">$ ${esc}</span>`);
    const f = cmds[v.toLowerCase()];
    const r = f ? f() : `command not found: ${esc}. Type 'help'.`;
    if (r) out(r);
  } else if (e.key === 'ArrowUp'){ if (hi > 0) ti.value = hist[--hi]; e.preventDefault(); }
  else if (e.key === 'ArrowDown'){ ti.value = hi < hist.length - 1 ? hist[++hi] : (hi = hist.length, ''); }
});

/* ---------- contact form ---------- */
const form = $('#form'), st = $('#status'), btn = $('#send');
function say(msg, ok){ st.className = 'status ' + (ok ? 'ok' : 'err'); st.textContent = msg; }
form.addEventListener('submit', async e => {
  e.preventDefault();
  const d = Object.fromEntries(new FormData(form));
  if (d._gotcha) return;
  if (!d.name.trim() || !/^\S+@\S+\.\S+$/.test(d.email) || !d.subject.trim() || !d.message.trim()) return say('> ERROR: please complete all fields with a valid email.', false);
  btn.disabled = true; btn.textContent = 'Transmitting...';
  try {
    if (CONFIG.formEndpoint){
      const r = await fetch(CONFIG.formEndpoint, {method:'POST', headers:{'Accept':'application/json','Content-Type':'application/json'}, body:JSON.stringify(d)});
      if (!r.ok) throw new Error('bad response');
      say('> SUCCESS: transmission received. I will respond shortly.', true); form.reset();
    } else {
      const body = encodeURIComponent(`${d.message}\n\n— ${d.name} (${d.email})`);
      location.href = `mailto:${CONFIG.email}?subject=${encodeURIComponent(d.subject)}&body=${body}`;
      say('> Opening your email app to send the message...', true);
    }
  } catch(err){ say('> ERROR: transmission failed. Please email me directly.', false); }
  btn.disabled = false; btn.innerHTML = 'Send Transmission &rarr;';
});
</script>
</body>
</html>
