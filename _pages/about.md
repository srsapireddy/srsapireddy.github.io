---
title: "About"
layout: single
permalink: /about/
author_profile: true
---

<style>
:root {
  --blue: #1a73e8;
  --blue2: #0b5bd3;
  --isu: #DC143C;
  --bg: #ffffff;
  --soft: #f6f9ff;
  --muted: #5f6368;
  --text: #0b1f44;
  --border: rgba(26,115,232,0.18);
  --shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
  --shadow2: 0 2px 10px rgba(0, 0, 0, 0.05);
  --radius: 18px;
  --radius2: 14px;
}

@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(14px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.about-wrap {
  animation: fadeInUp 0.8s ease-in-out;
}

/* Hero */
.about-hero {
  position: relative;
  overflow: hidden;
  border-radius: var(--radius);
  padding: 2.2rem 2rem;
  margin-bottom: 1.4rem;
  background:
    radial-gradient(circle at top right, rgba(220,20,60,0.13), transparent 32%),
    linear-gradient(135deg, #e9f3ff 0%, #ffffff 62%);
  border: 1px solid rgba(26,115,232,0.25);
  box-shadow: var(--shadow);
}

.about-hero::before {
  content: "";
  position: absolute;
  inset: 0;
  background-image:
    linear-gradient(rgba(26,115,232,0.06) 1px, transparent 1px),
    linear-gradient(90deg, rgba(26,115,232,0.06) 1px, transparent 1px);
  background-size: 34px 34px;
  pointer-events: none;
}

.about-hero-content {
  position: relative;
  z-index: 1;
}

.hero-kicker {
  display: inline-block;
  padding: 0.35rem 0.75rem;
  border-radius: 999px;
  background: #ffffff;
  border: 1px solid rgba(220,20,60,0.25);
  color: var(--isu);
  font-weight: 900;
  font-size: 0.88rem;
  box-shadow: var(--shadow2);
  margin-bottom: 0.9rem;
}

.about-hero h1 {
  margin: 0;
  font-size: 2.15rem;
  line-height: 1.15;
  color: var(--text);
}

.about-hero .subtitle {
  margin-top: 0.55rem;
  color: #202124;
  font-size: 1.08rem;
  font-weight: 650;
}

.about-hero p {
  margin: 0.8rem 0 0 0;
  color: var(--muted);
  font-size: 1.03rem;
  line-height: 1.65;
  max-width: 86ch;
}

/* Badges */
.badges {
  display: flex;
  flex-wrap: wrap;
  gap: 0.55rem;
  margin-top: 1rem;
}

.badge {
  display: inline-flex;
  align-items: center;
  gap: 0.35rem;
  padding: 0.38rem 0.75rem;
  border-radius: 999px;
  background: #ffffff;
  border: 1px solid rgba(26,115,232,0.22);
  box-shadow: var(--shadow2);
  font-size: 0.9rem;
  color: var(--text);
  font-weight: 800;
}

/* Buttons */
.hero-links {
  display: flex;
  flex-wrap: wrap;
  gap: 0.7rem;
  margin-top: 1.15rem;
}

.btn-link {
  display: inline-flex;
  align-items: center;
  gap: 0.45rem;
  padding: 0.58rem 0.92rem;
  border-radius: 12px;
  background: var(--blue);
  color: #ffffff !important;
  text-decoration: none !important;
  font-weight: 850;
  box-shadow: var(--shadow2);
  transition: 0.2s ease-in-out;
}

.btn-link:hover {
  background: var(--blue2);
  transform: translateY(-2px);
  text-decoration: none !important;
}

.btn-link.secondary {
  background: #ffffff;
  color: var(--blue) !important;
  border: 1px solid rgba(26,115,232,0.25);
}

/* Impact strip */
.impact-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 0.9rem;
  margin-bottom: 1.3rem;
}

.impact-card {
  text-align: center;
  padding: 1.05rem 0.9rem;
  border-radius: var(--radius2);
  background: linear-gradient(135deg, #ffffff 0%, #f7fbff 100%);
  border: 1px solid var(--border);
  box-shadow: var(--shadow2);
  transition: 0.22s ease-in-out;
}

.impact-card:hover {
  transform: translateY(-3px);
  box-shadow: var(--shadow);
}

.impact-card .big {
  color: var(--isu);
  font-size: 1.55rem;
  font-weight: 950;
  line-height: 1.1;
}

.impact-card .label {
  color: var(--text);
  font-weight: 850;
  margin-top: 0.35rem;
  font-size: 0.92rem;
}

.impact-card .small {
  color: var(--muted);
  font-size: 0.8rem;
  margin-top: 0.2rem;
}

/* General cards */
.section {
  position: relative;
  overflow: hidden;
  border: 1px solid var(--border);
  background: var(--bg);
  padding: 1.35rem 1.5rem;
  margin-bottom: 1.3rem;
  border-radius: var(--radius2);
  box-shadow: var(--shadow2);
  transition: 0.25s ease-in-out;
}

.section:hover {
  background: #fbfdff;
  transform: translateY(-2px);
  box-shadow: var(--shadow);
}

.section h2,
.section h3 {
  margin: 0;
  color: var(--text);
  font-size: 1.22rem;
  display: flex;
  align-items: center;
  gap: 0.55rem;
}

.section p {
  color: #202124;
  line-height: 1.65;
}

.section ul {
  padding-left: 1.2rem;
  margin-bottom: 0.4rem;
}

.section li {
  margin-bottom: 0.45rem;
  line-height: 1.5;
}

.divider {
  height: 1px;
  background: rgba(26,115,232,0.12);
  margin: 0.6rem 0 1rem 0;
}

/* Grids */
.grid-2 {
  display: grid;
  grid-template-columns: 1fr;
  gap: 1.2rem;
}

.grid-3 {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1.1rem;
  margin-bottom: 1.3rem;
}

@media (min-width: 900px) {
  .grid-2 {
    grid-template-columns: 1fr 1fr;
  }
}

@media (max-width: 950px) {
  .grid-3,
  .impact-grid {
    grid-template-columns: 1fr 1fr;
  }
}

@media (max-width: 600px) {
  .grid-3,
  .impact-grid {
    grid-template-columns: 1fr;
  }

  .about-hero {
    padding: 1.5rem 1.1rem;
  }

  .about-hero h1 {
    font-size: 1.65rem;
  }
}

/* Research identity cards */
.focus-card {
  position: relative;
  overflow: hidden;
  padding: 1.25rem;
  border-radius: 16px;
  background: linear-gradient(135deg, #ffffff 0%, #f4f9ff 100%);
  border: 1px solid var(--border);
  box-shadow: var(--shadow2);
  transition: 0.25s ease-in-out;
}

.focus-card:hover {
  transform: translateY(-4px);
  box-shadow: var(--shadow);
}

.focus-card::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  height: 5px;
  width: 100%;
  background: linear-gradient(90deg, var(--blue), var(--isu));
}

.focus-icon {
  width: 46px;
  height: 46px;
  border-radius: 14px;
  background: #e9f3ff;
  color: var(--blue);
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 1.45rem;
  margin-bottom: 0.85rem;
  box-shadow: 0 4px 12px rgba(26,115,232,0.16);
}

.focus-card h3 {
  margin: 0 0 0.55rem 0;
  font-size: 1.12rem;
  color: var(--text);
}

.focus-card p {
  margin: 0;
  color: #202124;
  line-height: 1.55;
  font-size: 0.95rem;
}

/* Timeline */
.timeline {
  position: relative;
  margin-top: 0.3rem;
  padding-left: 1.3rem;
}

.timeline::before {
  content: "";
  position: absolute;
  left: 0.25rem;
  top: 0.2rem;
  bottom: 0.2rem;
  width: 2px;
  background: linear-gradient(180deg, var(--blue), var(--isu));
}

.timeline-item {
  position: relative;
  margin-bottom: 1rem;
  padding-left: 1rem;
}

.timeline-item::before {
  content: "";
  position: absolute;
  left: -1.29rem;
  top: 0.25rem;
  width: 11px;
  height: 11px;
  border-radius: 50%;
  background: var(--isu);
  border: 3px solid #ffffff;
  box-shadow: 0 0 0 2px rgba(220,20,60,0.22);
}

.timeline-year {
  color: var(--isu);
  font-weight: 900;
  font-size: 0.88rem;
}

.timeline-title {
  color: var(--text);
  font-weight: 900;
  margin-top: 0.1rem;
}

.timeline-text {
  color: #202124;
  margin-top: 0.15rem;
  line-height: 1.5;
}

/* Publication cards */
.pub-card {
  padding: 1rem;
  border-radius: 14px;
  background: #ffffff;
  border: 1px solid var(--border);
  box-shadow: var(--shadow2);
  margin-bottom: 0.85rem;
}

.pub-venue {
  display: inline-block;
  padding: 0.25rem 0.58rem;
  border-radius: 999px;
  background: #f3f8ff;
  border: 1px solid rgba(26,115,232,0.16);
  color: var(--isu);
  font-size: 0.78rem;
  font-weight: 900;
  margin-bottom: 0.45rem;
}

.pub-title {
  color: var(--text);
  font-weight: 850;
  line-height: 1.45;
}

/* Tags */
.tag-cloud {
  display: flex;
  flex-wrap: wrap;
  gap: 0.55rem;
}

.tag {
  display: inline-flex;
  padding: 0.36rem 0.72rem;
  border-radius: 999px;
  background: #f3f8ff;
  border: 1px solid rgba(26,115,232,0.18);
  color: var(--text);
  font-size: 0.88rem;
  font-weight: 800;
}

/* Profile links */
.profile-grid {
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  gap: 0.8rem;
}

.profile-link {
  text-align: center;
  padding: 0.85rem 0.6rem;
  border-radius: 14px;
  background: #ffffff;
  border: 1px solid var(--border);
  color: var(--blue) !important;
  font-weight: 900;
  text-decoration: none !important;
  box-shadow: var(--shadow2);
  transition: 0.2s ease-in-out;
}

.profile-link:hover {
  transform: translateY(-2px);
  box-shadow: var(--shadow);
  background: #f3f8ff;
  text-decoration: none !important;
}

@media (max-width: 900px) {
  .profile-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (max-width: 520px) {
  .profile-grid {
    grid-template-columns: 1fr;
  }
}
</style>

<div class="about-wrap">

  <div class="about-hero">
    <div class="about-hero-content">
      <span class="hero-kicker">Assistant Professor · Electrical Engineering</span>

      <h1>Srinivas Rahul Sapireddy, Ph.D.</h1>

      <div class="subtitle">
        College of Engineering · Illinois State University
      </div>

      <p>
        My work connects hardware-aware artificial intelligence, RF signal intelligence,
        edge computing, and VLSI system design. I focus on building efficient learning and
        signal-processing methods that can operate reliably on resource-constrained computing platforms.
      </p>

      <div class="badges">
        <span class="badge">Hardware-Aware AI</span>
        <span class="badge">RF Signal Intelligence</span>
        <span class="badge">Edge Computing</span>
        <span class="badge">VLSI / Physical Design</span>
      </div>

      <div class="hero-links">
        <a class="btn-link" href="/insys-lab/">INSys Lab</a>
        <a class="btn-link secondary" href="/publications/">Publications</a>
        <a class="btn-link secondary" href="/teaching/">Teaching</a>
        <a class="btn-link secondary" href="/resume/">Resume</a>
      </div>
    </div>
  </div>

  <div class="impact-grid">
    <div class="impact-card">
      <div class="big">AI</div>
      <div class="label">Hardware-Aware ML</div>
      <div class="small">Efficient inference for edge systems</div>
    </div>

    <div class="impact-card">
      <div class="big">RF</div>
      <div class="label">Signal Intelligence</div>
      <div class="small">Modulation classification and sensing</div>
    </div>

    <div class="impact-card">
      <div class="big">VLSI</div>
      <div class="label">Physical Design</div>
      <div class="small">RTL-to-GDSII and hardware systems</div>
    </div>

    <div class="impact-card">
      <div class="big">Edge</div>
      <div class="label">Low-Power Computing</div>
      <div class="small">Deployment on constrained devices</div>
    </div>
  </div>

  <div class="grid-3">
    <div class="focus-card">
      <div class="focus-icon">🧠</div>
      <h3>Efficient AI</h3>
      <p>
        I design lightweight models, custom activations, and deployment-aware learning methods
        for hardware-constrained environments.
      </p>
    </div>

    <div class="focus-card">
      <div class="focus-icon">📡</div>
      <h3>RF Signal Intelligence</h3>
      <p>
        I develop statistical, time-frequency, and cyclostationary feature methods for
        RF signal classification and analysis.
      </p>
    </div>

    <div class="focus-card">
      <div class="focus-icon">⚙️</div>
      <h3>VLSI and Edge Systems</h3>
      <p>
        I work on physical design, hardware acceleration, RTL-to-GDSII flow, and efficient
        embedded computing systems.
      </p>
    </div>
  </div>

  <div class="grid-2">
    <div class="section">
      <h2>👋 About Me</h2>
      <div class="divider"></div>
      <p>
        I am an Assistant Professor in Electrical Engineering at Illinois State University.
        My research integrates signal processing, lightweight machine learning, and
        hardware-efficient architectures to enable accurate and energy-efficient computation
        in resource-constrained environments.
      </p>
      <p>
        My teaching interests include logic design, engineering computation, ASIC physical design,
        analog integrated circuits, embedded systems, and hardware-aware machine learning.
      </p>
    </div>

    <div class="section">
      <h2>🤝 Open to Collaboration</h2>
      <div class="divider"></div>
      <p>
        I welcome research collaborations in efficient edge AI, RF signal intelligence,
        hardware-software co-design, VLSI systems, and applied engineering education.
      </p>
      <p>
        I am also interested in mentoring undergraduate and graduate students through
        research projects, technical writing, and hands-on engineering design activities.
      </p>
    </div>
  </div>

  <div class="section">
    <h2>🔬 Research and Technical Focus</h2>
    <div class="divider"></div>

    <div class="tag-cloud">
      <span class="tag">Hardware-Aware Machine Learning</span>
      <span class="tag">Low-Power Edge AI</span>
      <span class="tag">RF Modulation Classification</span>
      <span class="tag">Cyclostationary Signal Processing</span>
      <span class="tag">Statistical Feature Engineering</span>
      <span class="tag">Custom Activation Functions</span>
      <span class="tag">VLSI Physical Design</span>
      <span class="tag">RTL-to-GDSII Flow</span>
      <span class="tag">Timing Analysis</span>
      <span class="tag">Embedded AI Accelerators</span>
      <span class="tag">System-on-Chip Architectures</span>
      <span class="tag">Hardware-Software Co-Design</span>
    </div>
  </div>

  <div class="grid-2">
    <div class="section">
      <h2>📍 Academic Path</h2>
      <div class="divider"></div>

      <div class="timeline">
        <div class="timeline-item">
          <div class="timeline-year">2026</div>
          <div class="timeline-title">Assistant Professor, Illinois State University</div>
          <div class="timeline-text">College of Engineering, Electrical Engineering.</div>
        </div>

        <div class="timeline-item">
          <div class="timeline-year">2025</div>
          <div class="timeline-title">Ph.D., Electrical and Computer Engineering</div>
          <div class="timeline-text">University of Missouri-Kansas City.</div>
        </div>

        <div class="timeline-item">
          <div class="timeline-year">Prior</div>
          <div class="timeline-title">Graduate Training in EE, CS, and AI</div>
          <div class="timeline-text">Electrical engineering, computer science, and artificial intelligence foundations.</div>
        </div>
      </div>
    </div>

    <div class="section">
      <h2>🏆 Awards and Recognitions</h2>
      <div class="divider"></div>
      <ul>
        <li>Best Paper Award, IEEE RFCoN 2025, Track 2, Session II</li>
        <li>Dean's International Scholar Award, University of Missouri-Kansas City</li>
        <li>IEEE-Eta Kappa Nu Honor Society Membership</li>
        <li>CS Balaji Memorial Travel Grant, 2025</li>
        <li>Second Place, Hack-A-Roo Fall 2022, Entrepreneur Track</li>
        <li>Third Place, Hack-A-Roo Fall 2021, CS/IT Track</li>
      </ul>
    </div>
  </div>

  <div class="grid-2">
    <div class="section">
      <h2>📝 Selected Publications</h2>
      <div class="divider"></div>

      <div class="pub-card">
        <span class="pub-venue">IEEE SoutheastCon 2026</span>
        <div class="pub-title">
          Bin-Based R-Value Statistical Envelope Analysis for RF Modulation Classification
        </div>
      </div>

      <div class="pub-card">
        <span class="pub-venue">ACM GLSVLSI 2025</span>
        <div class="pub-title">
          Hardware-Efficient Custom Activation Functions for LSTM Networks
        </div>
      </div>

      <div class="pub-card">
        <span class="pub-venue">IEEE RFCoN 2025</span>
        <div class="pub-title">
          Statistical Envelope Analysis for Lightweight RF Signal Classification
        </div>
      </div>

      <div class="pub-card">
        <span class="pub-venue">MDPI Electronics 2025</span>
        <div class="pub-title">
          Early Detection of Adversarial Examples in Internet-of-Things Networks
        </div>
      </div>

      <div class="pub-card">
        <span class="pub-venue">MDPI Memories 2024</span>
        <div class="pub-title">
          Piecewise Linear Approximations of Activation Functions for Neural Networks
        </div>
      </div>

      <p>
        <a href="/publications/">View complete list of publications</a>
      </p>
    </div>

    <div class="section">
      <h2>🛠️ Technical Expertise</h2>
      <div class="divider"></div>

      <div class="tag-cloud">
        <span class="tag">Python</span>
        <span class="tag">C/C++</span>
        <span class="tag">Verilog</span>
        <span class="tag">TCL</span>
        <span class="tag">PyTorch</span>
        <span class="tag">TensorFlow Lite</span>
        <span class="tag">Scikit-learn</span>
        <span class="tag">Docker</span>
        <span class="tag">Yosys</span>
        <span class="tag">OpenSTA</span>
        <span class="tag">Cadence</span>
        <span class="tag">Synopsys</span>
      </div>

      <p>
        My technical work spans machine learning development, RF signal analysis,
        digital hardware design, physical implementation, and deployment-oriented
        system optimization.
      </p>
    </div>
  </div>

  <div class="section">
    <h2>🌐 Professional Profiles</h2>
    <div class="divider"></div>

    <div class="profile-grid">
      <a class="profile-link" href="https://github.com/srsapireddy" target="_blank" rel="noopener">GitHub</a>
      <a class="profile-link" href="https://scholar.google.com/citations?user=08fgpdIAAAAJ" target="_blank" rel="noopener">Google Scholar</a>
      <a class="profile-link" href="https://orcid.org/0000-0002-9898-6810" target="_blank" rel="noopener">ORCID</a>
      <a class="profile-link" href="https://openreview.net/profile?id=~Srinivas_Rahul_Sapireddy1" target="_blank" rel="noopener">OpenReview</a>
      <a class="profile-link" href="https://medium.com/@srsapireddy" target="_blank" rel="noopener">Medium</a>
    </div>
  </div>

</div>
