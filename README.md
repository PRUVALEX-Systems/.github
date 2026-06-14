<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width,initial-scale=1.0"/>
<title>PRUVALEX — Enterprise AI Compliance OS & Zero-Cost Developer Tools</title>
<meta name="description" content="Mathematically provable AI compliance architectures and zero-cost developer tools. PruvaGraph reduces LLM costs by 99%+."/>
<meta property="og:title" content="PRUVALEX — Enterprise AI Compliance OS"/>
<meta property="og:description" content="99%+ LLM cost reduction. EU AI Act compliance. Built for developers who love Claude Code but not the bill."/>
<meta name="theme-color" content="#050510"/>
<link rel="preconnect" href="https://fonts.googleapis.com"/>
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin/>
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;400;500;600;700&family=JetBrains+Mono:wght@400;500;700&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet"/>
<style>
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
:root{
--bg:#050510;
--bg2:#0B0B1F;
--bg3:#12122A;
--bg4:#1A1A35;
--border:rgba(255,255,255,0.07);
--border2:rgba(255,255,255,0.14);
--text1:#F0F0FA;
--text2:#9090B8;
--text3:#5A5A80;
--indigo:#5B5BFF;
--indigo-dim:rgba(91,91,255,0.12);
--indigo-glow:rgba(91,91,255,0.25);
--green:#00E57A;
--green-dim:rgba(0,229,122,0.1);
--red:#FF3355;
--red-dim:rgba(255,51,85,0.1);
--yellow:#FFD166;
--radius:10px;
--radius-lg:16px;
}
html{scroll-behavior:smooth}
body{background:var(--bg);color:var(--text1);font-family:'Inter',sans-serif;font-size:16px;line-height:1.6;overflow-x:hidden}

