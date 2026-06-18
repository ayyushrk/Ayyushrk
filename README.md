<svg width="900" height="300" viewBox="0 0 900 300" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#050a08"/>
      <stop offset="50%" stop-color="#06120c"/>
      <stop offset="100%" stop-color="#020403"/>
    </linearGradient>

    <linearGradient id="titleGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#00ff9c"/>
      <stop offset="50%" stop-color="#39ff14"/>
      <stop offset="100%" stop-color="#00ffd5"/>
    </linearGradient>

    <linearGradient id="barGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#13201a"/>
      <stop offset="100%" stop-color="#0a1410"/>
    </linearGradient>

    <filter id="glow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="3.2" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <filter id="softGlow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="1.4" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <clipPath id="screenClip">
      <rect x="6" y="42" width="888" height="252" rx="10"/>
    </clipPath>

    <pattern id="scan" width="4" height="4" patternUnits="userSpaceOnUse">
      <rect width="4" height="4" fill="transparent"/>
      <line x1="0" y1="0" x2="4" y2="0" stroke="#00ff9c" stroke-opacity="0.035" stroke-width="1"/>
    </pattern>
  </defs>

  <!-- outer body -->
  <rect x="0" y="0" width="900" height="300" rx="14" fill="url(#bgGrad)"/>
  <rect x="1.5" y="1.5" width="897" height="297" rx="13" fill="none" stroke="#1d3a2c" stroke-width="1.5"/>

  <!-- title bar -->
  <rect x="0" y="0" width="900" height="40" rx="14" fill="url(#barGrad)"/>
  <rect x="0" y="26" width="900" height="14" fill="url(#barGrad)"/>
  <circle cx="26" cy="20" r="6.5" fill="#ff5f56"/>
  <circle cx="48" cy="20" r="6.5" fill="#ffbd2e"/>
  <circle cx="70" cy="20" r="6.5" fill="#27c93f"/>
  <text x="450" y="25" text-anchor="middle" font-family="'JetBrains Mono', 'Fira Code', monospace" font-size="12.5" fill="#5fae8c" letter-spacing="0.5">ayush@portfolio: ~/whoami</text>

  <!-- screen area -->
  <g clip-path="url(#screenClip)">
    <rect x="6" y="42" width="888" height="252" fill="#020a06"/>
    <rect x="6" y="42" width="888" height="252" fill="url(#scan)"/>

    <!-- matrix rain columns -->
    <g font-family="'JetBrains Mono', monospace" font-size="14" fill="#0f5132" opacity="0.55">
      <text x="40" y="0"><animate attributeName="y" values="40;380" dur="3.4s" repeatCount="indefinite"/>ﾊﾐﾑｴﾄｶ</text>
      <text x="95" y="0"><animate attributeName="y" values="-60;320" dur="4.1s" repeatCount="indefinite"/>01101</text>
      <text x="150" y="0"><animate attributeName="y" values="20;360" dur="2.9s" repeatCount="indefinite"/>git rebase</text>
      <text x="240" y="0"><animate attributeName="y" values="-100;300" dur="3.7s" repeatCount="indefinite"/>npm run</text>
      <text x="320" y="0"><animate attributeName="y" values="60;400" dur="4.5s" repeatCount="indefinite"/>ｳｱｵﾈﾆ</text>
      <text x="600" y="0"><animate attributeName="y" values="-40;340" dur="3.1s" repeatCount="indefinite"/>const dev</text>
      <text x="700" y="0"><animate attributeName="y" values="10;370" dur="3.9s" repeatCount="indefinite"/>10110</text>
      <text x="780" y="0"><animate attributeName="y" values="-80;310" dur="3.3s" repeatCount="indefinite"/>ﾜﾇﾑﾁｵ</text>
      <text x="840" y="0"><animate attributeName="y" values="30;380" dur="4.2s" repeatCount="indefinite"/>fix bug</text>
    </g>

    <!-- glitch headline group -->
    <g filter="url(#glow)">
      <text x="40" y="118" font-family="'JetBrains Mono', 'Fira Code', monospace" font-size="46" font-weight="700" fill="url(#titleGrad)">
        Ayush R Kumar
        <animate attributeName="opacity" values="1;1;0.85;1;1;0.9;1" dur="2.6s" repeatCount="indefinite"/>
      </text>
      <!-- glitch slice copies -->
      <text x="42" y="118" font-family="'JetBrains Mono', monospace" font-size="46" font-weight="700" fill="#ff2bd6" opacity="0">
        Ayush R Kumar
        <animate attributeName="opacity" values="0;0;0.5;0;0;0;0" dur="1.9s" repeatCount="indefinite"/>
        <animate attributeName="x" values="42;38;44;42" dur="1.9s" repeatCount="indefinite"/>
      </text>
      <text x="38" y="118" font-family="'JetBrains Mono', monospace" font-size="46" font-weight="700" fill="#00eaff" opacity="0">
        Ayush R Kumar
        <animate attributeName="opacity" values="0;0.45;0;0;0;0;0" dur="2.3s" repeatCount="indefinite"/>
        <animate attributeName="x" values="38;42;36;38" dur="2.3s" repeatCount="indefinite"/>
      </text>
    </g>

    <!-- typewriter command line -->
    <g font-family="'JetBrains Mono', monospace" font-size="20" filter="url(#softGlow)">
      <text x="40" y="165" fill="#39ff14">$&#160;</text>
      <text x="62" y="165" fill="#d6ffe9">
        <animate attributeName="opacity" values="0;0;1" dur="0.3s" begin="0.2s" fill="freeze"/>
        whoami --role
        <animate attributeName="opacity" values="1;1;1;0;0;1" dur="6s" begin="0s" repeatCount="indefinite"/>
      </text>
    </g>

    <!-- rotating identity lines, staggered reveal -->
    <g font-family="'JetBrains Mono', monospace" font-size="19" fill="#9be8c4">
      <text x="40" y="200" opacity="0">
        &gt; Design Lead @ NSSCE
        <animate attributeName="opacity" values="0;0;1;1;1;1;0" keyTimes="0;0.08;0.12;0.6;0.85;0.95;1" dur="7s" begin="0.6s" repeatCount="indefinite"/>
      </text>
      <text x="40" y="228" opacity="0">
        &gt; Joint Secretary @ STACS
        <animate attributeName="opacity" values="0;0;1;1;1;1;0" keyTimes="0;0.08;0.12;0.6;0.85;0.95;1" dur="7s" begin="1.1s" repeatCount="indefinite"/>
      </text>
      <text x="40" y="256" opacity="0" fill="#39ff14">
        &gt; building things that ship, not just things that compile_
        <animate attributeName="opacity" values="0;0;1;1;1;1;0" keyTimes="0;0.08;0.12;0.6;0.85;0.95;1" dur="7s" begin="1.6s" repeatCount="indefinite"/>
      </text>
    </g>

    <!-- blinking cursor -->
    <rect x="40" y="266" width="11" height="18" fill="#39ff14">
      <animate attributeName="opacity" values="1;1;0;0" dur="1s" repeatCount="indefinite"/>
    </rect>

    <!-- side decorative bracket / circuit accents -->
    <g stroke="#1d5c3f" stroke-width="1.4" fill="none" opacity="0.7">
      <path d="M 870 60 L 855 60 L 855 90 L 845 90"/>
      <path d="M 870 280 L 855 280 L 855 250 L 845 250"/>
      <circle cx="845" cy="90" r="2.6" fill="#39ff14"/>
      <circle cx="845" cy="250" r="2.6" fill="#39ff14"/>
    </g>
  </g>
