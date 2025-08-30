---
title: "Scholars"
permalink: /scholars/
---

<style>
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

<div class="group-title">Current Scholars</div>
<div class="sch-grid">

  <!-- Nimisha -->
  <div class="sch-card">
    <div class="sch-header">
      <!-- Replace with <img src="/assets/images/scholars/nimisha.jpg" alt="Nimisha" ...> later -->
      <div class="sch-avatar">NC</div>
      <div>
        <div class="sch-name">Nimisha Chandra</div>
        <div class="sch-sub">Current UMKC student — Master of Science in Electrical Engineering</div>
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
      <li>Co-author: From Rule based to Neural: RF Statistical Envolope Analysis (To be submitted)</li>
    </ul>
  </div>

</div>

<div class="group-title">Alumni Scholars</div>
<div class="sch-grid">

  <!-- Heamanth Bandi -->
  <div class="sch-card">
    <div class="sch-header">
      <!-- PHOTO PLACEHOLDER.
           When ready, replace this div with:
           <img src="/assets/images/scholars/heamanth.jpg" alt="Heamanth Bandi"
                style="width:80px;height:80px;object-fit:cover;border-radius:50%;box-shadow:0 2px 6px rgba(0,0,0,0.08);"> -->
      <div class="sch-avatar">HB</div>
      <div>
        <div class="sch-name">Hemanth Bandi</div>
        <div class="sch-sub">Alumni UMKC student — Master of Science in Computer Science</div>
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
      <!-- Replace with <img src="/assets/images/scholars/jahavani.jpg" alt="Jahavani" ...> later -->
      <div class="sch-avatar">JH</div>
      <div>
        <div class="sch-name">Jahavani</div>
        <div class="sch-sub">Alumni UMKC Student — B.S. Computer Science and Engineering, and Master of Science in Computer Science</div>
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


