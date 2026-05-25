---
title: "Publications"
layout: single
permalink: /publications/
author_profile: true
---

<style>
:root{
  --blue:#1a73e8;
  --blue2:#0b5bd3;
  --isu:#DC143C;
  --bg:#ffffff;
  --soft:#f6f9ff;
  --muted:#5f6368;
  --text:#0b1f44;
  --border:rgba(26,115,232,0.18);
  --shadow:0 10px 30px rgba(0,0,0,0.08);
  --shadow2:0 2px 10px rgba(0,0,0,0.05);
  --radius:18px;
  --radius2:14px;
}

@keyframes fadeInUp{
  from{opacity:0; transform:translateY(14px);}
  to{opacity:1; transform:translateY(0);}
}

@keyframes slideTrack{
  from{transform:translateX(0);}
  to{transform:translateX(-50%);}
}

.pub-wrap{
  animation:fadeInUp 0.8s ease-in-out;
}

/* Hero */
.pub-hero{
  position:relative;
  overflow:hidden;
  border-radius:var(--radius);
  padding:2.25rem 2rem;
  margin-bottom:1.25rem;
  background:
    radial-gradient(circle at top right, rgba(220,20,60,0.13), transparent 32%),
    linear-gradient(135deg,#e9f3ff 0%, #ffffff 62%);
  border:1px solid rgba(26,115,232,0.25);
  box-shadow:var(--shadow);
}

.pub-hero::before{
  content:"";
  position:absolute;
  inset:0;
  background-image:
    linear-gradient(rgba(26,115,232,0.06) 1px, transparent 1px),
    linear-gradient(90deg, rgba(26,115,232,0.06) 1px, transparent 1px);
  background-size:34px 34px;
  pointer-events:none;
}

.pub-hero-content{
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

.pub-hero h1{
  margin:0;
  font-size:2.15rem;
  line-height:1.15;
  color:var(--text);
}

.pub-hero .subtitle{
  margin-top:0.55rem;
  color:#202124;
  font-size:1.08rem;
  font-weight:650;
}

.pub-hero p{
  margin:0.8rem 0 0 0;
  color:var(--muted);
  font-size:1.03rem;
  line-height:1.65;
  max-width:90ch;
}

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
  animation:slideTrack 34s linear infinite;
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
  gap:0.9rem;
  margin-bottom:1.3rem;
}

.impact-card{
  text-align:center;
  padding:1.05rem 0.9rem;
  border-radius:var(--radius2);
  background:linear-gradient(135deg,#ffffff 0%,#f7fbff 100%);
  border:1px solid var(--border);
  box-shadow:var(--shadow2);
  transition:0.22s ease-in-out;
}

.impact-card:hover{
  transform:translateY(-3px);
  box-shadow:var(--shadow);
}

.impact-card .big{
  color:var(--isu);
  font-size:1.55rem;
  font-weight:950;
  line-height:1.1;
}

.impact-card .label{
  color:var(--text);
  font-weight:850;
  margin-top:0.35rem;
  font-size:0.92rem;
}

.impact-card .small{
  color:var(--muted);
  font-size:0.8rem;
  margin-top:0.2rem;
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
.grid-3{
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

/* Tags */
.tag-cloud{
  display:flex;
  flex-wrap:wrap;
  gap:0.55rem;
}

.tag{
  display:inline-flex;
  padding:0.36rem 0.72rem;
  border-radius:999px;
  background:#f3f8ff;
  border:1px solid rgba(26,115,232,0.18);
  color:var(--text);
  font-size:0.88rem;
  font-weight:850;
}

/* Filter tabs */
.pub-tabs{
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

/* Year blocks */
.year-section{
  margin-top:1rem;
  padding-top:0.3rem;
}

.year-header{
  display:flex;
  justify-content:space-between;
  align-items:center;
  gap:1rem;
  margin:1.2rem 0 0.9rem 0;
  padding:0.9rem 1rem;
  border-radius:14px;
  background:linear-gradient(135deg,#f7fbff 0%,#ffffff 100%);
  border:1px solid rgba(26,115,232,0.18);
}

.year-title{
  display:inline-flex;
  align-items:center;
  gap:0.55rem;
  font-size:1.22rem;
  font-weight:950;
  color:var(--text);
}

.year-pill{
  display:inline-flex;
  padding:0.3rem 0.75rem;
  border-radius:999px;
  background:rgba(220,20,60,0.08);
  border:1px solid rgba(220,20,60,0.22);
  color:var(--isu);
  font-weight:900;
  font-size:0.85rem;
}

/* Publication cards */
.publication-card{
  position:relative;
  padding:1.15rem 1.15rem 1.15rem 1.35rem;
  border-radius:16px;
  background:#ffffff;
  border:1px solid var(--border);
  box-shadow:var(--shadow2);
  margin-bottom:1rem;
  transition:0.22s ease-in-out;
}

.publication-card:hover{
  transform:translateY(-3px);
  box-shadow:var(--shadow);
  background:#fbfdff;
}

.publication-card::before{
  content:"";
  position:absolute;
  left:0;
  top:1rem;
  bottom:1rem;
  width:4px;
  border-radius:99px;
  background:linear-gradient(180deg,var(--blue),var(--isu));
}

.publication-card.placeholder{
  background:linear-gradient(135deg,#ffffff 0%,#fffaf2 100%);
  border-color:rgba(122,90,0,0.20);
}

.publication-card.placeholder::before{
  background:#b7791f;
}

.pub-top{
  display:flex;
  flex-wrap:wrap;
  gap:0.55rem;
  align-items:center;
  margin-bottom:0.65rem;
}

.pub-year,
.pub-type,
.pub-award,
.pub-status{
  display:inline-flex;
  padding:0.25rem 0.58rem;
  border-radius:999px;
  font-size:0.78rem;
  font-weight:900;
}

.pub-year{
  background:#f3f8ff;
  border:1px solid rgba(26,115,232,0.18);
  color:var(--blue);
}

.pub-type{
  background:#ffffff;
  border:1px solid rgba(26,115,232,0.20);
  color:var(--text);
}

.pub-award{
  background:rgba(220,20,60,0.08);
  border:1px solid rgba(220,20,60,0.25);
  color:var(--isu);
}

.pub-status{
  background:#fff6e6;
  border:1px solid rgba(122,90,0,0.25);
  color:#7a5a00;
}

.pub-title{
  color:var(--text);
  font-size:1.05rem;
  font-weight:950;
  line-height:1.45;
  margin-bottom:0.45rem;
}

.pub-authors{
  color:#202124;
  font-size:0.94rem;
  line-height:1.5;
  margin-bottom:0.35rem;
}

.pub-venue{
  color:var(--muted);
  font-size:0.92rem;
  line-height:1.45;
}

.pub-note{
  margin-top:0.55rem;
  color:#475569;
  font-size:0.9rem;
  line-height:1.55;
}

/* Buttons */
.pub-links{
  display:flex;
  flex-direction:row;
  flex-wrap:wrap;
  gap:0.55rem;
  margin-top:0.85rem;
  align-items:center;
}

.pub-link,
.pub-button{
  display:inline-flex;
  align-items:center;
  justify-content:center;
  padding:0.36rem 0.72rem;
  border-radius:999px;
  background:#f3f8ff;
  border:1px solid rgba(26,115,232,0.18);
  color:var(--blue) !important;
  text-decoration:none !important;
  font-size:0.84rem;
  font-weight:850;
  cursor:pointer;
  line-height:1.2;
  white-space:nowrap;
}

.pub-link:hover,
.pub-button:hover{
  background:#e9f3ff;
  text-decoration:none !important;
}

.pub-button.primary{
  background:var(--blue);
  color:#ffffff !important;
  border-color:var(--blue);
}

.pub-button.primary:hover{
  background:var(--blue2);
}

.pub-link.disabled{
  opacity:0.55;
  cursor:not-allowed;
}

.citation-box{
  display:none;
  margin-top:0.8rem;
  padding:0.9rem;
  border-radius:12px;
  background:#f7fbff;
  border:1px solid rgba(26,115,232,0.18);
  color:#202124;
  font-size:0.88rem;
  line-height:1.55;
  white-space:pre-wrap;
  overflow-x:auto;
}

/* Timeline/profile grid */
.grid-2{
  display:grid;
  grid-template-columns:1fr;
  gap:1.2rem;
}

.timeline{
  position:relative;
  margin-top:0.3rem;
  padding-left:1.3rem;
}

.timeline::before{
  content:"";
  position:absolute;
  left:0.25rem;
  top:0.2rem;
  bottom:0.2rem;
  width:2px;
  background:linear-gradient(180deg,var(--blue),var(--isu));
}

.timeline-item{
  position:relative;
  margin-bottom:1rem;
  padding-left:1rem;
}

.timeline-item::before{
  content:"";
  position:absolute;
  left:-1.29rem;
  top:0.25rem;
  width:11px;
  height:11px;
  border-radius:50%;
  background:var(--isu);
  border:3px solid #ffffff;
  box-shadow:0 0 0 2px rgba(220,20,60,0.22);
}

.timeline-year{
  color:var(--isu);
  font-weight:900;
  font-size:0.88rem;
}

.timeline-title{
  color:var(--text);
  font-weight:900;
  margin-top:0.1rem;
}

.timeline-text{
  color:#202124;
  margin-top:0.15rem;
  line-height:1.5;
}

/* Filtering */
.publication-card.hide-card,
.year-section.hide-year{
  display:none;
}

/* Responsive */
@media (min-width:900px){
  .grid-2{
    grid-template-columns:1fr 1fr;
  }
}

@media (max-width:950px){
  .grid-3,
  .impact-grid{
    grid-template-columns:1fr 1fr;
  }
}

@media (max-width:600px){
  .pub-hero{
    padding:1.5rem 1.1rem;
  }

  .pub-hero h1{
    font-size:1.65rem;
  }

  .grid-3,
  .impact-grid{
    grid-template-columns:1fr;
  }

  .year-header{
    align-items:flex-start;
    flex-direction:column;
  }
}

/* Scoped links */
.section a,
.pub-hero a{
  color:var(--blue);
  font-weight:800;
  text-decoration:none;
}

.section a:hover,
.pub-hero a:hover{
  text-decoration:underline;
}
</style>

<div class="pub-wrap">

  <div class="pub-hero">
    <div class="pub-hero-content">
      <span class="hero-kicker">Research Publications · RF · AI · VLSI · Edge Systems</span>

      <h1>Publications</h1>

      <div class="subtitle">
        Selected publications and research outputs organized year by year
      </div>

      <p>
        This page presents selected journal articles, conference papers, accepted manuscripts,
        awarded research contributions, and earlier research outputs across RF signal intelligence,
        hardware-aware AI, VLSI systems, edge computing, and secure intelligent systems.
      </p>

      <div class="hero-links">
        <a class="btn-link" href="https://scholar.google.com/citations?user=08fgpdIAAAAJ" target="_blank" rel="noopener">Google Scholar</a>
        <a class="btn-link secondary" href="https://orcid.org/0000-0002-9898-6810" target="_blank" rel="noopener">ORCID</a>
        <a class="btn-link secondary" href="https://openreview.net/profile?id=~Srinivas_Rahul_Sapireddy1" target="_blank" rel="noopener">OpenReview</a>
        <a class="btn-link secondary" href="/resume/">Resume</a>
      </div>
    </div>
  </div>

  <div class="sliding-bar">
    <div class="slide-track">
      <div class="slide-item"><span>●</span> RF Modulation Classification</div>
      <div class="slide-item"><span>●</span> Hardware-Aware AI</div>
      <div class="slide-item"><span>●</span> Custom Activation Functions</div>
      <div class="slide-item"><span>●</span> GPS Spoofing Detection</div>
      <div class="slide-item"><span>●</span> IoT Security</div>
      <div class="slide-item"><span>●</span> RF Fingerprinting</div>
      <div class="slide-item"><span>●</span> VLSI and Edge Systems</div>

      <div class="slide-item"><span>●</span> RF Modulation Classification</div>
      <div class="slide-item"><span>●</span> Hardware-Aware AI</div>
      <div class="slide-item"><span>●</span> Custom Activation Functions</div>
      <div class="slide-item"><span>●</span> GPS Spoofing Detection</div>
      <div class="slide-item"><span>●</span> IoT Security</div>
      <div class="slide-item"><span>●</span> RF Fingerprinting</div>
      <div class="slide-item"><span>●</span> VLSI and Edge Systems</div>
    </div>
  </div>

  <div class="impact-grid">
    <div class="impact-card">
      <div class="big">2026</div>
      <div class="label">Published Work</div>
      <div class="small">IEEE SoutheastCon</div>
    </div>

    <div class="impact-card">
      <div class="big">2025</div>
      <div class="label">Major Output Year</div>
      <div class="small">RF, AI, Security, VLSI</div>
    </div>

    <div class="impact-card">
      <div class="big">2024</div>
      <div class="label">Journal Publications</div>
      <div class="small">Activations and circuits</div>
    </div>

    <div class="impact-card">
      <div class="big">Earlier</div>
      <div class="label">Prior Research Outputs</div>
      <div class="small">2018 and 2016 entries</div>
    </div>
  </div>

  <div class="grid-3">
    <div class="focus-card">
      <div class="focus-icon">📡</div>
      <h3>RF Signal Intelligence</h3>
      <p>
        Publications on modulation classification, envelope statistics, GPS spoofing detection,
        RF fingerprinting, and signal-processing methods.
      </p>
    </div>

    <div class="focus-card">
      <div class="focus-icon">🧠</div>
      <h3>Hardware-Aware AI</h3>
      <p>
        Research on lightweight neural networks, custom activation functions, model efficiency,
        and deployment-aware learning.
      </p>
    </div>

    <div class="focus-card">
      <div class="focus-icon">⚙️</div>
      <h3>VLSI and Edge Systems</h3>
      <p>
        Work related to hardware acceleration, physical design, VLSI-oriented systems,
        and efficient embedded intelligence.
      </p>
    </div>
  </div>

  <div class="section">
    <h2>🧭 Research Themes</h2>
    <div class="divider"></div>

    <div class="tag-cloud">
      <span class="tag">RF Modulation Classification</span>
      <span class="tag">Envelope Statistics</span>
      <span class="tag">R-Value Features</span>
      <span class="tag">CAF-Based Feature Extraction</span>
      <span class="tag">STFT-Based Analysis</span>
      <span class="tag">GPS Spoofing Detection</span>
      <span class="tag">Hardware-Aware AI</span>
      <span class="tag">Custom Activation Functions</span>
      <span class="tag">LSTM Optimization</span>
      <span class="tag">Edge AI</span>
      <span class="tag">VLSI Design</span>
      <span class="tag">IoT Security</span>
      <span class="tag">RF Fingerprinting</span>
      <span class="tag">Polymorphic Circuits</span>
    </div>
  </div>

  <div class="section">
    <h2>📚 Publications by Year</h2>
    <div class="divider"></div>

    <p>
      The list below is grouped by year while remaining on one continuous page. Use the filters for quick navigation.
    </p>

    <div class="pub-tabs">
      <button class="tab-button active" onclick="filterPublications(event, 'all')">All</button>
      <button class="tab-button" onclick="filterPublications(event, 'conference')">Conference</button>
      <button class="tab-button" onclick="filterPublications(event, 'journal')">Journal</button>
      <button class="tab-button" onclick="filterPublications(event, 'award')">Awarded / Recognized</button>
      <button class="tab-button" onclick="filterPublications(event, 'earlier')">Earlier Work</button>
    </div>

    <div class="year-section" data-year-section="2026">
      <div class="year-header">
        <div class="year-title">📅 2026 Publications</div>
        <div class="year-pill">1 publication</div>
      </div>

      <div class="publication-card" data-type="conference">
        <div class="pub-top">
          <span class="pub-year">2026</span>
          <span class="pub-type">IEEE Conference</span>
          <span class="pub-award">Published</span>
        </div>

        <div class="pub-title">
          Bin-Based R: Resource-Efficient RF Modulation Classification Using Envelope Statistics
        </div>

        <div class="pub-authors">
          S. R. Sapireddy, G. Surekha, and H. Bandi
        </div>

        <div class="pub-venue">
          SoutheastCon 2026, Huntsville, AL, USA, 2026, pp. 1-6.
        </div>

        <div class="pub-note">
          DOI: 10.1109/SoutheastCon63549.2026.11476603
        </div>

        <div class="pub-links">
          <button class="pub-button primary" onclick="toggleCitation('cite-2026-southeastcon')">Citation</button>
          <button class="pub-button" onclick="copyCitation('cite-2026-southeastcon')">Copy Citation</button>
          <a class="pub-link" href="https://doi.org/10.1109/SoutheastCon63549.2026.11476603" target="_blank" rel="noopener">DOI</a>
          <a class="pub-link disabled" href="#" onclick="return false;">PDF pending</a>
        </div>

        <div id="cite-2026-southeastcon" class="citation-box">S. R. Sapireddy, G. Surekha, and H. Bandi, "Bin-Based R: Resource-Efficient RF Modulation Classification Using Envelope Statistics," SoutheastCon 2026, Huntsville, AL, USA, 2026, pp. 1-6, doi: 10.1109/SoutheastCon63549.2026.11476603.</div>
      </div>
    </div>

    <div class="year-section" data-year-section="2025">
      <div class="year-header">
        <div class="year-title">📅 2025 Publications</div>
        <div class="year-pill">6 publications</div>
      </div>

      <div class="publication-card" data-type="journal">
        <div class="pub-top">
          <span class="pub-year">2025</span>
          <span class="pub-type">Journal Article</span>
          <span class="pub-award">Published</span>
        </div>
      
        <div class="pub-title">
          Simplifying Activations with Linear Approximations in Neural Networks
        </div>
      
        <div class="pub-authors">
          Srinivas Rahul Sapireddy, Kazi Asifuzzaman, and Rahman Mostafizur
        </div>
      
        <div class="pub-venue">
          Memories - Materials, Devices, Circuits and Systems, Volume 11, 2025, Article 100134.
        </div>
      
        <div class="pub-note">
          ISSN: 2773-0646 | DOI: 10.1016/j.memori.2025.100134
        </div>
      
        <div class="pub-links">
          <button class="pub-button primary" onclick="toggleCitation('cite-2025-memories-linear')">Citation</button>
          <button class="pub-button" onclick="copyCitation('cite-2025-memories-linear')">Copy Citation</button>
          <a class="pub-link" href="https://doi.org/10.1016/j.memori.2025.100134" target="_blank" rel="noopener">DOI</a>
          <a class="pub-link disabled" href="#" onclick="return false;">PDF pending</a>
        </div>
      
        <div id="cite-2025-memories-linear" class="citation-box">S. R. Sapireddy, K. Asifuzzaman, and R. Mostafizur, "Simplifying activations with linear approximations in neural networks," Memories - Materials, Devices, Circuits and Systems, vol. 11, 2025, Art. no. 100134, doi: 10.1016/j.memori.2025.100134.</div>
      </div>
      <div class="publication-card" data-type="conference">
        <div class="pub-top">
          <span class="pub-year">2025</span>
          <span class="pub-type">ACM Conference</span>
        </div>

        <div class="pub-title">
          On the Effectiveness of Custom Activation Functions on Long-Term Short-Term Memory
        </div>

        <div class="pub-authors">
          Srinivas Rahul Sapireddy and collaborators
        </div>

        <div class="pub-venue">
          ACM Great Lakes Symposium on VLSI, GLSVLSI, 2025.
        </div>

        <div class="pub-links">
          <button class="pub-button primary" onclick="toggleCitation('cite-2025-glsvlsi')">Citation</button>
          <button class="pub-button" onclick="copyCitation('cite-2025-glsvlsi')">Copy Citation</button>
          <a class="pub-link disabled" href="#" onclick="return false;">DOI pending</a>
          <a class="pub-link disabled" href="#" onclick="return false;">PDF pending</a>
        </div>

        <div id="cite-2025-glsvlsi" class="citation-box">Srinivas Rahul Sapireddy and collaborators, "On the Effectiveness of Custom Activation Functions on Long-Term Short-Term Memory," ACM Great Lakes Symposium on VLSI, GLSVLSI, 2025.</div>
      </div>

      <div class="publication-card" data-type="journal">
        <div class="pub-top">
          <span class="pub-year">2025</span>
          <span class="pub-type">Journal</span>
        </div>

        <div class="pub-title">
          Simplifying Activations with Linear Approximations in Neural Networks
        </div>

        <div class="pub-authors">
          Srinivas Rahul Sapireddy and collaborators
        </div>

        <div class="pub-venue">
          Memories - Materials, Devices, Circuits and Systems, 2025.
        </div>

        <div class="pub-links">
          <button class="pub-button primary" onclick="toggleCitation('cite-2025-memories-linear')">Citation</button>
          <button class="pub-button" onclick="copyCitation('cite-2025-memories-linear')">Copy Citation</button>
          <a class="pub-link disabled" href="#" onclick="return false;">DOI pending</a>
          <a class="pub-link disabled" href="#" onclick="return false;">PDF pending</a>
        </div>

        <div id="cite-2025-memories-linear" class="citation-box">Srinivas Rahul Sapireddy and collaborators, "Simplifying Activations with Linear Approximations in Neural Networks," Memories - Materials, Devices, Circuits and Systems, 2025.</div>
      </div>

      <div class="publication-card" data-type="conference">
        <div class="pub-top">
          <span class="pub-year">2025</span>
          <span class="pub-type">Conference</span>
        </div>

        <div class="pub-title">
          Adversarial-Resilient RF Fingerprinting: A CNN-GAN Framework for Rogue Transmitter Detection
        </div>

        <div class="pub-authors">
          Srinivas Rahul Sapireddy and collaborators
        </div>

        <div class="pub-venue">
          ICMLA, 2025.
        </div>

        <div class="pub-links">
          <button class="pub-button primary" onclick="toggleCitation('cite-2025-icmla')">Citation</button>
          <button class="pub-button" onclick="copyCitation('cite-2025-icmla')">Copy Citation</button>
          <a class="pub-link disabled" href="#" onclick="return false;">DOI pending</a>
          <a class="pub-link disabled" href="#" onclick="return false;">PDF pending</a>
        </div>

        <div id="cite-2025-icmla" class="citation-box">Srinivas Rahul Sapireddy and collaborators, "Adversarial-Resilient RF Fingerprinting: A CNN-GAN Framework for Rogue Transmitter Detection," ICMLA, 2025.</div>
      </div>

      <div class="publication-card" data-type="conference award">
        <div class="pub-top">
          <span class="pub-year">2025</span>
          <span class="pub-type">IEEE Conference</span>
          <span class="pub-award">Recognized Paper</span>
        </div>

        <div class="pub-title">
          C/N0 Analysis-Based GPS Spoofing Detection with Variable Antenna Orientations
        </div>

        <div class="pub-authors">
          Srinivas Rahul Sapireddy and collaborators
        </div>

        <div class="pub-venue">
          IEEE CARS, 2025.
        </div>

        <div class="pub-note">
          Note: update this card with the exact CARS award wording if needed.
        </div>

        <div class="pub-links">
          <button class="pub-button primary" onclick="toggleCitation('cite-2025-cars')">Citation</button>
          <button class="pub-button" onclick="copyCitation('cite-2025-cars')">Copy Citation</button>
          <a class="pub-link disabled" href="#" onclick="return false;">DOI pending</a>
          <a class="pub-link disabled" href="#" onclick="return false;">PDF pending</a>
        </div>

        <div id="cite-2025-cars" class="citation-box">Srinivas Rahul Sapireddy and collaborators, "C/N0 Analysis-Based GPS Spoofing Detection with Variable Antenna Orientations," IEEE CARS, 2025.</div>
      </div>

      <div class="publication-card" data-type="journal">
        <div class="pub-top">
          <span class="pub-year">2025</span>
          <span class="pub-type">Journal</span>
        </div>

        <div class="pub-title">
          Early Detection of Adversarial Examples in Internet-of-Things Networks
        </div>

        <div class="pub-authors">
          Srinivas Rahul Sapireddy and collaborators
        </div>

        <div class="pub-venue">
          Electronics, 2025.
        </div>

        <div class="pub-links">
          <button class="pub-button primary" onclick="toggleCitation('cite-2025-electronics')">Citation</button>
          <button class="pub-button" onclick="copyCitation('cite-2025-electronics')">Copy Citation</button>
          <a class="pub-link disabled" href="#" onclick="return false;">DOI pending</a>
          <a class="pub-link disabled" href="#" onclick="return false;">PDF pending</a>
        </div>

        <div id="cite-2025-electronics" class="citation-box">Srinivas Rahul Sapireddy and collaborators, "Early Detection of Adversarial Examples in Internet-of-Things Networks," Electronics, 2025.</div>
      </div>
    </div>

    <div class="year-section" data-year-section="2024">
      <div class="year-header">
        <div class="year-title">📅 2024 Publications</div>
        <div class="year-pill">2 publications</div>
      </div>

      <div class="publication-card" data-type="journal">
        <div class="pub-top">
          <span class="pub-year">2024</span>
          <span class="pub-type">Journal</span>
        </div>

        <div class="pub-title">
          Piecewise Linear Approximation of Activation Functions for Neural Networks
        </div>

        <div class="pub-authors">
          Srinivas Rahul Sapireddy and collaborators
        </div>

        <div class="pub-venue">
          Memories - Materials, Devices, Circuits and Systems, 2024.
        </div>

        <div class="pub-links">
          <button class="pub-button primary" onclick="toggleCitation('cite-2024-piecewise')">Citation</button>
          <button class="pub-button" onclick="copyCitation('cite-2024-piecewise')">Copy Citation</button>
          <a class="pub-link disabled" href="#" onclick="return false;">DOI pending</a>
          <a class="pub-link disabled" href="#" onclick="return false;">PDF pending</a>
        </div>

        <div id="cite-2024-piecewise" class="citation-box">Srinivas Rahul Sapireddy and collaborators, "Piecewise Linear Approximation of Activation Functions for Neural Networks," Memories - Materials, Devices, Circuits and Systems, 2024.</div>
      </div>

      <div class="publication-card" data-type="journal">
        <div class="pub-top">
          <span class="pub-year">2024</span>
          <span class="pub-type">Journal</span>
        </div>

        <div class="pub-title">
          A Review of Crosstalk-Based Polymorphic Circuit Design
        </div>

        <div class="pub-authors">
          Srinivas Rahul Sapireddy and collaborators
        </div>

        <div class="pub-venue">
          Memories - Materials, Devices, Circuits and Systems, 2024.
        </div>

        <div class="pub-links">
          <button class="pub-button primary" onclick="toggleCitation('cite-2024-crosstalk')">Citation</button>
          <button class="pub-button" onclick="copyCitation('cite-2024-crosstalk')">Copy Citation</button>
          <a class="pub-link disabled" href="#" onclick="return false;">DOI pending</a>
          <a class="pub-link disabled" href="#" onclick="return false;">PDF pending</a>
        </div>

        <div id="cite-2024-crosstalk" class="citation-box">Srinivas Rahul Sapireddy and collaborators, "A Review of Crosstalk-Based Polymorphic Circuit Design," Memories - Materials, Devices, Circuits and Systems, 2024.</div>
      </div>
    </div>

    <div class="year-section" data-year-section="2018">
      <div class="year-header">
        <div class="year-title">📅 2018 Earlier Work</div>
        <div class="year-pill">update exact details</div>
      </div>

      <div class="publication-card placeholder" data-type="earlier">
        <div class="pub-top">
          <span class="pub-year">2018</span>
          <span class="pub-type">Earlier Research Output</span>
          <span class="pub-status">Replace with exact title</span>
        </div>

        <div class="pub-title">
          Add exact 2018 publication title here
        </div>

        <div class="pub-authors">
          Add exact author list here
        </div>

        <div class="pub-venue">
          Add exact venue, conference, journal, workshop, or institutional publication details here.
        </div>

        <div class="pub-note">
          Replace this placeholder with the exact 2018 publication details.
        </div>

        <div class="pub-links">
          <button class="pub-button primary" onclick="toggleCitation('cite-2018-placeholder')">Citation</button>
          <button class="pub-button" onclick="copyCitation('cite-2018-placeholder')">Copy Citation</button>
          <a class="pub-link disabled" href="#" onclick="return false;">Update link</a>
        </div>

        <div id="cite-2018-placeholder" class="citation-box">Add exact 2018 citation here.</div>
      </div>
    </div>

    <div class="year-section" data-year-section="2016">
      <div class="year-header">
        <div class="year-title">📅 2016 Earlier Work</div>
        <div class="year-pill">update exact details</div>
      </div>

      <div class="publication-card placeholder" data-type="earlier">
        <div class="pub-top">
          <span class="pub-year">2016</span>
          <span class="pub-type">Earlier Research Output</span>
          <span class="pub-status">Replace with exact title</span>
        </div>

        <div class="pub-title">
          Add exact 2016 publication title here
        </div>

        <div class="pub-authors">
          Add exact author list here
        </div>

        <div class="pub-venue">
          Add exact venue, conference, journal, workshop, or institutional publication details here.
        </div>

        <div class="pub-note">
          Replace this placeholder with the exact 2016 publication details.
        </div>

        <div class="pub-links">
          <button class="pub-button primary" onclick="toggleCitation('cite-2016-placeholder')">Citation</button>
          <button class="pub-button" onclick="copyCitation('cite-2016-placeholder')">Copy Citation</button>
          <a class="pub-link disabled" href="#" onclick="return false;">Update link</a>
        </div>

        <div id="cite-2016-placeholder" class="citation-box">Add exact 2016 citation here.</div>
      </div>
    </div>

  </div>

  <div class="grid-2">
    <div class="section">
      <h2>📍 Publication Timeline</h2>
      <div class="divider"></div>

      <div class="timeline">
        <div class="timeline-item">
          <div class="timeline-year">2026</div>
          <div class="timeline-title">IEEE SoutheastCon</div>
          <div class="timeline-text">
            Bin-Based R framework for resource-efficient RF modulation classification using envelope statistics.
          </div>
        </div>

        <div class="timeline-item">
          <div class="timeline-year">2025</div>
          <div class="timeline-title">RF, AI, Security, and VLSI Publications</div>
          <div class="timeline-text">
            Work across RFCoN, GLSVLSI, ICMLA, IEEE CARS, Electronics, and Memories.
          </div>
        </div>

        <div class="timeline-item">
          <div class="timeline-year">2024</div>
          <div class="timeline-title">Activation Functions and Circuit Design</div>
          <div class="timeline-text">
            Journal work on piecewise activation approximation and polymorphic circuit design.
          </div>
        </div>

        <div class="timeline-item">
          <div class="timeline-year">2018 / 2016</div>
          <div class="timeline-title">Earlier Research Outputs</div>
          <div class="timeline-text">
            Replace the placeholder cards above with exact title, author, venue, DOI, and PDF details.
          </div>
        </div>
      </div>
    </div>

    <div class="section">
      <h2>🌐 Publication Profiles</h2>
      <div class="divider"></div>

      <p>
        For updated indexing, citation counts, and official metadata, please visit my public scholarly profiles.
      </p>

      <div class="pub-links">
        <a class="pub-link" href="https://scholar.google.com/citations?user=08fgpdIAAAAJ" target="_blank" rel="noopener">Google Scholar</a>
        <a class="pub-link" href="https://orcid.org/0000-0002-9898-6810" target="_blank" rel="noopener">ORCID</a>
        <a class="pub-link" href="https://openreview.net/profile?id=~Srinivas_Rahul_Sapireddy1" target="_blank" rel="noopener">OpenReview</a>
        <a class="pub-link" href="/resume/">Resume</a>
      </div>
    </div>
  </div>

</div>

<script>
function toggleCitation(id) {
  const box = document.getElementById(id);
  if (!box) return;

  if (box.style.display === "block") {
    box.style.display = "none";
  } else {
    box.style.display = "block";
  }
}

function copyCitation(id) {
  const box = document.getElementById(id);
  if (!box) return;

  const text = box.innerText;

  if (navigator.clipboard) {
    navigator.clipboard.writeText(text).then(function () {
      alert("Citation copied to clipboard.");
    }).catch(function () {
      alert("Unable to copy automatically. Please copy the citation manually.");
    });
  } else {
    alert("Clipboard not supported. Please copy the citation manually.");
  }
}

function filterPublications(event, filterType) {
  const buttons = document.querySelectorAll(".tab-button");
  const cards = document.querySelectorAll(".publication-card");
  const yearSections = document.querySelectorAll(".year-section");

  buttons.forEach(function(button) {
    button.classList.remove("active");
  });

  if (event && event.currentTarget) {
    event.currentTarget.classList.add("active");
  }

  cards.forEach(function(card) {
    const type = card.getAttribute("data-type") || "";

    if (filterType === "all" || type.includes(filterType)) {
      card.classList.remove("hide-card");
    } else {
      card.classList.add("hide-card");
    }
  });

  yearSections.forEach(function(section) {
    const visibleCards = section.querySelectorAll(".publication-card:not(.hide-card)");
    if (visibleCards.length === 0) {
      section.classList.add("hide-year");
    } else {
      section.classList.remove("hide-year");
    }
  });
}
</script>
