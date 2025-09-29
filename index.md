<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8"/>
  <title>Soumya Ranjan – Firmware & Fun</title>
  <meta name="viewport" content="width=device-width, initial-scale=1"/>
  <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css"/>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700&family=Share+Tech+Mono&display=swap" rel="stylesheet">
  <style>
  :root{--bg:#0d1117;--fg:#c9d1d9;--accent:#58a6ff;--pink:#f778ba;--mono:'Share Tech Mono',monospace;}
  *{box-sizing:border-box;margin:0;padding:0;font-family:Inter,sans-serif;}
  body{background:var(--bg);color:var(--fg);}
  header{padding:2rem 1rem;text-align:center;}
  #headshot{width:140px;height:140px;border-radius:50%;border:3px solid var(--accent);box-shadow:0 0 12px var(--accent);object-fit:cover;}
  #glitch{font-size:2.6rem;font-weight:700;letter-spacing:-.02em;margin-top:.5rem;}
  #emoji-row{font-size:1.4rem;margin-top:.5rem;letter-spacing:.3rem;}
  .tabs{display:flex;justify-content:center;gap:.4rem;margin:1.5rem 0 2rem 0;flex-wrap:wrap;}
  .tab{padding:.6rem 1rem;border:1px solid #30363d;border-radius:6px;cursor:pointer;transition:all .2s ease;background:#161b22;font-size:.9rem;}
  .tab:hover,.tab.active{border-color:var(--accent);box-shadow:0 0 8px var(--accent),0 0 16px var(--accent);}
  .pane{display:none;animation:fade .6s;}
  .pane.active{display:block;}
  @keyframes fade{from{opacity:0;transform:translateY(10px);}to{opacity:1;transform:translateY(0);}}
  .card{background:#161b22;border:1px solid #30363d;border-radius:8px;padding:1.5rem;margin-bottom:1.2rem;}
  .skill-tag{display:inline-block;background:#21262d;border:1px solid #30363d;border-radius:4px;padding:.25rem .5rem;margin:.15rem;font-size:.8rem;}
  table{width:100%;border-collapse:collapse;margin-top:1rem;}
  th,td{padding:.5rem;text-align:left;border-bottom:1px solid #30363d;}
  progress{width:100%;}
  .sub-tabs{display:flex;gap:.4rem;margin-bottom:1rem;}
  .sub-tab{padding:.4rem .8rem;border:1px solid #30363d;border-radius:4px;cursor:pointer;background:#0d1117;font-size:.8rem;}
  .sub-tab.active{border-color:var(--pink);color:var(--pink);}
  .sub-pane{display:none;}
  .sub-pane.active{display:block;}
  .logo-strip{display:flex;gap:1.5rem;justify-content:center;flex-wrap:wrap;margin:1rem 0;}
  .logo-strip img{height:40px;filter:grayscale(80%) opacity(.9);transition:.2s;}
  .logo-strip img:hover{filter:none;}
  #map{height:400px;border-radius:8px;border:1px solid #30363d;}
  details{margin-top:1rem;}
  summary{cursor:pointer;font-weight:700;color:var(--accent);}
  </style>
<base target="_blank">
</head>
<body>

<header>
  <img id="headshot" src="Ranjan.jpg" alt="Soumya Ranjan"/>
  <div id="glitch">Soumya Ranjan</div>
  <div id="emoji-row">
    <span title="Firmware">⚙️</span><span title="Systems">🖥️</span><span title="Robots">🤖</span><span title="Machine Learning">🧠</span><span title="Travel">✈️</span><span title="Football">⚽</span><span title="Anime">🎌</span><span title="Movies">🎬</span><span title="Television">📺</span><span title="Gaming">🎮</span>
  </div>
</header>

<div class="tabs">
  <div class="tab active" data-pane="about">About</div>
  <div class="tab" data-pane="exp">Experience</div>
  <div class="tab" data-pane="proj">Projects</div>
  <div class="tab" data-pane="travel">Travel</div>
  <div class="tab" data-pane="entertainment">Entertainment</div>
</div>

<!-- =========================================================
                         ABOUT
============================================================ -->
<div class="pane active" id="about">
  <section>
    <div class="card">
      <p>
        Currently working as a Software Engineer on the Bluetooth Firmware team at Qualcomm, I specialize in optimizing software for performance and memory utilization. I hold a Master’s degree in Computer Engineering (Embedded Systems) and a Bachelor’s degree in Electrical and Electronics Engineering.
      </p>
      <p>
        My journey is fueled by a passion for creating innovative solutions and a solid foundation in Low-Level Drivers, Operating Systems, Compilers, Parallel & GPU Programming, Hardware Design, Signal & Image Processing, Machine Learning and IoT.
      </p>
      <p>
        Outside of work you’ll find me scoring goals on the football field, listening to rock music, or competitively gaming. Oh—and I’m a Manchester United fan. <strong>#GGMU</strong>
      </p>

      <details>
        <summary>Technical Skills ▾</summary>
        <div style="margin-top:1rem;">
          <h4>Programming Languages</h4>
          <span class="skill-tag">C</span><span class="skill-tag">C++</span><span class="skill-tag">Python</span><span class="skill-tag">Embedded C</span><span class="skill-tag">Assembly</span><span class="skill-tag">SystemC</span><span class="skill-tag">Bash</span><span class="skill-tag">Rust</span><span class="skill-tag">CUDA</span>
          <h4>Software Tools</h4>
          <span class="skill-tag">Git</span><span class="skill-tag">Altium</span><span class="skill-tag">Proteus</span><span class="skill-tag">Make</span><span class="skill-tag">CMake</span><span class="skill-tag">MATLAB</span><span class="skill-tag">Simulink</span><span class="skill-tag">FreeRTOS</span><span class="skill-tag">TensorFlow</span><span class="skill-tag">PyTorch</span><span class="skill-tag">Keil</span><span class="skill-tag">Trace32</span><span class="skill-tag">OpenBMC</span>
          <h4>Technologies</h4>
          <span class="skill-tag">Firmware</span><span class="skill-tag">RTOS</span><span class="skill-tag">Image Processing</span><span class="skill-tag">Embedded Linux</span><span class="skill-tag">Machine Learning</span><span class="skill-tag">Deep Learning</span><span class="skill-tag">Networking</span><span class="skill-tag">Robotics</span><span class="skill-tag">PCB Design</span><span class="skill-tag">Compilers (GCC/Clang/LLVM)</span><span class="skill-tag">ARM / RISC-V / x86</span>
        </div>
      </details>
    </div>
  </section>
</div>

<!-- =========================================================
                       EXPERIENCE
============================================================ -->
<div class="pane" id="exp">
  <section>
    <h2>Experience</h2>
    <div class="logo-strip">
      <img src="qualcomm.png" alt="Qualcomm"/><img src="raptee.png" alt="Raptee"/>
      <img src="expleo.png" alt="Expleo"/><img src="mistral.png" alt="Mistral"/>
      <img src="wimera.png" alt="Wimera"/><img src="bosch.png" alt="Bosch"/>
    </div>

    <div class="card">
      <h3>Qualcomm – Software Engineer (Feb 2024 – Present)</h3>
      <ul><li>BT/BLE features 2.4/5 GHz pre- → post-silicon; co-existence BT/Wi-Fi/UWB; chained crash-dump framework.</li></ul>
    </div>
    <div class="card">
      <h3>Qualcomm – Software Engineer Intern (Jun – Sep 2023)</h3>
      <ul><li>Automated OTP macro generation from JSON; IOP/SPI ring-buffer loggers; ELF call-tree generator.</li></ul>
    </div>
    <div class="card">
      <h3>Raptee Motors – Firmware Engineer (Jun – Sep 2022)</h3>
      <ul><li>Cut boot-time 50 % with shared-mem IPC & semaphores; BLE vehicle unlock on BeagleBone-AI SoC; CMake refactor.</li></ul>
    </div>
    <div class="card">
      <h3>Expleo Group – Software Engineer (Oct 2021 – Jun 2022)</h3>
      <ul><li>ECU models in Simulink; CAN→LSTM dataset generator; deployed 80 % acc. anomaly detector (PyTorch) on ECU.</li></ul>
    </div>
    <div class="card">
      <h3>Mistral Solutions – Hardware Intern (Jan – Sep 2021)</h3>
      <ul><li>9 GHz DAC on JESD204B; FMCW radar modules; Sitara AM263x driver bring-up.</li></ul>
    </div>
    <div class="card">
      <h3>Wimera Systems – R&D Intern (May – Jun 2019)</h3>
      <ul><li>Battery-management with charge-pumps; OTA updates on CC3220; RS232 peripheral link.</li></ul>
    </div>
    <div class="card">
      <h3>Bosch – Electrical Maint. Intern (May – Jun 2018)</h3>
      <ul><li>Servo-drive install & PLC/sensor upkeep; machine maintenance.</li></ul>
    </div>
  </section>
</div>

<!-- =========================================================
                        PROJECTS
============================================================ -->
<div class="pane" id="proj">
  <section>
    <h2>Projects</h2>
    <div class="card">
      <h3>Handy – Smart Glove for Blind People</h3>
      <p>Camera + GPT-4o obstacle narration, haptic feedback, fall detection, indoor & outdoor navigation.</p>
    </div>
    <div class="card">
      <h3>Smart IoT-based Pollution Monitoring & Purifying System</h3>
      <p>ESP8266/ESP32 + PMS5003, MQTT over WebSocket, MATLAB Thing-Speak dashboard, auto-triggered purifier.</p>
    </div>
    <div class="card">
      <h3>Battery Cell Voltage Balancing Techniques</h3>
      <p>Fly-back converter cell balancing (2/4/6-cell) in Simulink for ultra-light EVs.</p>
    </div>
    <div class="card">
      <h3>Human Following Robot</h3>
      <p>Arduino UNO + IR & Ultrasonic sensors; wooden chassis; servo-driven locomotion.</p>
    </div>
    <div class="card">
      <h3>Intelligent Helmet for Coal Miners</h3>
      <p>LM35, MQ2, DHT11 → Arduino → Zigbee mesh; real-time enviro-alerts.</p>
    </div>
    <div class="card">
      <h3>Optical Coherence Tomography (OCT) Camera</h3>
      <p>27 kHz line-scan camera with OpenCV + spectral analysis on FPGA for medical imaging. <a href="https://www.warse.org/IJETER/static/pdf/file/ijeter1308102020.pdf" target="_blank">Paper</a></p>
    </div>
    <div class="card">
      <h3>Smart Traffic Management with Violation Detection</h3>
      <p>FPGA-based system + solar battery module; published research.</p>
    </div>
    <div class="card">
      <h3>Drowsiness Detection with CNN</h3>
      <p>4 K-sample Kaggle dataset; MATLAB CNN; facial-parameter based alert.</p>
    </div>
    <div class="card">
      <h3>Reusable Rocket Landing Control</h3>
      <p>State-space modelling, Jacobian linearisation, pole-placement controller in MATLAB/Simulink.</p>
    </div>
    <div class="card">
      <h3>Smart Parking System (Android)</h3>
      <p>GPS + IR vacancy detection; native Android app guides drivers to free slots.</p>
    </div>
    <div class="card">
      <h3>Gyro Stabilization Platform</h3>
      <p>MPU6050 → Arduino UNO; 3-servo self-balancing platform with closed-loop control.</p>
    </div>
  </section>
</div>

<!-- =========================================================
                         TRAVEL
============================================================ -->
<div class="pane" id="travel">
  <section>
    <h2>Travel</h2>
    <div class="sub-tabs">
      <div class="sub-tab active" data-sub="world">World Map</div>
      <div class="sub-tab" data-sub="usa">USA</div>
    </div>

    <div class="sub-pane active" id="world">
      <div id="map"></div>
    </div>

    <div class="sub-pane" id="usa">
      <div class="card">
        <h3>States Visited</h3>
        <p>CA, TX, NY, WA, OR, NV, AZ, UT, CO, IL, FL, MA, VA, MD, PA, NJ, OH, MI, NC, GA …</p>
      </div>
      <div class="card">
        <h3>National Parks</h3>
        <p>Yosemite, Grand Canyon, Zion, Bryce, Arches, Rocky Mountain, Great Smoky Mountains, Everglades, Joshua Tree, Sequoia …</p>
      </div>
    </div>
  </section>
</div>

<!-- =========================================================
                      ENTERTAINMENT
============================================================ -->
<div class="pane" id="entertainment">
  <section>
    <h2>Entertainment</h2>
    <div class="sub-tabs">
      <div class="sub-tab active" data-sub="movies">Movies</div>
      <div class="sub-tab" data-sub="anime">Anime</div>
      <div class="sub-tab" data-sub="tv">TV Shows</div>
      <div class="sub-tab" data-sub="gaming">Gaming</div>
    </div>

    <div class="sub-pane active" id="movies">
      <p>Movie list coming soon …</p>
    </div>
    <div class="sub-pane" id="anime">
      <p>Anime list coming soon …</p>
    </div>
    <div class="sub-pane" id="tv">
      <p>TV list coming soon …</p>
    </div>
    <div class="sub-pane" id="gaming">
      <p>Gaming list coming soon …</p>
    </div>
  </section>
</div>

<!-- ==================  JS  ================== -->
<script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>
<script>
/* ----- main tab switcher ----- */
document.querySelectorAll('.tab').forEach(tab=>{
  tab.addEventListener('click',()=>{
    document.querySelectorAll('.tab').forEach(t=>t.classList.remove('active'));
    document.querySelectorAll('.pane').forEach(p=>p.classList.remove('active'));
    tab.classList.add('active');
    document.getElementById(tab.dataset.pane).classList.add('active');
  });
});

/* ----- travel sub-tab switcher ----- */
document.querySelectorAll('.sub-tab').forEach(sub=>{
  sub.addEventListener('click',()=>{
    const parent = sub.closest('.pane');
    parent.querySelectorAll('.sub-tab').forEach(s=>s.classList.remove('active'));
    parent.querySelectorAll('.sub-pane').forEach(p=>p.classList.remove('active'));
    sub.classList.add('active');
    document.getElementById(sub.dataset.sub).classList.add('active');
  });
});

/* ----- leaflet world map ----- */
const map = L.map('map').setView([20,0], 2);
L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png',{
  attribution:'© OpenStreetMap'
}).addTo(map);

fetch('markers.json')
  .then(r=>r.json())
  .then(arr=>{
    arr.forEach(m=>{
      const flag = m.flag ? `<img src="${m.flag}" width="20" style="border:1px solid #ccc"> ` : '';
      L.marker(m.coords)
       .addTo(map)
       .bindPopup(`${flag}<b>${m.country}</b>`);
    });
  });
</script>
</body>
</html>
