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
  --bg: #ffffff;
  --muted: #5f6368;
  --shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
  --shadow2: 0 2px 10px rgba(0, 0, 0, 0.05);
  --radius: 16px;
  --radius2: 12px;
}

/* Hero */
.page-hero {
  border-radius: var(--radius);
  padding: 2rem 1.8rem;
  margin-bottom: 1.6rem;
  background: linear-gradient(135deg, #e9f3ff 0%, #ffffff 60%);
  border: 1px solid rgba(26,115,232,0.25);
  box-shadow: var(--shadow);
}
.page-hero h2 {
  margin: 0 0 0.4rem 0;
  font-size: 1.9rem;
  line-height: 1.2;
  color: #0b1f44;
}
.page-hero p {
  margin: 0.5rem 0 0 0;
  color: var(--muted);
  font-size: 1.05rem;
  max-width: 80ch;
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
  padding: 0.35rem 0.7rem;
  border-radius: 999px;
  background: #ffffff;
  border: 1px solid rgba(26,115,232,0.22);
  box-shadow: var(--shadow2);
  font-size: 0.92rem;
  color: #0b1f44;
  font-weight: 600;
}

/* Buttons */
.hero-links {
  display: flex;
  flex-wrap: wrap;
  gap: 0.7rem;
  margin-top: 1.1rem;
}
.btn-link {
  display: inline-flex;
  align-items: center;
  gap: 0.45rem;
  padding: 0.55rem 0.9rem;
  border-radius: 10px;
  background: var(--blue);
  color: #ffffff !important;
  text-decoration: none !important;
  font-weight: 700;
  box-shadow: var(--shadow2);
  transition: 0.2s ease-in-out;
}
.btn-link:hover {
  background: var(--blue2);
  transform: translateY(-1px);
}
.btn-link.secondary {
  background: #ffffff;
  color: var(--blue) !important;
  border: 1px solid rgba(26,115,232,0.25);
}

/* Cards */
.section {
  border: 1px solid rgba(26,115,232,0.18);
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
.section h3 {
  margin-top: 0;
  color: #0b1f44;
  font-size: 1.15rem;
  display: flex;
  align-items: center;
  gap: 0.55rem;
}
.section p { color: #202124; }
.section ul { padding-left: 1.2rem; margin-bottom: 0.4rem; }
.section li { margin-bottom: 0.4rem; }

/* Scoped links */
.section a, .page-hero a {
  color: var(--blue);
  font-weight: 700;
  text-decoration: none;
}
.section a:hover, .page-hero a:hover { text-decoration: underline; }

/* Divider */
.divider { height: 1px; background: rgba(26,115,232,0.12); margin: 0.3rem 0 0.9rem 0; }

/* Grid */
.grid-2 { display: grid; grid-template-columns: 1fr; gap: 1.3rem; }
@media (min-width: 900px) { .grid-2 { grid-template-columns: 1fr 1fr; } }
</style>

<div class="page-hero">
  <h2>Srinivas Rahul Sapireddy, Ph.D.</h2>
  <p>
    Assistant Professor, College of Engineering, Illinois State University (ISU). My research focuses on low-power, hardware-aware artificial intelligence,
    RF signal classification, and VLSI design, with an emphasis on edge-intelligent systems.
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
  </div>
</div>

<div class="grid-2">
  <div class="section">
    <h3>👤 About Me</h3>
    <div class="divider"></div>
    <p>
      I integrate signal processing, lightweight machine learning, and hardware-efficient architectures to enable accurate and energy-efficient computation
      in resource-constrained environments.
    </p>
    <p>
      My teaching includes Logic Design and Engineering Computation, with prior instructional experience in ASIC Physical Design and Analog IC Design.
    </p>
  </div>

  <div class="section">
    <h3>🧭 Open to Collaboration</h3>
    <div class="divider"></div>
    <p>
      I welcome research collaborations in efficient edge AI, signal intelligence, and hardware–software co-design.
      I am also interested in mentoring students and engaging in interdisciplinary research discussions.
    </p>
  </div>
</div>

<div class="section">
  <h3>🔬 Research and Technical Focus</h3>
  <div class="divider"></div>
  <ul>
    <li>Hardware-aware and low-power machine learning for edge-intelligent systems</li>
    <li>RF signal and modulation classification using time-frequency and statistical feature analysis</li>
    <li>Design of hardware-efficient neural networks, including custom and piecewise-linear activation functions</li>
    <li>VLSI system design and physical implementation, including RTL-to-GDSII flow and timing analysis</li>
    <li>Embedded AI accelerators and system-on-chip (SoC) architectures</li>
  </ul>
  <p>
    Prior experience includes research and development roles at the Missouri Institute of Defense and Energy and industry experience as an
    AI Intern at SmartBridge Pvt. Ltd.
  </p>
</div>

<div class="grid-2">
  <div class="section">
    <h3>📚 Selected Publications</h3>
    <div class="divider"></div>
    <ul>
      <li>IEEE SoutheastCon, Alabama, USA, 2026 (accepted): <em>Bin-Based R-Value Statistical Envelope Analysis for RF Modulation Classification</em></li>
      <li>ACM GLSVLSI, New Orleans, USA, 2025: <em>Hardware-Efficient Custom Activation Functions for LSTM Networks</em></li>
      <li>IEEE RFCoN, 2025: <em>Statistical Envelope Analysis for Lightweight RF Signal Classification</em></li>
      <li>MDPI Electronics, 2025: <em>Early Detection of Adversarial Examples in Internet-of-Things Networks</em></li>
      <li>MDPI Memories, 2024: <em>Piecewise Linear Approximations of Activation Functions for Neural Networks</em></li>
    </ul>
    <p><a href="/publications/">View complete list of publications</a></p>
  </div>

  <div class="section">
    <h3>🏆 Awards and Recognitions</h3>
    <div class="divider"></div>
    <ul>
      <li>Best Paper Award, IEEE RFCoN 2025 (Track 2, Session II)</li>
      <li>Dean’s International Scholar Award, University of Missouri–Kansas City</li>
      <li>IEEE–Eta Kappa Nu (HKN) Honor Society Membership</li>
      <li>CS Balaji Memorial Travel Grant, 2025</li>
      <li>Second Place, Hack-A-Roo Fall 2022 (Entrepreneur Track)</li>
      <li>Third Place, Hack-A-Roo Fall 2021 (CS/IT Track)</li>
    </ul>
  </div>
</div>

<div class="section">
  <h3>🧰 Professional Development and Technical Expertise</h3>
  <div class="divider"></div>
  <ul>
    <li>Professional training in product management and technology commercialization (CII)</li>
    <li>Advanced training in artificial intelligence and MLOps (Duke University, CDAC)</li>
    <li>Statistical learning and machine learning foundations (Stanford University)</li>
    <li>Mathematics for machine learning (Imperial College London)</li>
  </ul>
  <p>
    Technical expertise includes hardware design and analysis using Verilog, Yosys, and OpenSTA,
    as well as machine learning development and deployment using PyTorch, TensorFlow Lite,
    Docker, and Scikit-learn.
  </p>
</div>

<div class="section">
  <h3>🔗 Professional Profiles</h3>
  <div class="divider"></div>
  <ul>
    <li>GitHub: <a href="https://github.com/srsapireddy" target="_blank" rel="noopener">github.com/srsapireddy</a></li>
    <li>Google Scholar: <a href="https://scholar.google.com/citations?user=08fgpdIAAAAJ" target="_blank" rel="noopener">Publication Profile</a></li>
    <li>ORCID: <a href="https://orcid.org/0000-0002-9898-6810" target="_blank" rel="noopener">0000-0002-9898-6810</a></li>
    <li>OpenReview: <a href="https://openreview.net/profile?id=~Srinivas_Rahul_Sapireddy1" target="_blank" rel="noopener">Reviewer Profile</a></li>
    <li>Medium: <a href="https://medium.com/@srsapireddy" target="_blank" rel="noopener">Technical Blog</a></li>
  </ul>
</div>
