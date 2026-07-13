<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Kevin Yeon — Startup Ecosystem Leader & Management Advisor</title>
<meta name="description" content="Kevin (Kyuhwang) Yeon — three decades building entrepreneurs and bridging Korea's innovation economy with global markets. Former Gartner & IDC Korea leader, CCEI Daegu President, KPC Senior Advisor." />
<link rel="preconnect" href="https://fonts.googleapis.com" />
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
<link href="https://fonts.googleapis.com/css2?family=EB+Garamond:ital,wght@0,400;0,500;0,600;1,400&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet" />
<style>
  :root {
    --navy: #0f1c2e;
    --navy-soft: #1b2c44;
    --slate: #3a4a5f;
    --ink: #16202e;
    --muted: #6b7888;
    --line: #e4e7ec;
    --cream: #f7f5f0;
    --paper: #ffffff;
    --gold: #b08544;
    --gold-soft: #c9a86a;
    --accent-bg: #fbf9f4;
    --shadow: 0 1px 2px rgba(16,28,46,.04), 0 8px 30px rgba(16,28,46,.06);
    --maxw: 1080px;
  }

  * { box-sizing: border-box; margin: 0; padding: 0; }

  html { scroll-behavior: smooth; }

  body {
    font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Pretendard', sans-serif;
    color: var(--ink);
    background: var(--cream);
    line-height: 1.65;
    -webkit-font-smoothing: antialiased;
    text-rendering: optimizeLegibility;
  }

  h1, h2, h3 { font-family: 'EB Garamond', Georgia, serif; font-weight: 500; line-height: 1.15; letter-spacing: -0.01em; }

  a { color: inherit; text-decoration: none; }

  .wrap { max-width: var(--maxw); margin: 0 auto; padding: 0 32px; }

  /* ---------- NAV ---------- */
  nav {
    position: sticky; top: 0; z-index: 50;
    background: rgba(247,245,240,.82);
    backdrop-filter: saturate(180%) blur(12px);
    border-bottom: 1px solid var(--line);
  }
  nav .wrap { display: flex; align-items: center; justify-content: space-between; height: 64px; }
  .brand { font-family: 'EB Garamond', serif; font-size: 1.25rem; font-weight: 600; letter-spacing: .02em; }
  .brand span { color: var(--gold); }
  .navlinks { display: flex; gap: 30px; }
  .navlinks a { font-size: .82rem; letter-spacing: .04em; text-transform: uppercase; color: var(--muted); transition: color .2s; }
  .navlinks a:hover { color: var(--ink); }
  @media (max-width: 720px) { .navlinks { display: none; } }

  /* ---------- HERO ---------- */
  header.hero {
    background: linear-gradient(160deg, var(--navy) 0%, var(--navy-soft) 100%);
    color: #f3f1ec;
    position: relative;
    overflow: hidden;
  }
  header.hero::after {
    content: ""; position: absolute; right: -120px; top: -120px;
    width: 480px; height: 480px; border-radius: 50%;
    background: radial-gradient(circle, rgba(176,133,68,.18), transparent 70%);
  }
  .hero .wrap { padding-top: 92px; padding-bottom: 92px; position: relative; z-index: 2; }
  .eyebrow {
    display: inline-flex; align-items: center; gap: 10px;
    font-size: .78rem; letter-spacing: .22em; text-transform: uppercase;
    color: var(--gold-soft); margin-bottom: 26px;
  }
  .eyebrow::before { content: ""; width: 34px; height: 1px; background: var(--gold-soft); }
  .hero h1 { font-size: clamp(2.6rem, 6vw, 4.4rem); color: #fff; margin-bottom: 8px; }
  .hero .ko-name { font-size: 1.1rem; color: var(--gold-soft); letter-spacing: .08em; margin-bottom: 22px; font-family: 'Inter', sans-serif; }
  .hero .title { font-size: clamp(1.15rem, 2.4vw, 1.55rem); font-family: 'EB Garamond', serif; font-style: italic; color: #d9d4ca; max-width: 720px; }
  .hero .meta { display: flex; flex-wrap: wrap; gap: 26px; margin-top: 38px; font-size: .92rem; color: #b9c0cb; }
  .hero .meta span { display: inline-flex; align-items: center; gap: 8px; }
  .hero .meta svg { width: 16px; height: 16px; opacity: .8; }
  .cta { margin-top: 42px; display: flex; gap: 14px; flex-wrap: wrap; }
  .btn {
    display: inline-block; padding: 13px 26px; border-radius: 2px; font-size: .85rem;
    letter-spacing: .05em; transition: all .22s; cursor: pointer; border: 1px solid transparent;
  }
  .btn.primary { background: var(--gold); color: #fff; }
  .btn.primary:hover { background: var(--gold-soft); transform: translateY(-1px); }
  .btn.ghost { border-color: rgba(255,255,255,.28); color: #f3f1ec; }
  .btn.ghost:hover { border-color: var(--gold-soft); color: #fff; }

  /* ---------- STAT BAR ---------- */
  .stats { background: var(--navy-soft); color: #f3f1ec; border-top: 1px solid rgba(255,255,255,.08); }
  .stats .wrap { display: grid; grid-template-columns: repeat(4, 1fr); gap: 24px; padding: 40px 32px; }
  .stat { text-align: center; }
  .stat .num { font-family: 'EB Garamond', serif; font-size: 2.4rem; color: var(--gold-soft); line-height: 1; }
  .stat .lbl { font-size: .76rem; letter-spacing: .12em; text-transform: uppercase; color: #aab2bd; margin-top: 10px; }
  @media (max-width: 720px) { .stats .wrap { grid-template-columns: repeat(2, 1fr); gap: 32px 16px; } }

  /* ---------- SECTIONS ---------- */
  section { padding: 84px 0; }
  section.alt { background: var(--paper); }
  .sec-head { margin-bottom: 52px; max-width: 760px; }
  .sec-kicker { font-size: .78rem; letter-spacing: .2em; text-transform: uppercase; color: var(--gold); margin-bottom: 14px; }
  .sec-head h2 { font-size: clamp(1.9rem, 4vw, 2.8rem); color: var(--navy); }
  .sec-head p { color: var(--slate); font-size: 1.08rem; margin-top: 18px; }

  /* ---------- ABOUT ---------- */
  .about-grid { display: grid; grid-template-columns: 1fr; gap: 40px; }
  .lead { font-family: 'EB Garamond', serif; font-size: 1.5rem; line-height: 1.5; color: var(--ink); }
  .lead .hl { color: var(--gold); font-style: italic; }
  .about-body { columns: 2; column-gap: 48px; color: var(--slate); font-size: 1.02rem; }
  .about-body p { margin-bottom: 16px; break-inside: avoid; }
  @media (max-width: 720px) { .about-body { columns: 1; } .lead { font-size: 1.25rem; } }

  /* ---------- EXPERTISE ---------- */
  .exp-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 1px; background: var(--line); border: 1px solid var(--line); }
  .exp-card { background: var(--paper); padding: 34px 30px; transition: background .25s; }
  .exp-card:hover { background: var(--accent-bg); }
  .exp-card .ico { width: 40px; height: 40px; display: grid; place-items: center; border: 1px solid var(--gold); border-radius: 50%; color: var(--gold); margin-bottom: 20px; }
  .exp-card .ico svg { width: 20px; height: 20px; }
  .exp-card h3 { font-size: 1.3rem; color: var(--navy); margin-bottom: 10px; }
  .exp-card p { font-size: .95rem; color: var(--slate); }
  @media (max-width: 880px) { .exp-grid { grid-template-columns: repeat(2,1fr); } }
  @media (max-width: 560px) { .exp-grid { grid-template-columns: 1fr; } }

  /* ---------- TIMELINE ---------- */
  .tl-group-label {
    font-size: .8rem; letter-spacing: .18em; text-transform: uppercase; color: var(--gold);
    margin: 0 0 30px; display: flex; align-items: center; gap: 16px;
  }
  .tl-group-label::after { content: ""; flex: 1; height: 1px; background: var(--line); }
  .tl-group-label.second { margin-top: 64px; }
  .timeline { position: relative; padding-left: 34px; }
  .timeline::before { content: ""; position: absolute; left: 7px; top: 8px; bottom: 8px; width: 1px; background: var(--line); }
  .tl-item { position: relative; padding-bottom: 38px; }
  .tl-item:last-child { padding-bottom: 0; }
  .tl-item::before {
    content: ""; position: absolute; left: -34px; top: 7px; width: 15px; height: 15px;
    border-radius: 50%; background: var(--paper); border: 2px solid var(--gold); box-sizing: border-box;
  }
  .tl-item.current::before { background: var(--gold); box-shadow: 0 0 0 4px rgba(176,133,68,.16); }
  .tl-role { font-family: 'EB Garamond', serif; font-size: 1.4rem; color: var(--navy); line-height: 1.25; }
  .tl-org { font-size: 1rem; font-weight: 600; color: var(--gold); margin-top: 3px; }
  .tl-dates { font-size: .82rem; color: var(--muted); letter-spacing: .03em; margin-top: 6px; display: flex; flex-wrap: wrap; gap: 6px 14px; align-items: center; }
  .tl-dates .badge { background: var(--accent-bg); border: 1px solid var(--line); padding: 1px 9px; border-radius: 20px; font-size: .72rem; letter-spacing: .04em; color: var(--slate); }
  .tl-desc { font-size: .96rem; color: var(--slate); margin-top: 12px; max-width: 680px; }
  .tl-desc a { color: var(--gold); border-bottom: 1px solid rgba(176,133,68,.4); }

  /* ---------- ENGAGEMENTS ---------- */
  .eng-grid { display: grid; grid-template-columns: repeat(2, 1fr); gap: 18px; }
  .eng-card { background: var(--paper); border: 1px solid var(--line); border-left: 3px solid var(--gold); padding: 24px 26px; transition: transform .2s, box-shadow .2s; }
  .eng-card:hover { transform: translateY(-2px); box-shadow: var(--shadow); }
  .eng-card .yr { font-size: .78rem; letter-spacing: .1em; color: var(--gold); font-weight: 600; }
  .eng-card h3 { font-size: 1.18rem; color: var(--navy); margin: 6px 0 4px; }
  .eng-card p { font-size: .9rem; color: var(--slate); }
  @media (max-width: 620px) { .eng-grid { grid-template-columns: 1fr; } }

  /* ---------- CONTACT ---------- */
  footer { background: var(--navy); color: #e9e6df; padding: 80px 0 50px; position: relative; overflow: hidden; }
  footer::before { content: ""; position: absolute; left: -100px; bottom: -100px; width: 380px; height: 380px; border-radius: 50%; background: radial-gradient(circle, rgba(176,133,68,.14), transparent 70%); }
  footer .wrap { position: relative; z-index: 2; }
  footer h2 { font-size: clamp(2rem, 4vw, 3rem); color: #fff; max-width: 640px; }
  footer p.sub { color: #aeb6c1; margin-top: 18px; font-size: 1.05rem; max-width: 560px; }
  .contact-links { display: flex; flex-wrap: wrap; gap: 14px; margin-top: 38px; }
  .contact-links a {
    display: inline-flex; align-items: center; gap: 10px; padding: 13px 22px;
    border: 1px solid rgba(255,255,255,.22); border-radius: 2px; font-size: .9rem; transition: all .22s;
  }
  .contact-links a:hover { border-color: var(--gold-soft); background: rgba(176,133,68,.12); }
  .contact-links a.mail { background: var(--gold); border-color: var(--gold); color: #fff; font-weight: 500; letter-spacing: .02em; }
  .contact-links a.mail:hover { background: var(--gold-soft); border-color: var(--gold-soft); transform: translateY(-1px); }
  .contact-links a.wa { background: #1f9d5b; border-color: #1f9d5b; color: #fff; font-weight: 500; letter-spacing: .02em; white-space: nowrap; }
  .contact-links a.wa:hover { background: #27b56b; border-color: #27b56b; transform: translateY(-1px); }
  .contact-links svg { width: 18px; height: 18px; }
  .foot-bottom { margin-top: 60px; padding-top: 26px; border-top: 1px solid rgba(255,255,255,.1); display: flex; justify-content: space-between; flex-wrap: wrap; gap: 12px; font-size: .82rem; color: #8b93a0; }

  /* ---------- REVEAL ANIMATION ---------- */
  .reveal { opacity: 0; transform: translateY(22px); transition: opacity .7s ease, transform .7s ease; }
  .reveal.in { opacity: 1; transform: none; }

  @media print {
    nav, .cta, footer .contact-links { display: none; }
    body { background: #fff; }
    section { padding: 28px 0; }
    .reveal { opacity: 1; transform: none; }
  }
</style>
</head>
<body>

<!-- NAV -->
<nav>
  <div class="wrap">
    <div class="brand">Kevin <span>Yeon</span></div>
    <div class="navlinks">
      <a href="#about">About</a>
      <a href="#expertise">Expertise</a>
      <a href="#experience">Experience</a>
      <a href="#engagements">Engagements</a>
      <a href="#contact">Contact</a>
    </div>
  </div>
</nav>

<!-- HERO -->
<header class="hero">
  <div class="wrap">
    <div class="eyebrow">Startup Ecosystem Leader · Management Advisor</div>
    <h1>Kevin Yeon</h1>
    <div class="ko-name">연규황 · Kyu Hwang Yeon</div>
    <p class="title">Three decades building entrepreneurs and bridging Korea's innovation economy with the global market.</p>
    <div class="meta">
      <span>
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0118 0z"/><circle cx="12" cy="10" r="3"/></svg>
        Seoul, Republic of Korea
      </span>
      <span>
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6"><circle cx="12" cy="12" r="10"/><path d="M2 12h20M12 2a15 15 0 010 20M12 2a15 15 0 000 20"/></svg>
        Global Programs · Asia · Europe · Africa
      </span>
      <span>
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6"><rect x="2" y="7" width="20" height="14" rx="2"/><path d="M16 7V5a2 2 0 00-2-2h-4a2 2 0 00-2 2v2"/></svg>
        30+ Years of Experience
      </span>
    </div>
    <div class="cta">
      <a href="#contact" class="btn primary">Get in Touch</a>
      <a href="https://www.linkedin.com/in/kyuhwang-yeon-59003710a/?locale=en" target="_blank" rel="noopener" class="btn ghost">View LinkedIn</a>
    </div>
  </div>
</header>

<!-- STATS -->
<div class="stats">
  <div class="wrap">
    <div class="stat"><div class="num">30+</div><div class="lbl">Years in the Field</div></div>
    <div class="stat"><div class="num">5</div><div class="lbl">Active Advisory Roles</div></div>
    <div class="stat"><div class="num">3</div><div class="lbl">Continents Mentored</div></div>
    <div class="stat"><div class="num">100s</div><div class="lbl">Startups Supported</div></div>
  </div>
</div>

<!-- ABOUT -->
<section id="about" class="alt">
  <div class="wrap reveal">
    <div class="sec-head">
      <div class="sec-kicker">About</div>
      <h2>From global IT consulting to building the next generation of founders.</h2>
    </div>
    <div class="about-grid">
      <p class="lead">
        Kevin Yeon is a seasoned <span class="hl">startup ecosystem leader</span> and management advisor whose career spans the worlds of global technology research, public innovation policy, and hands-on entrepreneurship development across <span class="hl">Asia, Europe, and Africa.</span>
      </p>
      <div class="about-body">
        <p>His journey began in management consulting, where he rose to lead consulting practices at <strong>Gartner Korea</strong> and later served as Managing Director and Country Manager of <strong>IDC Korea</strong> — shaping how Korean enterprises understood global IT trends, strategy, and market direction.</p>
        <p>From 2014, he turned that expertise toward Korea's innovation economy, serving as Vice President and then President of the <strong>Center for Creative Economy and Innovation (CCEI) in Daegu</strong>, a flagship government agency dedicated to regional innovation and startup growth.</p>
        <p>Today he operates at the intersection of mentorship, investment, and global expansion — advising on startup ecosystems at the <strong>Korea Productivity Center</strong>, mentoring CEOs through the <strong>K-ICT Startup Mentoring Center</strong>, leading <strong>Global Class</strong> in Seoul, and bridging Korean ventures to international markets through <strong>Tansley Korea.</strong></p>
        <p>A recognized voice in entrepreneurship, he has delivered keynotes and mentorship training from India and Portugal to Senegal and Laos.</p>
      </div>
    </div>
  </div>
</section>

<!-- EXPERTISE -->
<section id="expertise">
  <div class="wrap reveal">
    <div class="sec-head">
      <div class="sec-kicker">Areas of Expertise</div>
      <h2>Where strategy meets the founder's journey.</h2>
    </div>
    <div class="exp-grid">
      <div class="exp-card">
        <div class="ico"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6"><path d="M3 21h18M5 21V7l7-4 7 4v14M9 21v-6h6v6"/></svg></div>
        <h3>Startup Ecosystem Building</h3>
        <p>Designing and leading regional and national programs that grow founders, accelerators, and innovation infrastructure.</p>
      </div>
      <div class="exp-card">
        <div class="ico"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6"><circle cx="9" cy="7" r="3"/><path d="M2 21v-2a6 6 0 016-6M16 11l2 2 4-4"/></svg></div>
        <h3>CEO & Founder Mentoring</h3>
        <p>One-on-one and cohort mentorship for early- and growth-stage founders across global mentorship programs.</p>
      </div>
      <div class="exp-card">
        <div class="ico"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6"><path d="M3 3v18h18"/><path d="M7 14l4-4 3 3 5-6"/></svg></div>
        <h3>Global Go-to-Market Strategy</h3>
        <p>Advising ventures on cross-border expansion, IT market trends, and international growth strategy.</p>
      </div>
      <div class="exp-card">
        <div class="ico"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6"><path d="M12 1v22M17 5H9.5a3.5 3.5 0 000 7h5a3.5 3.5 0 010 7H6"/></svg></div>
        <h3>Startup Investment & Acceleration</h3>
        <p>Sourcing, evaluating, and nurturing promising startups as an investment director and accelerator advisor.</p>
      </div>
      <div class="exp-card">
        <div class="ico"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6"><path d="M2 3h6l2 5-3 2a14 14 0 006 6l2-3 5 2v6a2 2 0 01-2 2A18 18 0 012 5a2 2 0 010-2z"/></svg></div>
        <h3>Technology & Market Advisory</h3>
        <p>Decades of enterprise IT research and consulting leadership at Gartner and IDC, translating trends into strategy.</p>
      </div>
      <div class="exp-card">
        <div class="ico"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6"><circle cx="12" cy="12" r="10"/><path d="M2 12h20M12 2a15 15 0 010 20M12 2a15 15 0 000 20"/></svg></div>
        <h3>International Programs</h3>
        <p>Keynote speaking and mentorship training across India, Portugal, Senegal, and Laos for global development bodies.</p>
      </div>
    </div>
  </div>
</section>

<!-- EXPERIENCE -->
<section id="experience" class="alt">
  <div class="wrap reveal">
    <div class="sec-head">
      <div class="sec-kicker">Experience</div>
      <h2>A career spanning research, policy, and entrepreneurship.</h2>
    </div>

    <div class="tl-group-label">Current Roles</div>
    <div class="timeline">
      <div class="tl-item current">
        <div class="tl-role">Technology Startup Instructor</div>
        <div class="tl-org">Korea Entrepreneurship Foundation</div>
        <div class="tl-dates"><span class="badge">Contract</span> Jan 2025 – Present · Seoul, Korea · Hybrid</div>
      </div>
      <div class="tl-item current">
        <div class="tl-role">City Lead — Seoul</div>
        <div class="tl-org">Global Class</div>
        <div class="tl-dates"><span class="badge">Part-time</span> Nov 2023 – Present · Seoul, Korea · Hybrid</div>
        <p class="tl-desc">Spreading the Global Class methodology — created by Wall Street Journal bestselling authors Klaus Wehage and Aaron McDaniel — through local programs and events, building ecosystems of "Interpreneurs" who are creating the next generation of global companies. <a href="https://www.globalgrowthmasterclass.com" target="_blank" rel="noopener">Learn more →</a></p>
      </div>
      <div class="tl-item current">
        <div class="tl-role">CEO Mentor</div>
        <div class="tl-org">K-ICT Startup Mentoring Center</div>
        <div class="tl-dates"><span class="badge">Contract</span> Mar 2023 – Present · Seoul, Korea · Hybrid</div>
        <p class="tl-desc">Mentoring founders and CEOs through Korea's national ICT startup mentoring program. <a href="https://gomentoring.or.kr/" target="_blank" rel="noopener">gomentoring.or.kr →</a></p>
      </div>
      <div class="tl-item current">
        <div class="tl-role">Chief Executive Officer</div>
        <div class="tl-org">Tansley Korea</div>
        <div class="tl-dates"><span class="badge">Self-employed</span> Feb 2023 – Present · Seoul, Korea · Hybrid</div>
        <p class="tl-desc">A service provider that facilitates a bridge between Korean ventures and the global startup ecosystem.</p>
      </div>
      <div class="tl-item current">
        <div class="tl-role">Senior Startup Ecosystem Advisor</div>
        <div class="tl-org">KPC — Korea Productivity Center</div>
        <div class="tl-dates"><span class="badge">Contract</span> Aug 2021 – Present · Seoul, Korea</div>
        <p class="tl-desc">Startup and Entrepreneurship Development Center.</p>
      </div>
    </div>

    <div class="tl-group-label second">Previous Roles</div>
    <div class="timeline">
      <div class="tl-item">
        <div class="tl-role">Investment Director</div>
        <div class="tl-org">Apple Adventure</div>
        <div class="tl-dates"><span class="badge">Full-time</span> Aug 2022 – Mar 2025 · Seoul, Korea · Hybrid</div>
        <p class="tl-desc">A prestigious online marketing service company and startup accelerator based in Daegu, discovering and nurturing promising startups in selected business fields. <a href="https://www.applead.co.kr/" target="_blank" rel="noopener">applead.co.kr →</a></p>
      </div>
      <div class="tl-item">
        <div class="tl-role">Internal Auditor</div>
        <div class="tl-org">Korea Accelerator Association (KAA)</div>
        <div class="tl-dates"><span class="badge">Contract</span> Feb 2022 – Feb 2024 · Daejeon, Korea</div>
        <p class="tl-desc">A non-profit organization registered under the Ministry of SMEs and Startups to foster the startup ecosystem in Korea. <a href="https://www.k-ac.or.kr/" target="_blank" rel="noopener">k-ac.or.kr →</a></p>
      </div>
      <div class="tl-item">
        <div class="tl-role">Chief Expert</div>
        <div class="tl-org">APO — Asian Productivity Organization</div>
        <div class="tl-dates"><span class="badge">Contract</span> Feb 2023 – Dec 2023 · Korea · Remote</div>
        <p class="tl-desc">Led "Emerging Needs Research" across APO member countries.</p>
      </div>
      <div class="tl-item">
        <div class="tl-role">Senator</div>
        <div class="tl-org">World Business Angels Investment Forum (WBAF)</div>
        <div class="tl-dates"><span class="badge">Contract</span> Apr 2021 – Dec 2022 · Seoul, Korea · Hybrid</div>
        <p class="tl-desc">Served as 2021 WBAF Korea Chair, championing angel investment and early-stage financing.</p>
      </div>
      <div class="tl-item">
        <div class="tl-role">President (Head) of CCEI, Daegu</div>
        <div class="tl-org">Center for Creative Economy and Innovation — Daegu</div>
        <div class="tl-dates"><span class="badge">Full-time</span> Jun 2017 – Jun 2020 · Daegu, Korea</div>
        <p class="tl-desc">Led the flagship government agency under the Ministry of SMEs and Startups, driving regional innovation and startup growth.</p>
      </div>
      <div class="tl-item">
        <div class="tl-role">Vice President, Regional Innovation &amp; Startup Strategy</div>
        <div class="tl-org">Center for Creative Economy and Innovation — Daegu</div>
        <div class="tl-dates"><span class="badge">Full-time</span> Jul 2014 – Jun 2017 · Daegu, Korea</div>
        <p class="tl-desc">A government agency under the Ministry of Science, ICT &amp; Future Planning.</p>
      </div>
      <div class="tl-item">
        <div class="tl-role">Chief Executive Officer</div>
        <div class="tl-org">Khypartners</div>
        <div class="tl-dates"><span class="badge">Full-time</span> Mar 2011 – Jun 2014 · Seoul, Korea</div>
        <p class="tl-desc">Global go-to-market strategy and IT-trend, strategy, and IT-market business consulting services.</p>
      </div>
      <div class="tl-item">
        <div class="tl-role">Managing Director (Country Manager)</div>
        <div class="tl-org">IDC Korea</div>
        <div class="tl-dates"><span class="badge">Full-time</span> Feb 2008 – Jul 2010 · Seoul, Korea · On-site</div>
        <p class="tl-desc">Led the Korean operations of the global IT market intelligence firm as Country Manager.</p>
      </div>
      <div class="tl-item">
        <div class="tl-role">Managing Partner</div>
        <div class="tl-org">Gartner</div>
        <div class="tl-dates"><span class="badge">Full-time</span> Aug 2000 – Jan 2008 · Seoul, Korea</div>
        <p class="tl-desc">Consulting leader at Gartner Inc. (Korea office), guiding enterprise clients on technology strategy.</p>
      </div>
      <div class="tl-item">
        <div class="tl-role">Senior Consultant</div>
        <div class="tl-org">KPC — Korea Productivity Center</div>
        <div class="tl-dates"><span class="badge">Full-time</span> Jan 1991 – Apr 1992 · Korea</div>
        <p class="tl-desc">Office Automation (OA) Consulting Division.</p>
      </div>
    </div>
  </div>
</section>

<!-- ENGAGEMENTS -->
<section id="engagements">
  <div class="wrap reveal">
    <div class="sec-head">
      <div class="sec-kicker">Speaking & Global Engagements</div>
      <h2>Sharing the entrepreneurial mindset across the world.</h2>
    </div>
    <div class="eng-grid">
      <div class="eng-card">
        <div class="yr">2022</div>
        <h3>Mentorship Summer Training — UCAD, Senegal</h3>
        <p>Graduation ceremony for 20 successful mentor trainees. #MentorshipSummerTraining</p>
      </div>
      <div class="eng-card">
        <div class="yr">Program</div>
        <h3>Mentorship Training — Laos Youth Union</h3>
        <p>Capacity-building mentorship training for emerging founders in Laos.</p>
      </div>
      <div class="eng-card">
        <div class="yr">2018</div>
        <h3>AICTE Startup Event — India</h3>
        <p>Keynote speech to Indian engineering students on entrepreneurship and innovation.</p>
      </div>
      <div class="eng-card">
        <div class="yr">2017</div>
        <h3>INL Conference — Braga, Portugal</h3>
        <p>International conference engagement at the Iberian Nanotechnology Laboratory.</p>
      </div>
      <div class="eng-card">
        <div class="yr">2019</div>
        <h3>Daegu Startup Awards</h3>
        <p>Hosting and recognizing the region's most promising founders and ventures.</p>
      </div>
      <div class="eng-card">
        <div class="yr">2014</div>
        <h3>KBS Documentary — "Startup for Future"</h3>
        <p>Featured in a national broadcast exploring Korea's startup movement.</p>
      </div>
    </div>
  </div>
</section>

<!-- CONTACT -->
<footer id="contact">
  <div class="wrap">
    <h2>Let's build the next generation of global companies.</h2>
    <p class="sub">Open to advisory engagements, mentorship, keynote speaking, and cross-border collaboration between Korea and the world.</p>
    <div class="contact-links">
      <a class="mail" href="mailto:kyeon7@gmail.com?subject=Inquiry%20from%20your%20CV%20website" aria-label="Send an email to kyeon7@gmail.com" title="Email kyeon7@gmail.com">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.7"><rect x="2.5" y="4.5" width="19" height="15" rx="2"/><path d="M3 6l9 6.5L21 6"/></svg>
        kyeon7@gmail.com
      </a>
      <a class="wa" href="https://wa.me/821051006540" target="_blank" rel="noopener" aria-label="Chat on WhatsApp: +82 10 5100 6540" title="WhatsApp +82 10 5100 6540">
        <svg viewBox="0 0 24 24" fill="currentColor"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"/></svg>
        WhatsApp · +82 10 5100 6540
      </a>
    </div>
    <div class="foot-bottom">
      <span>© 2026 Kevin (Kyuhwang) Yeon · 연규황</span>
      <span>Seoul, Republic of Korea</span>
    </div>
  </div>
</footer>

<script>
  const io = new IntersectionObserver((entries) => {
    entries.forEach(e => { if (e.isIntersecting) { e.target.classList.add('in'); io.unobserve(e.target); } });
  }, { threshold: 0.12 });
  document.querySelectorAll('.reveal').forEach(el => io.observe(el));

  // Anchor navigation: smooth scroll with an instant-jump fallback for
  // environments where smooth scrolling is unavailable (reduced motion, webviews).
  const navH = document.querySelector('nav').offsetHeight;
  document.querySelectorAll('a[href^="#"]').forEach(a => {
    a.addEventListener('click', (e) => {
      const target = document.querySelector(a.getAttribute('href'));
      if (!target) return;
      e.preventDefault();
      const top = target.getBoundingClientRect().top + window.scrollY - navH;
      const startY = window.scrollY;
      window.scrollTo({ top, behavior: 'smooth' });
      history.pushState(null, '', a.getAttribute('href'));
      setTimeout(() => {
        if (Math.abs(window.scrollY - startY) < 2 && Math.abs(top - startY) > 2) {
          window.scrollTo({ top, behavior: 'instant' });
        }
      }, 300);
    });
  });
</script>
</body>
</html>
