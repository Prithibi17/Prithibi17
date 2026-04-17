<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 900 140" width="900" height="140">
  <defs>
    <radialGradient id="fOuterGlow" cx="50%" cy="55%" r="50%">
      <stop offset="0%"   stop-color="#D4AF37" stop-opacity="0.35"/>
      <stop offset="50%"  stop-color="#8B6914" stop-opacity="0.12"/>
      <stop offset="100%" stop-color="#D4AF37" stop-opacity="0"/>
    </radialGradient>
    <radialGradient id="fCoreGlow" cx="50%" cy="50%" r="50%">
      <stop offset="0%"   stop-color="#FFD700" stop-opacity="0.95"/>
      <stop offset="40%"  stop-color="#D4AF37" stop-opacity="0.6"/>
      <stop offset="100%" stop-color="#8B6914" stop-opacity="0"/>
    </radialGradient>
    <radialGradient id="fInnerCore" cx="50%" cy="50%" r="50%">
      <stop offset="0%"   stop-color="#FFFDE7" stop-opacity="1"/>
      <stop offset="60%"  stop-color="#FFD700" stop-opacity="0.8"/>
      <stop offset="100%" stop-color="#D4AF37" stop-opacity="0.4"/>
    </radialGradient>
    <filter id="fGlow">
      <feGaussianBlur stdDeviation="4" result="blur"/>
      <feComposite in="SourceGraphic" in2="blur" operator="over"/>
    </filter>
    <filter id="fInnerGlow">
      <feGaussianBlur stdDeviation="2" result="blur"/>
      <feComposite in="SourceGraphic" in2="blur" operator="over"/>
    </filter>
    <clipPath id="fClip"><rect width="900" height="140"/></clipPath>
  </defs>

  <!-- Outer pulse rings (expanding) -->
  <circle cx="450" cy="72" r="42" fill="none" stroke="#D4AF37" stroke-width="0.8" stroke-opacity="0.12">
    <animate attributeName="r"             values="42;72;42"    dur="4s" begin="0s"   repeatCount="indefinite"/>
    <animate attributeName="stroke-opacity" values="0.12;0;0.12" dur="4s" begin="0s"   repeatCount="indefinite"/>
  </circle>
  <circle cx="450" cy="72" r="42" fill="none" stroke="#D4AF37" stroke-width="0.7" stroke-opacity="0.09">
    <animate attributeName="r"             values="42;85;42"   dur="4s" begin="0.8s" repeatCount="indefinite"/>
    <animate attributeName="stroke-opacity" values="0.09;0;0.09" dur="4s" begin="0.8s" repeatCount="indefinite"/>
  </circle>
  <circle cx="450" cy="72" r="42" fill="none" stroke="#D4AF37" stroke-width="0.5" stroke-opacity="0.06">
    <animate attributeName="r"             values="42;100;42"  dur="4s" begin="1.6s" repeatCount="indefinite"/>
    <animate attributeName="stroke-opacity" values="0.06;0;0.06" dur="4s" begin="1.6s" repeatCount="indefinite"/>
  </circle>
  <!-- Hex ring -->
  <polygon points="450,30 485,50 485,90 450,110 415,90 415,50" fill="none" stroke="#D4AF37" stroke-width="0.8" stroke-opacity="0.2">
    <animateTransform attributeName="transform" type="rotate" values="0,450,72; 360,450,72" dur="20s" repeatCount="indefinite"/>
    <animate attributeName="stroke-opacity" values="0.2;0.4;0.2" dur="4s" repeatCount="indefinite"/>
  </polygon>
  <polygon points="450,20 495,45 495,95 450,120 405,95 405,45" fill="none" stroke="#D4AF37" stroke-width="0.5" stroke-opacity="0.12">
    <animateTransform attributeName="transform" type="rotate" values="30,450,72; 390,450,72" dur="25s" repeatCount="indefinite"/>
  </polygon>

  <!-- Outer glow -->
  <circle cx="450" cy="72" r="40" fill="url(#fOuterGlow)" filter="url(#fGlow)">
    <animate attributeName="r" values="40;50;38;46;40" dur="3s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="1;0.7;1;0.85;1" dur="3s" repeatCount="indefinite"/>
  </circle>

  <!-- Main flame -->
  <g filter="url(#fGlow)">
    <!-- outer flame -->
    <g>
      <animateTransform attributeName="transform" type="translate" values="450,72; 450,67; 450,72" dur="1.4s" repeatCount="indefinite"/>
      <path d="M0,-30 Q8,-16 5,0 Q10,-8 14,-20 Q18,-4 12,10 Q18,2 22,8 Q15,22 6,28 Q0,32 -6,28 Q-15,22 -22,8 Q-18,2 -12,10 Q-18,-4 -14,-20 Q-10,-8 -5,0 Q-8,-16 0,-30Z"
            fill="url(#fCoreGlow)" filter="url(#fInnerGlow)"/>
    </g>
    <!-- inner flame -->
    <g>
      <animateTransform attributeName="transform" type="translate" values="450,72; 450,66; 450,72" dur="1s" repeatCount="indefinite"/>
      <path d="M0,-18 Q5,-9 3,0 Q7,-5 9,-12 Q12,-2 7,7 Q11,1 14,5 Q9,14 4,18 Q0,20 -4,18 Q-9,14 -14,5 Q-11,1 -7,7 Q-12,-2 -9,-12 Q-7,-5 -3,0 Q-5,-9 0,-18Z"
            fill="url(#fInnerCore)"/>
    </g>
    <!-- core -->
    <ellipse cx="450" cy="75" rx="7" ry="5" fill="#FFFDE7" opacity="0.95">
      <animate attributeName="ry" values="5;8;4;7;5" dur="1s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.95;0.7;1;0.85;0.95" dur="1s" repeatCount="indefinite"/>
    </ellipse>
  </g>

  <!-- Floating sparks -->
  <circle cx="438" cy="50" r="2.5" fill="#FFD700" opacity="0">
    <animate attributeName="cy"      values="72;38;25"  dur="2.2s" begin="0s"    repeatCount="indefinite"/>
    <animate attributeName="cx"      values="438;432;426" dur="2.2s" begin="0s"    repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0;0.9;0"   dur="2.2s" begin="0s"    repeatCount="indefinite"/>
    <animate attributeName="r"       values="2.5;1.5;0" dur="2.2s" begin="0s"    repeatCount="indefinite"/>
  </circle>
  <circle cx="462" cy="50" r="2" fill="#FFD700" opacity="0">
    <animate attributeName="cy"      values="72;42;28"  dur="1.9s" begin="0.4s"  repeatCount="indefinite"/>
    <animate attributeName="cx"      values="462;468;474" dur="1.9s" begin="0.4s"  repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0;0.8;0"   dur="1.9s" begin="0.4s"  repeatCount="indefinite"/>
    <animate attributeName="r"       values="2;1.2;0"   dur="1.9s" begin="0.4s"  repeatCount="indefinite"/>
  </circle>
  <circle cx="450" cy="45" r="1.8" fill="#D4AF37" opacity="0">
    <animate attributeName="cy"      values="68;40;22"   dur="2.5s" begin="0.9s"  repeatCount="indefinite"/>
    <animate attributeName="cx"      values="450;444;440" dur="2.5s" begin="0.9s"  repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0;0.7;0"    dur="2.5s" begin="0.9s"  repeatCount="indefinite"/>
    <animate attributeName="r"       values="1.8;1;0"    dur="2.5s" begin="0.9s"  repeatCount="indefinite"/>
  </circle>
  <circle cx="456" cy="50" r="2.2" fill="#D4AF37" opacity="0">
    <animate attributeName="cy"      values="70;44;30"   dur="2.1s" begin="1.5s"  repeatCount="indefinite"/>
    <animate attributeName="cx"      values="456;462;466" dur="2.1s" begin="1.5s"  repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0;0.65;0"   dur="2.1s" begin="1.5s"  repeatCount="indefinite"/>
    <animate attributeName="r"       values="2.2;1.3;0"  dur="2.1s" begin="1.5s"  repeatCount="indefinite"/>
  </circle>
  <circle cx="444" cy="52" r="1.5" fill="#FFD700" opacity="0">
    <animate attributeName="cy"      values="70;46;32"   dur="1.7s" begin="0.2s"  repeatCount="indefinite"/>
    <animate attributeName="cx"      values="444;438;434" dur="1.7s" begin="0.2s"  repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0;0.75;0"   dur="1.7s" begin="0.2s"  repeatCount="indefinite"/>
    <animate attributeName="r"       values="1.5;0.8;0"  dur="1.7s" begin="0.2s"  repeatCount="indefinite"/>
  </circle>

  <!-- Flanking rune text -->
  <text x="220" y="77" text-anchor="middle" fill="#D4AF37" font-size="10" font-family="monospace" opacity="0.38" letter-spacing="3">◈  THE FORGE NEVER SLEEPS  ◈</text>
  <text x="680" y="77" text-anchor="middle" fill="#D4AF37" font-size="10" font-family="monospace" opacity="0.38" letter-spacing="3">◈  THE FORGE NEVER SLEEPS  ◈</text>

  <!-- Inscription -->
  <text x="450" y="132" text-anchor="middle" fill="#D4AF37" font-size="10" font-family="monospace" opacity="0.4" letter-spacing="5">🔥  CORE OF ALL CREATION  🔥</text>
</svg>
