---
title: "iNEURON Systems Lab"
permalink: /scholars/
---

<style>

  #lab-map {
    height: 420px;
    margin-top: 2rem;
    border-radius: 10px;
    border: 1px solid #e5e7eb;
  }
  .visits-table {
    border-collapse: collapse;
    width: 100%;
    max-width: 560px;
  }
  .visits-table th, .visits-table td {
    padding: 6px 10px;
    border-bottom: 1px solid #e5e7eb;
  }
  .visits-table th { text-align: left; }
  .visits-table td:last-child, .visits-table th:last-child { text-align: right; }

  
/* Reuse the card/grid vibe from Publications */
.sch-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 1.2rem;
  margin-top: 1.2rem;
}

@media (min-width: 720px) {
  .sch-grid {
    grid-template-columns: 1fr 1fr;
  }
}

.sch-card {
  border: 2px solid #1a73e8;
  border-radius: 12px;
  padding: 1.2rem 1.5rem;
  background: #fff;
  transition: 0.3s ease;
}

.sch-card:hover {
  background-color: #f0f8ff;
  transform: scale(1.01);
  box-shadow: 0 4px 12px rgba(26, 115, 232, 0.1);
}

/* Header with (future) photo + name + subtitle */
.sch-header {
  display: flex;
  gap: 1rem;
  align-items: flex-start;
}

/* Photo placeholder; replace with <img> later */
.sch-avatar {
  width: 80px;
  height: 80px;
  border-radius: 50%;
  background:#e9eefc;
  color:#1a73e8;
  display:flex;
  align-items:center;
  justify-content:center;
  font-weight: 700;
  font-size: 1.2rem;
  box-shadow: 0 2px 6px rgba(0,0,0,0.08);
  user-select:none;
}

.sch-name {
  font-size: 1.05rem;
  font-weight: 600;
  margin-bottom: 0.15rem;
  color: #111;
}

.sch-sub {
  font-size: 0.95rem;
  color: #333;
  opacity: 0.9;
}

/* Section titles & lists */
.sch-sec {
  font-size: 0.92rem;
  margin-top: 0.8rem;
  opacity: 0.9;
  text-transform: uppercase;
  letter-spacing: 0.02em;
}

.sch-list {
  margin: 0.25rem 0 0.25rem 1.1rem;
}

/* Badges for status/keywords */
.badge {
  display: inline-block;
  padding: 4px 10px;
  border-radius: 12px;
  font-weight: 600;
  font-size: 0.82rem;
  margin-right: 0.35rem;
}

.logo {
  max-height: 30px;
  max-width: 60px;
  object-fit: contain;
  float: right;
  margin-left: 6px;
}

.badge.guide {
  background-color: #ff9800; /* orange for distinction */
  color: white;
}
  
.sch-photo {
  width: 60px;          /* adjust size */
  height: 60px;         /* keep it square */
  border-radius: 50%;   /* makes it circular */
  object-fit: cover;    /* crops the image instead of stretching */
  margin-right: 10px;   /* spacing from text */
}
  