</svg>

---

### 🧩 about me

I move between code and design without really switching gears — React in one tab, Figma in the next. Currently **Design Lead** at NSSCE and **Joint Secretary** at STACS, and lately spending evenings teaching juniors that `git rebase` isn't actually trying to ruin their lives.

I came up through µLearn's **µFIFA** program — real tasks instead of tutorials, public track record instead of certificates. Outside of that, I'm the kind of person who debugs at 2 AM and still shows up for a 6 AM football match. There's no separating the two.

---

### 💻 what my terminal looks like

<div align="center">
<img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&size=16&pause=1500&color=39FF14&background=0D1117FF&center=true&vCenter=true&width=600&height=140&lines=%24+git+commit+-m+%22fix%3A+actually+fix+it+this+time%22;%24+git+push+origin+main;Resolving+deltas%3A+100%25+(47%2F47)%2C+done.;%24+npm+run+dev;%E2%9C%93+ready+in+312ms" />
</div>

---

### 🛠️ tech stack

<div align="center">
<img src="https://skillicons.dev/icons?i=react,nodejs,express,mongodb,mysql,figma,git,github,javascript,html,css&theme=dark" />
</div>

---

### 📊 github stats

<div align="center">
<img src="https://github-readme-stats.vercel.app/api?username=ayyushrk&show_icons=true&theme=tokyonight&hide_border=true" width="48%" />
<img src="https://github-readme-streak-stats.herokuapp.com/?user=ayyushrk&theme=tokyonight&hide_border=true" width="48%" />
</div>

<div align="center">
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=ayyushrk&layout=compact&theme=tokyonight&hide_border=true" width="50%" />
</div>

---

### 🏆 trophy case

<div align="center">
<img src="https://github-profile-trophy.vercel.app/?username=ayyushrk&theme=tokyonight&no-frame=true&row=1&column=6" />
</div>

---

### 🐍 contribution snake

<div align="center">
<img src="https://raw.githubusercontent.com/ayyushrk/ayyushrk/output/github-contribution-grid-snake.svg" />
</div>



---

### 📈 activity graph

<div align="center">
<img src="https://github-readme-activity-graph.vercel.app/graph?username=ayyushrk&theme=react-dark&hide_border=true&area=true" />
</div>

---

### ⚡ currently

- 🎯 Building player cards and validators for **µFIFA 2026**
- 🐙 Running a 3-day virtual **Git & GitHub workshop** for beginners
- 🧠 Chipping away at [LeetCode](https://leetcode.com/u/AyushRkumar) — one problem a day, streak status: *ambitious*
- ⚽ Arguing that football tactics and clean commit history require the exact same discipline

---

### 📫 reach me

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/your-handle)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://instagram.com/your-handle)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://your-portfolio.link)

</div>

<div align="center">
<img src="https://komarev.com/ghpvc/?username=ayyushrk&style=flat-square&color=2C5364" />
</div>

<div align="center">
<sub>if it works, don't touch it. if it doesn't, blame the merge conflict.</sub>
</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2C5364,100:0F2027&height=120&section=footer" />
