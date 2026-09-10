<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 900 2050" width="100%" height="100%">
  <defs>
    <linearGradient id="mainCanvas" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#0b0f17" />
      <stop offset="40%" stop-color="#111827" />
      <stop offset="80%" stop-color="#131b2c" />
      <stop offset="100%" stop-color="#0b0f17" />
    </linearGradient>

    <linearGradient id="cardGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#151d2e" />
      <stop offset="100%" stop-color="#192337" />
    </linearGradient>

    <linearGradient id="headerGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#0f172a" />
      <stop offset="60%" stop-color="#172236" />
      <stop offset="100%" stop-color="#1e2d47" />
    </linearGradient>

    <filter id="glow" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="12" result="blur" />
      <feComposite in="SourceGraphic" in2="blur" operator="over" />
    </filter>

    <pattern id="grid" width="32" height="32" patternUnits="userSpaceOnUse">
      <path d="M 32 0 L 0 0 0 32" fill="none" stroke="#1f2c42" stroke-width="0.7" opacity="0.45" />
    </pattern>

    <clipPath id="avatarClip">
      <rect x="0" y="0" width="180" height="230" rx="14" />
    </clipPath>

    <style>
      .hero-name { font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif; font-size: 38px; font-weight: 800; fill: #ECEFF4; letter-spacing: -0.5px; }
      .hero-tag { font-family: 'Fira Code', Consolas, monospace; font-size: 13.5px; font-weight: 600; fill: #88C0D0; letter-spacing: 1.5px; }
      .badge-avail { font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif; font-size: 11px; font-weight: 700; fill: #ECEFF4; }

      .section-h { font-family: 'Fira Code', monospace; font-size: 16px; font-weight: 700; fill: #ECEFF4; letter-spacing: 0.5px; }
      .th { font-family: 'Fira Code', monospace; font-size: 11.5px; font-weight: 700; fill: #88C0D0; letter-spacing: 0.8px; }

      .row-title { font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif; font-size: 13.5px; font-weight: 700; fill: #ECEFF4; }
      .row-link { font-family: 'Fira Code', monospace; font-size: 11px; font-weight: 600; fill: #88C0D0; text-decoration: none; }
      .row-link:hover { fill: #81A1C1; text-decoration: underline; }
      .desc { font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif; font-size: 12px; fill: #C8D1E0; }

      .bio-p { font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif; font-size: 13px; line-height: 1.6; fill: #D8DEE9; }
      .bullet-t { font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif; font-size: 12.5px; fill: #E5E9F0; }
      .bullet-c { font-family: 'Fira Code', monospace; font-size: 11.5px; fill: #88C0D0; }

      .pill-bg { rx: 4px; }
      .pill-txt { font-family: 'Fira Code', monospace; font-size: 10px; font-weight: 600; fill: #ECEFF4; }
      .divider { stroke: #233045; stroke-width: 1; }

      .footer-t1 { font-family: 'Fira Code', monospace; font-size: 13.5px; font-weight: 600; fill: #88C0D0; letter-spacing: 0.8px; }
      .footer-t2 { font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif; font-size: 12px; fill: #8896AB; }

      @keyframes pulseDot {
        0%, 100% { opacity: 1; transform: scale(1); }
        50% { opacity: 0.3; transform: scale(0.85); }
      }
      @keyframes floatBeam {
        0%, 100% { transform: translateX(0px); }
        50% { transform: translateX(40px); }
      }
      .pulse { animation: pulseDot 2s infinite ease-in-out; transform-origin: 72px 42px; }
      .beam { animation: floatBeam 8s infinite ease-in-out; }
    </style>
  </defs>

  <rect width="900" height="2050" rx="20" fill="url(#mainCanvas)" />
  <rect width="900" height="2050" rx="20" fill="url(#grid)" />
  <rect width="898" height="2048" x="1" y="1" rx="19" fill="none" stroke="#223047" stroke-width="1.5" />

  <!-- 1. TOP HEADER BANNER -->
  <g transform="translate(35, 35)">
    <rect width="830" height="230" rx="16" fill="url(#headerGrad)" stroke="#25354e" stroke-width="1.2" />

    <g class="beam" opacity="0.25">
      <circle cx="160" cy="50" r="110" fill="#88C0D0" filter="url(#glow)" />
      <circle cx="700" cy="180" r="130" fill="#5E81AC" filter="url(#glow)" />
    </g>

    <g transform="translate(45, 26)">
      <rect width="195" height="25" rx="12.5" fill="#101725" stroke="#2b3b54" stroke-width="1" />
      <circle cx="13" cy="12.5" r="4.5" fill="#A3BE8C" class="pulse" />
      <text x="27" y="16.5" class="badge-avail">OPEN FOR WORK &amp; COLLABS</text>
    </g>

    <g transform="translate(45, 96)">
      <text x="0" y="0" class="hero-name">Fatir Gibran</text>
      <text x="0" y="28" class="hero-tag">FULL-STACK &amp; APPLIED AI ENGINEER</text>
    </g>

    <g transform="translate(45, 160)">
      <g transform="translate(0, 0)">
        <rect width="120" height="32" rx="6" fill="#121a29" stroke="#2a3a52" stroke-width="1" />
        <text x="60" y="20" class="pill-txt" text-anchor="middle">⚡ Next.js / TS</text>
      </g>
      <g transform="translate(132, 0)">
        <rect width="115" height="32" rx="6" fill="#121a29" stroke="#2a3a52" stroke-width="1" />
        <text x="57.5" y="20" class="pill-txt" text-anchor="middle">🐍 Python AI</text>
      </g>
      <g transform="translate(259, 0)">
        <rect width="105" height="32" rx="6" fill="#121a29" stroke="#2a3a52" stroke-width="1" />
        <text x="52.5" y="20" class="pill-txt" text-anchor="middle">🐹 Golang</text>
      </g>
      <g transform="translate(376, 0)">
        <rect width="155" height="32" rx="6" fill="#121a29" stroke="#2a3a52" stroke-width="1" />
        <text x="77.5" y="20" class="pill-txt" text-anchor="middle">👁️ Computer Vision</text>
      </g>
    </g>

    <g transform="translate(620, 26)">
      <rect width="165" height="178" rx="10" fill="#0d1421" stroke="#25354e" stroke-width="1.2" />
      <line x1="0" y1="28" x2="165" y2="28" stroke="#25354e" stroke-width="1" />
      <circle cx="15" cy="14" r="3.5" fill="#BF616A" />
      <circle cx="28" cy="14" r="3.5" fill="#EBCB8B" />
      <circle cx="41" cy="14" r="3.5" fill="#A3BE8C" />
      <rect x="18" y="44" width="55" height="5" rx="2.5" fill="#88C0D0" opacity="0.8" />
      <rect x="18" y="60" width="105" height="4" rx="2" fill="#4C566A" />
      <rect x="18" y="74" width="80" height="4" rx="2" fill="#4C566A" />
      <rect x="18" y="88" width="120" height="4" rx="2" fill="#4C566A" />
      <rect x="18" y="112" width="45" height="5" rx="2.5" fill="#81A1C1" opacity="0.8" />
      <rect x="18" y="128" width="90" height="4" rx="2" fill="#4C566A" />
      <rect x="18" y="142" width="115" height="4" rx="2" fill="#3B4252" />
    </g>
  </g>

  <!-- 2. ABOUT ME & PORTRAIT -->
  <g transform="translate(35, 290)">
    <rect width="830" height="280" rx="16" fill="url(#cardGrad)" stroke="#25354e" stroke-width="1.2" />

    <text x="35" y="38" class="section-h">💫 Profile &amp; Engineering Focus</text>

    <!-- Embedded Portrait Frame -->
    <g transform="translate(35, 60)">
      <g clip-path="url(#avatarClip)">
        <image href="https://raw.githubusercontent.com/Fatirrr08/Fatirrr08/main/foto.jpeg" xlink:href="https://raw.githubusercontent.com/Fatirrr08/Fatirrr08/main/foto.jpeg" x="-10" y="-12" width="200" height="255" preserveAspectRatio="xMidYMid slice" />
      </g>
      <rect width="180" height="230" rx="14" fill="none" stroke="#88C0D0" stroke-width="1.5" opacity="0.85" />
    </g>

    <g transform="translate(240, 70)">
      <text x="0" y="0" class="bio-p">Halo! Saya <tspan font-weight="700" fill="#ECEFF4">Fatir Gibran</tspan>, mahasiswa IT yang berfokus pada perancangan</text>
      <text x="0" y="20" class="bio-p"><tspan font-weight="700" fill="#ECEFF4">Modern Web Architecture</tspan>, backend performa tinggi, dan komputasi cerdas</text>
      <text x="0" y="40" class="bio-p">berbasis <tspan font-weight="700" fill="#88C0D0">Artificial Intelligence &amp; Computer Vision</tspan>.</text>

      <g transform="translate(0, 76)">
        <text x="0" y="0" font-size="13">🌱</text>
        <text x="22" y="-1" class="bullet-t"><tspan class="bullet-c">Current Stack:</tspan> Go (Golang), Python, Next.js / TypeScript, &amp; Cloud (GCP).</text>
      </g>
      <g transform="translate(0, 106)">
        <text x="0" y="0" font-size="13">💡</text>
        <text x="22" y="-1" class="bullet-t"><tspan class="bullet-c">Specialization:</tspan> Semantic / Vector Search, Gesture Interfaces, &amp; Microservices.</text>
      </g>
      <g transform="translate(0, 136)">
        <text x="0" y="0" font-size="13">🎓</text>
        <text x="22" y="-1" class="bullet-t"><tspan class="bullet-c">Credentials:</tspan> Samsung Innovation Campus B8 | Lab Asdos Algoritma &amp; Pemrograman.</text>
      </g>
      <g transform="translate(0, 166)">
        <text x="0" y="0" font-size="13">📫</text>
        <text x="22" y="-1" class="bullet-t"><tspan class="bullet-c">Collaboration:</tspan> Terbuka untuk magang rekayasa perangkat lunak &amp; riset open-source.</text>
      </g>
    </g>
  </g>

  <!-- 3. FEATURED PROJECTS -->
  <g transform="translate(35, 595)">
    <rect width="830" height="570" rx="16" fill="url(#cardGrad)" stroke="#25354e" stroke-width="1.2" />

    <text x="35" y="38" class="section-h">🚀 Featured Projects &amp; AI Systems</text>

    <rect x="35" y="55" width="760" height="30" rx="6" fill="#111827" />
    <text x="50" y="75" class="th">PROJECT / REPOSITORY</text>
    <text x="270" y="75" class="th">DESCRIPTION &amp; ARCHITECTURAL HIGHLIGHTS</text>
    <text x="660" y="75" class="th">TECH STACK</text>

    <!-- Row 1: mini-semantic-search -->
    <g transform="translate(0, 95)">
      <text x="50" y="20" class="row-title">🔍 mini-semantic-search</text>
      <a href="https://github.com/Fatirrr08/mini-semantic-search" target="_blank">
        <text x="50" y="38" class="row-link">Repo Link ↗</text>
      </a>
      <text x="270" y="20" class="desc">Penelusuran semantik berbasis embedding vektor kalimat dan</text>
      <text x="270" y="38" class="desc">Cosine Similarity untuk pencocokan konteks dokumen relevan.</text>
      <rect x="660" y="14" width="55" height="18" class="pill-bg" fill="#3776AB" />
      <text x="687.5" y="27" class="pill-txt" text-anchor="middle">Python</text>
      <rect x="722" y="14" width="72" height="18" class="pill-bg" fill="#4C566A" />
      <text x="758" y="27" class="pill-txt" text-anchor="middle">Vector NLP</text>
      <line x1="35" y1="58" x2="795" y2="58" class="divider" />
    </g>

    <!-- Row 2: el_gestur_v2 -->
    <g transform="translate(0, 168)">
      <text x="50" y="20" class="row-title">👁️ el_gestur_v2</text>
      <a href="https://github.com/aariffaqiih/el_gestur_v2" target="_blank">
        <text x="50" y="38" class="row-link">Repo Link ↗</text>
      </a>
      <text x="270" y="20" class="desc">Sistem kontrol presentasi (Canva, PPT) hands-free berbasis</text>
      <text x="270" y="38" class="desc">Computer Vision real-time &amp; integrasi perintah suara.</text>
      <rect x="660" y="14" width="55" height="18" class="pill-bg" fill="#3776AB" />
      <text x="687.5" y="27" class="pill-txt" text-anchor="middle">Python</text>
      <rect x="722" y="14" width="58" height="18" class="pill-bg" fill="#D08770" />
      <text x="751" y="27" class="pill-txt" text-anchor="middle">YOLOv8</text>
      <line x1="35" y1="58" x2="795" y2="58" class="divider" />
    </g>

    <!-- Row 3: FocuSync -->
    <g transform="translate(0, 241)">
      <text x="50" y="20" class="row-title">⚡ FocuSync</text>
      <a href="https://github.com/Fatirrr08/FocuSync" target="_blank">
        <text x="50" y="38" class="row-link">Repo Link ↗</text>
      </a>
      <text x="270" y="20" class="desc">Platform presentasi kolaboratif berbasis Next.js App Router</text>
      <text x="270" y="38" class="desc">dengan sinkronisasi state instan via realtime cloud service.</text>
      <rect x="660" y="14" width="60" height="18" class="pill-bg" fill="#000000" stroke="#4C566A" stroke-width="0.8" />
      <text x="690" y="27" class="pill-txt" text-anchor="middle">Next.js</text>
      <rect x="727" y="14" width="68" height="18" class="pill-bg" fill="#3ECF8E" />
      <text x="761" y="27" class="pill-txt" text-anchor="middle" fill="#0b0f17">Supabase</text>
      <line x1="35" y1="58" x2="795" y2="58" class="divider" />
    </g>

    <!-- Row 4: salin-gaya-web -->
    <g transform="translate(0, 314)">
      <text x="50" y="20" class="row-title">🛍️ salin-gaya-web</text>
      <a href="https://github.com/Fatirrr08/salin-gaya-web" target="_blank">
        <text x="50" y="38" class="row-link">Repo Link ↗</text>
      </a>
      <text x="270" y="20" class="desc">E-commerce curated fashion dengan rekomendasi cerdas</text>
      <text x="270" y="38" class="desc">berbasis Gemini AI &amp; sistem transaksi payment Midtrans.</text>
      <rect x="660" y="14" width="46" height="18" class="pill-bg" fill="#20232A" stroke="#61DAFB" stroke-width="0.8" />
      <text x="683" y="27" class="pill-txt" text-anchor="middle" fill="#61DAFB">React</text>
      <rect x="712" y="14" width="30" height="18" class="pill-bg" fill="#007ACC" />
      <text x="727" y="27" class="pill-txt" text-anchor="middle">TS</text>
      <rect x="748" y="14" width="48" height="18" class="pill-bg" fill="#FFA000" />
      <text x="772" y="27" class="pill-txt" text-anchor="middle" fill="#000">Base</text>
      <line x1="35" y1="58" x2="795" y2="58" class="divider" />
    </g>

    <!-- Row 5: kline-app -->
    <g transform="translate(0, 387)">
      <text x="50" y="20" class="row-title">📊 kline-app</text>
      <a href="https://github.com/Fatirrr08/kline-app" target="_blank">
        <text x="50" y="38" class="row-link">Repo Link ↗</text>
      </a>
      <text x="270" y="20" class="desc">Aplikasi visualisasi data candlestick interaktif untuk analisis</text>
      <text x="270" y="38" class="desc">dan pemantauan pergerakan pasar finansial secara teknikal.</text>
      <rect x="660" y="14" width="32" height="18" class="pill-bg" fill="#F7DF1E" />
      <text x="676" y="27" class="pill-txt" text-anchor="middle" fill="#000">JS</text>
      <rect x="698" y="14" width="76" height="18" class="pill-bg" fill="#88C0D0" />
      <text x="736" y="27" class="pill-txt" text-anchor="middle" fill="#0b0f17">Analytics</text>
      <line x1="35" y1="58" x2="795" y2="58" class="divider" />
    </g>

    <!-- Row 6: Web_HMIF -->
    <g transform="translate(0, 460)">
      <text x="50" y="20" class="row-title">🏛️ Web_HMIF</text>
      <a href="https://github.com/Fatirrr08/Web_HMIF" target="_blank">
        <text x="50" y="38" class="row-link">Repo Link ↗</text>
      </a>
      <text x="270" y="20" class="desc">Situs portal resmi himpunan mahasiswa dengan tata</text>
      <text x="270" y="38" class="desc">letak antarmuka responsif dan ramah optimasi SEO.</text>
      <rect x="660" y="14" width="45" height="18" class="pill-bg" fill="#E34F26" />
      <text x="682.5" y="27" class="pill-txt" text-anchor="middle">HTML</text>
      <rect x="711" y="14" width="38" height="18" class="pill-bg" fill="#1572B6" />
      <text x="730" y="27" class="pill-txt" text-anchor="middle">CSS</text>
      <rect x="755" y="14" width="32" height="18" class="pill-bg" fill="#F7DF1E" />
      <text x="771" y="27" class="pill-txt" text-anchor="middle" fill="#000">JS</text>
    </g>
  </g>

  <!-- 4. BACKEND & SYSTEMS -->
  <g transform="translate(35, 1190)">
    <rect width="830" height="420" rx="16" fill="url(#cardGrad)" stroke="#25354e" stroke-width="1.2" />

    <text x="35" y="38" class="section-h">⚙️ Backend, Systems &amp; Computing Fundamentals</text>

    <rect x="35" y="55" width="760" height="30" rx="6" fill="#111827" />
    <text x="50" y="75" class="th">ASSIGNMENT / REPO</text>
    <text x="270" y="75" class="th">CORE ARCHITECTURE &amp; LOW-LEVEL IMPLEMENTATION</text>
    <text x="660" y="75" class="th">TECH STACK</text>

    <!-- Row 1: Latihan-Golang -->
    <g transform="translate(0, 95)">
      <text x="50" y="20" class="row-title">🐹 Latihan-Golang</text>
      <a href="https://github.com/Fatirrr08/Latihan-Golang" target="_blank">
        <text x="50" y="38" class="row-link">Repo Link ↗</text>
      </a>
      <text x="270" y="20" class="desc">Eksplorasi konkurensi (Goroutines &amp; Channels), implementasi</text>
      <text x="270" y="38" class="desc">RESTful API idiomatik, dan manipulasi memori performa tinggi.</text>
      <rect x="660" y="14" width="32" height="18" class="pill-bg" fill="#00ADD8" />
      <text x="676" y="27" class="pill-txt" text-anchor="middle">Go</text>
      <rect x="698" y="14" width="80" height="18" class="pill-bg" fill="#4C566A" />
      <text x="738" y="27" class="pill-txt" text-anchor="middle">APIs Backend</text>
      <line x1="35" y1="58" x2="795" y2="58" class="divider" />
    </g>

    <!-- Row 2: JARKOM-TUBES -->
    <g transform="translate(0, 168)">
      <text x="50" y="20" class="row-title">🔌 JARKOM-TUBES</text>
      <a href="https://github.com/Fatirrr08/JARKOM-TUBES" target="_blank">
        <text x="50" y="38" class="row-link">Repo Link ↗</text>
      </a>
      <text x="270" y="20" class="desc">Pemrograman socket jaringan, simulasi transfer paket protokol</text>
      <text x="270" y="38" class="desc">TCP/UDP, dan arsitektur komunikasi data multi-client.</text>
      <rect x="660" y="14" width="55" height="18" class="pill-bg" fill="#3776AB" />
      <text x="687.5" y="27" class="pill-txt" text-anchor="middle">Python</text>
      <rect x="722" y="14" width="60" height="18" class="pill-bg" fill="#D08770" />
      <text x="752" y="27" class="pill-txt" text-anchor="middle">Sockets</text>
      <line x1="35" y1="58" x2="795" y2="58" class="divider" />
    </g>

    <!-- Row 3: Library-Pro -->
    <g transform="translate(0, 241)">
      <text x="50" y="20" class="row-title">📚 Library-Pro</text>
      <a href="https://github.com/Fatirrr08/Library-Pro" target="_blank">
        <text x="50" y="38" class="row-link">Repo Link ↗</text>
      </a>
      <text x="270" y="20" class="desc">Sistem Informasi Perpustakaan berbasis arsitektur MVC terintegrasi</text>
      <text x="270" y="38" class="desc">manajemen skema relasional SQL transaksional.</text>
      <rect x="660" y="14" width="40" height="18" class="pill-bg" fill="#ED8B00" />
      <text x="680" y="27" class="pill-txt" text-anchor="middle">Java</text>
      <rect x="706" y="14" width="55" height="18" class="pill-bg" fill="#4479A1" />
      <text x="733.5" y="27" class="pill-txt" text-anchor="middle">MySQL</text>
      <line x1="35" y1="58" x2="795" y2="58" class="divider" />
    </g>

    <!-- Row 4: AKA -->
    <g transform="translate(0, 314)">
      <text x="50" y="20" class="row-title">📐 AKA (Analisis Algoritma)</text>
      <a href="https://github.com/Fatirrr08/AKA" target="_blank">
        <text x="50" y="38" class="row-link">Repo Link ↗</text>
      </a>
      <text x="270" y="20" class="desc">Benchmarking empiris efisiensi algoritma (Big-O ruang &amp; waktu)</text>
      <text x="270" y="38" class="desc">serta manipulasi struktur data komputasi dinamis.</text>
      <rect x="660" y="14" width="55" height="18" class="pill-bg" fill="#3776AB" />
      <text x="687.5" y="27" class="pill-txt" text-anchor="middle">Python</text>
      <rect x="722" y="14" width="75" height="18" class="pill-bg" fill="#B48EAD" />
      <text x="759.5" y="27" class="pill-txt" text-anchor="middle">Algorithms</text>
    </g>
  </g>

  <!-- 5. INTEGRATED FOOTER -->
  <g transform="translate(35, 1635)">
    <rect width="830" height="375" rx="16" fill="url(#headerGrad)" stroke="#25354e" stroke-width="1.2" />

    <g transform="translate(415, 55)">
      <text x="0" y="0" class="footer-t1" text-anchor="middle">⚡ Designed &amp; Engineered by Fatir Gibran</text>
      <text x="0" y="24" class="footer-t2" text-anchor="middle">"Code is like humor. When you have to explain it, it’s bad."</text>
      <text x="0" y="44" class="footer-t2" text-anchor="middle">⭐️ Terimakasih telah berkunjung ke profil saya!</text>
    </g>

    <g transform="translate(195, 135)">
      <rect width="95" height="30" rx="6" fill="#0077B5" />
      <text x="47.5" y="19" class="pill-txt" text-anchor="middle">LinkedIn</text>
      <rect x="110" y="0" width="85" height="30" rx="6" fill="#24292e" />
      <text x="152.5" y="19" class="pill-txt" text-anchor="middle">GitHub</text>
      <rect x="210" y="0" width="90" height="30" rx="6" fill="#D14836" />
      <text x="255" y="19" class="pill-txt" text-anchor="middle">Email</text>
      <rect x="315" y="0" width="115" height="30" rx="6" fill="#E4405F" />
      <text x="372.5" y="19" class="pill-txt" text-anchor="middle">Instagram</text>
    </g>

    <g transform="translate(140, 200)">
      <rect width="550" height="135" rx="12" fill="#0d1421" stroke="#25354e" stroke-width="1" />
      
      <g transform="translate(100, 48)">
        <text x="0" y="0" class="hero-name" font-size="28" text-anchor="middle" fill="#88C0D0">18+</text>
        <text x="0" y="24" class="pill-txt" text-anchor="middle" fill="#8896AB">REPOSITORIES</text>
      </g>
      
      <line x1="200" y1="25" x2="200" y2="110" stroke="#233045" stroke-width="1" />

      <g transform="translate(285, 48)">
        <text x="0" y="0" class="hero-name" font-size="28" text-anchor="middle" fill="#A3BE8C">100%</text>
        <text x="0" y="24" class="pill-txt" text-anchor="middle" fill="#8896AB">ACTIVE COMMIT</text>
      </g>

      <line x1="370" y1="25" x2="370" y2="110" stroke="#233045" stroke-width="1" />

      <g transform="translate(460, 48)">
        <text x="0" y="0" class="hero-name" font-size="28" text-anchor="middle" fill="#EBCB8B">AI / WEB</text>
        <text x="0" y="24" class="pill-txt" text-anchor="middle" fill="#8896AB">CORE FOCUS</text>
      </g>
    </g>
  </g>
</svg>