/* NAV */
nav{position:fixed;top:0;left:0;right:0;z-index:100;padding:0 2rem;height:64px;display:flex;align-items:center;justify-content:space-between;border-bottom:1px solid transparent;transition:background 0.3s,border-color 0.3s;backdrop-filter:blur(0px)}
nav.scrolled{background:rgba(5,5,16,0.92);border-color:var(--border);backdrop-filter:blur(20px)}
.nav-logo{display:flex;align-items:center;gap:10px;text-decoration:none}
.nav-logo-icon{width:34px;height:34px;background:var(--indigo);border-radius:8px;display:flex;align-items:center;justify-content:center;font-family:'Space Grotesk',sans-serif;font-weight:700;font-size:16px;color:#fff;letter-spacing:-0.5px}
.nav-logo-text{font-family:'Space Grotesk',sans-serif;font-weight:600;font-size:16px;color:var(--text1);letter-spacing:0.02em}
.nav-links{display:flex;align-items:center;gap:1.5rem}
.nav-links a{color:var(--text2);text-decoration:none;font-size:14px;font-weight:500;transition:color 0.2s}
.nav-links a:hover{color:var(--text1)}
.nav-cta{background:var(--indigo);color:#fff;padding:8px 18px;border-radius:8px;font-size:14px;font-weight:600;text-decoration:none;transition:opacity 0.2s}
.nav-cta:hover{opacity:0.85}

/* HERO */
.hero{position:relative;min-height:100vh;display:flex;align-items:center;justify-content:center;overflow:hidden;padding:120px 2rem 80px}
#hero-canvas{position:absolute;inset:0;opacity:0.35}
.hero-inner{position:relative;z-index:2;max-width:900px;margin:0 auto;text-align:center}
.hero-badge{display:inline-flex;align-items:center;gap:8px;background:var(--indigo-dim);border:1px solid rgba(91,91,255,0.3);border-radius:100px;padding:6px 16px;font-size:13px;font-weight:500;color:var(--indigo);margin-bottom:2rem;font-family:'Space Grotesk',sans-serif;letter-spacing:0.04em}
.hero-badge-dot{width:6px;height:6px;background:var(--green);border-radius:50%;animation:pulse 2s infinite}
@keyframes pulse{0%,100%{opacity:1;transform:scale(1)}50%{opacity:0.5;transform:scale(0.85)}}
.hero h1{font-family:'Space Grotesk',sans-serif;font-size:clamp(2.6rem,6vw,5rem);font-weight:700;line-height:1.08;letter-spacing:-0.03em;color:var(--text1);margin-bottom:1.5rem}
.hero h1 span.accent{color:var(--indigo)}
.hero h1 span.accent-green{color:var(--green)}
.hero-sub{font-size:clamp(1rem,2vw,1.2rem);color:var(--text2);max-width:640px;margin:0 auto 2.5rem;font-weight:400;line-height:1.7}
.hero-savings{display:flex;align-items:center;justify-content:center;gap:1.5rem;margin-bottom:3rem;flex-wrap:wrap}
.savings-box{background:var(--bg3);border:1px solid var(--border2);border-radius:var(--radius-lg);padding:1.25rem 2rem;text-align:center}
.savings-box .label{font-size:12px;color:var(--text3);text-transform:uppercase;letter-spacing:0.1em;font-weight:600;margin-bottom:4px}
.savings-box .val{font-family:'Space Grotesk',sans-serif;font-size:2rem;font-weight:700;color:var(--red)}
.savings-box .val.green{color:var(--green)}
.savings-arrow{font-size:1.5rem;color:var(--text3)}
.savings-tag{background:var(--green-dim);border:1px solid rgba(0,229,122,0.25);border-radius:8px;padding:0.5rem 1rem;font-family:'Space Grotesk',sans-serif;font-size:1.4rem;font-weight:700;color:var(--green)}
.hero-btns{display:flex;gap:1rem;justify-content:center;flex-wrap:wrap}
.btn-primary{background:var(--indigo);color:#fff;padding:14px 28px;border-radius:10px;font-size:15px;font-weight:600;text-decoration:none;transition:transform 0.2s,opacity 0.2s;font-family:'Space Grotesk',sans-serif}
.btn-primary:hover{transform:translateY(-1px);opacity:0.9}
.btn-ghost{background:transparent;color:var(--text1);padding:13px 28px;border-radius:10px;font-size:15px;font-weight:600;text-decoration:none;border:1px solid var(--border2);transition:background 0.2s,border-color 0.2s;font-family:'Space Grotesk',sans-serif}
.btn-ghost:hover{background:var(--bg3);border-color:var(--border2)}

/* STATS STRIP */
.stats-strip{background:var(--bg2);border-top:1px solid var(--border);border-bottom:1px solid var(--border);padding:1.25rem 2rem}
.stats-inner{max-width:1100px;margin:0 auto;display:flex;align-items:center;justify-content:space-around;gap:1.5rem;flex-wrap:wrap}
.stat-item{text-align:center}
.stat-item .n{font-family:'Space Grotesk',sans-serif;font-size:1.75rem;font-weight:700;color:var(--text1)}
.stat-item .n .unit{font-size:1rem;color:var(--text2)}
.stat-item .d{font-size:12px;color:var(--text3);text-transform:uppercase;letter-spacing:0.08em;font-weight:600;margin-top:2px}
.stat-divider{width:1px;height:40px;background:var(--border);display:none}
@media(min-width:600px){.stat-divider{display:block}}

/* SECTION COMMON */
section{padding:6rem 2rem}
.section-inner{max-width:1100px;margin:0 auto}
.eyebrow{font-family:'Space Grotesk',sans-serif;font-size:12px;font-weight:700;letter-spacing:0.12em;text-transform:uppercase;color:var(--indigo);margin-bottom:0.75rem}
.section-title{font-family:'Space Grotesk',sans-serif;font-size:clamp(1.8rem,4vw,2.8rem);font-weight:700;line-height:1.15;letter-spacing:-0.025em;color:var(--text1);margin-bottom:1rem}
.section-sub{font-size:1.05rem;color:var(--text2);max-width:600px;line-height:1.7}

/* COMPARE TABLE */
.compare-wrap{overflow-x:auto;margin-top:3rem}
table.compare{width:100%;border-collapse:collapse;font-size:15px}
table.compare th{font-family:'Space Grotesk',sans-serif;font-weight:600;font-size:13px;padding:12px 20px;text-align:left;border-bottom:1px solid var(--border2)}
table.compare th:first-child{color:var(--text2)}
table.compare th.h-other{color:var(--text2)}
table.compare th.h-pruva{color:var(--green);background:var(--green-dim);border-radius:8px 8px 0 0}
table.compare td{padding:14px 20px;border-bottom:1px solid var(--border);font-size:14px}
table.compare td:first-child{color:var(--text2);font-weight:500}
table.compare td.bad{color:var(--red)}
table.compare td.good{color:var(--green)}
table.compare tr:hover td{background:var(--bg2)}

/* LAYERS */
.layers-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:1.5rem;margin-top:3rem}
.layer-card{background:var(--bg2);border:1px solid var(--border);border-radius:var(--radius-lg);padding:1.75rem;transition:border-color 0.2s,transform 0.2s;position:relative;overflow:hidden}
.layer-card::before{content:'';position:absolute;top:0;left:0;right:0;height:2px;background:var(--indigo);opacity:0;transition:opacity 0.2s}
.layer-card:hover{border-color:var(--border2);transform:translateY(-2px)}
.layer-card:hover::before{opacity:1}
.layer-num{font-family:'JetBrains Mono',monospace;font-size:11px;font-weight:700;color:var(--indigo);letter-spacing:0.08em;text-transform:uppercase;margin-bottom:0.75rem}
.layer-title{font-family:'Space Grotesk',sans-serif;font-size:1.05rem;font-weight:600;color:var(--text1);margin-bottom:0.5rem}
.layer-desc{font-size:14px;color:var(--text2);line-height:1.65}
.layer-saving{display:inline-flex;align-items:center;gap:6px;background:var(--green-dim);border:1px solid rgba(0,229,122,0.2);border-radius:6px;padding:4px 10px;font-size:12px;font-weight:700;color:var(--green);font-family:'Space Grotesk',sans-serif;margin-top:1rem;letter-spacing:0.03em}

/* PIPELINE */
.pipeline{margin-top:3rem;display:flex;flex-direction:column;gap:0}
.pipe-step{display:flex;gap:1.5rem;align-items:flex-start;position:relative}
.pipe-step:not(:last-child)::after{content:'';position:absolute;left:20px;top:44px;width:1px;height:calc(100% + 0px);background:var(--border2)}
.pipe-num{flex-shrink:0;width:40px;height:40px;background:var(--bg3);border:1px solid var(--border2);border-radius:50%;display:flex;align-items:center;justify-content:center;font-family:'JetBrains Mono',monospace;font-size:13px;font-weight:700;color:var(--indigo);position:relative;z-index:1}
.pipe-body{padding:0.25rem 0 2.5rem}
.pipe-title{font-family:'Space Grotesk',sans-serif;font-weight:600;font-size:1rem;color:var(--text1);margin-bottom:0.35rem}
.pipe-desc{font-size:14px;color:var(--text2);line-height:1.65}
.pipe-tag{display:inline-block;background:var(--indigo-dim);border:1px solid rgba(91,91,255,0.2);border-radius:5px;padding:2px 8px;font-size:12px;color:var(--indigo);font-family:'JetBrains Mono',monospace;margin-top:6px}
.pipe-tag.free{background:var(--green-dim);border-color:rgba(0,229,122,0.2);color:var(--green)}

/* TERMINAL */
.terminal{background:#0D0D0D;border:1px solid rgba(255,255,255,0.1);border-radius:var(--radius-lg);overflow:hidden;margin-top:3rem;font-family:'JetBrains Mono',monospace}
.terminal-bar{background:#1A1A1A;padding:12px 16px;display:flex;align-items:center;gap:8px;border-bottom:1px solid rgba(255,255,255,0.06)}
.term-dot{width:12px;height:12px;border-radius:50%}
.term-dot.r{background:#FF5F57}
.term-dot.y{background:#FEBC2E}
.term-dot.g{background:#28C840}
.terminal-title{flex:1;text-align:center;font-size:12px;color:rgba(255,255,255,0.3);font-family:'Inter',sans-serif}
.terminal-body{padding:1.5rem 1.75rem;font-size:13.5px;line-height:2;overflow-x:auto}
.t-comment{color:#5A5A7A}
.t-cmd{color:#E0E0FF}
.t-flag{color:var(--indigo)}
.t-green{color:var(--green)}
.t-yellow{color:var(--yellow)}
.t-dim{color:#555580}

/* MCP TOOLS */
.tools-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(280px,1fr));gap:1.25rem;margin-top:3rem}
.tool-card{background:var(--bg2);border:1px solid var(--border);border-radius:var(--radius-lg);padding:1.5rem;display:flex;gap:1rem;align-items:flex-start;transition:border-color 0.2s}
.tool-card:hover{border-color:rgba(91,91,255,0.35)}
.tool-icon{flex-shrink:0;width:42px;height:42px;background:var(--indigo-dim);border:1px solid rgba(91,91,255,0.2);border-radius:10px;display:flex;align-items:center;justify-content:center;font-size:18px}
.tool-body .tool-name{font-family:'JetBrains Mono',monospace;font-size:13px;font-weight:700;color:var(--indigo);margin-bottom:4px}
.tool-body .tool-q{font-size:13.5px;color:var(--text2);line-height:1.55;font-style:italic}

/* LANG GRID */
.lang-categories{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:1.25rem;margin-top:3rem}
.lang-cat{background:var(--bg2);border:1px solid var(--border);border-radius:var(--radius-lg);padding:1.25rem 1.5rem}
.lang-cat-name{font-family:'Space Grotesk',sans-serif;font-size:13px;font-weight:600;text-transform:uppercase;letter-spacing:0.08em;color:var(--text3);margin-bottom:0.75rem}
.lang-tags{display:flex;flex-wrap:wrap;gap:6px}
.lang-tag{background:var(--bg3);border:1px solid var(--border);border-radius:6px;padding:4px 10px;font-size:12.5px;color:var(--text2);font-family:'JetBrains Mono',monospace}

/* IDE GRID */
.ide-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(160px,1fr));gap:1rem;margin-top:3rem}
.ide-card{background:var(--bg2);border:1px solid var(--border);border-radius:var(--radius-lg);padding:1.5rem;text-align:center;transition:border-color 0.2s}
.ide-card:hover{border-color:rgba(91,91,255,0.3)}
.ide-card .ide-icon{font-size:2rem;margin-bottom:0.75rem}
.ide-card .ide-name{font-family:'Space Grotesk',sans-serif;font-weight:600;font-size:14px;color:var(--text1);margin-bottom:4px}
.ide-card .ide-method{font-size:12px;color:var(--text3)}
.ide-badge{display:inline-block;background:var(--green-dim);border:1px solid rgba(0,229,122,0.2);border-radius:5px;padding:2px 8px;font-size:11px;font-weight:700;color:var(--green);margin-top:8px}

/* COMPLIANCE */
.compliance-section{background:var(--bg2);border-top:1px solid var(--border);border-bottom:1px solid var(--border)}
.compliance-inner{max-width:1100px;margin:0 auto;padding:6rem 2rem;display:grid;grid-template-columns:1fr 1fr;gap:4rem;align-items:center}
@media(max-width:768px){.compliance-inner{grid-template-columns:1fr;gap:2rem}}
.gears-grid{display:grid;grid-template-columns:1fr;gap:1rem}
.gear-card{background:var(--bg3);border:1px solid var(--border);border-radius:var(--radius-lg);padding:1.25rem 1.5rem;display:flex;gap:1rem;align-items:flex-start}
.gear-icon-box{flex-shrink:0;width:40px;height:40px;border-radius:10px;display:flex;align-items:center;justify-content:center;font-size:18px}
.gear-icon-box.purple{background:rgba(120,80,255,0.12);border:1px solid rgba(120,80,255,0.25)}
.gear-icon-box.blue{background:rgba(50,100,255,0.12);border:1px solid rgba(50,100,255,0.25)}
.gear-icon-box.teal{background:rgba(0,200,150,0.12);border:1px solid rgba(0,200,150,0.25)}
.gear-title{font-family:'Space Grotesk',sans-serif;font-weight:600;font-size:14px;color:var(--text1);margin-bottom:4px}
.gear-desc{font-size:13px;color:var(--text2);line-height:1.6}

/* PRICING */
.pricing-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:1rem;margin-top:3rem}
.price-card{background:var(--bg2);border:1px solid var(--border);border-radius:var(--radius-lg);padding:1.5rem;transition:border-color 0.2s}
.price-card.highlight{border-color:rgba(0,229,122,0.4);background:var(--green-dim)}
.price-tier{font-family:'Space Grotesk',sans-serif;font-size:11px;font-weight:700;letter-spacing:0.1em;text-transform:uppercase;margin-bottom:0.5rem}
.price-tier.free{color:var(--green)}
.price-tier.cheap{color:var(--yellow)}
.price-tier.medium{color:#FF9855}
.price-tier.premium{color:var(--indigo)}
.price-model{font-family:'Space Grotesk',sans-serif;font-size:1rem;font-weight:600;color:var(--text1);margin-bottom:0.75rem}
.price-val{font-family:'Space Grotesk',sans-serif;font-size:2rem;font-weight:700;color:var(--text1);margin-bottom:4px}
.price-unit{font-size:12px;color:var(--text3)}
.price-note{font-size:13px;color:var(--text2);margin-top:0.75rem;line-height:1.5}

/* INSTALL */
.install-section{text-align:center;padding:6rem 2rem}
.install-block{max-width:700px;margin:2.5rem auto 0}
.install-cmd{background:var(--bg2);border:1px solid var(--border2);border-radius:var(--radius-lg);padding:1.25rem 1.75rem;display:flex;align-items:center;gap:1rem;margin-bottom:1rem;text-align:left}
.install-cmd code{font-family:'JetBrains Mono',monospace;font-size:15px;color:var(--green);flex:1}
.copy-btn{background:var(--bg3);border:1px solid var(--border);border-radius:8px;padding:8px 14px;font-size:12px;color:var(--text2);cursor:pointer;font-family:'Space Grotesk',sans-serif;font-weight:600;transition:background 0.2s,color 0.2s;white-space:nowrap}
.copy-btn:hover{background:var(--bg4);color:var(--text1)}
.install-sub{font-size:14px;color:var(--text3);margin-top:0.5rem}
.install-links{display:flex;gap:1.5rem;justify-content:center;margin-top:2rem;flex-wrap:wrap}
.install-links a{color:var(--text2);text-decoration:none;font-size:14px;font-weight:500;transition:color 0.2s;display:flex;align-items:center;gap:6px}
.install-links a:hover{color:var(--text1)}

/* OUTPUT FILES */
.output-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:1rem;margin-top:2.5rem}
.output-card{background:var(--bg2);border:1px solid var(--border);border-radius:var(--radius-lg);padding:1.25rem 1.5rem;display:flex;gap:12px;align-items:flex-start}
.output-icon{flex-shrink:0;font-size:24px}
.output-file{font-family:'JetBrains Mono',monospace;font-size:13px;font-weight:700;color:var(--indigo);margin-bottom:4px}
.output-desc{font-size:13px;color:var(--text2);line-height:1.55}

/* FOOTER */
footer{background:var(--bg2);border-top:1px solid var(--border);padding:3rem 2rem}
.footer-inner{max-width:1100px;margin:0 auto;display:flex;align-items:flex-start;justify-content:space-between;gap:2rem;flex-wrap:wrap}
.footer-brand .logo-text{font-family:'Space Grotesk',sans-serif;font-weight:700;font-size:18px;color:var(--text1);margin-bottom:0.5rem}
.footer-brand p{font-size:13px;color:var(--text3);max-width:280px;line-height:1.6}
.footer-cols{display:flex;gap:3rem;flex-wrap:wrap}
.footer-col h4{font-family:'Space Grotesk',sans-serif;font-size:13px;font-weight:700;text-transform:uppercase;letter-spacing:0.08em;color:var(--text3);margin-bottom:1rem}
.footer-col a{display:block;color:var(--text2);text-decoration:none;font-size:14px;margin-bottom:0.5rem;transition:color 0.2s}
.footer-col a:hover{color:var(--text1)}
.footer-bottom{max-width:1100px;margin:2rem auto 0;padding-top:1.5rem;border-top:1px solid var(--border);display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:1rem}
.footer-bottom p{font-size:13px;color:var(--text3)}
.mit-badge{background:var(--bg3);border:1px solid var(--border);border-radius:6px;padding:4px 10px;font-size:12px;color:var(--text3);font-family:'JetBrains Mono',monospace}

/* SECTION DIVIDER */
.section-divider{border:none;border-top:1px solid var(--border);margin:0}

/* SCROLL REVEAL */
.reveal{opacity:0;transform:translateY(20px);transition:opacity 0.5s ease,transform 0.5s ease}
.reveal.visible{opacity:1;transform:translateY(0)}

@media(max-width:768px){
nav{padding:0 1rem}
.nav-links a:not(.nav-cta){display:none}
section{padding:4rem 1.25rem}
.hero{padding:100px 1.25rem 60px}
.install-cmd code{font-size:13px}
}
</style>
</head>
<body>

<!-- NAVIGATION -->
<nav id="navbar">
  <a href="#" class="nav-logo">
    <div class="nav-logo-icon">P</div>
    <span class="nav-logo-text">PRUVALEX</span>
  </a>
  <div class="nav-links">
    <a href="#pruvagraph">PruvaGraph</a>
    <a href="#compliance">Compliance OS</a>
    <a href="#mcp">MCP Tools</a>
    <a href="#install">Install</a>
    <a href="https://github.com/PRUVALEX-Systems/pruvagraph" class="nav-cta">★ GitHub</a>
  </div>
</nav>

<!-- HERO -->
<section class="hero">
  <canvas id="hero-canvas"></canvas>
  <div class="hero-inner">
    <div class="hero-badge">
      <span class="hero-badge-dot"></span>
      v1.0.1 — Live on VS Code Marketplace
    </div>
    <h1>
      Your AI is costing you<br/>
      <span class="accent">a fortune.</span><br/>
      <span class="accent-green">It doesn't have to.</span>
    </h1>
    <p class="hero-sub">
      PRUVALEX engineers mathematically provable AI compliance architectures and zero-cost developer tools.
      Built for developers who love Claude Code — but not the bill.
    </p>

    <div class="hero-savings">
      <div class="savings-box">
        <div class="label">Without PruvaGraph</div>
        <div class="val" id="counter-before">$313</div>
        <div style="font-size:12px;color:var(--text3);margin-top:4px">per month</div>
      </div>
      <div class="savings-arrow">→</div>
      <div class="savings-box">
        <div class="label">With PruvaGraph</div>
        <div class="val green">$0.30</div>
        <div style="font-size:12px;color:var(--text3);margin-top:4px">per month</div>
      </div>
      <div class="savings-tag">99.9% saved</div>
    </div>

    <div class="hero-btns">
      <a href="#install" class="btn-primary">Get Started Free →</a>
      <a href="https://github.com/PRUVALEX-Systems/pruvagraph" class="btn-ghost">View on GitHub</a>
    </div>
  </div>
</section>

<!-- STATS STRIP -->
<div class="stats-strip">
  <div class="stats-inner">
    <div class="stat-item">
      <div class="n">99<span class="unit">%+</span></div>
      <div class="d">LLM Cost Reduction</div>
    </div>
    <div class="stat-divider"></div>
    <div class="stat-item">
      <div class="n">30<span class="unit">+</span></div>
      <div class="d">Languages (Free)</div>
    </div>
    <div class="stat-divider"></div>
    <div class="stat-item">
      <div class="n">$0<span class="unit"></span></div>
      <div class="d">Cost for All Code Files</div>
    </div>
    <div class="stat-divider"></div>
    <div class="stat-item">
      <div class="n">6</div>
      <div class="d">MCP Tools</div>
    </div>
    <div class="stat-divider"></div>
    <div class="stat-item">
      <div class="n">MIT</div>
      <div class="d">Open Source License</div>
    </div>
  </div>
</div>

<!-- PRUVAGRAPH SECTION -->
<section id="pruvagraph">
  <div class="section-inner reveal">
    <div class="eyebrow">Flagship Open-Source Tool</div>
    <h2 class="section-title">Introducing PruvaGraph</h2>
    <p class="section-sub">
      Your entire codebase, converted into a queryable knowledge graph.
      AI tools read the graph — not the raw files — saving 99%+ tokens on every run.
    </p>

    <div class="compare-wrap">
      <table class="compare">
        <thead>
          <tr>
            <th></th>
            <th class="h-other">Other Tools</th>
            <th class="h-pruva">PruvaGraph</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>10,000-file repo, daily CI</td>
            <td class="bad">~3,300,000 LLM calls/month</td>
            <td class="good">~3,140 calls/month</td>
          </tr>
          <tr>
            <td>Monthly cost (Claude Sonnet)</td>
            <td class="bad">~$313/month</td>
            <td class="good">~$0.30/month</td>
          </tr>
          <tr>
            <td>Re-run (unchanged files)</td>
            <td class="bad">Full LLM scan again</td>
            <td class="good">Instant cache hit</td>
          </tr>
          <tr>
            <td>Changed files only</td>
            <td class="bad">Re-scans everything</td>
            <td class="good">Re-scans changed files only</td>
          </tr>
          <tr>
            <td>Semantic duplicate detection</td>
            <td class="bad">None</td>
            <td class="good">Groups similar files → 1 LLM call</td>
          </tr>
          <tr>
            <td>Code file analysis cost</td>
            <td class="bad">API calls per file</td>
            <td class="good">$0.00 — tree-sitter local AST</td>
          </tr>
          <tr>
            <td>Data sovereignty</td>
            <td class="bad">Cloud dependent</td>
            <td class="good">100% local, no server</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</section>

<hr class="section-divider"/>

<!-- 4 LAYERS -->
<section>
  <div class="section-inner reveal">
    <div class="eyebrow">Cost Architecture</div>
    <h2 class="section-title">4 Layers of Savings</h2>
    <p class="section-sub">Every request passes through four optimization layers before a single token is spent.</p>

    <div class="layers-grid">
      <div class="layer-card">
        <div class="layer-num">Layer 01 — cache.py</div>
        <div class="layer-title">SHA-256 Hash Cache</div>
        <div class="layer-desc">Fingerprints every file. If unchanged since last run → 0 API calls. File size + last-modified timestamp verified before any processing begins.</div>
        <div class="layer-saving">↓ 80–90% on re-runs</div>
      </div>
      <div class="layer-card">
        <div class="layer-num">Layer 02 — dedup.py</div>
        <div class="layer-title">Semantic MinHash Dedup</div>
        <div class="layer-desc">40 similar React components? One LLM call — the rest are copied. Jaccard similarity ≥ 0.82 groups files together. Threshold is configurable from 0.5 to 1.0.</div>
        <div class="layer-saving">↓ 40–60% additional</div>
      </div>
      <div class="layer-card">
        <div class="layer-num">Layer 03 — batch.py</div>
        <div class="layer-title">Smart Batch Packing</div>
        <div class="layer-desc">10+ files sent in a single LLM call instead of one call per file. Default batch size: 12,000 tokens. Other tools burn calls — PruvaGraph packs them.</div>
        <div class="layer-saving">↓ 5×–10× fewer calls</div>
      </div>
      <div class="layer-card">
        <div class="layer-num">Layer 04 — router.py</div>
        <div class="layer-title">3-Tier Cascade Router</div>
        <div class="layer-desc">Automatically picks the cheapest model for each task. Code files → free tree-sitter. Small docs → Ollama (free). Medium → Gemini Flash ($0.075/M). Complex → Claude Sonnet only when needed.</div>
        <div class="layer-saving">↓ Auto-optimize cost</div>
      </div>
    </div>
  </div>
</section>

<hr class="section-divider"/>

<!-- PIPELINE -->
<section>
  <div class="section-inner reveal">
    <div class="eyebrow">How It Works</div>
    <h2 class="section-title">5-Stage Pipeline</h2>
    <p class="section-sub">From raw repository to queryable knowledge graph, fully automated.</p>

    <div class="pipeline">
      <div class="pipe-step">
        <div class="pipe-num">1</div>
        <div class="pipe-body">
          <div class="pipe-title">File Discovery</div>
          <div class="pipe-desc">Collects all files — code and docs. Automatically excludes <code style="font-size:13px;color:var(--indigo)">.git</code>, <code style="font-size:13px;color:var(--indigo)">node_modules</code>, and <code style="font-size:13px;color:var(--indigo)">dist</code> directories.</div>
        </div>
      </div>
      <div class="pipe-step">
        <div class="pipe-num">2</div>
        <div class="pipe-body">
          <div class="pipe-title">Code Files — Tree-sitter AST</div>
          <div class="pipe-desc">Python, JS, TS, Go, Rust, Java, and 30+ languages parsed locally. Zero API calls, zero internet needed. Cache hit = instant skip.</div>
          <div class="pipe-tag free">ZERO COST</div>
        </div>
      </div>
      <div class="pipe-step">
        <div class="pipe-num">3</div>
        <div class="pipe-body">
          <div class="pipe-title">Docs & Images — LLM (with Dedup + Batching)</div>
          <div class="pipe-desc">.md, .pdf, .docx, and images processed with semantic dedup first, then batch packed, then routed to the cheapest viable model tier. Dry run mode estimates cost without spending.</div>
          <div class="pipe-tag">OPTIMIZED</div>
        </div>
      </div>
      <div class="pipe-step">
        <div class="pipe-num">4</div>
        <div class="pipe-body">
          <div class="pipe-title">Graph Build + Community Detection</div>
          <div class="pipe-desc">NetworkX graph constructed with nodes and edges. Leiden algorithm detects architectural clusters — automatically surfacing how modules relate to each other.</div>
          <div class="pipe-tag">SMART</div>
        </div>
      </div>
      <div class="pipe-step">
        <div class="pipe-num">5</div>
        <div class="pipe-body">
          <div class="pipe-title">Analyze + Export</div>
          <div class="pipe-desc">God nodes identified (highest-connectivity files). GRAPH_REPORT.md, graph.json, interactive graph.html, and cost_report.json saved to pruvagraph-out/.</div>
          <div class="pipe-tag free">COMPLETE</div>
        </div>
      </div>
    </div>
  </div>
</section>

<hr class="section-divider"/>

<!-- TERMINAL / CLI -->
<section>
  <div class="section-inner reveal">
    <div class="eyebrow">CLI Reference</div>
    <h2 class="section-title">Everything from the Terminal</h2>
    <p class="section-sub">One command to build. Many commands to query, export, and integrate.</p>

    <div class="terminal">
      <div class="terminal-bar">
        <div class="term-dot r"></div>
        <div class="term-dot y"></div>
        <div class="term-dot g"></div>
        <div class="terminal-title">pruvagraph — zsh</div>
      </div>
      <div class="terminal-body">
        <div class="t-comment"># ── MAIN COMMANDS ─────────────────────────────────────────</div>
        <div><span class="t-green">pruvagraph</span> <span class="t-cmd">.</span>  <span class="t-dim"># Build graph (current folder)</span></div>
        <div><span class="t-green">pruvagraph</span> <span class="t-cmd">./src</span>  <span class="t-dim"># Build graph (src/ only)</span></div>
        <div>&nbsp;</div>
        <div class="t-comment"># ── BACKEND OPTIONS ────────────────────────────────────────</div>
        <div><span class="t-green">pruvagraph</span> <span class="t-cmd">.</span> <span class="t-flag">--backend</span> <span class="t-yellow">claude</span>    <span class="t-dim"># Claude Sonnet (default)</span></div>
        <div><span class="t-green">pruvagraph</span> <span class="t-cmd">.</span> <span class="t-flag">--backend</span> <span class="t-yellow">gemini</span>    <span class="t-dim"># Gemini Flash (cheapest)</span></div>
        <div><span class="t-green">pruvagraph</span> <span class="t-cmd">.</span> <span class="t-flag">--backend</span> <span class="t-yellow">ollama</span>    <span class="t-dim"># Local Ollama (FREE)</span></div>
        <div><span class="t-green">pruvagraph</span> <span class="t-cmd">.</span> <span class="t-flag">--cascade</span>            <span class="t-dim"># Auto 3-tier routing</span></div>
        <div>&nbsp;</div>
        <div class="t-comment"># ── SMART OPTIONS ──────────────────────────────────────────</div>
        <div><span class="t-green">pruvagraph</span> <span class="t-cmd">.</span> <span class="t-flag">--update</span>             <span class="t-dim"># Changed files only</span></div>
        <div><span class="t-green">pruvagraph</span> <span class="t-cmd">.</span> <span class="t-flag">--dry-run</span>            <span class="t-dim"># Cost estimate, no spend</span></div>
        <div><span class="t-green">pruvagraph</span> <span class="t-cmd">.</span> <span class="t-flag">--budget</span> <span class="t-yellow">2.00</span>         <span class="t-dim"># Hard cap — max $2</span></div>
        <div><span class="t-green">pruvagraph</span> <span class="t-cmd">.</span> <span class="t-flag">--force</span>              <span class="t-dim"># Ignore cache</span></div>
        <div>&nbsp;</div>
        <div class="t-comment"># ── QUERY ──────────────────────────────────────────────────</div>
        <div><span class="t-green">pruvagraph</span> query <span class="t-yellow">"auth module kaise kaam karta hai?"</span></div>
        <div><span class="t-green">pruvagraph</span> query <span class="t-yellow">"top 5 god nodes kya hain?"</span></div>
        <div>&nbsp;</div>
        <div class="t-comment"># ── EXPORT ─────────────────────────────────────────────────</div>
        <div><span class="t-green">pruvagraph</span> export <span class="t-flag">--format</span> <span class="t-yellow">html</span>      <span class="t-dim"># Interactive browser viz</span></div>
        <div><span class="t-green">pruvagraph</span> export <span class="t-flag">--format</span> <span class="t-yellow">cypher</span>    <span class="t-dim"># Neo4j import</span></div>
        <div><span class="t-green">pruvagraph</span> export <span class="t-flag">--format</span> <span class="t-yellow">obsidian</span>  <span class="t-dim"># Obsidian vault</span></div>
        <div>&nbsp;</div>
        <div class="t-comment"># ── IDE INTEGRATION ────────────────────────────────────────</div>
        <div><span class="t-green">pruvagraph</span> install                   <span class="t-dim"># All IDEs</span></div>
        <div><span class="t-green">pruvagraph</span> install <span class="t-flag">--claude-code</span>    <span class="t-dim"># Claude Code MCP only</span></div>
        <div><span class="t-green">pruvagraph</span> watch <span class="t-cmd">.</span>                <span class="t-dim"># Auto-rebuild on file change</span></div>
        <div><span class="t-green">pruvagraph</span> hook install              <span class="t-dim"># Git commit auto-update</span></div>
      </div>
    </div>
  </div>
</section>

<hr class="section-divider"/>

<!-- OUTPUT FILES -->
<section>
  <div class="section-inner reveal">
    <div class="eyebrow">Output</div>
    <h2 class="section-title">What You Get</h2>
    <p class="section-sub">Every run produces four output files in <code style="font-family:'JetBrains Mono';font-size:14px;color:var(--indigo)">pruvagraph-out/</code></p>

    <div class="output-grid">
      <div class="output-card">
        <div class="output-icon">📊</div>
        <div>
          <div class="output-file">graph.json</div>
          <div class="output-desc">Queryable knowledge graph in NetworkX format. Used by MCP tools and AI agents.</div>
        </div>
      </div>
      <div class="output-card">
        <div class="output-icon">🌐</div>
        <div>
          <div class="output-file">graph.html</div>
          <div class="output-desc">Interactive browser visualizer. Drag nodes, explore edges, zoom into clusters.</div>
        </div>
      </div>
      <div class="output-card">
        <div class="output-icon">📋</div>
        <div>
          <div class="output-file">GRAPH_REPORT.md</div>
          <div class="output-desc">Architecture summary — god nodes, communities, surprising connections between modules.</div>
        </div>
      </div>
      <div class="output-card">
        <div class="output-icon">💰</div>
        <div>
          <div class="output-file">cost_report.json</div>
          <div class="output-desc">Exact API calls made, tokens consumed, and money saved versus baseline approach.</div>
        </div>
      </div>
    </div>
  </div>
</section>

<hr class="section-divider"/>

<!-- MCP TOOLS -->
<section id="mcp">
  <div class="section-inner reveal">
    <div class="eyebrow">MCP Server</div>
    <h2 class="section-title">6 Tools for Claude Code & Cursor</h2>
    <p class="section-sub">
      <code style="font-family:'JetBrains Mono';font-size:14px;color:var(--indigo)">mcp_server.py</code> — auto-configures for Claude Code, Cursor, VS Code, and Windsurf.
    </p>

    <div class="tools-grid">
      <div class="tool-card">
        <div class="tool-icon">🔍</div>
        <div class="tool-body">
          <div class="tool-name">query_graph</div>
          <div class="tool-q">"auth module database se kaise connect hai?"</div>
        </div>
      </div>
      <div class="tool-card">
        <div class="tool-icon">🔗</div>
        <div class="tool-body">
          <div class="tool-name">get_dependencies</div>
          <div class="tool-q">"AuthService kya-kya use karta hai?"</div>
        </div>
      </div>
      <div class="tool-card">
        <div class="tool-icon">📞</div>
        <div class="tool-body">
          <div class="tool-name">find_callers</div>
          <div class="tool-q">"processPayment() kaun-kaun call karta hai?"</div>
        </div>
      </div>
      <div class="tool-card">
        <div class="tool-icon">📝</div>
        <div class="tool-body">
          <div class="tool-name">get_summary</div>
          <div class="tool-q">"UserController ka ek line summary do"</div>
        </div>
      </div>
      <div class="tool-card">
        <div class="tool-icon">🏗️</div>
        <div class="tool-body">
          <div class="tool-name">list_communities</div>
          <div class="tool-q">"Is codebase ke architectural modules kya hain?"</div>
        </div>
      </div>
      <div class="tool-card">
        <div class="tool-icon">💸</div>
        <div class="tool-body">
          <div class="tool-name">cost_report</div>
          <div class="tool-q">"Last run mein kitna paisa bacha?"</div>
        </div>
      </div>
    </div>
  </div>
</section>

<hr class="section-divider"/>

<!-- LANGUAGE SUPPORT -->
<section>
  <div class="section-inner reveal">
    <div class="eyebrow">Language Support</div>
    <h2 class="section-title">30+ Languages — All Free via Tree-sitter</h2>
    <p class="section-sub">Local AST parsing. No API. No internet. No cost.</p>

    <div class="lang-categories">
      <div class="lang-cat">
        <div class="lang-cat-name">Web</div>
        <div class="lang-tags">
          <span class="lang-tag">TypeScript</span>
          <span class="lang-tag">TSX</span>
          <span class="lang-tag">JavaScript</span>
          <span class="lang-tag">JSX</span>
          <span class="lang-tag">Vue</span>
          <span class="lang-tag">Svelte</span>
          <span class="lang-tag">Astro</span>
          <span class="lang-tag">CSS</span>
          <span class="lang-tag">HTML</span>
        </div>
      </div>
      <div class="lang-cat">
        <div class="lang-cat-name">Backend</div>
        <div class="lang-tags">
          <span class="lang-tag">Python</span>
          <span class="lang-tag">Go</span>
          <span class="lang-tag">Rust</span>
          <span class="lang-tag">Java</span>
          <span class="lang-tag">C#</span>
          <span class="lang-tag">PHP</span>
          <span class="lang-tag">Ruby</span>
          <span class="lang-tag">Elixir</span>
          <span class="lang-tag">Scala</span>
        </div>
      </div>
      <div class="lang-cat">
        <div class="lang-cat-name">Mobile</div>
        <div class="lang-tags">
          <span class="lang-tag">Kotlin</span>
          <span class="lang-tag">Swift</span>
          <span class="lang-tag">Dart</span>
          <span class="lang-tag">Objective-C</span>
        </div>
      </div>
      <div class="lang-cat">
        <div class="lang-cat-name">Systems</div>
        <div class="lang-tags">
          <span class="lang-tag">C</span>
          <span class="lang-tag">C++</span>
          <span class="lang-tag">Zig</span>
        </div>
      </div>
      <div class="lang-cat">
        <div class="lang-cat-name">Data / Infra</div>
        <div class="lang-tags">
          <span class="lang-tag">SQL</span>
          <span class="lang-tag">YAML</span>
          <span class="lang-tag">Terraform</span>
          <span class="lang-tag">Dockerfile</span>
          <span class="lang-tag">Bash</span>
        </div>
      </div>
      <div class="lang-cat">
        <div class="lang-cat-name">Docs (LLM)</div>
        <div class="lang-tags">
          <span class="lang-tag">PDF</span>
          <span class="lang-tag">DOCX</span>
          <span class="lang-tag">Markdown</span>
          <span class="lang-tag">Images</span>
        </div>
      </div>
    </div>
  </div>
</section>

<hr class="section-divider"/>

<!-- IDE INTEGRATION -->
<section>
  <div class="section-inner reveal">
    <div class="eyebrow">IDE Integration</div>
    <h2 class="section-title">Works Everywhere You Do</h2>
    <p class="section-sub">One install command configures all your IDEs simultaneously.</p>

    <div class="ide-grid">
      <div class="ide-card">
        <div class="ide-icon">🆚</div>
        <div class="ide-name">VS Code</div>
        <div class="ide-method">.vsix / Marketplace</div>
        <div class="ide-badge">✓ Ready</div>
      </div>
      <div class="ide-card">
        <div class="ide-icon">⌨️</div>
        <div class="ide-name">Cursor</div>
        <div class="ide-method">.vsix / Open VSX</div>
        <div class="ide-badge">✓ Ready</div>
      </div>
      <div class="ide-card">
        <div class="ide-icon">🌊</div>
        <div class="ide-name">Windsurf</div>
        <div class="ide-method">.vsix drag-and-drop</div>
        <div class="ide-badge">✓ Ready</div>
      </div>
      <div class="ide-card">
        <div class="ide-icon">🤖</div>
        <div class="ide-name">Claude Code</div>
        <div class="ide-method">MCP auto-config</div>
        <div class="ide-badge">✓ Ready</div>
      </div>
      <div class="ide-card">
        <div class="ide-icon">💻</div>
        <div class="ide-name">Any Terminal</div>
        <div class="ide-method">pip install</div>
        <div class="ide-badge">✓ Ready</div>
      </div>
      <div class="ide-card">
        <div class="ide-icon">☁️</div>
        <div class="ide-name">Gitpod</div>
        <div class="ide-method">Open VSX Registry</div>
        <div class="ide-badge">✓ Ready</div>
      </div>
    </div>
  </div>
</section>

<hr class="section-divider"/>

<!-- COMPLIANCE OS -->
<div class="compliance-section" id="compliance">
  <div class="compliance-inner">
    <div class="reveal">
      <div class="eyebrow">Enterprise Platform</div>
      <h2 class="section-title">The PRUVALEX Compliance OS</h2>
      <p class="section-sub" style="margin-bottom:1.5rem">
        PruvaGraph is the open-source flagship. Behind it lies a full enterprise ecosystem
        built for organizations operating AI in regulated sectors.
      </p>
      <p style="font-size:14px;color:var(--text3);line-height:1.7">
        We engineer mathematically provable AI compliance architectures. Our infrastructure
        allows high-risk AI systems deployed in regulated industries to maintain absolute
        compliance while drastically reducing operational overhead.
      </p>
      <div style="margin-top:1.5rem">
        <a href="https://pruvalex.eu" class="btn-ghost" style="display:inline-flex;align-items:center;gap:8px;font-size:14px">
          Official Website →
        </a>
      </div>
    </div>
    <div class="gears-grid reveal">
      <div class="gear-card">
        <div class="gear-icon-box purple">🔐</div>
        <div>
          <div class="gear-title">Sovereign AI Vault</div>
          <div class="gear-desc">Cryptographic evidence and WORM audit trails for deployment verification. ML-DSA-65 (NIST FIPS 204) signed.</div>
        </div>
      </div>
      <div class="gear-card">
        <div class="gear-icon-box blue">⏱️</div>
        <div>
          <div class="gear-title">Regulatory Time-Traveler</div>
          <div class="gear-desc">Point-in-time compliance snapshots. Know exactly what state your AI system was in at any past moment — for audits, litigation, or regulatory review.</div>
        </div>
      </div>
      <div class="gear-card">
        <div class="gear-icon-box teal">🌐</div>
        <div>
          <div class="gear-title">Global Law-Sync</div>
          <div class="gear-desc">Automated technical gears for EU AI Act Reg. 2024/1689. Systematic coverage that keeps your compliance current as regulations evolve.</div>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- PRICING TABLE -->
<section>
  <div class="section-inner reveal">
    <div class="eyebrow">LLM Pricing</div>
    <h2 class="section-title">The Cascade Router Always Picks Cheapest</h2>
    <p class="section-sub">Every task is automatically matched to the most cost-effective model tier. You set a budget cap — we never exceed it.</p>

    <div class="pricing-grid">
      <div class="price-card highlight">
        <div class="price-tier free">Tier 1 — Free</div>
        <div class="price-model">Ollama (Local)</div>
        <div class="price-val">$0<span style="font-size:1rem;color:var(--green)">.000</span></div>
        <div class="price-unit">per million tokens</div>
        <div class="price-note">Code files &lt; 1,500 tokens. Zero API key, zero cost, zero cloud.</div>
      </div>
      <div class="price-card">
        <div class="price-tier cheap">Tier 2 — Cheap</div>
        <div class="price-model">Gemini 2.0 Flash</div>
        <div class="price-val">$0.075</div>
        <div class="price-unit">per million tokens</div>
        <div class="price-note">Medium docs &lt; 8,000 tokens. 40× cheaper than Claude Sonnet.</div>
      </div>
      <div class="price-card">
        <div class="price-tier medium">Tier 3 — Medium</div>
        <div class="price-model">GPT-4o-mini</div>
        <div class="price-val">$0.400</div>
        <div class="price-unit">per million tokens</div>
        <div class="price-note">When Gemini is not suitable. Still 7.5× cheaper than Claude.</div>
      </div>
      <div class="price-card">
        <div class="price-tier premium">Tier 4 — Premium</div>
        <div class="price-model">Claude Sonnet 4.6</div>
        <div class="price-val">$3.000</div>
        <div class="price-unit">per million tokens</div>
        <div class="price-note">Complex PDFs and large batches only. Used as a last resort.</div>
      </div>
    </div>
  </div>
</section>

<hr class="section-divider"/>

<!-- INSTALL -->
<section class="install-section" id="install">
  <div class="section-inner">
    <div class="reveal">
      <div class="eyebrow">Get Started</div>
      <h2 class="section-title">Zero Setup. One Command.</h2>
      <p class="section-sub" style="margin:0 auto 0">
        Install the package, point it at your repo, and watch your AI costs collapse.
      </p>

      <div class="install-block">
        <div class="install-cmd">
          <code>pip install pruvagraph</code>
          <button class="copy-btn" onclick="copyCmd('pip install pruvagraph',this)">Copy</button>
        </div>
        <div class="install-cmd">
          <code>pruvagraph . --cascade --dry-run</code>
          <button class="copy-btn" onclick="copyCmd('pruvagraph . --cascade --dry-run',this)">Copy</button>
        </div>
        <div class="install-cmd">
          <code>pruvagraph install</code>
          <button class="copy-btn" onclick="copyCmd('pruvagraph install',this)">Copy</button>
        </div>
        <div class="install-sub">Installs VS Code extension + configures Claude Code MCP + Cursor + CLAUDE.md</div>

        <div class="install-links">
          <a href="https://github.com/PRUVALEX-Systems/pruvagraph">★ GitHub Repository</a>
          <a href="https://marketplace.visualstudio.com/publishers/pruvalex">VS Code Marketplace</a>
          <a href="https://pruvalex.eu">Official Website</a>
          <a href="mailto:security@pruvalex.eu">Contact Security</a>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- FOOTER -->
<footer>
  <div class="footer-inner">
    <div class="footer-brand">
      <div class="logo-text">PRUVALEX</div>
      <p>The Enterprise Operating System for AI Compliance & Cost Optimization. Open source, MIT licensed.</p>
    </div>
    <div class="footer-cols">
      <div class="footer-col">
        <h4>Open Source</h4>
        <a href="https://github.com/PRUVALEX-Systems/pruvagraph">PruvaGraph</a>
        <a href="https://github.com/PRUVALEX-Systems/pruvagraph/releases">Releases</a>
        <a href="https://github.com/PRUVALEX-Systems/pruvagraph/issues">Issues</a>
        <a href="https://github.com/PRUVALEX-Systems">All Repos</a>
      </div>
      <div class="footer-col">
        <h4>Product</h4>
        <a href="https://marketplace.visualstudio.com/publishers/pruvalex">VS Code Extension</a>
        <a href="#mcp">MCP Server</a>
        <a href="#compliance">Compliance OS</a>
        <a href="#install">Installation</a>
      </div>
      <div class="footer-col">
        <h4>Company</h4>
        <a href="https://pruvalex.eu">pruvalex.eu</a>
        <a href="mailto:security@pruvalex.eu">Security Contact</a>
        <a href="https://pruvalex.eu">EU AI Act Compliance</a>
      </div>
    </div>
  </div>
  <div class="footer-bottom">
    <p>© 2025 PRUVALEX Systems. Built for developers who love Claude Code but not the bill.</p>
    <span class="mit-badge">MIT License</span>
  </div>
</footer>

<script>
// NAV scroll effect
const navbar=document.getElementById('navbar');
window.addEventListener('scroll',()=>{
  navbar.classList.toggle('scrolled',window.scrollY>20);
});

// Copy button
function copyCmd(text,btn){
  navigator.clipboard.writeText(text).then(()=>{
    const orig=btn.textContent;
    btn.textContent='Copied!';
    btn.style.color='var(--green)';
    btn.style.borderColor='rgba(0,229,122,0.3)';
    setTimeout(()=>{btn.textContent=orig;btn.style.color='';btn.style.borderColor='';},1800);
  });
}

// Scroll reveal
const reveals=document.querySelectorAll('.reveal');
const io=new IntersectionObserver((entries)=>{
  entries.forEach(e=>{
    if(e.isIntersecting){e.target.classList.add('visible');io.unobserve(e.target);}
  });
},{threshold:0.1});
reveals.forEach(el=>io.observe(el));

// Hero canvas network animation
(function(){
  const canvas=document.getElementById('hero-canvas');
  const ctx=canvas.getContext('2d');
  let W,H,nodes=[];
  
  function resize(){
    W=canvas.width=canvas.offsetWidth;
    H=canvas.height=canvas.offsetHeight;
  }
  resize();
  window.addEventListener('resize',()=>{resize();initNodes();});
  
  function initNodes(){
    nodes=[];
    const count=Math.floor((W*H)/14000);
    for(let i=0;i<count;i++){
      nodes.push({
        x:Math.random()*W,
        y:Math.random()*H,
        vx:(Math.random()-0.5)*0.3,
        vy:(Math.random()-0.5)*0.3,
        r:Math.random()*2+1
      });
    }
  }
  initNodes();
  
  function draw(){
    ctx.clearRect(0,0,W,H);
    const maxDist=140;
    
    for(let i=0;i<nodes.length;i++){
      const n=nodes[i];
      n.x+=n.vx;n.y+=n.vy;
      if(n.x<0||n.x>W)n.vx*=-1;
      if(n.y<0||n.y>H)n.vy*=-1;
      
      for(let j=i+1;j<nodes.length;j++){
        const m=nodes[j];
        const dx=n.x-m.x,dy=n.y-m.y;
        const dist=Math.sqrt(dx*dx+dy*dy);
        if(dist<maxDist){
          const alpha=(1-dist/maxDist)*0.4;
          ctx.beginPath();
          ctx.moveTo(n.x,n.y);
          ctx.lineTo(m.x,m.y);
          ctx.strokeStyle=`rgba(91,91,255,${alpha})`;
          ctx.lineWidth=0.5;
          ctx.stroke();
        }
      }
      
      ctx.beginPath();
      ctx.arc(n.x,n.y,n.r,0,Math.PI*2);
      ctx.fillStyle='rgba(91,91,255,0.6)';
      ctx.fill();
    }
    requestAnimationFrame(draw);
  }
  draw();
})();
</script>
</body>
</html>
