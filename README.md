<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>연규황 (延圭晃) | Profile</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;500;600;700&family=Inter:wght@300;400;500;600;700&family=Noto+Serif+KR:wght@400;500;600;700&display=swap" rel="stylesheet">
<style>
  :root {
    --bg: #f4f1ec;
    --paper: #ffffff;
    --ink: #0f1a2e;
    --ink-soft: #334155;
    --muted: #6b7280;
    --line: #e2ddd4;
    --accent: #8b6f3f;
    --accent-deep: #6b5530;
    --navy: #0b2545;
    --navy-light: #15366b;
  }

  * { box-sizing: border-box; }
  html, body { margin: 0; padding: 0; }

  body {
    font-family: "Inter", "Noto Serif KR", -apple-system, BlinkMacSystemFont, sans-serif;
    background: var(--bg);
    color: var(--ink);
    line-height: 1.65;
    -webkit-font-smoothing: antialiased;
  }

  /* ───── Top Nav ───── */
  nav.top {
    position: sticky;
    top: 0;
    z-index: 50;
    background: rgba(255, 255, 255, 0.92);
    backdrop-filter: blur(12px);
    border-bottom: 1px solid var(--line);
  }

  .nav-inner {
    max-width: 1080px;
    margin: 0 auto;
    padding: 14px 32px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .brand {
    font-family: "Cormorant Garamond", serif;
    font-size: 18px;
    font-weight: 600;
    letter-spacing: 4px;
    color: var(--navy);
  }

  .brand span { color: var(--accent); }

  .nav-links {
    display: flex;
    gap: 28px;
    font-size: 12px;
    letter-spacing: 1.5px;
    text-transform: uppercase;
  }

  .nav-links a {
    color: var(--ink-soft);
    text-decoration: none;
    transition: color 0.2s;
    font-weight: 500;
  }

  .nav-links a:hover { color: var(--accent); }

  /* ───── Hero ───── */
  .hero {
    background: linear-gradient(135deg, var(--navy) 0%, var(--navy-light) 100%);
    color: #fff;
    padding: 100px 32px 80px;
    position: relative;
    overflow: hidden;
  }

  .hero::before {
    content: "";
    position: absolute;
    inset: 0;
    background-image:
      radial-gradient(circle at 80% 20%, rgba(139, 111, 63, 0.22), transparent 50%),
      radial-gradient(circle at 10% 90%, rgba(139, 111, 63, 0.12), transparent 50%);
    pointer-events: none;
  }

  .hero-inner {
    max-width: 1080px;
    margin: 0 auto;
    position: relative;
    z-index: 1;
    display: grid;
    grid-template-columns: 1fr auto;
    gap: 48px;
    align-items: center;
  }

  .eyebrow {
    font-family: "Cormorant Garamond", serif;
    font-size: 13px;
    letter-spacing: 8px;
    color: var(--accent);
    text-transform: uppercase;
    margin-bottom: 24px;
    font-weight: 500;
  }

  .hero h1 {
    font-family: "Noto Serif KR", serif;
    font-size: 72px;
    font-weight: 600;
    margin: 0 0 12px;
    letter-spacing: -2px;
    line-height: 1;
  }

  .hero h1 .hanja {
    font-size: 36px;
    color: rgba(255, 255, 255, 0.45);
    font-weight: 400;
    margin-left: 12px;
  }

  .hero .en {
    font-family: "Cormorant Garamond", serif;
    font-size: 24px;
    color: rgba(255, 255, 255, 0.7);
    letter-spacing: 8px;
    margin-bottom: 32px;
    text-transform: uppercase;
  }

  .hero .lede {
    font-family: "Cormorant Garamond", "Noto Serif KR", serif;
    font-size: 22px;
    font-style: italic;
    color: rgba(255, 255, 255, 0.9);
    line-height: 1.6;
    max-width: 620px;
    margin: 0 0 36px;
    font-weight: 400;
    padding-left: 20px;
    border-left: 2px solid var(--accent);
  }

  .pill-row {
    display: flex;
    gap: 10px;
    flex-wrap: wrap;
  }

  .pill {
    padding: 7px 16px;
    border: 1px solid rgba(255, 255, 255, 0.25);
    border-radius: 100px;
    font-size: 12px;
    letter-spacing: 1px;
    color: rgba(255, 255, 255, 0.9);
    background: rgba(255, 255, 255, 0.05);
  }

  .portrait {
    width: 220px;
    height: 280px;
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.08), rgba(255, 255, 255, 0.02));
    border: 1px solid rgba(255, 255, 255, 0.15);
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
  }

  .portrait::before {
    content: "延圭晃";
    font-family: "Noto Serif KR", serif;
    font-size: 64px;
    color: rgba(255, 255, 255, 0.12);
    letter-spacing: 4px;
    writing-mode: vertical-rl;
  }

  .portrait::after {
    content: "";
    position: absolute;
    top: 16px; right: 16px;
    width: 24px;
    height: 24px;
    border-top: 2px solid var(--accent);
    border-right: 2px solid var(--accent);
  }

  /* ───── Quick Stats ───── */
  .stats {
    background: var(--paper);
    border-top: 1px solid var(--line);
    border-bottom: 1px solid var(--line);
  }

  .stats-inner {
    max-width: 1080px;
    margin: 0 auto;
    padding: 36px 32px;
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 32px;
  }

  .stat {
    text-align: center;
    border-right: 1px solid var(--line);
  }

  .stat:last-child { border-right: none; }

  .stat-num {
    font-family: "Cormorant Garamond", serif;
    font-size: 48px;
    font-weight: 600;
    color: var(--navy);
    line-height: 1;
    letter-spacing: -1px;
  }

  .stat-num .plus {
    color: var(--accent);
    font-size: 32px;
    vertical-align: super;
  }

  .stat-label {
    font-size: 11px;
    letter-spacing: 2px;
    text-transform: uppercase;
    color: var(--muted);
    margin-top: 10px;
  }

  /* ───── Sections ───── */
  section.block {
    max-width: 1080px;
    margin: 0 auto;
    padding: 80px 32px;
  }

  .block-head {
    display: flex;
    align-items: baseline;
    gap: 24px;
    margin-bottom: 48px;
    padding-bottom: 16px;
    border-bottom: 1px solid var(--line);
  }

  .block-num {
    font-family: "Cormorant Garamond", serif;
    font-size: 14px;
    letter-spacing: 3px;
    color: var(--accent);
    font-weight: 600;
  }

  .block-head h2 {
    font-family: "Noto Serif KR", serif;
    font-size: 36px;
    font-weight: 600;
    color: var(--navy);
    margin: 0;
    letter-spacing: -1px;
  }

  .block-head .en {
    font-family: "Cormorant Garamond", serif;
    font-style: italic;
    color: var(--muted);
    font-size: 16px;
    margin-left: auto;
    letter-spacing: 1px;
  }

  /* ───── About ───── */
  #about {
    background: var(--paper);
  }

  .about-grid {
    display: grid;
    grid-template-columns: 1fr 320px;
    gap: 64px;
  }

  .about-text p {
    font-size: 16px;
    color: var(--ink-soft);
    line-height: 1.9;
    margin: 0 0 18px;
  }

  .about-text p:first-of-type::first-letter {
    font-family: "Cormorant Garamond", serif;
    font-size: 64px;
    float: left;
    line-height: 1;
    margin: 6px 12px 0 0;
    color: var(--accent);
    font-weight: 600;
  }

  .info-card {
    background: #faf8f4;
    border: 1px solid var(--line);
    padding: 32px;
  }

  .info-card h3 {
    font-family: "Cormorant Garamond", serif;
    font-size: 12px;
    letter-spacing: 3px;
    text-transform: uppercase;
    color: var(--accent-deep);
    margin: 0 0 18px;
    padding-bottom: 10px;
    border-bottom: 1.5px solid var(--accent);
  }

  .info-card dl {
    margin: 0;
    font-size: 13.5px;
  }

  .info-card dt {
    color: var(--muted);
    font-size: 10.5px;
    letter-spacing: 1.5px;
    text-transform: uppercase;
    margin-top: 16px;
    margin-bottom: 3px;
    font-weight: 600;
  }

  .info-card dt:first-child { margin-top: 0; }

  .info-card dd {
    margin: 0;
    color: var(--ink-soft);
    line-height: 1.6;
  }

  /* ───── Timeline ───── */
  #experience { background: #faf8f4; }

  .timeline {
    position: relative;
    padding-left: 0;
    list-style: none;
    margin: 0;
  }

  .timeline::before {
    content: "";
    position: absolute;
    left: 120px;
    top: 8px;
    bottom: 8px;
    width: 1.5px;
    background: var(--line);
  }

  .tl-item {
    display: grid;
    grid-template-columns: 100px 40px 1fr;
    gap: 16px;
    padding-bottom: 28px;
    position: relative;
  }

  .tl-period {
    font-family: "Cormorant Garamond", serif;
    font-size: 13px;
    font-weight: 600;
    color: var(--accent-deep);
    letter-spacing: 1px;
    text-align: right;
    padding-top: 4px;
  }

  .tl-dot {
    width: 14px;
    height: 14px;
    border-radius: 50%;
    background: var(--paper);
    border: 2.5px solid var(--accent);
    margin: 8px auto 0;
    position: relative;
    z-index: 1;
  }

  .tl-item.current .tl-dot {
    background: var(--accent);
    box-shadow: 0 0 0 4px rgba(139, 111, 63, 0.18);
  }

  .tl-content {
    background: var(--paper);
    border: 1px solid var(--line);
    padding: 18px 22px;
    transition: all 0.2s;
  }

  .tl-content:hover {
    border-color: var(--accent);
    box-shadow: 0 8px 20px -8px rgba(139, 111, 63, 0.2);
  }

  .tl-org {
    font-family: "Noto Serif KR", serif;
    font-size: 16px;
    font-weight: 600;
    color: var(--ink);
    margin: 0 0 4px;
    letter-spacing: -0.3px;
  }

  .tl-role {
    font-size: 13.5px;
    color: var(--ink-soft);
    margin: 0;
  }

  .tl-tag {
    display: inline-block;
    margin-left: 8px;
    padding: 2px 8px;
    background: var(--accent);
    color: #fff;
    font-size: 9.5px;
    letter-spacing: 1px;
    text-transform: uppercase;
    font-weight: 600;
    vertical-align: middle;
  }

  /* ───── Highlights / Cards ───── */
  #insights { background: var(--paper); }

  .grid-3 {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 24px;
  }

  .card {
    background: #faf8f4;
    border: 1px solid var(--line);
    padding: 32px 28px;
    transition: all 0.2s;
  }

  .card:hover {
    border-color: var(--accent);
    transform: translateY(-3px);
  }

  .card-icon {
    font-family: "Cormorant Garamond", serif;
    font-size: 28px;
    color: var(--accent);
    margin-bottom: 14px;
    font-style: italic;
    font-weight: 600;
  }

  .card h3 {
    font-family: "Noto Serif KR", serif;
    font-size: 18px;
    font-weight: 600;
    color: var(--navy);
    margin: 0 0 10px;
  }

  .card p {
    font-size: 14px;
    color: var(--ink-soft);
    line-height: 1.7;
    margin: 0;
  }

  /* ───── Media & Speaking ───── */
  #media { background: #faf8f4; }

  .two-col {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 48px;
  }

  .sub-block h3 {
    font-family: "Cormorant Garamond", serif;
    font-size: 13px;
    letter-spacing: 2.5px;
    text-transform: uppercase;
    color: var(--accent-deep);
    margin: 0 0 18px;
    padding-bottom: 10px;
    border-bottom: 1.5px solid var(--accent);
  }

  .item-list {
    list-style: none;
    padding: 0;
    margin: 0;
  }

  .item-list li {
    padding: 14px 0;
    border-bottom: 1px dashed var(--line);
    font-size: 14px;
    color: var(--ink-soft);
    line-height: 1.6;
    display: grid;
    grid-template-columns: 80px 1fr;
    gap: 16px;
    align-items: baseline;
  }

  .item-list li:last-child { border-bottom: none; }

  .item-date {
    font-family: "Cormorant Garamond", serif;
    font-size: 12px;
    color: var(--accent-deep);
    font-weight: 600;
    letter-spacing: 0.5px;
  }

  .item-outlet {
    font-weight: 600;
    color: var(--ink);
  }

  /* ───── Global / Publications ───── */
  #global { background: var(--paper); }

  .global-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 20px;
  }

  .global-card {
    border: 1px solid var(--line);
    padding: 24px;
    display: flex;
    gap: 18px;
    align-items: flex-start;
  }

  .flag {
    width: 44px;
    height: 44px;
    background: var(--navy);
    color: var(--accent);
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: "Cormorant Garamond", serif;
    font-weight: 700;
    font-size: 14px;
    letter-spacing: 1px;
    flex-shrink: 0;
  }

  .global-card h4 {
    font-family: "Noto Serif KR", serif;
    font-size: 15px;
    margin: 0 0 4px;
    color: var(--ink);
    line-height: 1.4;
  }

  .global-card p {
    font-size: 12.5px;
    color: var(--muted);
    margin: 0;
    line-height: 1.5;
  }

  .global-card .city {
    color: var(--accent-deep);
    font-weight: 600;
  }

  /* ───── Footer ───── */
  footer {
    background: var(--navy);
    color: rgba(255, 255, 255, 0.7);
    padding: 56px 32px 32px;
    text-align: center;
  }

  footer .seal {
    font-family: "Cormorant Garamond", serif;
    font-size: 16px;
    font-style: italic;
    color: var(--accent);
    margin-bottom: 12px;
    letter-spacing: 1px;
  }

  footer .copy {
    font-size: 11px;
    letter-spacing: 2px;
    text-transform: uppercase;
    color: rgba(255, 255, 255, 0.45);
    margin-top: 24px;
    padding-top: 24px;
    border-top: 1px solid rgba(255, 255, 255, 0.12);
  }

  /* ───── Responsive ───── */
  @media (max-width: 860px) {
    .hero { padding: 64px 24px 56px; }
    .hero-inner { grid-template-columns: 1fr; }
    .portrait { width: 100%; height: 200px; }
    .hero h1 { font-size: 48px; }
    .hero h1 .hanja { font-size: 24px; }
    .hero .lede { font-size: 17px; }
    .stats-inner { grid-template-columns: repeat(2, 1fr); gap: 24px; }
    .stat:nth-child(2) { border-right: none; }
    section.block { padding: 56px 24px; }
    .block-head h2 { font-size: 26px; }
    .block-head .en { display: none; }
    .about-grid { grid-template-columns: 1fr; gap: 32px; }
    .two-col { grid-template-columns: 1fr; gap: 32px; }
    .grid-3 { grid-template-columns: 1fr; }
    .global-grid { grid-template-columns: 1fr; }
    .timeline::before { left: 70px; }
    .tl-item { grid-template-columns: 60px 24px 1fr; gap: 10px; }
    .tl-period { font-size: 11px; }
    .nav-links { display: none; }
  }

  @media print {
    body { background: #fff; }
    nav.top { display: none; }
  }
</style>
</head>
<body>

  <nav class="top">
    <div class="nav-inner">
      <div class="brand">YEON <span>·</span> KH</div>
      <div class="nav-links">
        <a href="#about">About</a>
        <a href="#experience">Career</a>
        <a href="#insights">Expertise</a>
        <a href="#media">Media</a>
        <a href="#global">Global</a>
      </div>
    </div>
  </nav>

  <!-- HERO -->
  <header class="hero">
    <div class="hero-inner">
      <div>
        <div class="eyebrow">Personal Profile · Mar 2026</div>
        <h1>연규황<span class="hanja">延圭晃</span></h1>
        <div class="en">YEON KYU HWANG</div>
        <p class="lede">
          글로벌 IT 어드바이저리에서 출발해 지역 혁신 생태계와 스타트업 투자까지 —
          25년간 전략·정책·자본을 잇는 다리를 놓아 온 시니어 프로페셔널.
        </p>
        <div class="pill-row">
          <span class="pill">Startup Investment</span>
          <span class="pill">Innovation Strategy</span>
          <span class="pill">Mentorship</span>
          <span class="pill">Global Ecosystem</span>
        </div>
      </div>
      <div class="portrait"></div>
    </div>
  </header>

  <!-- STATS -->
  <section class="stats">
    <div class="stats-inner">
      <div class="stat">
        <div class="stat-num">25<span class="plus">+</span></div>
        <div class="stat-label">Years of Practice</div>
      </div>
      <div class="stat">
        <div class="stat-num">100<span class="plus">+</span></div>
        <div class="stat-label">Lectures Delivered</div>
      </div>
      <div class="stat">
        <div class="stat-num">5</div>
        <div class="stat-label">Int'l Keynotes</div>
      </div>
      <div class="stat">
        <div class="stat-num">6</div>
        <div class="stat-label">Active Roles</div>
      </div>
    </div>
  </section>

  <!-- ABOUT -->
  <section id="about" class="block">
    <div class="block-head">
      <span class="block-num">01</span>
      <h2>About</h2>
      <span class="en">— Profile</span>
    </div>

    <div class="about-grid">
      <div class="about-text">
        <p>
          연규황은 글로벌 리서치·자문 기관에서 출발해 산업 컨설팅, 공공 혁신 기관, 그리고 벤처 투자
          영역까지 폭넓은 경력을 쌓아 온 시니어 전문가입니다. Gartner Research Advisory Korea의
          매니징 파트너와 한국 IDC 지사장을 거치며 국내외 대기업의 IT 전략 의사결정을 자문해 왔고,
          이후 대구창조경제혁신센터 2대 센터장으로 부임해 지역 단위 창업 생태계 구축을 총괄했습니다.
        </p>
        <p>
          현재는 포스케일1호 펀드 투자팀장, 탠슬리 코리아 대표, Global Class Seoul City Lead로
          활동하며 초기 스타트업 투자와 글로벌 시장 진출 자문에 집중하고 있습니다. 동시에
          한국기업가정신재단의 I-Corps 인스트럭터·K-ICT 멘토, 한국창업학회 부회장으로 학계와
          정책 현장을 잇는 가교 역할을 이어가고 있습니다.
        </p>
        <p>
          OECD, UNDP, AICTE 등 국제 기구와 컨퍼런스에서 한국의 창업·혁신 전략을 영문으로 발표해
          왔으며, APO(Asian Productivity Organization)의 SME 사업연속성 보고서 Chief Editor로
          참여하는 등 글로벌 무대에서도 한국형 혁신 모델의 사례를 알리고 있습니다.
        </p>
      </div>

      <aside class="info-card">
        <h3>At a Glance</h3>
        <dl>
          <dt>姓 名</dt>
          <dd>연규황 (延圭晃)</dd>

          <dt>生年月日</dt>
          <dd>1964. 4. 30</dd>

          <dt>Education</dt>
          <dd>
            영국 Aston University<br>경영학 박사수료 · 1997<br><br>
            영국 University of Hull<br>경영과학 석사 · 1988
          </dd>

          <dt>Domains</dt>
          <dd>Venture Investment · Innovation Policy · IT Advisory · Entrepreneurship Education</dd>

          <dt>Languages</dt>
          <dd>Korean (Native) · English (Professional)</dd>
        </dl>
      </aside>
    </div>
  </section>

  <!-- EXPERIENCE -->
  <section id="experience" class="block">
    <div class="block-head">
      <span class="block-num">02</span>
      <h2>Career</h2>
      <span class="en">— Professional Journey</span>
    </div>

    <ul class="timeline">
      <li class="tl-item current">
        <div class="tl-period">2024 — 現</div>
        <div class="tl-dot"></div>
        <div class="tl-content">
          <h3 class="tl-org">포스케일1호 펀드 <span class="tl-tag">Current</span></h3>
          <p class="tl-role">전문엔젤 · 투자팀장</p>
        </div>
      </li>
      <li class="tl-item current">
        <div class="tl-period">2024 — 現</div>
        <div class="tl-dot"></div>
        <div class="tl-content">
          <h3 class="tl-org">Global Class</h3>
          <p class="tl-role">Seoul City Lead</p>
        </div>
      </li>
      <li class="tl-item current">
        <div class="tl-period">2024 — 現</div>
        <div class="tl-dot"></div>
        <div class="tl-content">
          <h3 class="tl-org">한국기업가정신재단</h3>
          <p class="tl-role">I-Corps 인스트럭터</p>
        </div>
      </li>
      <li class="tl-item current">
        <div class="tl-period">2023 — 現</div>
        <div class="tl-dot"></div>
        <div class="tl-content">
          <h3 class="tl-org">탠슬리 코리아 (Tansley Korea)</h3>
          <p class="tl-role">대표</p>
        </div>
      </li>
      <li class="tl-item current">
        <div class="tl-period">2023 — 現</div>
        <div class="tl-dot"></div>
        <div class="tl-content">
          <h3 class="tl-org">한국창업학회 · 창업벤처학회</h3>
          <p class="tl-role">한국창업학회 부회장 · 창업벤처학회 이사</p>
        </div>
      </li>
      <li class="tl-item current">
        <div class="tl-period">2023 — 現</div>
        <div class="tl-dot"></div>
        <div class="tl-content">
          <h3 class="tl-org">K-ICT 멘토링센터</h3>
          <p class="tl-role">멘토 · 한국기업가정신재단</p>
        </div>
      </li>
      <li class="tl-item current">
        <div class="tl-period">2022 — 現</div>
        <div class="tl-dot"></div>
        <div class="tl-content">
          <h3 class="tl-org">㈜애플애드벤처</h3>
          <p class="tl-role">투자부 이사</p>
        </div>
      </li>
      <li class="tl-item">
        <div class="tl-period">2022 — 23</div>
        <div class="tl-dot"></div>
        <div class="tl-content">
          <h3 class="tl-org">㈜한국엑셀러레이터협회</h3>
          <p class="tl-role">감사</p>
        </div>
      </li>
      <li class="tl-item">
        <div class="tl-period">2021 — 22</div>
        <div class="tl-dot"></div>
        <div class="tl-content">
          <h3 class="tl-org">한국생산성본부 스타트업지원센터</h3>
          <p class="tl-role">수석전문위원</p>
        </div>
      </li>
      <li class="tl-item">
        <div class="tl-period">2014 — 20</div>
        <div class="tl-dot"></div>
        <div class="tl-content">
          <h3 class="tl-org">대구창조경제혁신센터</h3>
          <p class="tl-role">제2대 센터장 · 본부장</p>
        </div>
      </li>
      <li class="tl-item">
        <div class="tl-period">2011 — 14</div>
        <div class="tl-dot"></div>
        <div class="tl-content">
          <h3 class="tl-org">㈜카이파트너스</h3>
          <p class="tl-role">대표 컨설턴트</p>
        </div>
      </li>
      <li class="tl-item">
        <div class="tl-period">2008 — 10</div>
        <div class="tl-dot"></div>
        <div class="tl-content">
          <h3 class="tl-org">㈜한국IDC (IDC Korea)</h3>
          <p class="tl-role">한국 지사장</p>
        </div>
      </li>
      <li class="tl-item">
        <div class="tl-period">2000 — 08</div>
        <div class="tl-dot"></div>
        <div class="tl-content">
          <h3 class="tl-org">㈜가트너리서치 어드바이저리 코리아 (Gartner)</h3>
          <p class="tl-role">컨설팅 매니징 파트너</p>
        </div>
      </li>
    </ul>
  </section>

  <!-- INSIGHTS / EXPERTISE -->
  <section id="insights" class="block">
    <div class="block-head">
      <span class="block-num">03</span>
      <h2>Expertise</h2>
      <span class="en">— Core Domains</span>
    </div>

    <div class="grid-3">
      <div class="card">
        <div class="card-icon">i.</div>
        <h3>Venture Investment</h3>
        <p>포스케일1호 펀드 투자팀장 및 애플애드벤처 투자이사로 초기·시리즈 스타트업 발굴과 투자 의사결정을 주도.</p>
      </div>
      <div class="card">
        <div class="card-icon">ii.</div>
        <h3>Innovation Policy</h3>
        <p>대구창조경제혁신센터 센터장으로 지역 단위 창업 생태계를 설계·운영한 경험. OECD·UNDP 등에서 사례 발표.</p>
      </div>
      <div class="card">
        <div class="card-icon">iii.</div>
        <h3>Global Market Entry</h3>
        <p>Global Class Seoul City Lead로 국내 스타트업의 해외 진출과 해외 기업의 한국 시장 진입을 자문.</p>
      </div>
      <div class="card">
        <div class="card-icon">iv.</div>
        <h3>IT Strategy Advisory</h3>
        <p>Gartner Research Advisory 매니징 파트너, 한국IDC 지사장으로 국내외 대기업 IT 전략 자문을 다년간 수행.</p>
      </div>
      <div class="card">
        <div class="card-icon">v.</div>
        <h3>Entrepreneurship Education</h3>
        <p>I-Corps 인스트럭터, K-ICT 멘토, 겸임교수로 100회 이상의 창업·기업가정신 강연 및 멘토링 수행.</p>
      </div>
      <div class="card">
        <div class="card-icon">vi.</div>
        <h3>Academic Leadership</h3>
        <p>한국창업학회 부회장, 창업벤처학회 이사. APO SME 보고서 Chief Editor 등 학술 활동도 활발.</p>
      </div>
    </div>
  </section>

  <!-- MEDIA -->
  <section id="media" class="block">
    <div class="block-head">
      <span class="block-num">04</span>
      <h2>Media &amp; Press</h2>
      <span class="en">— Selected Coverage</span>
    </div>

    <div class="two-col">
      <div class="sub-block">
        <h3>Broadcast · TV / Radio</h3>
        <ul class="item-list">
          <li><span class="item-date">2016.12</span><span><span class="item-outlet">TBC 대구</span> · 시사진단 쾌 — “위기의 창조경제혁신센터”</span></li>
          <li><span class="item-date">2015.09</span><span><span class="item-outlet">KBS 대구</span> · 대구경북 시사진단 — “벤처신화 가능한가?”</span></li>
          <li><span class="item-date">2015.02</span><span><span class="item-outlet">SBS CNBC</span> · 숨가쁘게 달려온 대구창조경제혁신센터 5개월</span></li>
          <li><span class="item-date">2014.12</span><span><span class="item-outlet">KBS</span> · 다큐멘터리 「미래를 창업하라」 1·2부</span></li>
          <li><span class="item-date">2014.10</span><span><span class="item-outlet">SBS CNBC</span> · 창조경제의 요람 — 대구창조경제혁신센터의 이모저모</span></li>
          <li><span class="item-date">2015.08</span><span><span class="item-outlet">대구교통방송</span> · 라디오 생방송</span></li>
        </ul>
      </div>

      <div class="sub-block">
        <h3>Print &amp; Online Press</h3>
        <ul class="item-list">
          <li><span class="item-date">2020.03</span><span><span class="item-outlet">전자신문</span> · 대구창조경제혁신센터, 전국 최초 4개 창업패키지 그랜드슬램</span></li>
          <li><span class="item-date">2020.02</span><span><span class="item-outlet">전자신문</span> · CES 2020에서 느낀 IT 집중화와 분권화에 대한 小考</span></li>
          <li><span class="item-date">2019.09</span><span><span class="item-outlet">Startup Today</span> · 아시아 10대 창업도시를 꿈꾸다</span></li>
          <li><span class="item-date">2019.05</span><span><span class="item-outlet">전자신문</span> · 투자와 성장 연계한 스케일업 지원</span></li>
          <li><span class="item-date">2018.08</span><span><span class="item-outlet">경북신문</span> · 無에서 有를 창조한 연규황 센터장</span></li>
          <li><span class="item-date">2017.06</span><span><span class="item-outlet">영남일보</span> · [이슈경제인] 연규황 센터장</span></li>
        </ul>
      </div>
    </div>
  </section>

  <!-- GLOBAL -->
  <section id="global" class="block">
    <div class="block-head">
      <span class="block-num">05</span>
      <h2>Global Stage</h2>
      <span class="en">— International Speaking &amp; Publications</span>
    </div>

    <h3 style="font-family:'Cormorant Garamond',serif;font-size:13px;letter-spacing:2.5px;text-transform:uppercase;color:var(--accent-deep);margin:0 0 24px;padding-bottom:10px;border-bottom:1.5px solid var(--accent);display:inline-block;">Invited Talks Abroad</h3>

    <div class="global-grid">
      <div class="global-card">
        <div class="flag">FR</div>
        <div>
          <h4>OECD Expert Meeting on Broadening Innovation Policy</h4>
          <p><span class="city">Paris, France</span> · 2018.12 — Workshop 4: Managing Disruptive Technologies. 대구의 와해성 기술주도 지역혁신 사례 발표.</p>
        </div>
      </div>
      <div class="global-card">
        <div class="flag">IN</div>
        <div>
          <h4>Startup Mentorship Program 2018 · AICTE</h4>
          <p><span class="city">India</span> · 2018.06 — All India Council for Technical Education 초청, 기업가정신 기조 강연.</p>
        </div>
      </div>
      <div class="global-card">
        <div class="flag">PT</div>
        <div>
          <h4>INL Summit 2017</h4>
          <p><span class="city">Braga, Portugal</span> · 2017.10 — Session 4: Nanotechnology, Arts and Education 라운드 테이블 패널. 한국의 창조경제혁신전략 소개.</p>
        </div>
      </div>
      <div class="global-card">
        <div class="flag">TR</div>
        <div>
          <h4>UNDP Turkey · 2nd Int'l Conf. on Total Factor Productivity</h4>
          <p><span class="city">Istanbul, Turkey</span> · 2017.03 — Session 6: Learning from International Experience. 한국의 창조경제혁신 전략 소개.</p>
        </div>
      </div>
      <div class="global-card">
        <div class="flag">BR</div>
        <div>
          <h4>The 25th ANPROTEC Conference</h4>
          <p><span class="city">Cuiabá, Brazil</span> · 2015.10 — 한국의 창조경제혁신전략 소개.</p>
        </div>
      </div>
      <div class="global-card">
        <div class="flag">RU</div>
        <div>
          <h4>The 33rd IASP World Conference</h4>
          <p><span class="city">Moscow, Russia</span> · 2016.09 — “An International Cooperation Scheme for STPs and AIs: The Framework of Creative Economy Promotion Program” 공동 발표.</p>
        </div>
      </div>
    </div>

    <h3 style="font-family:'Cormorant Garamond',serif;font-size:13px;letter-spacing:2.5px;text-transform:uppercase;color:var(--accent-deep);margin:56px 0 24px;padding-bottom:10px;border-bottom:1.5px solid var(--accent);display:inline-block;">Selected Publications</h3>

    <ul class="item-list" style="max-width:880px;">
      <li><span class="item-date">2023</span><span><span class="item-outlet">Asian Productivity Organization, Tokyo</span> · Chief Editor / Expert — “Best Strategies Ensuring SME Business Continuity in Advanced APO Economies: Management Practices for Challenging Times”</span></li>
      <li><span class="item-date">2016</span><span><span class="item-outlet">IASP World Conference</span> · Co-author — “An International Cooperation Scheme for STPs and AIs: The Framework of Creative Economy Promotion Program”</span></li>
      <li><span class="item-date">2014</span><span><span class="item-outlet">정보화진흥원</span> · 공저 — ICT 산업의 신수요 창출을 위한 국가정보화전략 정책 연구</span></li>
      <li><span class="item-date">2003</span><span><span class="item-outlet">한국전자거래학회</span> · 공저 — 국내 기업정보화수준평가 실태조사와 평가시스템 발전방안 연구</span></li>
      <li><span class="item-date">1996</span><span><span class="item-outlet">John Wiley &amp; Sons (UK)</span> · Co-author with F. Hewitt — “BPR Perceptions, Practices and Expectations: A UK Study”, <em>The Journal of Corporate Transformation</em>, 3(3), pp. 47–55</span></li>
    </ul>

    <h3 style="font-family:'Cormorant Garamond',serif;font-size:13px;letter-spacing:2.5px;text-transform:uppercase;color:var(--accent-deep);margin:56px 0 24px;padding-bottom:10px;border-bottom:1.5px solid var(--accent);display:inline-block;">Teaching</h3>

    <ul class="item-list" style="max-width:880px;">
      <li><span class="item-date">'18 — '20</span><span><span class="item-outlet">대구가톨릭대학교 · 계명대학교</span> · 겸임교수</span></li>
      <li><span class="item-date">'17 — 現</span><span><span class="item-outlet">경북대 · 계명대 · DGIST · 선문대 외</span> · 100회 이상의 창업·기업가정신 특강 및 행사 참여</span></li>
    </ul>
  </section>

  <!-- FOOTER -->
  <footer>
    <div class="seal">— Yeon Kyu Hwang · 延圭晃 —</div>
    <div style="font-family:'Cormorant Garamond',serif;font-style:italic;font-size:14px;letter-spacing:1px;">
      Bridging Strategy, Capital and People · since 2000
    </div>
    <div class="copy">Profile · March 2026 · Confidential</div>
  </footer>

</body>
</html>
