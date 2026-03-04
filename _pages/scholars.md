---
title: ""
layout: single
permalink: /scholars/
author_profile: true
toc: false
---

<style>
:root{
  --blue:#1a73e8;
  --blue2:#0b5bd3;
  --isu:#DC143C;
  --bg:#ffffff;
  --muted:#5f6368;
  --shadow:0 10px 30px rgba(0,0,0,0.08);
  --shadow2:0 2px 10px rgba(0,0,0,0.05);
  --radius:16px;
  --radius2:12px;
  --border:rgba(26,115,232,0.18);
}

/* Hero */
.page-hero{
  border-radius:var(--radius);
  padding:2rem 1.8rem;
  margin-bottom:1.6rem;
  background:linear-gradient(135deg,#e9f3ff 0%, #ffffff 60%);
  border:1px solid rgba(26,115,232,0.25);
  box-shadow:var(--shadow);
}
.page-hero h2{
  margin:0 0 0.35rem 0;
  font-size:1.9rem;
  line-height:1.2;
  color:#0b1f44;
}
.page-hero p{
  margin:0.55rem 0 0 0;
  color:var(--muted);
  font-size:1.05rem;
  max-width:95ch;
}

/* Buttons */
.hero-links{
  display:flex;
  flex-wrap:wrap;
  gap:0.7rem;
  margin-top:1.1rem;
}
.btn-link{
  display:inline-flex;
  align-items:center;
  gap:0.45rem;
  padding:0.55rem 0.9rem;
  border-radius:10px;
  background:var(--blue);
  color:#ffffff !important;
  text-decoration:none !important;
  font-weight:800;
  box-shadow:var(--shadow2);
  transition:0.2s ease-in-out;
}
.btn-link:hover{ background:var(--blue2); transform:translateY(-1px); }
.btn-link.secondary{
  background:#ffffff;
  color:var(--blue) !important;
  border:1px solid rgba(26,115,232,0.25);
}

/* Section */
.section{
  border:1px solid var(--border);
  background:var(--bg);
  padding:1.35rem 1.5rem;
  margin-bottom:1.3rem;
  border-radius:var(--radius2);
  box-shadow:var(--shadow2);
  transition:0.25s ease-in-out;
}
.section:hover{
  background:#fbfdff;
  transform:translateY(-2px);
  box-shadow:var(--shadow);
}
.section h3{
  margin-top:0;
  color:#0b1f44;
  font-size:1.15rem;
  display:flex;
  align-items:center;
  gap:0.55rem;
}
.divider{ height:1px; background:rgba(26,115,232,0.12); margin:0.3rem 0 0.9rem 0; }

/* Grid */
.sch-grid{
  display:grid;
  grid-template-columns:1fr;
  gap:1rem;
  margin-top:0.9rem;
}
@media (min-width: 900px){
  .sch-grid{ grid-template-columns:repeat(2, 1fr); }
}

/* Scholar card */
.sch-card{
  background:#ffffff;
  border:1px solid rgba(26,115,232,0.16);
  border-radius:14px;
  padding:1.05rem 1.15rem;
  box-shadow:var(--shadow2);
  transition:0.2s ease-in-out;
  position:relative;
  overflow:hidden;
}
.sch-card:hover{
  transform:translateY(-2px);
  box-shadow:var(--shadow);
  background:#fbfdff;
}
.sch-card::before{
  content:"";
  position:absolute;
  left:0;
  top:0;
  height:100%;
  width:6px;
  border-top-left-radius:14px;
  border-bottom-left-radius:14px;
  background:rgba(26,115,232,0.65);
}

/* Variant accents */
.sch-card.lead::before{ background:rgba(220,20,60,0.80); }
.sch-card.current::before{ background:rgba(26,115,232,0.70); }
.sch-card.alumni::before{ background:rgba(26,127,61,0.70); }

/* Header row */
.sch-header{
  display:flex;
  gap:0.9rem;
  align-items:flex-start;
}
.sch-photo{
  width:64px;
  height:64px;
  border-radius:50%;
  object-fit:cover;
  background:#e9eefc;
  box-shadow:0 2px 8px rgba(0,0,0,0.08);
}
.sch-title{
  flex:1;
  min-width:0;
}
.sch-name{
  font-size:1.05rem;
  font-weight:900;
  margin:0;
  color:#0b1f44;
  line-height:1.25;
}
.sch-sub{
  margin-top:0.25rem;
  font-size:0.95rem;
  color:var(--muted);
}

/* Icons/logos */
.inline-icons{
  display:inline-flex;
  align-items:center;
  gap:0.4rem;
  margin-left:0.35rem;
}
.icon{
  width:18px; height:18px;
  vertical-align:middle;
}
.logo{
  width:34px; height:34px;
  object-fit:contain;
  vertical-align:middle;
}

/* Pills */
.pills{
  display:flex;
  flex-wrap:wrap;
  gap:0.45rem;
  margin-top:0.55rem;
}
.pill{
  display:inline-flex;
  align-items:center;
  gap:0.35rem;
  padding:0.28rem 0.6rem;
  border-radius:999px;
  border:1px solid rgba(26,115,232,0.20);
  background:#ffffff;
  box-shadow:var(--shadow2);
  font-size:0.84rem;
  font-weight:900;
  color:#0b1f44;
}
.pill.role-lead{ border-color:rgba(220,20,60,0.30); color:#7a0b1f; }
.pill.role-current{ border-color:rgba(26,115,232,0.25); color:#0a539e; }
.pill.role-alumni{ border-color:rgba(26,127,61,0.25); color:#1a7f3d; }
.pill.tag{ color:var(--blue); background:#f3f8ff; border-color:rgba(26,115,232,0.20); }

/* Sections inside card */
.sch-sec{
  margin-top:0.85rem;
  font-size:0.82rem;
  letter-spacing:0.04em;
  text-transform:uppercase;
  font-weight:900;
  color:#0b1f44;
  opacity:0.9;
}
.sch-list{
  margin:0.35rem 0 0 1.1rem;
  color:#202124;
}
.sch-list li{ margin:0.25rem 0; }

/* Scoped links */
.section a, .page-hero a{
  color:var(--blue);
  font-weight:800;
  text-decoration:none;
}
.section a:hover, .page-hero a:hover{ text-decoration:underline; }

/* Footer flags area */
.flags{
  text-align:center;
  margin-top:1.2rem;
}
</style>

<div class="page-hero">
  <h2>Scholars</h2>
  <p>
    This page highlights scholars who collaborate with me on research, publications, and project development, including current students and alumni.
  </p>
  <div class="hero-links">
    <a class="btn-link secondary" href="/insys-lab/">INSys Lab</a>
    <a class="btn-link" href="/publications/">Publications</a>
    <a class="btn-link secondary" href="/service/">Service</a>
  </div>
</div>

<div class="section">
  <h3>Research Lead</h3>
  <div class="divider"></div>

  <div class="sch-grid">
    <div class="sch-card lead">
      <div class="sch-header">
        <img src="/images/rahul.png" alt="Srinivas Rahul Sapireddy" class="sch-photo">
        <div class="sch-title">
          <div class="sch-name">
            Srinivas Rahul Sapireddy, Ph.D.
            <span class="inline-icons">
              <a href="https://www.linkedin.com/in/srsapireddy2020/" target="_blank" rel="noopener">
                <img src="/images/linkedin.png" alt="LinkedIn" class="icon">
              </a>
              <img src="/images/isu.png" alt="ISU Logo" class="logo">
            </span>
          </div>
          <div class="sch-sub">Assistant Professor, College of Engineering, Illinois State University</div>

          <div class="pills">
            <span class="pill role-lead">Guide</span>
            <span class="pill tag">Hardware-Aware AI</span>
            <span class="pill tag">RF Signal Classification</span>
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
    </div>
  </div>
</div>

<div class="section">
  <h3>Current Students</h3>
  <div class="divider"></div>

  <div class="sch-grid">

    <div class="sch-card current">
      <div class="sch-header">
        <img src="/images/place.jpg" alt="Abreham Mesfin" class="sch-photo">
        <div class="sch-title">
          <div class="sch-name">
            Abreham Mesfin
            <span class="inline-icons">
              <a href="https://www.linkedin.com/in/abreham-mesfin-820084301?original_referer=https%3A%2F%2Fwww.google.com%2F" target="_blank" rel="noopener">
                <img src="/images/linkedin.png" alt="LinkedIn" class="icon">
              </a>
              <img src="/images/UMKC.png" alt="UMKC Logo" class="logo">
            </span>
          </div>
          <div class="sch-sub">UMKC — B.S. Electrical and Computer Engineering (Expected 2028)</div>

          <div class="pills">
            <span class="pill role-current">Current</span>
            <span class="pill tag">Logic Design</span>
            <span class="pill tag">Engineering Computation</span>
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
    </div>

  </div>
</div>

<div class="section">
  <h3>Alumni</h3>
  <div class="divider"></div>

  <div class="sch-grid">

    

  </div>
</div>

<div class="flags">
  <a href="https://info.flagcounter.com/UCHm" target="_blank" rel="noopener">
    <img src="https://s01.flagcounter.com/map/UCHm/size_l/txt_121AFF/border_CCCCCC/pageviews_1/viewers_0/flags_0/" alt="Flag Counter" border="0">
  </a>
</div>

<div class="flags">
  <a href="https://info.flagcounter.com/3uG8" target="_blank" rel="noopener">
    <img src="https://s05.flagcounter.com/countxl_US/3uG8/bg_FFFFFF/txt_1239FF/border_C9CCC8/columns_8/maxflags_40/viewers_0/labels_1/pageviews_1/flags_0/percent_0/" alt="Flag Counter" border="0">
  </a>
</div>
