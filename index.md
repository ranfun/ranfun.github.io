---
layout: default
title: Soumya Ranjan – Firmware | Fun
---

<style>
:root{
  --bg:#0d1117;
  --fg:#c9d1d9;
  --accent:#58a6ff;
  --pink:#f778ba;
  --mono:"SF Mono",Monaco,monospace;
}
body{background:var(--bg);color:var(--fg);font-family:-apple-system,BlinkMacSystemFont,"Segoe UI",Helvetica,Arial,sans-serif;margin:0;padding:0;}
a{color:var(--accent);text-decoration:none;}
h1,h2,h3{letter-spacing:-.02em;}
header{text-align:center;padding:6rem 1rem 3rem;}
header h1{font-size:3rem;margin:0;}
header p{font-size:1.2rem;color:var(--pink);}
nav{display:flex;gap:1rem;justify-content:center;margin-bottom:3rem;}
section{max-width:800px;margin:0 auto;padding:2rem 1rem;}
.card{background:#161b22;border:1px solid #30363d;border-radius:8px;padding:1.5rem;margin-bottom:1.5rem;}
.skill-tag{display:inline-block;background:#21262d;border:1px solid #30363d;border-radius:6px;padding:.25rem .5rem;margin:.15rem;font-size:.8rem;}
table{width:100%;border-collapse:collapse;margin-top:1rem;}
th,td{padding:.5rem;text-align:left;border-bottom:1px solid #30363d;}
progress{width:100%;}
</style>

<header>
  <h1>Soumya Ranjan</h1>
  <p>Firmware Engineer • Silicon bring-up enthusiast • Anime binge-watcher</p>
  <nav>
    <a href="#about">About</a>
    <a href="#exp">Experience</a>
    <a href="#proj">Projects</a>
    <a href="#entertainment">Entertainment</a>
  </nav>
</header>

<section id="about">
  <h2>About / Skills</h2>
  <div class="card">
    <p>Master’s Computer Engineering @ UCI • ex-Qualcomm, Raptee, Expleo.<br>
    I make radios play nice together, shrink boot times, and occasionally teach GPUs to see.</p>
    <h3>Languages</h3>
    <span class="skill-tag">C</span><span class="skill-tag">C++</span><span class="skill-tag">Python</span><span class="skill-tag">Rust</span><span class="skill-tag">CUDA</span><span class="skill-tag">Assembly</span>
    <h3>Tooling</h3>
    <span class="skill-tag">Git</span><span class="skill-tag">FreeRTOS</span><span class="skill-tag">TensorFlow</span><span class="skill-tag">Keil</span><span class="skill-tag">Altium</span><span class="skill-tag">Jira (kidding)</span>
  </div>
</section>

<section id="exp">
  <h2>Experience</h2>
  <div class="card">
    <h3>Qualcomm – Software Engineer</h3>
    <em>Feb 2024 – now</em>
    <ul>
      <li>Shipped BT/BLE features on 2.4/5 GHz from pre- to post-silicon.</li>
      <li>Built chained crash-dump framework cutting debug time by 30 %.</li>
    </ul>
  </div>
  <div class="card">
    <h3>Raptee Motors – Firmware Engineer (intern)</h3>
    <em>Jun – Sep 2022</em>
    <ul>
      <li>Slashed boot time 50 % via shared-memory IPC & semaphore tuning.</li>
      <li>Bluetooth-based vehicle unlock on custom BeagleBone-AI SoC.</li>
    </ul>
  </div>
  <!-- add more cards -->
</section>

<section id="proj">
  <h2>Featured Projects</h2>
  <div class="card">
    <h3>Handy – AI haptic glove for the visually impaired</h3>
    <p>Camera + GPT-4o obstacle narration, fall detection, edge-optimized inference on RP2040.</p>
    <a href="https://github.com/ranfun/Handy">GitHub →</a>
  </div>
  <div class="card">
    <h3>F1/10th Autonomous Racer</h3>
    <p>ROS2, LiDAR, pure-pursuit + MPC @ 40 mph. Top-10 at IEEE race.</p>
  </div>
</section>

<section id="entertainment">
  <h2>Entertainment Consumed 🍿</h2>

  | Title | Type | Year | Rating /5 | Finished |
  |---|---|---|---|---|
  | *Steins;Gate* | Anime | 2011 | 5 | ✅ |
  | *Blade Runner 2049* | Movie | 2017 | 5 | ✅ |
  | *Cyberpunk: Edgerunners* | Anime | 2022 | 4.5 | ✅ |
  | *Dune: Part Two* | Movie | 2024 | 4.5 | ✅ |
  | *Shōgun* | TV | 2024 | 4 | ✅ |

  <p><em>CSV-friendly table—swap in your own <a href="https://simkl.com" target="_blank">Simkl</a> or <a href="https://myanimelist.net" target="_blank">MAL</a> export.</em></p>

  <h3>2025 Watch-progress</h3>
  <label>Attack on Titan Final Season (ep 87/89)</label>
  <progress value="87" max="89"></progress>

  <label>Monogatari Series (65/100)</label>
  <progress value="65" max="100"></progress>

  <p>
    <a href="https://anilist.co/user/ranfun" target="_blank">Full AniList stats →</a>
  </p>
</section>

<footer style="text-align:center;padding:4rem 1rem;font-size:.8rem;color:#8b949e;">
  Built with ☕ & Markdown – <a href="https://github.com/ranfun/ranfun.github.io">source</a>
</footer>
