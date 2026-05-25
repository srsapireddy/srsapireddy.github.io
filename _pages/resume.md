---
title: "Publications"
layout: single
permalink: /publications/
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
  --shadow: 0 10px 30px rgba(0,0,0,0.08);
  --shadow2: 0 2px 10px rgba(0,0,0,0.05);
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

.pub-wrap {
  animation: fadeInUp 0.8s ease-in-out;
}

/* Hero */
.pub-hero {
  position: relative;
  overflow: hidden;
  border-radius: var(--radius);
  padding: 2.2rem 2rem;
  margin-bottom: 1.35rem;
  background:
    radial-gradient(circle at top right, rgba(220,20,60,0.13), transparent 32%),
    linear-gradient(135deg, #e9f3ff 0%, #ffffff 62%);
  border: 1px solid rgba(26,115,232,0.25);
  box-shadow: var(--shadow);
}

.pub-hero::before {
  content: "";
  position: absolute;
  inset: 0;
  background-image:
    linear-gradient(rgba(26,115,232,0.06) 1px, transparent 1px),
    linear-gradient(90deg, rgba(26,115,232,0.06) 1px, transparent 1px);
  background-size: 34px 34px;
  pointer-events: none;
}

.pub-hero-content {
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

.pub-hero h1 {
  margin: 0;
  font-size: 2.15rem;
  line-height: 1.15;
  color: var(--text);
}

.pub-hero .subtitle {
  margin-top: 0.55rem;
  color: #202124;
  font-size: 1.08rem;
  font-weight: 650;
}

.pub-hero p {
  margin: 0.8rem 0 0 0;
  color: var(--muted);
  font-size: 1.03rem;
  line-height: 1.65;
  max-width: 86ch;
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
  padding: 0.38rem 0.75rem;
  border-radius: 999px;
  background: #ffffff;
  border: 1px solid rgba(26,115,232,0.22);
  box-shadow: var(--shadow2);
  font-size: 0.9rem;
  color: var(--text);
  font-weight: 800;
}

/* Impact cards */
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

/* General sections */
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

  .pub-hero {
    padding: 1.5rem 1.1rem;
  }

  .pub-hero h1 {
    font-size: 1.65rem;
  }
}

/* Research category cards */
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

/* Publication cards */
.publication-card {
  position: relative;
  padding: 1.15rem 1.15rem;
  border-radius: 16px;
  background: #ffffff;
  border: 1px solid var(--border);
  box-shadow: var(--shadow2);
  margin-bottom: 1rem;
  transition: 0.22s ease-in-out;
}

.publication-card:hover {
  transform: translateY(-3px);
  box-shadow: var(--shadow);
  background: #fbfdff;
}

.publication-card::before {
  content: "";
  position: absolute;
  left: 0;
  top: 1rem;
  bottom: 1rem;
  width: 4px;
  border-radius: 99px;
  background: linear-gradient(180deg, var(--blue), var(--isu));
}

.pub-top {
  display: flex;
  flex-wrap: wrap;
  gap: 0.55rem;
  align-items: center;
  margin-bottom: 0.65rem;
}

.pub-year,
.pub-type,
.pub-award {
  display: inline-flex;
  padding: 0.25rem 0.58rem;
  border-radius: 999px;
  font-size: 0.78rem;
  font-weight: 900;
}

.pub-year {
  background: #f3f8ff;
  border: 1px solid rgba(26,115,232,0.18);
  color: var(--blue);
}

.pub-type {
  background: #ffffff;
  border: 1px solid rgba(26,115,232,0.20);
  color: var(--text);
}

.pub-award {
  background: rgba(220,20,60,0.08);
  border: 1px solid rgba(220,20,60,0.25);
  color: var(--isu);
}

.pub-title {
  color: var(--text);
  font-size: 1.05rem;
  font-weight: 900;
  line-height: 1.45;
  margin-bottom: 0.45rem;
}

.pub-authors {
  color: #202124;
  font-size: 0.94rem;
  line-height: 1.5;
  margin-bottom: 0.35rem;
}

.pub-venue {
  color: var(--muted);
  font-size: 0.92rem;
  line-height: 1.45;
}

.pub-links {
  display: flex;
  flex-wrap: wrap;
  gap: 0.55rem;
  margin-top: 0.75rem;
}

.pub-link {
  display: inline-flex;
  align-items: center;
  padding: 0.32rem 0.65rem;
  border-radius: 999px;
  background: #f3f8ff;
  border: 1px solid rgba(26,115,232,0.18);
  color: var(--blue) !important;
  text-decoration: none !important;
  font-size: 0.84rem;
  font-weight: 850;
}

.pub-link:hover {
  background: #e9f3ff;
  text-decoration: none !important;
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

.timeline-item:last-child {
  margin-bottom: 0;
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

/* Scoped links */
.section a,
.pub-hero a {
  color: var(--blue);
  font-weight: 800;
  text-decoration: none;
}

.section a:hover,
.pub-hero a:hover {
  text-decoration: underline;
}
</style>

<div class="pub-wrap">

  <div class="pub-hero">
    <div class="pub-hero-content">
      <span class="hero-kicker">Research Publications · RF · AI · VLSI · Edge Systems</span>

      <h1>Publications</h1>

      <div class="subtitle">
        Scholarly work in hardware-aware AI, RF signal intelligence, edge computing, and VLSI systems
      </div>

      <p>
        My publications focus on resource-efficient signal processing, lightweight machine learning,
        hardware-aware neural networks, custom activation functions, adversarial resilience, and
        VLSI-oriented computing systems. The work emphasizes practical deployment on constrained
        platforms and the connection between algorithms and hardware implementation.
      </p>

      <div class="badges">
        <span class="badge">Hardware-Aware AI</span>
        <span class="badge">RF Modulation Classification</span>
        <span class="badge">Custom Activations</span>
        <span class="badge">VLSI Systems</span>
      </div>

      <div class="hero-links">
        <a class="btn-link" href="https://scholar.google.com/citations?user=08fgpdIAAAAJ" target="_blank" rel="noopener">Google Scholar</a>
        <a class="btn-link secondary" href="/resume/">Resume</a>
        <a class="btn-link secondary" href="/insys-lab/">INSys Lab</a>
        <a class="btn-link secondary" href="/about/">About</a>
      </div>
    </div>
  </div>

  <div class="impact-grid">
    <div class="impact-card">
      <div class="big">RF</div>
      <div class="label">Signal Classification</div>
      <div class="small">Envelope, CAF, STFT, PDE</div>
    </div>

    <div class="impact-card">
      <div class="big">AI</div>
      <div class="label">Efficient Learning</div>
      <div class="small">Low-power neural models</div>
    </div>

    <div class="impact-card">
      <div class="big">VLSI</div>
      <div class="label">Hardware Design</div>
      <div class="small">RTL, physical design, acceleration</div>
    </div>

    <div class="impact-card">
      <div class="big">Edge</div>
      <div class="label">Deployment Focus</div>
      <div class="small">Resource-constrained systems</div>
    </div>
  </div>

  <div class="grid-3">
    <div class="focus-card">
      <div class="focus-icon">📡</div>
      <h3>RF Signal Intelligence</h3>
      <p>
        Publications on modulation classification, envelope statistics, cyclostationary features,
        and signal-processing methods for communication systems.
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
        Work related to hardware acceleration, physical design, SoC-aware computation,
        and efficient embedded intelligence.
      </p>
    </div>
  </div>

  <div class="section">
    <h2>🏆 Featured Publications</h2>
    <div class="divider"></div>

    <div class="publication-card">
      <div class="pub-top">
        <span class="pub-year">2026</span>
        <span class="pub-type">Conference</span>
        <span class="pub-award">Accepted</span>
      </div>
      <div class="pub-title">
        Re-Defining R: Resource-Efficient Modulation Classification Using Bin-Based Envelope Features
      </div>
      <div class="pub-authors">
        Srinivas Rahul Sapireddy and collaborators
      </div>
      <div class="pub-venue">
        IEEE SoutheastCon, 2026.
      </div>
    </div>

    <div class="publication-card">
      <div class="pub-top">
        <span class="pub-year">2025</span>
        <span class="pub-type">Conference</span>
        <span class="pub-award">Best Paper Award</span>
      </div>
      <div class="pub-title">
        Re-Visiting R: Statistical Envelope Analysis for Lightweight RF Signal Classification
      </div>
      <div class="pub-authors">
        Srinivas Rahul Sapireddy and collaborators
      </div>
      <div class="pub-venue">
        IEEE International Conference on Radio Frequency Communication and Networks, RFCoN, 2025.
      </div>
    </div>

    <div class="publication-card">
      <div class="pub-top">
        <span class="pub-year">2025</span>
        <span class="pub-type">Conference</span>
      </div>
      <div class="pub-title">
        Hardware-Efficient Custom Activation Functions for LSTM Networks
      </div>
      <div class="pub-authors">
        Srinivas Rahul Sapireddy and collaborators
      </div>
      <div class="pub-venue">
        ACM Great Lakes Symposium on VLSI, GLSVLSI, 2025.
      </div>
    </div>
  </div>

  <div class="grid-2">
    <div class="section">
      <h2>📡 RF Signal Processing and Communication Systems</h2>
      <div class="divider"></div>

      <div class="publication-card">
        <div class="pub-top">
          <span class="pub-year">2026</span>
          <span class="pub-type">IEEE Conference</span>
        </div>
        <div class="pub-title">
          Re-Defining R: Resource-Efficient Modulation Classification Using Bin-Based Envelope Features
        </div>
        <div class="pub-venue">
          IEEE SoutheastCon, 2026.
        </div>
      </div>

      <div class="publication-card">
        <div class="pub-top">
          <span class="pub-year">2025</span>
          <span class="pub-type">IEEE Conference</span>
          <span class="pub-award">Best Paper</span>
        </div>
        <div class="pub-title">
          Re-Visiting R: Statistical Envelope Analysis for Lightweight RF Signal Classification
        </div>
        <div class="pub-venue">
          IEEE RFCoN, 2025.
        </div>
      </div>

      <div class="publication-card">
        <div class="pub-top">
          <span class="pub-year">2025</span>
          <span class="pub-type">IEEE Conference</span>
        </div>
        <div class="pub-title">
          C/N0 Analysis-Based GPS Spoofing Detection with Variable Antenna Orientations
        </div>
        <div class="pub-venue">
          IEEE CARS, 2025.
        </div>
      </div>
    </div>

    <div class="section">
      <h2>🧠 Hardware-Aware AI and Neural Networks</h2>
      <div class="divider"></div>

      <div class="publication-card">
        <div class="pub-top">
          <span class="pub-year">2025</span>
          <span class="pub-type">ACM Conference</span>
        </div>
        <div class="pub-title">
          On the Effectiveness of Custom Activation Functions on Long-Term Short-Term Memory
        </div>
        <div class="pub-venue">
          ACM GLSVLSI, 2025.
        </div>
      </div>

      <div class="publication-card">
        <div class="pub-top">
          <span class="pub-year">2025</span>
          <span class="pub-type">Journal</span>
        </div>
        <div class="pub-title">
          Simplifying Activations with Linear Approximations in Neural Networks
        </div>
        <div class="pub-venue">
          Memories - Materials, Devices, Circuits and Systems, 2025.
        </div>
      </div>

      <div class="publication-card">
        <div class="pub-top">
          <span class="pub-year">2025</span>
          <span class="pub-type">Conference</span>
        </div>
        <div class="pub-title">
          Adversarial-Resilient RF Fingerprinting: A CNN-GAN Framework for Rogue Transmitter Detection
        </div>
        <div class="pub-venue">
          ICMLA, 2025.
        </div>
      </div>
    </div>
  </div>

  <div class="grid-2">
    <div class="section">
      <h2>⚙️ VLSI, Circuits, and Hardware Systems</h2>
      <div class="divider"></div>

      <div class="publication-card">
        <div class="pub-top">
          <span class="pub-year">2024</span>
          <span class="pub-type">Journal</span>
        </div>
        <div class="pub-title">
          Piecewise Linear Approximation of Activation Functions for Neural Networks
        </div>
        <div class="pub-venue">
          Memories - Materials, Devices, Circuits and Systems, 2024.
        </div>
      </div>

      <div class="publication-card">
        <div class="pub-top">
          <span class="pub-year">2024</span>
          <span class="pub-type">Journal</span>
        </div>
        <div class="pub-title">
          A Review of Crosstalk-Based Polymorphic Circuit Design
        </div>
        <div class="pub-venue">
          Memories - Materials, Devices, Circuits and Systems, 2024.
        </div>
      </div>
    </div>

    <div class="section">
      <h2>🛡️ Security, IoT, and Applied AI</h2>
      <div class="divider"></div>

      <div class="publication-card">
        <div class="pub-top">
          <span class="pub-year">2025</span>
          <span class="pub-type">Journal</span>
        </div>
        <div class="pub-title">
          Early Detection of Adversarial Examples in Internet-of-Things Networks
        </div>
        <div class="pub-venue">
          Electronics, 2025.
        </div>
      </div>

      <div class="publication-card">
        <div class="pub-top">
          <span class="pub-year">2025</span>
          <span class="pub-type">Conference</span>
        </div>
        <div class="pub-title">
          Adversarial-Resilient RF Fingerprinting: A CNN-GAN Framework for Rogue Transmitter Detection
        </div>
        <div class="pub-venue">
          ICMLA, 2025.
        </div>
      </div>
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
      <span class="tag">Hardware-Aware AI</span>
      <span class="tag">Custom Activation Functions</span>
      <span class="tag">LSTM Optimization</span>
      <span class="tag">Edge AI</span>
      <span class="tag">VLSI Design</span>
      <span class="tag">IoT Security</span>
      <span class="tag">RF Fingerprinting</span>
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
          <div class="timeline-text">Resource-efficient modulation classification using bin-based envelope features.</div>
        </div>

        <div class="timeline-item">
          <div class="timeline-year">2025</div>
          <div class="timeline-title">RF, AI, Security, and VLSI Publications</div>
          <div class="timeline-text">Work across RFCoN, GLSVLSI, ICMLA, CARS, Electronics, and related venues.</div>
        </div>

        <div class="timeline-item">
          <div class="timeline-year">2024</div>
          <div class="timeline-title">Activation Functions and Circuit Design</div>
          <div class="timeline-text">Journal work on piecewise activation approximation and polymorphic circuit design.</div>
        </div>
      </div>
    </div>

    <div class="section">
      <h2>🌐 Publication Profiles</h2>
      <div class="divider"></div>

      <p>
        For citation details, publication metadata, and updated indexing information, please visit my public scholarly profiles.
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
