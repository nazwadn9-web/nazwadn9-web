<svg width="800" height="400" viewBox="0 0 800 400" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
  <defs>
    <!-- Background gradient -->
    <linearGradient id="bg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#1a0533"/>
      <stop offset="50%" stop-color="#2d0f5e"/>
      <stop offset="100%" stop-color="#0d0221"/>
    </linearGradient>
    <radialGradient id="glow1" cx="80%" cy="20%" r="40%">
      <stop offset="0%" stop-color="#7b2ff7" stop-opacity="0.2"/>
      <stop offset="100%" stop-color="#7b2ff7" stop-opacity="0"/>
    </radialGradient>
    <radialGradient id="glow2" cx="15%" cy="80%" r="35%">
      <stop offset="0%" stop-color="#a855f7" stop-opacity="0.15"/>
      <stop offset="100%" stop-color="#a855f7" stop-opacity="0"/>
    </radialGradient>
    <linearGradient id="nameGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#a855f7"/>
      <stop offset="100%" stop-color="#f0c060"/>
    </linearGradient>
    <!-- Robot float animation -->
    <style>
      @keyframes float {
        0%,100% { transform: translateY(0); }
        50%      { transform: translateY(-9px); }
      }
      @keyframes blink {
        0%,88%,100% { transform: scaleY(1); }
        94%         { transform: scaleY(0.08); }
      }
      @keyframes pulse {
        0%,100% { opacity: 0.6; }
        50%     { opacity: 1; }
      }
      @keyframes twinkle0 { 0%,100%{opacity:.1} 50%{opacity:.9} }
      @keyframes twinkle1 { 0%,100%{opacity:.15} 50%{opacity:.8} }
      @keyframes twinkle2 { 0%,100%{opacity:.05} 50%{opacity:1} }
      @keyframes wag {
        0%,100% { transform: rotate(-12deg); }
        50%     { transform: rotate(14deg); }
      }
      @keyframes fadeIn {
        from { opacity: 0; transform: translateX(-14px); }
        to   { opacity: 1; transform: translateX(0); }
      }
      @keyframes popBadge {
        from { opacity: 0; transform: scale(0.6); }
        to   { opacity: 1; transform: scale(1); }
      }
      @keyframes chestPulse {
        0%,100% { r: 5; opacity: 1; }
        50%     { r: 6.5; opacity: 0.7; }
      }
      @keyframes scanline {
        0%   { transform: translateY(0); opacity: 0.4; }
        100% { transform: translateY(42px); opacity: 0; }
      }

      .robot-group { animation: float 3s ease-in-out infinite; }
      .eye-group   { animation: blink 4.5s ease-in-out infinite; transform-origin: 120px 148px; }
      .ant-light   { animation: pulse 2s ease-in-out infinite; }
      .star-a      { animation: twinkle0 var(--d) ease-in-out infinite; }
      .star-b      { animation: twinkle1 var(--d) ease-in-out infinite; }
      .star-c      { animation: twinkle2 var(--d) ease-in-out infinite; }
      .fox-tail    { animation: wag 1.3s ease-in-out infinite; transform-origin: 710px 350px; }
      .greeting    { animation: fadeIn .7s ease both .2s; }
      .badge1      { animation: popBadge .5s ease both .6s; }
      .badge2      { animation: popBadge .5s ease both .75s; }
      .badge3      { animation: popBadge .5s ease both .9s; }
      .chest-inner { animation: chestPulse 2s ease-in-out infinite; }
      .scanline    { animation: scanline 2.5s linear infinite; }
    </style>
  </defs>

  <!-- Background -->
  <rect width="800" height="400" fill="url(#bg)" rx="18"/>
  <rect width="800" height="400" fill="url(#glow1)" rx="18"/>
  <rect width="800" height="400" fill="url(#glow2)" rx="18"/>

  <!-- Border -->
  <rect width="800" height="400" rx="18" fill="none" stroke="#4a1a8c" stroke-width="1.5"/>

  <!-- Stars -->
  <!-- Group A: fast -->
  <circle class="star-a" style="--d:1.8s" cx="42"  cy="22"  r="1.5" fill="white" opacity=".3"/>
  <circle class="star-a" style="--d:2.1s" cx="170" cy="18"  r="1"   fill="white" opacity=".25"/>
  <circle class="star-a" style="--d:1.6s" cx="310" cy="12"  r="1.2" fill="white" opacity=".3"/>
  <circle class="star-a" style="--d:2.4s" cx="480" cy="28"  r="1"   fill="white" opacity=".2"/>
  <circle class="star-a" style="--d:1.9s" cx="620" cy="14"  r="1.5" fill="white" opacity=".35"/>
  <circle class="star-a" style="--d:2.2s" cx="755" cy="35"  r="1.1" fill="white" opacity=".25"/>
  <circle class="star-a" style="--d:1.7s" cx="68"  cy="380" r="1.2" fill="white" opacity=".2"/>
  <circle class="star-a" style="--d:2.0s" cx="230" cy="370" r="1"   fill="white" opacity=".3"/>
  <!-- Group B: medium -->
  <circle class="star-b" style="--d:2.8s" cx="95"  cy="60"  r="1.3" fill="white" opacity=".2"/>
  <circle class="star-b" style="--d:3.2s" cx="260" cy="40"  r="1"   fill="white" opacity=".15"/>
  <circle class="star-b" style="--d:2.6s" cx="560" cy="50"  r="1.4" fill="white" opacity=".25"/>
  <circle class="star-b" style="--d:3.0s" cx="700" cy="70"  r="1"   fill="white" opacity=".2"/>
  <circle class="star-b" style="--d:2.9s" cx="380" cy="360" r="1.2" fill="white" opacity=".18"/>
  <circle class="star-b" style="--d:3.3s" cx="650" cy="380" r="1"   fill="white" opacity=".2"/>
  <!-- Group C: slow -->
  <circle class="star-c" style="--d:4.0s" cx="140" cy="100" r="1.5" fill="white" opacity=".1"/>
  <circle class="star-c" style="--d:4.5s" cx="400" cy="80"  r="1.2" fill="white" opacity=".12"/>
  <circle class="star-c" style="--d:3.8s" cx="780" cy="200" r="1.4" fill="white" opacity=".15"/>
  <circle class="star-c" style="--d:4.2s" cx="20"  cy="200" r="1"   fill="white" opacity=".1"/>

  <!-- ═══════════ ROBOT ═══════════ -->
  <g class="robot-group" style="transform-origin:120px 200px">
    <!-- Shadow -->
    <ellipse cx="120" cy="315" rx="42" ry="7" fill="rgba(123,47,247,0.25)"/>
    <!-- Arms -->
    <rect x="58"  y="170" width="22" height="50" rx="8" fill="#4a1a8c"/>
    <rect x="160" y="170" width="22" height="50" rx="8" fill="#4a1a8c"/>
    <rect x="61"  y="185" width="16" height="20" rx="5" fill="#7b2ff7" opacity=".6"/>
    <rect x="163" y="185" width="16" height="20" rx="5" fill="#7b2ff7" opacity=".6"/>
    <!-- Hands -->
    <rect x="64"  y="215" width="14" height="20" rx="7" fill="#2d0f5e"/>
    <rect x="163" y="215" width="14" height="20" rx="7" fill="#2d0f5e"/>
    <!-- Legs -->
    <rect x="88"  y="270" width="16" height="30" rx="8" fill="#4a1a8c"/>
    <rect x="136" y="270" width="16" height="30" rx="8" fill="#4a1a8c"/>
    <rect x="88"  y="288" width="16" height="18" rx="7" fill="#2d0f5e"/>
    <rect x="136" y="288" width="16" height="18" rx="7" fill="#2d0f5e"/>
    <!-- Body -->
    <rect x="72"  y="162" width="96" height="112" rx="14" fill="#2d0f5e"/>
    <rect x="80"  y="170" width="80" height="96"  rx="10" fill="#150929"/>
    <!-- Scanline effect on chest screen -->
    <clipPath id="screenClip"><rect x="80" y="170" width="80" height="96" rx="10"/></clipPath>
    <rect class="scanline" clip-path="url(#screenClip)" x="80" y="170" width="80" height="3" fill="#a855f7" opacity=".3"/>
    <!-- Chest orb -->
    <circle cx="120" cy="210" r="20" fill="rgba(123,47,247,0.25)" stroke="#7b2ff7" stroke-width="1"/>
    <circle class="chest-inner" cx="120" cy="210" r="12" fill="#a855f7"/>
    <circle cx="120" cy="210" r="6"  fill="#e9d5ff"/>
    <!-- Chest mini LEDs -->
    <rect x="83"  y="240" width="10" height="5" rx="2.5" fill="#4a1a8c"/>
    <rect x="96"  y="240" width="10" height="5" rx="2.5" fill="#7b2ff7"/>
    <rect x="109" y="240" width="10" height="5" rx="2.5" fill="#4a1a8c"/>
    <rect x="122" y="240" width="10" height="5" rx="2.5" fill="#7b2ff7"/>
    <rect x="135" y="240" width="10" height="5" rx="2.5" fill="#4a1a8c"/>
    <!-- Head -->
    <rect x="68"  y="85"  width="104" height="82" rx="18" fill="#3a1270"/>
    <rect x="78"  y="93"  width="84"  height="66" rx="12" fill="#150929"/>
    <!-- Eyes -->
    <g class="eye-group">
      <ellipse cx="100" cy="128" rx="13" ry="15" fill="#0d0221"/>
      <ellipse cx="140" cy="128" rx="13" ry="15" fill="#0d0221"/>
      <circle  cx="100" cy="128" r="10" fill="#7b2ff7"/>
      <circle  cx="140" cy="128" r="10" fill="#7b2ff7"/>
      <circle  cx="100" cy="128" r="5.5" fill="white"/>
      <circle  cx="140" cy="128" r="5.5" fill="white"/>
      <circle  cx="102" cy="125" r="2.2" fill="#c084fc"/>
      <circle  cx="142" cy="125" r="2.2" fill="#c084fc"/>
    </g>
    <!-- Smile -->
    <path d="M106 142 Q120 152 134 142" stroke="#7b2ff7" stroke-width="2.5" fill="none" stroke-linecap="round"/>
    <!-- Ears -->
    <circle cx="66"  cy="122" r="7" fill="#4a1a8c" opacity=".7"/>
    <circle cx="174" cy="122" r="7" fill="#4a1a8c" opacity=".7"/>
    <!-- Antenna -->
    <rect x="112" y="68" width="16" height="20" rx="8" fill="#4a1a8c"/>
    <g class="ant-light">
      <circle cx="120" cy="64" r="10" fill="#2d0f5e" stroke="#7b2ff7" stroke-width="1.2"/>
      <circle cx="120" cy="64" r="5"  fill="#a855f7"/>
      <circle cx="120" cy="64" r="2.5" fill="#f0c060" opacity=".9"/>
    </g>
  </g>

  <!-- ═══════════ TEXT AREA ═══════════ -->
  <!-- Greeting line -->
  <text class="greeting" x="240" y="100" font-family="'Courier New',monospace" font-size="13" fill="#c084fc" letter-spacing="3">// Hello, World!</text>

  <!-- Main name -->
  <text x="238" y="152" font-family="Arial,sans-serif" font-size="46" font-weight="700" fill="white">nasuka</text>
  <text x="452" y="152" font-family="Arial,sans-serif" font-size="46" font-weight="700" fill="url(#nameGrad)">cheese</text>

  <!-- Tagline -->
  <text x="240" y="182" font-family="'Courier New',monospace" font-size="13" fill="#a855f7">✦ Creative Developer &amp; Night Coder</text>

  <!-- Divider line -->
  <line x1="240" y1="198" x2="760" y2="198" stroke="#4a1a8c" stroke-width="1"/>

  <!-- Badges -->
  <!-- Badge 1: Open Source -->
  <g class="badge1">
    <rect x="240" y="210" width="110" height="26" rx="13" fill="rgba(123,47,247,0.2)" stroke="#a855f7" stroke-width="1"/>
    <text x="295" y="227" font-family="'Courier New',monospace" font-size="11" fill="#c084fc" text-anchor="middle">✦ Open Source</text>
  </g>
  <!-- Badge 2: Fast Learner -->
  <g class="badge2">
    <rect x="360" y="210" width="114" height="26" rx="13" fill="rgba(240,192,96,0.15)" stroke="#f0c060" stroke-width="1"/>
    <text x="417" y="227" font-family="'Courier New',monospace" font-size="11" fill="#f0c060" text-anchor="middle">⚡ Fast Learner</text>
  </g>
  <!-- Badge 3: Night Coder -->
  <g class="badge3">
    <rect x="484" y="210" width="110" height="26" rx="13" fill="rgba(103,232,249,0.1)" stroke="#67e8f9" stroke-width="1"/>
    <text x="539" y="227" font-family="'Courier New',monospace" font-size="11" fill="#67e8f9" text-anchor="middle">◈ Night Coder</text>
  </g>

  <!-- Divider 2 -->
  <line x1="240" y1="252" x2="760" y2="252" stroke="#2d0f5e" stroke-width="1"/>

  <!-- Gmail card -->
  <rect x="240" y="264" width="220" height="46" rx="10" fill="rgba(255,255,255,0.05)" stroke="rgba(168,85,247,0.3)" stroke-width="1"/>
  <!-- Gmail icon -->
  <rect x="254" y="272" width="22" height="22" rx="4" fill="rgba(123,47,247,0.25)"/>
  <path d="M257 277 h16 v12 h-16 z" fill="none" stroke="#c084fc" stroke-width="1"/>
  <path d="M257 278 l8 6 8-6" stroke="#a855f7" stroke-width="1.2" fill="none" stroke-linecap="round"/>
  <text x="282" y="279" font-family="'Courier New',monospace" font-size="9" fill="#7b2ff7">GMAIL</text>
  <text x="282" y="293" font-family="'Courier New',monospace" font-size="12" fill="#e9d5ff">nasukacheese</text>

  <!-- TikTok card -->
  <rect x="474" y="264" width="200" height="46" rx="10" fill="rgba(255,255,255,0.05)" stroke="rgba(168,85,247,0.3)" stroke-width="1"/>
  <!-- TikTok icon -->
  <rect x="488" y="272" width="22" height="22" rx="4" fill="rgba(123,47,247,0.25)"/>
  <circle cx="495" cy="289" r="3.5" fill="none" stroke="#c084fc" stroke-width="1"/>
  <path d="M499 279 c0 3 2 5 4.5 5.5" stroke="#a855f7" stroke-width="1.2" stroke-linecap="round" fill="none"/>
  <line x1="499" y1="279" x2="499" y2="287" stroke="#a855f7" stroke-width="1.2" stroke-linecap="round"/>
  <text x="516" y="279" font-family="'Courier New',monospace" font-size="9" fill="#7b2ff7">TIKTOK</text>
  <text x="516" y="293" font-family="'Courier New',monospace" font-size="12" fill="#e9d5ff">@viol_118</text>

  <!-- Stats row -->
  <!-- Repo box -->
  <rect x="240" y="326" width="152" height="54" rx="10" fill="rgba(255,255,255,0.04)" stroke="rgba(168,85,247,0.2)" stroke-width="1"/>
  <text x="316" y="352" font-family="Arial,sans-serif" font-size="22" font-weight="700" fill="#a855f7" text-anchor="middle">42</text>
  <text x="316" y="368" font-family="'Courier New',monospace" font-size="10" fill="#7b2ff7" text-anchor="middle">Repositories</text>

  <!-- Contrib box -->
  <rect x="404" y="326" width="152" height="54" rx="10" fill="rgba(255,255,255,0.04)" stroke="rgba(168,85,247,0.2)" stroke-width="1"/>
  <text x="480" y="352" font-family="Arial,sans-serif" font-size="22" font-weight="700" fill="#a855f7" text-anchor="middle">128</text>
  <text x="480" y="368" font-family="'Courier New',monospace" font-size="10" fill="#7b2ff7" text-anchor="middle">Contributions</text>

  <!-- LOC box -->
  <rect x="568" y="326" width="152" height="54" rx="10" fill="rgba(255,255,255,0.04)" stroke="rgba(168,85,247,0.2)" stroke-width="1"/>
  <text x="644" y="355" font-family="Arial,sans-serif" font-size="22" font-weight="700" fill="#a855f7" text-anchor="middle">∞</text>
  <text x="644" y="368" font-family="'Courier New',monospace" font-size="10" fill="#7b2ff7" text-anchor="middle">Lines of Code</text>

  <!-- ═══════════ FOX ═══════════ -->
  <!-- Fox tail (animated) -->
  <g class="fox-tail">
    <ellipse cx="718" cy="353" rx="28" ry="14" fill="#7b2ff7" opacity=".85"/>
    <ellipse cx="728" cy="343" rx="18" ry="10" fill="#4a1a8c"/>
    <ellipse cx="734" cy="338" rx="9"  ry="6"  fill="#e9d5ff" opacity=".4"/>
  </g>
  <!-- Fox shadow -->
  <ellipse cx="700" cy="390" rx="28" ry="7" fill="rgba(123,47,247,0.2)"/>
  <!-- Fox legs -->
  <rect x="686" y="350" width="12" height="28" rx="6" fill="#4a1a8c"/>
  <rect x="702" y="350" width="12" height="28" rx="6" fill="#4a1a8c"/>
  <rect x="688" y="364" width="10" height="16" rx="5" fill="#2d0f5e"/>
  <rect x="704" y="364" width="10" height="16" rx="5" fill="#2d0f5e"/>
  <!-- Fox body -->
  <ellipse cx="700" cy="340" rx="26" ry="22" fill="#3a1270"/>
  <ellipse cx="700" cy="343" rx="20" ry="16" fill="#4a1a8c"/>
  <!-- Fox ears -->
  <ellipse cx="686" cy="323" rx="8" ry="12" fill="#3a1270" transform="rotate(-20 686 323)"/>
  <ellipse cx="714" cy="323" rx="8" ry="12" fill="#3a1270" transform="rotate(20 714 323)"/>
  <ellipse cx="686" cy="324" rx="4" ry="6"  fill="#7b2ff7" transform="rotate(-20 686 324)"/>
  <ellipse cx="714" cy="324" rx="4" ry="6"  fill="#7b2ff7" transform="rotate(20 714 324)"/>
  <!-- Fox eyes -->
  <circle cx="694" cy="338" r="5.5" fill="#0d0221"/>
  <circle cx="706" cy="338" r="5.5" fill="#0d0221"/>
  <circle cx="694" cy="338" r="3.2" fill="#a855f7"/>
  <circle cx="706" cy="338" r="3.2" fill="#a855f7"/>
  <circle cx="694.8" cy="336.8" r="1.3" fill="white"/>
  <circle cx="706.8" cy="336.8" r="1.3" fill="white"/>
  <!-- Fox nose & mouth -->
  <ellipse cx="700" cy="346" rx="5" ry="3" fill="#7b2ff7" opacity=".5"/>
  <circle  cx="700" cy="346" r="2" fill="#c084fc"/>
  <path d="M697 349 Q700 352.5 703 349" stroke="#a855f7" stroke-width="1.2" fill="none" stroke-linecap="round"/>
</svg>
