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
  --green:#1a7f3d;
  --bg:#ffffff;
  --soft:#f6f9ff;
  --muted:#5f6368;
  --text:#0b1f44;
  --shadow:0 10px 30px rgba(0,0,0,0.08);
  --shadow2:0 2px 10px rgba(0,0,0,0.05);
  --radius:18px;
  --radius2:14px;
  --border:rgba(26,115,232,0.18);
}

@keyframes fadeInUp{
  from{ opacity:0; transform:translateY(14px); }
  to{ opacity:1; transform:translateY(0); }
}

@keyframes slideTrack{
  from{ transform:translateX(0); }
  to{ transform:translateX(-50%); }
}

.scholars-wrap{
  animation:fadeInUp 0.8s ease-in-out;
}

/* Hero */
.page-hero{
  position:relative;
  overflow:hidden;
  border-radius:var(--radius);
  padding:2.2rem 2rem;
  margin-bottom:1.3rem;
  background:
    radial-gradient(circle at top right, rgba(220,20,60,0.13), transparent 32%),
    linear-gradient(135deg,#e9f3ff 0%, #ffffff 62%);
  border:1px solid rgba(26,115,232,0.25);
  box-shadow:var(--shadow);
}

.page-hero::before{
  content:"";
  position:absolute;
  inset:0;
  background-image:
    linear-gradient(rgba(26,115,232,0.06) 1px, transparent 1px),
    linear-gradient(90deg, rgba(26,115,232,0.06) 1px, transparent 1px);
  background-size:34px 34px;
  pointer-events:none;
}

.hero-content{
  position:relative;
  z-index:1;
}

.hero-kicker{
  display:inline-block;
  padding:0.35rem 0.75rem;
  border-radius:999px;
  background:#ffffff;
  border:1px solid rgba(220,20,60,0.25);
  color:var(--isu);
  font-weight:900;
  font-size:0.88rem;
  box-shadow:var(--shadow2);
  margin-bottom:0.85rem;
}

.page-hero h1{
  margin:0;
  font-size:2.15rem;
  line-height:1.15;
  color:var(--text);
}

.page-hero p{
  margin:0.75rem 0 0 0;
  color:var(--muted);
  font-size:1.04rem;
  line-height:1.65;
  max-width:92ch;
}

/* Buttons */
.hero-links{
  display:flex;
  flex-wrap:wrap;
  gap:0.7rem;
  margin-top:1.15rem;
}

.btn-link{
  display:inline-flex;
  align-items:center;
  gap:0.45rem;
  padding:0.58rem 0.92rem;
  border-radius:12px;
  background:var(--blue);
  color:#ffffff !important;
  text-decoration:none !important;
  font-weight:850;
  box-shadow:var(--shadow2);
  transition:0.2s ease-in-out;
}

.btn-link:hover{
  background:var(--blue2);
  transform:translateY(-2px);
  text-decoration:none !important;
}

.btn-link.secondary{
  background:#ffffff;
  color:var(--blue) !important;
  border:1px solid rgba(26,115,232,0.25);
}

/* Sliding bar */
.sliding-bar{
  overflow:hidden;
  border-radius:16px;
  border:1px solid rgba(26,115,232,0.18);
  background:#ffffff;
  box-shadow:var(--shadow2);
  margin-bottom:1.3rem;
}

.slide-track{
  display:flex;
  width:max-content;
  animation:slideTrack 32s linear infinite;
}

.sliding-bar:hover .slide-track{
  animation-play-state:paused;
}

.slide-item{
  display:inline-flex;
  align-items:center;
  gap:0.4rem;
  padding:0.75rem 1.2rem;
  color:var(--text);
  font-weight:900;
  white-space:nowrap;
  border-right:1px solid rgba(26,115,232,0.10);
}

.slide-item span{
  color:var(--isu);
}

/* Impact cards */
.impact-grid{
  display:grid;
  grid-template-columns:repeat(4,1fr);
  gap:1rem;
  margin-bottom:1.3rem;
}

.impact-card{
  padding:1.1rem 1rem;
  border-radius:16px;
  background:linear-gradient(135deg,#ffffff 0%,#f7fbff 100%);
  border:1px solid rgba(26,115,232,0.18);
  box-shadow:var(--shadow2);
  text-align:center;
  transition:0.25s ease-in-out;
}

.impact-card:hover{
  transform:translateY(-3px);
  box-shadow:var(--shadow);
}

.impact-number{
  font-size:1.65rem;
  font-weight:950;
  color:var(--isu);
  line-height:1.1;
}

.impact-label{
  margin-top:0.35rem;
  font-size:0.92rem;
  color:var(--text);
  font-weight:850;
}

.impact-sub{
  margin-top:0.2rem;
  font-size:0.82rem;
  color:var(--muted);
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

.section h2,
.section h3{
  margin:0;
  color:var(--text);
  font-size:1.22rem;
  display:flex;
  align-items:center;
  gap:0.55rem;
}

.section p{
  color:#202124;
  line-height:1.65;
}

.divider{
  height:1px;
  background:rgba(26,115,232,0.12);
  margin:0.6rem 0 1rem 0;
}

/* Research focus cards */
.focus-grid{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:1.1rem;
  margin-bottom:1.3rem;
}

.focus-card{
  position:relative;
  overflow:hidden;
  padding:1.25rem;
  border-radius:16px;
  background:linear-gradient(135deg,#ffffff 0%,#f4f9ff 100%);
  border:1px solid var(--border);
  box-shadow:var(--shadow2);
  transition:0.25s ease-in-out;
}

.focus-card:hover{
  transform:translateY(-4px);
  box-shadow:var(--shadow);
}

.focus-card::before{
  content:"";
  position:absolute;
  top:0;
  left:0;
  height:5px;
  width:100%;
  background:linear-gradient(90deg,var(--blue),var(--isu));
}

.focus-icon{
  width:46px;
  height:46px;
  border-radius:14px;
  background:#e9f3ff;
  color:var(--blue);
  display:flex;
  align-items:center;
  justify-content:center;
  font-size:1.45rem;
  margin-bottom:0.85rem;
  box-shadow:0 4px 12px rgba(26,115,232,0.16);
}

.focus-card h3{
  margin:0 0 0.55rem 0;
  font-size:1.12rem;
  color:var(--text);
}

.focus-card p{
  margin:0;
  color:#202124;
  line-height:1.55;
  font-size:0.95rem;
}

/* Tabs */
.sch-tabs{
  display:flex;
  flex-wrap:wrap;
  gap:0.7rem;
  margin-bottom:1.1rem;
}

.tab-button{
  border:1px solid rgba(26,115,232,0.22);
  background:#ffffff;
  color:var(--blue);
  padding:0.62rem 1rem;
  border-radius:999px;
  cursor:pointer;
  font-weight:900;
  box-shadow:var(--shadow2);
  transition:0.2s ease-in-out;
}

.tab-button:hover{
  transform:translateY(-2px);
  background:#f3f8ff;
}

.tab-button.active{
  background:var(--blue);
  color:#ffffff;
  border-color:var(--blue);
}

.tab-panel{
  display:none;
  animation:fadeInUp 0.45s ease-in-out;
}

.tab-panel.active{
  display:block;
}

/* Scholar grid */
.sch-grid{
  display:grid;
  grid-template-columns:1fr;
  gap:1rem;
  margin-top:0.9rem;
}

@media (min-width:900px){
  .sch-grid{
    grid-template-columns:repeat(2,1fr);
  }
}

/* Scholar cards */
.sch-card{
  background:#ffffff;
  border:1px solid rgba(26,115,232,0.16);
  border-radius:16px;
  padding:1.1rem 1.15rem;
  box-shadow:var(--shadow2);
  transition:0.22s ease-in-out;
  position:relative;
  overflow:hidden;
}

.sch-card:hover{
  transform:translateY(-3px);
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
  border-top-left-radius:16px;
  border-bottom-left-radius:16px;
  background:rgba(26,115,232,0.65);
}

.sch-card.lead::before{
  background:rgba(220,20,60,0.85);
}

.sch-card.current::before{
  background:rgba(26,115,232,0.75);
}

.sch-card.alumni::before{
  background:rgba(26,127,61,0.75);
}

.sch-header{
  display:flex;
  gap:0.95rem;
  align-items:flex-start;
}

.sch-photo{
  width:70px;
  height:70px;
  border-radius:50%;
  object-fit:cover;
  background:#e9eefc;
  box-shadow:0 3px 10px rgba(0,0,0,0.10);
  border:3px solid #ffffff;
}

.sch-title{
  flex:1;
  min-width:0;
}

.sch-name{
  font-size:1.07rem;
  font-weight:950;
  margin:0;
  color:var(--text);
  line-height:1.25;
}

.sch-sub{
  margin-top:0.28rem;
  font-size:0.95rem;
  color:var(--muted);
  line-height:1.45;
}

/* Icons/logos */
.inline-icons{
  display:inline-flex;
  align-items:center;
  gap:0.4rem;
  margin-left:0.35rem;
}

.icon{
  width:18px;
  height:18px;
  vertical-align:middle;
}

.logo{
  width:34px;
  height:34px;
  object-fit:contain;
  vertical-align:middle;
}

/* Pills */
.pills{
  display:flex;
  flex-wrap:wrap;
  gap:0.45rem;
  margin-top:0.65rem;
}

.pill{
  display:inline-flex;
  align-items:center;
  gap:0.35rem;
  padding:0.3rem 0.62rem;
  border-radius:999px;
  border:1px solid rgba(26,115,232,0.20);
  background:#ffffff;
  box-shadow:var(--shadow2);
  font-size:0.84rem;
  font-weight:900;
  color:var(--text);
}

.pill.role-lead{
  border-color:rgba(220,20,60,0.30);
  color:#7a0b1f;
  background:rgba(220,20,60,0.06);
}

.pill.role-current{
  border-color:rgba(26,115,232,0.25);
  color:#0a539e;
  background:#f3f8ff;
}

.pill.role-alumni{
  border-color:rgba(26,127,61,0.25);
  color:var(--green);
  background:rgba(26,127,61,0.06);
}

.pill.tag{
  color:var(--blue);
  background:#f3f8ff;
  border-color:rgba(26,115,232,0.20);
}

/* Inside scholar card */
.sch-sec{
  margin-top:0.9rem;
  font-size:0.82rem;
  letter-spacing:0.04em;
  text-transform:uppercase;
  font-weight:950;
  color:var(--text);
  opacity:0.9;
}

.sch-list{
  margin:0.35rem 0 0 1.1rem;
  color:#202124;
  line-height:1.5;
}

.sch-list li{
  margin:0.28rem 0;
}

/* Mentoring cards */
.pathway-grid{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:1rem;
}

.pathway-card{
  padding:1rem;
  border-radius:14px;
  background:linear-gradient(135deg,#ffffff 0%,#f7fbff 100%);
  border:1px solid rgba(26,115,232,0.18);
  box-shadow:var(--shadow2);
  transition:0.22s ease-in-out;
}

.pathway-card:hover{
  transform:translateY(-3px);
  box-shadow:var(--shadow);
}

.pathway-card h3{
  margin:0 0 0.45rem 0;
  font-size:1rem;
}

.pathway-card p{
  margin:0;
  font-size:0.92rem;
}

/* Scoped links */
.section a,
.page-hero a{
  color:var(--blue);
  font-weight:850;
  text-decoration:none;
}

.section a:hover,
.page-hero a:hover{
  text-decoration:underline;
}

/* Footer flags */
.flags{
  text-align:center;
  margin-top:1.2rem;
}

/* Responsive */
@media (max-width:950px){
  .impact-grid,
  .focus-grid,
  .pathway-grid{
    grid-template-columns:1fr 1fr;
  }
}

@media (max-width:700px){
  .page-hero{
    padding:1.5rem 1.1rem;
  }

  .page-hero h1{
    font-size:1.65rem;
  }

  .impact-grid,
  .focus-grid,
  .pathway-grid{
    grid-template-columns:1fr;
  }

  .sch-header{
    flex-direction:column;
  }
}
</style>

<div class="scholars-wrap">

  <div class="page-hero">
    <div class="hero-content">
      <span class="hero-kicker">INSys Lab · Student Research · Mentoring</span>

      <h1>Scholars</h1>

      <p>
        This page highlights scholars who collaborate with me on research, publications, and project development.
        The group includes current students, alumni, and collaborators working across RF signal processing,
        hardware-aware AI, digital systems, and efficient computing.
      </p>

      <div class="hero-links">
        <a class="btn-link secondary" href="/insys-lab/">INSys Lab</a>
        <a class="btn-link" href="/publications/">Publications</a>
        <a class="btn-link secondary" href="/service/">Service</a>
        <a class="btn-link secondary" href="mailto:ssapire@illinoisstate.edu">Contact</a>
      </div>
    </div>
  </div>

  <div class="sliding-bar">
    <div class="slide-track">
      <div class="slide-item"><span>●</span> Student Research Mentoring</div>
      <div class="slide-item"><span>●</span> RF Signal Classification</div>
      <div class="slide-item"><span>●</span> Hardware-Aware AI</div>
      <div class="slide-item"><span>●</span> Digital Circuit Optimization</div>
      <div class="slide-item"><span>●</span> Edge Intelligence</div>
      <div class="slide-item"><span>●</span> Publication-Oriented Projects</div>

      <div class="slide-item"><span>●</span> Student Research Mentoring</div>
      <div class="slide-item"><span>●</span> RF Signal Classification</div>
      <div class="slide-item"><span>●</span> Hardware-Aware AI</div>
      <div class="slide-item"><span>●</span> Digital Circuit Optimization</div>
      <div class="slide-item"><span>●</span> Edge Intelligence</div>
      <div class="slide-item"><span>●</span> Publication-Oriented Projects</div>
    </div>
  </div>

  <div class="impact-grid">
    <div class="impact-card">
      <div class="impact-number">Lead</div>
      <div class="impact-label">Research Guidance</div>
      <div class="impact-sub">INSys Lab research direction</div>
    </div>

    <div class="impact-card">
      <div class="impact-number">Current</div>
      <div class="impact-label">Student Projects</div>
      <div class="impact-sub">Active mentoring and development</div>
    </div>

    <div class="impact-card">
      <div class="impact-number">Alumni</div>
      <div class="impact-label">Past Scholars</div>
      <div class="impact-sub">Research and publication outcomes</div>
    </div>

    <div class="impact-card">
      <div class="impact-number">Pubs</div>
      <div class="impact-label">Research Output</div>
      <div class="impact-sub">Manuscripts, submissions, and papers</div>
    </div>
  </div>

  <div class="focus-grid">
    <div class="focus-card">
      <div class="focus-icon">📡</div>
      <h3>RF and Signal Intelligence</h3>
      <p>
        Student projects include modulation recognition, signal-domain feature extraction,
        envelope statistics, and lightweight RF classification.
      </p>
    </div>

    <div class="focus-card">
      <div class="focus-icon">🧠</div>
      <h3>Hardware-Aware AI</h3>
      <p>
        Research mentoring emphasizes efficient machine learning, model simplification,
        low-power inference, and deployment-aware evaluation.
      </p>
    </div>

    <div class="focus-card">
      <div class="focus-icon">⚙️</div>
      <h3>Digital Systems</h3>
      <p>
        Student work includes logic design, Boolean minimization, circuit optimization,
        and hardware-oriented computing foundations.
      </p>
    </div>
  </div>

  <div class="section">
    <h2>👥 Scholars Directory</h2>
    <div class="divider"></div>

    <div class="sch-tabs">
      <button class="tab-button active" onclick="openScholarTab(event, 'lead-tab')">Research Lead</button>
      <button class="tab-button" onclick="openScholarTab(event, 'current-tab')">Current Students</button>
      <button class="tab-button" onclick="openScholarTab(event, 'alumni-tab')">Alumni</button>
    </div>

    <div id="lead-tab" class="tab-panel active">
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

              <div class="sch-sub">
                Assistant Professor, College of Engineering, Illinois State University
              </div>

              <div class="pills">
                <span class="pill role-lead">Research Lead</span>
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

    <div id="current-tab" class="tab-panel">
  <div class="sch-grid">

    <div class="sch-card current">
      <div class="sch-header">
        <img src="/images/place.jpg" alt="Sai Anirudh Godavarthi" class="sch-photo">

        <div class="sch-title">
          <div class="sch-name">
            Sai Anirudh Godavarthi
            <span class="inline-icons">
              <img src="/images/UMKC.png" alt="UMKC Logo" class="logo">
            </span>
          </div>

          <div class="sch-sub">
            UMKC — M.S. Computer Science (Present)
          </div>

          <div class="pills">
            <span class="pill role-current">Current</span>
            <span class="pill tag">RF Communications</span>
            <span class="pill tag">Antenna Design</span>
          </div>

          <div class="sch-sec">Research interests</div>
          <ul class="sch-list">
            <li>RF communications</li>
            <li>Antenna design and simulation</li>
          </ul>

          <div class="sch-sec">Active topics / papers</div>
          <ul class="sch-list">
            <li>RF communication and antenna design project in progress</li>
          </ul>
        </div>
      </div>
    </div>

  </div>
</div>

<div id="alumni-tab" class="tab-panel">
  <div class="sch-grid">

    <div class="sch-card alumni">
      <div class="sch-header">
        <img src="/images/hemanth.png" alt="Hemanth Bandi" class="sch-photo">

        <div class="sch-title">
          <div class="sch-name">
            Hemanth Bandi
            <span class="inline-icons">
              <a href="https://www.linkedin.com/in/hemanth-bandi-095266859317574524/" target="_blank" rel="noopener">
                <img src="/images/linkedin.png" alt="LinkedIn" class="icon">
              </a>
              <img src="/images/UMKC.png" alt="UMKC Logo" class="logo">
            </span>
          </div>

          <div class="sch-sub">
            UMKC — M.S. Computer Science (Spring 2023)
          </div>

          <div class="pills">
            <span class="pill role-alumni">Alumni</span>
            <span class="pill tag">RF</span>
            <span class="pill tag">Deep Learning</span>
            <span class="pill tag">Reinforcement Learning</span>
          </div>

          <div class="sch-sec">Research interests</div>
          <ul class="sch-list">
            <li>RF modulation recognition</li>
            <li>Reinforcement learning</li>
          </ul>

          <div class="sch-sec">Active topics / papers</div>
          <ul class="sch-list">
            <li>Reinforcement Learning manuscript (Springer, To be submitted)</li>
            <li>Benchmarking R-aware binning with envelope-feature baselines (IEEE, submitted)</li>
          </ul>
        </div>
      </div>
    </div>

    <div class="sch-card alumni">
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

          <div class="sch-sub">
            UMKC — B.S. Electrical and Computer Engineering
          </div>

          <div class="pills">
            <span class="pill role-alumni">Alumni</span>
            <span class="pill tag">Logic Design</span>
            <span class="pill tag">Engineering Computation</span>
          </div>

          <div class="sch-sec">Research interests</div>
          <ul class="sch-list">
            <li>Minimization techniques for Boolean functions</li>
            <li>Low-power circuit implementations</li>
          </ul>

          <div class="sch-sec">Research topics / papers</div>
          <ul class="sch-list">
            <li>Digital Circuit Optimization Techniques</li>
          </ul>
        </div>
      </div>
    </div>

  </div>
</div>

  <div class="section">
    <h2>🧭 Mentoring Pathways</h2>
    <div class="divider"></div>

    <div class="pathway-grid">
      <div class="pathway-card">
        <h3>Research Foundations</h3>
        <p>
          Students begin with literature review, technical reading, experimental setup,
          and reproducible research workflows.
        </p>
      </div>

      <div class="pathway-card">
        <h3>Project Development</h3>
        <p>
          Students contribute to simulation, feature extraction, model evaluation,
          circuit optimization, or signal-processing pipelines.
        </p>
      </div>

      <div class="pathway-card">
        <h3>Publication Preparation</h3>
        <p>
          Advanced students work toward manuscript development, result analysis,
          presentation preparation, and conference/journal submissions.
        </p>
      </div>
    </div>
  </div>

  <div class="section">
    <h2>🤝 Interested in Joining?</h2>
    <div class="divider"></div>

    <p>
      Students interested in RF signal processing, hardware-aware AI, digital systems,
      low-power computing, or research-oriented engineering projects are welcome to reach out.
      Please include your research interests, relevant coursework, technical skills, and any prior project experience.
    </p>

    <div class="hero-links">
      <a class="btn-link" href="mailto:ssapire@illinoisstate.edu">Email</a>
      <a class="btn-link secondary" href="/insys-lab/">INSys Lab</a>
      <a class="btn-link secondary" href="/publications/">Publications</a>
    </div>
  </div>

  <div class="flags">
    <a href="https://info.flagcounter.com/UCHm" target="_blank" rel="noopener">
      <img src="https://s01.flagcounter.com/map/UCHm/size_l/txt_121AFF/border_CCCCCC/pageviews_1/viewers_0/flags_0/" alt="Flag Counter" border="0">
    </a>
  </div>

  <div class="section" style="margin-top: 20px; text-align: center;">
    <a href="https://info.flagcounter.com/ghXp">
      <img 
        src="https://s01.flagcounter.com/map/ghXp/size_m/txt_000000/border_CCCCCC/pageviews_1/viewers_0/flags_0/" 
        alt="Flag Counter"
        style="border: 0; max-width: 100%; height: auto;">
    </a>
  </div>

</div>

<script>
function openScholarTab(event, panelId) {
  const panels = document.querySelectorAll(".tab-panel");
  const buttons = document.querySelectorAll(".tab-button");

  panels.forEach(function(panel) {
    panel.classList.remove("active");
  });

  buttons.forEach(function(button) {
    button.classList.remove("active");
  });

  const selectedPanel = document.getElementById(panelId);
  if (selectedPanel) {
    selectedPanel.classList.add("active");
  }

  if (event && event.currentTarget) {
    event.currentTarget.classList.add("active");
  }
}
</script>