.badge.current { color: #0a539e; background: #e5f1ff; }
.badge.alumni  { color: #1a7f3d; background: #dcfce7; }
.badge.tag     { color: #1a73e8; background: #eef5ff; }

/* Optional section headers for groups */
.group-title {
  margin-top: 2rem;
  font-size: 1.1rem;
  text-align: left;
  color: #0a539e;
  border-left: 4px solid #1a73e8;
  padding-left: 0.5rem;
}
</style>

<p>
This page highlights scholars — both current UMKC students and alumni — who collaborate with me on research and publications.
</p>

<section class="lab-section">
<!-- Logo goes here -->
  <!-- Logo + Lab name side by side -->
<div style="display:flex; align-items:center; gap:1rem; margin-bottom:1rem;">
  <!-- Logo -->
  <img src="/images/neuron.png" alt="iNEURON Systems Lab Logo" style="max-width:150px; height:auto;">
  
  <!-- Lab name -->
  <h2 style="margin:0;">
    iNEURON Systems Lab<span style="font-weight:normal; font-size:0.8em;"><br>
    Intelligent Neural Energy-efficient Understanding for RF and Optimization in Networks Lab
    </span>
  </h2>
</div>

  <p>
    The <strong>iNEURON Systems Lab</strong> at UMKC focuses on the design of 
    <em>energy-efficient intelligent systems</em> for <em>RF signal classification</em> and 
    <em>low-power deep learning</em>. Our work bridges <em>algorithm design</em> and 
    <em>hardware-aware optimization</em>, enabling scalable solutions for 
    <em>real-time communication</em>, <em>sensing</em>, and <em>defense applications</em>.
</p>


  <ul>
    <li><strong>RF Signal Classification:</strong> Designing lightweight, reliable methods for classifying communication signals across diverse environments, combining statistical feature extraction with machine learning.</li>
    <li><strong>Low-Power Deep Learning:</strong> Developing hardware-efficient neural networks using techniques such as piecewise linear activation functions and compiler-driven optimizations, ensuring scalability on GPUs, FPGAs, and edge devices.</li>
    <li><strong>Hardware-Software Co-Design:</strong> Bridging algorithmic innovations with hardware constraints to achieve energy-aware, real-time deployment for communication, sensing, and defense applications.</li>
  </ul>
</section>


<div class="group-title">Research Lead</div>
<div class="sch-grid">

  <!-- Nimisha -->
  <div class="sch-card">
    <div class="sch-header">
      <img src="/images/rahul.png" alt="Rahul" class="sch-photo">  
      <div>
        <div class="sch-name">Srinivas Rahul Sapireddy, PhD 
          <a href="https://www.linkedin.com/in/srsapireddy2020/" target="_blank">
          <img src="/images/linkedin.png" alt="LinkedIn" style="width:18px; height:18px; margin-left:6px; vertical-align:middle;"><img src="/images/UMKC.png" alt="UMKC Logo" class="logo">
        </a>
        </div>
        <div class="sch-sub">Instructor, School of Science & Engineering — UMKC</div>
        <div style="margin-top:0.35rem;">
          <span class="badge guide">Guide</span>
          <span class="badge tag">Hardware-Aware AI</span>
          <span class="badge tag">RF Signal Classification</span>
        </div>
      </div>
    </div>
    <div class="sch-sec">Research interests</div>
    <ul class="sch-list">
      <li>Hardware-efficient deep learning models</li>
      <li>Low-power RF signal classification</li>
    </ul>
    <div class="sch-sec">Active topics / papers</div>
    <ul class="sch-list">
      <li>Efficient Deep Neural Networks</li>
    </ul>
  </div>

</div>

<div class="group-title">Current Students</div>
<div class="sch-grid">

  <!-- Nimisha -->
  <div class="sch-card">
    <div class="sch-header">
      <img src="/images/nimisha.jpeg" alt="Nimisha" class="sch-photo">  
      <div>
        <div class="sch-name">Nimisha Chandra 
          <a href="https://www.linkedin.com/in/nimisha-chandra-99130a20/?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=ios_app" target="_blank">
          <img src="/images/linkedin.png" alt="LinkedIn" style="width:18px; height:18px; margin-left:6px; vertical-align:middle;"><img src="/images/UMKC.png" alt="UMKC Logo" class="logo">
        </a>
        </div>
        <div class="sch-sub">Current UMKC student — Master of Science in Electrical Engineering, Spring 2026</div>
        <div style="margin-top:0.35rem;">
          <span class="badge current">Current</span>
          <span class="badge tag">RF Signal Classification</span>
          <span class="badge tag">Nanoscale Manufacturing</span>
        </div>
      </div>
    </div>
    <div class="sch-sec">Research interests</div>
    <ul class="sch-list">
      <li>Machine Learning and Deep Learning</li>
      <li>Runtime and memory optimization for edge inference</li>
    </ul>
    <div class="sch-sec">Active topics / papers</div>
    <ul class="sch-list">
      <li>Co-author: From Rule based to Neural: RF Statistical Envelope Analysis (To be submitted)</li>
    </ul>
  </div>

</div>

<div class="group-title">Alumni</div>
<div class="sch-grid">

  <!-- Heamanth Bandi -->
  <div class="sch-card">
    <div class="sch-header">
           <img src="/images/hemanth.png" alt="Hemanth" class="sch-photo">  
      <div>
        <div class="sch-name">Hemanth Bandi
        <a href="https://www.linkedin.com/in/hemanth-bandi-095266859317574524/" target="_blank">
          <img src="/images/linkedin.png" alt="LinkedIn" style="width:18px; height:18px; margin-left:6px; vertical-align:middle;"><img src="/images/UMKC.png" alt="UMKC Logo" class="logo">
        </a>
        </div>
        <div class="sch-sub">Alumni UMKC student — Master of Science in Computer Science, Spring 2023</div>
        <div style="margin-top:0.35rem;">
          <span class="badge alumni">Alumni</span>
          <span class="badge tag">RF</span>
          <span class="badge tag">Deep Learning</span>
          <span class="badge tag">Reinforcement Learning</span>
        </div>
      </div>
    </div>
    <div class="sch-sec">Research interests</div>
    <ul class="sch-list">
      <li>RF modulation recognition </li>
      <li>Reinforcement Learning</li>
    </ul>
    <div class="sch-sec">Active topics / papers</div>
    <ul class="sch-list">
      <li>Reinforcement Learning manuscript (Springer, To be submitted)</li>
      <li>Benchmarking R-aware binning with envelope-feature baselines (IEEE, submitted)</li>
    </ul>
  </div>

  <!-- Jahavani -->
  <div class="sch-card">
    <div class="sch-header">
      <img src="/images/jahvani.jpeg" alt="Jahvani" class="sch-photo">  
      <div>
        <div class="sch-name">Jahnavi Sri Kavya Bollimuntha
        <a href="https://www.linkedin.com/in/jahnavi-sri-kavya-bollimuntha/" target="_blank">
          <img src="/images/linkedin.png" alt="LinkedIn" style="width:18px; height:18px; margin-left:6px; vertical-align:middle;"><img src="/images/UMKC.png" alt="UMKC Logo" class="logo">
        </a>
        </div>
        <div class="sch-sub">Alumni UMKC Student — B.S. Computer Science and Engineering, and Master of Science in Computer Science, Fall 2023</div>
        <div style="margin-top:0.35rem;">
          <span class="badge alumni">Alumni</span>
          <span class="badge tag">Deep Learning</span>
          <span class="badge tag">Radio Frequence Signal Classification</span>
        </div>
      </div>
    </div>
    <div class="sch-sec">Research interests</div>
    <ul class="sch-list">
      <li>Deep Learning</li>
      <li>Modulation Recognition and Classification</li>
      <li>Envelope statistics (R-values), Dataset Engineering</li>
    </ul>
    <div class="sch-sec">Active topics / papers</div>
    <ul class="sch-list">
      <li>Collaborative paper on RF signal analysis (draft in progress)</li>
    </ul>
  </div>

</div>


<!-- Title + Map + Counters -->
<h2 class="group-title">Global Visitors & Collaborations</h2>

<link rel="stylesheet" href="https://unpkg.com/leaflet/dist/leaflet.css"/>
<div id="lab-map" role="region" aria-label="World map of visits and collaborations"></div>

<div style="margin-top: 1rem;">
  <div>Total Visits: <span id="total-visits">–</span></div>
</div>

<h3 style="margin-top:1rem">Visits by Country</h3>
<div id="visits-by-country">Loading…</div>

<!-- Scripts -->
<script src="https://unpkg.com/leaflet/dist/leaflet.js"></script>
<script>
/* ========= CONFIG (change NAMESPACE to your own stable key) ========= */
const NAMESPACE = "srsapireddy.github.io/scholars"; 
const COUNTRIES_TO_SHOW = {
  "US":"United States","IN":"India","CA":"Canada","GB":"United Kingdom","DE":"Germany",
  "FR":"France","IT":"Italy","ES":"Spain","BR":"Brazil","MX":"Mexico","AU":"Australia",
  "CN":"China","JP":"Japan","KR":"South Korea","AE":"United Arab Emirates","SA":"Saudi Arabia",
  "TR":"Türkiye","SG":"Singapore","NL":"Netherlands","SE":"Sweden","NO":"Norway","FI":"Finland",
  "DK":"Denmark","CH":"Switzerland","BE":"Belgium","IE":"Ireland"
};
/* Approx country centroids (add more as needed) */
const COUNTRY_CENTROIDS = {
  US:[39.8,-98.6], IN:[22.8,79.6], CA:[62.0,-96.0], GB:[54.0,-2.0], DE:[51.2,10.4],
  FR:[46.2,2.2], IT:[42.8,12.5], ES:[40.2,-3.7], BR:[-10.8,-52.9], MX:[23.6,-102.5],
  AU:[-25.3,133.8], CN:[35.9,104.2], JP:[36.2,138.3], KR:[36.5,127.9], AE:[24.3,54.4],
  SA:[23.9,45.1], TR:[39.0,35.2], SG:[1.35,103.82], NL:[52.1,5.3], SE:[62.8,16.7],
  NO:[61.2,8.0], FI:[64.9,26.0], DK:[56.2,9.5], CH:[46.8,8.2], BE:[50.6,4.6], IE:[53.1,-8.0]
};

/* ========= Utilities ========= */
async function fetchJSON(url) {
  const r = await fetch(url, { cache: "no-store" });
  if (!r.ok) throw new Error("HTTP " + r.status);
  return r.json();
}
async function getCountryCode() {
  // Try ipwho.is
  try {
    const geo = await fetchJSON("https://ipwho.is/");
    if (geo && geo.country_code) return geo.country_code;
  } catch {}
  // Fallback ipapi.co
  try {
    const geo2 = await fetchJSON("https://ipapi.co/json/");
    if (geo2 && geo2.country) return geo2.country;
  } catch {}
  // (Optional) add more providers if needed
  return null; // country unknown
}
async function countAPI_hit(key) {
  try {
    const url = `https://api.countapi.xyz/hit/${encodeURIComponent(NAMESPACE)}/${encodeURIComponent(key)}`;
    const r = await fetch(url, { cache: "no-store" });
    return r.ok;
  } catch { return false; }
}
async function countAPI_get(key) {
  try {
    const url = `https://api.countapi.xyz/get/${encodeURIComponent(NAMESPACE)}/${encodeURIComponent(key)}`;
    const r = await fetch(url, { cache: "no-store" });
    if (!r.ok) return 0;
    const data = await r.json();
    return typeof data.value === "number" ? data.value : 0;
  } catch { return 0; }
}

/* ========= Map setup ========= */
let map, markersLayer;
function initMap() {
  if (map) return;
  map = L.map("lab-map", { scrollWheelZoom: false }).setView([20, 0], 2);
  L.tileLayer("https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png", {
    attribution: "&copy; OpenStreetMap contributors"
  }).addTo(map);
  markersLayer = L.layerGroup().addTo(map);

  // Optional: fixed collaboration pins (add yours here)
  // L.marker([39.0997,-94.5786]).addTo(markersLayer).bindPopup("UMKC - iNEURON Systems Lab");
  // L.marker([40.1164,-88.2434]).addTo(markersLayer).bindPopup("UIUC - Collaboration");
}
function updateMapMarkers(countryList) {
  if (!markersLayer) return;
  markersLayer.clearLayers();
  countryList.forEach(({ iso2, name, count }) => {
    const c = COUNTRY_CENTROIDS[iso2];
    if (c) L.marker(c).addTo(markersLayer).bindPopup(`${name}: ${count} visit${count===1?"":"s"}`);
  });
}

/* ========= Render stats ========= */
async function renderStats() {
  const total = await countAPI_get("total");
  const totalEl = document.getElementById("total-visits");
  if (totalEl) totalEl.textContent = total.toLocaleString();

  const entries = await Promise.all(
    Object.entries(COUNTRIES_TO_SHOW).map(async ([iso2, name]) => {
      const v = await countAPI_get(iso2);
      return { iso2, name, count: v };
    })
  );
  const nonzero = entries.filter(e => e.count > 0).sort((a,b) => b.count - a.count);

  const container = document.getElementById("visits-by-country");
  if (!container) return;
  if (nonzero.length === 0) {
    container.textContent = "No country-level visits recorded yet.";
  } else {
    container.innerHTML = `
      <table class="visits-table">
        <thead><tr><th>Country</th><th>Visits</th></tr></thead>
        <tbody>
          ${nonzero.map(e => `<tr><td>${e.name}</td><td>${e.count}</td></tr>`).join("")}
        </tbody>
      </table>
    `;
  }
  updateMapMarkers(nonzero);
}

/* ========= Boot sequence (increment FIRST, then render) ========= */
(async function boot() {
  initMap();

  // Increment total
  await countAPI_hit("total");

  // Increment by country (if we can detect it)
  const cc = await getCountryCode();
  if (cc) await countAPI_hit(cc);

  // Now render counts so first load reflects the increment
  await renderStats();

  // Refresh every 60s for open pages
  setInterval(renderStats, 60000);
})();
</script>
