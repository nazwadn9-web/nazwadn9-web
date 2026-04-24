<svg width="800" height="390" viewBox="0 0 800 390" xmlns="http://www.w3.org/2000/svg">

  <defs>
    <linearGradient id="bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%"   stop-color="#1a0533"/>
      <stop offset="50%"  stop-color="#2d0f5e"/>
      <stop offset="100%" stop-color="#0d0221"/>
    </linearGradient>
    <linearGradient id="nameGrad" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0%"   stop-color="#a855f7"/>
      <stop offset="100%" stop-color="#f0c060"/>
    </linearGradient>
    <linearGradient id="chestGrad" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%"   stop-color="#a855f7"/>
      <stop offset="100%" stop-color="#6d28d9"/>
    </linearGradient>
    <radialGradient id="glowRight" cx="85%" cy="15%" r="40%">
      <stop offset="0%"   stop-color="#7b2ff7" stop-opacity="0.18"/>
      <stop offset="100%" stop-color="#7b2ff7" stop-opacity="0"/>
    </radialGradient>
    <radialGradient id="glowLeft" cx="10%" cy="85%" r="35%">
      <stop offset="0%"   stop-color="#a855f7" stop-opacity="0.12"/>
      <stop offset="100%" stop-color="#a855f7" stop-opacity="0"/>
    </radialGradient>
  </defs>

  <!-- Background -->
  <rect width="800" height="390" rx="16" fill="url(#bg)"/>
  <rect width="800" height="390" rx="16" fill="url(#glowRight)"/>
  <rect width="800" height="390" rx="16" fill="url(#glowLeft)"/>
  <rect width="800" height="390" rx="16" fill="none" stroke="#4a1a8c" stroke-width="1.5"/>

  <!-- ── STARS (SMIL twinkle) ── -->
  <circle cx="45"  cy="20"  r="1.5" fill="white">
    <animate attributeName="opacity" values="0.1;0.9;0.1" dur="1.8s" repeatCount="indefinite"/>
  </circle>
  <circle cx="175" cy="16"  r="1.1" fill="white">
    <animate attributeName="opacity" values="0.1;0.8;0.1" dur="2.3s" repeatCount="indefinite" begin="0.4s"/>
  </circle>
  <circle cx="320" cy="11"  r="1.3" fill="white">
    <animate attributeName="opacity" values="0.05;0.95;0.05" dur="1.6s" repeatCount="indefinite" begin="1s"/>
  </circle>
  <circle cx="490" cy="25"  r="1.0" fill="white">
    <animate attributeName="opacity" values="0.1;0.7;0.1" dur="2.5s" repeatCount="indefinite" begin="0.2s"/>
  </circle>
  <circle cx="640" cy="13"  r="1.5" fill="white">
    <animate attributeName="opacity" values="0.15;0.9;0.15" dur="2.0s" repeatCount="indefinite" begin="0.8s"/>
  </circle>
  <circle cx="760" cy="32"  r="1.2" fill="white">
    <animate attributeName="opacity" values="0.1;0.8;0.1" dur="2.2s" repeatCount="indefinite" begin="1.5s"/>
  </circle>
  <circle cx="90"  cy="55"  r="1.0" fill="white">
    <animate attributeName="opacity" values="0.1;0.7;0.1" dur="3.0s" repeatCount="indefinite" begin="0.6s"/>
  </circle>
  <circle cx="270" cy="38"  r="1.1" fill="white">
    <animate attributeName="opacity" values="0.1;0.85;0.1" dur="2.7s" repeatCount="indefinite" begin="1.2s"/>
  </circle>
  <circle cx="555" cy="48"  r="1.3" fill="white">
    <animate attributeName="opacity" values="0.1;0.9;0.1" dur="1.9s" repeatCount="indefinite" begin="0.3s"/>
  </circle>
  <circle cx="700" cy="65"  r="1.0" fill="white">
    <animate attributeName="opacity" values="0.1;0.75;0.1" dur="2.8s" repeatCount="indefinite" begin="0.9s"/>
  </circle>
  <circle cx="30"  cy="200" r="1.2" fill="white">
    <animate attributeName="opacity" values="0.05;0.8;0.05" dur="3.5s" repeatCount="indefinite" begin="1.8s"/>
  </circle>
  <circle cx="400" cy="75"  r="1.1" fill="white">
    <animate attributeName="opacity" values="0.1;0.7;0.1" dur="4.0s" repeatCount="indefinite" begin="0.7s"/>
  </circle>
  <circle cx="785" cy="195" r="1.3" fill="white">
    <animate attributeName="opacity" values="0.1;0.9;0.1" dur="3.2s" repeatCount="indefinite" begin="2.1s"/>
  </circle>
  <circle cx="240" cy="368" r="1.0" fill="white">
    <animate attributeName="opacity" values="0.1;0.8;0.1" dur="2.6s" repeatCount="indefinite" begin="1.4s"/>
  </circle>
  <circle cx="650" cy="375" r="1.2" fill="white">
    <animate attributeName="opacity" values="0.1;0.85;0.1" dur="2.1s" repeatCount="indefinite" begin="0.5s"/>
  </circle>

  <!-- ── ROBOT (SMIL float) ── -->
  <g>
    <animateTransform attributeName="transform" type="translate"
      values="0,0; 0,-9; 0,0" dur="3s" repeatCount="indefinite" calcMode="spline"
      keySplines="0.45 0 0.55 1; 0.45 0 0.55 1"/>

    <!-- Shadow (counter-animate so it stays on ground) -->
    <ellipse cx="120" cy="315" rx="40" ry="6" fill="#7b2ff7" opacity="0.2">
      <animateTransform attributeName="transform" type="translate"
        values="0,0; 0,9; 0,0" dur="3s" repeatCount="indefinite" calcMode="spline"
        keySplines="0.45 0 0.55 1; 0.45 0 0.55 1"/>
      <animate attributeName="rx" values="40;32;40" dur="3s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.2;0.12;0.2" dur="3s" repeatCount="indefinite"/>
    </ellipse>

    <!-- Arms -->
    <rect x="58"  y="168" width="20" height="48" rx="8" fill="#4a1a8c"/>
    <rect x="162" y="168" width="20" height="48" rx="8" fill="#4a1a8c"/>
    <rect x="61"  y="183" width="14" height="18" rx="4" fill="#7b2ff7" opacity="0.6"/>
    <rect x="165" y="183" width="14" height="18" rx="4" fill="#7b2ff7" opacity="0.6"/>
    <!-- Hands -->
    <rect x="63"  y="212" width="13" height="18" rx="6" fill="#2d0f5e"/>
    <rect x="164" y="212" width="13" height="18" rx="6" fill="#2d0f5e"/>
    <!-- Legs -->
    <rect x="88"  y="270" width="15" height="28" rx="7" fill="#4a1a8c"/>
    <rect x="137" y="270" width="15" height="28" rx="7" fill="#4a1a8c"/>
    <rect x="88"  y="284" width="15" height="16" rx="6" fill="#2d0f5e"/>
    <rect x="137" y="284" width="15" height="16" rx="6" fill="#2d0f5e"/>
    <!-- Body -->
    <rect x="72"  y="160" width="96" height="114" rx="14" fill="#2d0f5e"/>
    <rect x="80"  y="168" width="80" height="98"  rx="10" fill="#150929"/>
    <!-- Chest orb glow -->
    <circle cx="120" cy="208" r="22" fill="#7b2ff7" opacity="0.2">
      <animate attributeName="r"       values="22;26;22" dur="2s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.2;0.08;0.2" dur="2s" repeatCount="indefinite"/>
    </circle>
    <!-- Chest orb -->
    <circle cx="120" cy="208" r="14" fill="url(#chestGrad)">
      <animate attributeName="r" values="14;16;14" dur="2s" repeatCount="indefinite"/>
    </circle>
    <circle cx="120" cy="208" r="6.5" fill="#e9d5ff">
      <animate attributeName="opacity" values="1;0.6;1" dur="2s" repeatCount="indefinite"/>
    </circle>
    <!-- Chest LEDs -->
    <rect x="83"  y="238" width="9" height="5" rx="2.5" fill="#4a1a8c"/>
    <rect x="95"  y="238" width="9" height="5" rx="2.5" fill="#7b2ff7"/>
    <rect x="107" y="238" width="9" height="5" rx="2.5" fill="#4a1a8c"/>
    <rect x="119" y="238" width="9" height="5" rx="2.5" fill="#7b2ff7"/>
    <rect x="131" y="238" width="9" height="5" rx="2.5" fill="#4a1a8c"/>
    <!-- Head -->
    <rect x="66"  y="82"  width="108" height="82" rx="18" fill="#3a1270"/>
    <rect x="76"  y="90"  width="88"  height="66" rx="12" fill="#150929"/>
    <!-- Eyes (blink via scaleY on the eye group) -->
    <g>
      <animateTransform attributeName="transform" type="scale"
        values="1,1; 1,1; 1,1; 1,1; 1,1; 1,1; 1,1; 1,1; 1,0.08; 1,1"
        dur="4.5s" repeatCount="indefinite" additive="sum"
        keyTimes="0;0.1;0.2;0.3;0.4;0.5;0.6;0.7;0.8;1"/>
      <!-- Eye whites -->
      <ellipse cx="100" cy="126" rx="13" ry="14" fill="#0d0221"/>
      <ellipse cx="140" cy="126" rx="13" ry="14" fill="#0d0221"/>
      <circle  cx="100" cy="126" r="10"  fill="#7b2ff7"/>
      <circle  cx="140" cy="126" r="10"  fill="#7b2ff7"/>
      <circle  cx="100" cy="126" r="5.5" fill="white"/>
      <circle  cx="140" cy="126" r="5.5" fill="white"/>
      <circle  cx="102" cy="123" r="2.2" fill="#c084fc"/>
      <circle  cx="142" cy="123" r="2.2" fill="#c084fc"/>
    </g>
    <!-- Smile -->
    <path d="M106 142 Q120 153 134 142" stroke="#7b2ff7" stroke-width="2.5" fill="none" stroke-linecap="round"/>
    <!-- Ears -->
    <circle cx="64"  cy="120" r="7" fill="#4a1a8c" opacity="0.7"/>
    <circle cx="176" cy="120" r="7" fill="#4a1a8c" opacity="0.7"/>
    <!-- Antenna stem -->
    <rect x="113" y="66" width="14" height="18" rx="7" fill="#4a1a8c"/>
    <!-- Antenna light -->
    <circle cx="120" cy="62" r="10" fill="#2d0f5e" stroke="#7b2ff7" stroke-width="1.2">
      <animate attributeName="opacity" values="0.7;1;0.7" dur="2s" repeatCount="indefinite"/>
    </circle>
    <circle cx="120" cy="62" r="5"   fill="#a855f7">
      <animate attributeName="opacity" values="0.7;1;0.7" dur="2s" repeatCount="indefinite"/>
    </circle>
    <circle cx="120" cy="62" r="2.5" fill="#f0c060">
      <animate attributeName="opacity" values="0.8;1;0.8" dur="2s" repeatCount="indefinite"/>
    </circle>
  </g>

  <!-- ── DIVIDER LINE ── -->
  <line x1="230" y1="33" x2="230" y2="355" stroke="#4a1a8c" stroke-width="1"/>

  <!-- ── TEXT CONTENT ── -->
  <!-- greeting -->
  <text x="250" y="78" font-family="Courier New, monospace" font-size="13" fill="#c084fc" letter-spacing="3">// Hello, World!</text>

  <!-- name: nasuka + cheese (two fills) -->
  <text x="248" y="136" font-family="Arial Black, Arial, sans-serif" font-size="48" font-weight="900" fill="white">nasuka</text>
  <text x="460" y="136" font-family="Arial Black, Arial, sans-serif" font-size="48" font-weight="900" fill="url(#nameGrad)">cheese</text>

  <!-- tagline -->
  <text x="250" y="165" font-family="Courier New, monospace" font-size="13" fill="#a855f7">✦ Creative Developer &amp; Night Coder</text>

  <!-- separator -->
  <line x1="250" y1="182" x2="775" y2="182" stroke="#4a1a8c" stroke-width="1"/>

  <!-- ── BADGES ── -->
  <!-- Open Source -->
  <rect x="250" y="194" width="116" height="26" rx="13" fill="#3b0d75" stroke="#a855f7" stroke-width="1"/>
  <text x="308" y="211" font-family="Courier New, monospace" font-size="11" fill="#c084fc" text-anchor="middle">✦ Open Source</text>
  <!-- Fast Learner -->
  <rect x="375" y="194" width="118" height="26" rx="13" fill="#2a1a00" stroke="#f0c060" stroke-width="1"/>
  <text x="434" y="211" font-family="Courier New, monospace" font-size="11" fill="#f0c060" text-anchor="middle">⚡ Fast Learner</text>
  <!-- Night Coder -->
  <rect x="503" y="194" width="112" height="26" rx="13" fill="#001a1c" stroke="#67e8f9" stroke-width="1"/>
  <text x="559" y="211" font-family="Courier New, monospace" font-size="11" fill="#67e8f9" text-anchor="middle">◈ Night Coder</text>

  <!-- separator 2 -->
  <line x1="250" y1="234" x2="775" y2="234" stroke="#2d0f5e" stroke-width="1"/>

  <!-- ── GMAIL CARD ── -->
  <rect x="250" y="246" width="230" height="50" rx="10" fill="#1e0840" stroke="#4a1a8c" stroke-width="1"/>
  <!-- Gmail icon bg -->
  <rect x="263" y="256" width="24" height="22" rx="4" fill="#2d0f5e"/>
  <!-- Gmail envelope outline -->
  <rect x="265" y="258" width="20" height="16" rx="1" fill="none" stroke="#c084fc" stroke-width="1"/>
  <polyline points="265,259 275,267 285,259" fill="none" stroke="#a855f7" stroke-width="1.2"/>
  <!-- Gmail labels -->
  <text x="294" y="261" font-family="Courier New, monospace" font-size="9"  fill="#7b2ff7">GMAIL</text>
  <text x="294" y="277" font-family="Courier New, monospace" font-size="13" fill="#e9d5ff">nasukacheese</text>

  <!-- ── TIKTOK CARD ── -->
  <rect x="492" y="246" width="210" height="50" rx="10" fill="#1e0840" stroke="#4a1a8c" stroke-width="1"/>
  <!-- TikTok icon bg -->
  <rect x="505" y="256" width="24" height="22" rx="4" fill="#2d0f5e"/>
  <!-- TikTok note icon (simplified) -->
  <circle cx="513" cy="274" r="4" fill="none" stroke="#c084fc" stroke-width="1"/>
  <line x1="517" y1="261" x2="517" y2="270" stroke="#a855f7" stroke-width="1.5" stroke-linecap="round"/>
  <line x1="517" y1="265" x2="522" y2="264" stroke="#a855f7" stroke-width="1.5" stroke-linecap="round"/>
  <!-- TikTok labels -->
  <text x="536" y="261" font-family="Courier New, monospace" font-size="9"  fill="#7b2ff7">TIKTOK</text>
  <text x="536" y="277" font-family="Courier New, monospace" font-size="13" fill="#e9d5ff">@viol_118</text>

  <!-- separator 3 -->
  <line x1="250" y1="312" x2="775" y2="312" stroke="#2d0f5e" stroke-width="1"/>

  <!-- ── STAT BOXES ── -->
  <!-- Repos -->
  <rect x="250" y="324" width="154" height="52" rx="10" fill="#1e0840" stroke="#4a1a8c" stroke-width="1"/>
  <text x="327" y="349" font-family="Arial, sans-serif" font-size="22" font-weight="700" fill="#a855f7" text-anchor="middle">42</text>
  <text x="327" y="365" font-family="Courier New, monospace" font-size="10" fill="#7b2ff7" text-anchor="middle">Repositories</text>
  <!-- Contributions -->
  <rect x="414" y="324" width="154" height="52" rx="10" fill="#1e0840" stroke="#4a1a8c" stroke-width="1"/>
  <text x="491" y="349" font-family="Arial, sans-serif" font-size="22" font-weight="700" fill="#a855f7" text-anchor="middle">128</text>
  <text x="491" y="365" font-family="Courier New, monospace" font-size="10" fill="#7b2ff7" text-anchor="middle">Contributions</text>
  <!-- LOC -->
  <rect x="578" y="324" width="154" height="52" rx="10" fill="#1e0840" stroke="#4a1a8c" stroke-width="1"/>
  <text x="655" y="352" font-family="Arial, sans-serif" font-size="24" font-weight="700" fill="#a855f7" text-anchor="middle">∞</text>
  <text x="655" y="365" font-family="Courier New, monospace" font-size="10" fill="#7b2ff7" text-anchor="middle">Lines of Code</text>

  <!-- ── FOX (SMIL wag tail) ── -->
  <!-- Fox tail group -->
  <g>
    <animateTransform attributeName="transform" type="rotate"
      values="-12,710,350; 14,710,350; -12,710,350"
      dur="1.3s" repeatCount="indefinite" calcMode="spline"
      keySplines="0.45 0 0.55 1; 0.45 0 0.55 1"/>
    <ellipse cx="720" cy="348" rx="28" ry="13" fill="#7b2ff7" opacity="0.85"/>
    <ellipse cx="730" cy="338" rx="18" ry="10" fill="#4a1a8c"/>
    <ellipse cx="736" cy="333" rx="9"  ry="6"  fill="#e9d5ff" opacity="0.4"/>
  </g>
  <!-- Fox body (static) -->
  <ellipse cx="700" cy="385" rx="28" ry="6" fill="#7b2ff7" opacity="0.18"/>
  <rect x="683" y="358" width="12" height="26" rx="6" fill="#4a1a8c"/>
  <rect x="705" y="358" width="12" height="26" rx="6" fill="#4a1a8c"/>
  <rect x="685" y="370" width="10" height="16" rx="5" fill="#2d0f5e"/>
  <rect x="707" y="370" width="10" height="16" rx="5" fill="#2d0f5e"/>
  <ellipse cx="700" cy="344" rx="26" ry="22" fill="#3a1270"/>
  <ellipse cx="700" cy="347" rx="20" ry="16" fill="#4a1a8c"/>
  <!-- Fox ears -->
  <ellipse cx="686" cy="326" rx="8" ry="12" fill="#3a1270" transform="rotate(-20,686,326)"/>
  <ellipse cx="714" cy="326" rx="8" ry="12" fill="#3a1270" transform="rotate(20,714,326)"/>
  <ellipse cx="686" cy="327" rx="4" ry="6"  fill="#7b2ff7" transform="rotate(-20,686,327)"/>
  <ellipse cx="714" cy="327" rx="4" ry="6"  fill="#7b2ff7" transform="rotate(20,714,327)"/>
  <!-- Fox eyes -->
  <circle cx="694" cy="342" r="5.5" fill="#0d0221"/>
  <circle cx="706" cy="342" r="5.5" fill="#0d0221"/>
  <circle cx="694" cy="342" r="3.2" fill="#a855f7"/>
  <circle cx="706" cy="342" r="3.2" fill="#a855f7"/>
  <circle cx="695" cy="340" r="1.3" fill="white"/>
  <circle cx="707" cy="340" r="1.3" fill="white"/>
  <!-- Fox nose & smile -->
  <ellipse cx="700" cy="350" rx="5" ry="3" fill="#7b2ff7" opacity="0.5"/>
  <circle  cx="700" cy="350" r="2"  fill="#c084fc"/>
  <path d="M697 353 Q700 357 703 353" stroke="#a855f7" stroke-width="1.2" fill="none" stroke-linecap="round"/>

</svg>
