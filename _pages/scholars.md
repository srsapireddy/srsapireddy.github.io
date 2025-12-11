---
title: "Scholars"
permalink: /scholars/
---

<style>

.centered {
  text-align: center;
  margin: 1rem 0;
}


  
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
        <div class="sch-sub">Assistant Professor, College of Engineering — Illinois State University</div>
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
      <img src="/images/place.jpg" alt="Abreham" class="sch-photo">  
      <div>
        <div class="sch-name">Abreham Mesfin 
          <a href="https://www.linkedin.com/in/abreham-mesfin-820084301?original_referer=https%3A%2F%2Fwww.google.com%2F" target="_blank">
          <img src="/images/linkedin.png" alt="LinkedIn" style="width:18px; height:18px; margin-left:6px; vertical-align:middle;"><img src="/images/UMKC.png" alt="UMKC Logo" class="logo">
        </a>
        </div>
        <div class="sch-sub">Current UMKC student — Bachelor of Science in Electrical and Computer Engineering, 2028</div>
        <div style="margin-top:0.35rem;">
          <span class="badge current">Current</span>
          <span class="badge tag">Logic Design</span>
          <span class="badge tag">Engineering Computation</span>
        </div>
      </div>
    </div>
    <div class="sch-sec">Research interests</div>
    <ul class="sch-list">
      <li>Minimization techniques for Boolean functions</li>
      <li>Low-power circuit implementations</li>
    </ul>
    <div class="sch-sec">Active topics / papers</div>
    <ul class="sch-list">
      <li>Digital Circuit Optimization Techniques (To be submitted)</li>
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
<br>
<br>

<div style="text-align:center; margin-top:1rem;">
<a href="https://info.flagcounter.com/UCHm"><img src="https://s01.flagcounter.com/map/UCHm/size_l/txt_121AFF/border_CCCCCC/pageviews_1/viewers_0/flags_0/" alt="Flag Counter" border="0"></a>
</div>
<br>
<br>
<div style="text-align:center; margin-top:1rem;">
<a href="https://info.flagcounter.com/3uG8"><img src="https://s05.flagcounter.com/countxl_US/3uG8/bg_FFFFFF/txt_1239FF/border_C9CCC8/columns_8/maxflags_40/viewers_0/labels_1/pageviews_1/flags_0/percent_0/" alt="Flag Counter" border="0"></a>
</div>

