---
title: ""
subtitle: "Intelligent Neural & Signal Systems Laboratory"
layout: single
permalink: /insys-lab/
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

@keyframes slideTrack {
  from {
    transform: translateX(0);
  }
  to {
    transform: translateX(-50%);
  }
}

.insys-wrap {
  animation: fadeInUp 0.8s ease-in-out;
}

/* Hero */
.insys-hero {
  position: relative;
  overflow: hidden;
  border-radius: var(--radius);
  padding: 2.25rem 2rem;
  margin-bottom: 1.35rem;
  background:
    radial-gradient(circle at top right, rgba(220,20,60,0.13), transparent 32%),
    linear-gradient(135deg, #e9f3ff 0%, #ffffff 62%);
  border: 1px solid rgba(26,115,232,0.25);
  box-shadow: var(--shadow);
}

.insys-hero::before {
  content: "";
  position: absolute;
  inset: 0;
  background-image:
    linear-gradient(rgba(26,115,232,0.06) 1px, transparent 1px),
    linear-gradient(90deg, rgba(26,115,232,0.06) 1px, transparent 1px);
  background-size: 34px 34px;
  pointer-events: none;
}

.insys-hero-content {
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

.insys-hero h1 {
  margin: 0;
  font-size: 2.15rem;
  line-height: 1.15;
  color: var(--text);
}

.insys-hero .subtitle {
  margin-top: 0.55rem;
  color: #202124;
  font-size: 1.08rem;
  font-weight: 650;
}

.insys-hero p {
  margin: 0.8rem 0 0 0;
  color: var(--muted);
  font-size: 1.03rem;
  line-height: 1.65;
  max-width: 88ch;
}

/* Hero badges */
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

/* Sliding research bar */
.sliding-bar {
  overflow: hidden;
  border-radius: 16px;
  border: 1px solid rgba(26,115,232,0.18);
  background: #ffffff;
  box-shadow: var(--shadow2);
  margin-bottom: 1.3rem;
}

.slide-track {
  display: flex;
  width: max-content;
  animation: slideTrack 28s linear infinite;
}

.sliding-bar:hover .slide-track {
  animation-play-state: paused;
}

.slide-item {
  display: inline-flex;
  align-items: center;
  gap: 0.4rem;
  padding: 0.75rem 1.2rem;
  color: var(--text);
  font-weight: 900;
  white-space: nowrap;
  border-right: 1px solid rgba(26,115,232,0.10);
}

.slide-item span {
  color: var(--isu);
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

/* General section */
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

  .insys-hero {
    padding: 1.5rem 1.1rem;
  }

  .insys-hero h1 {
    font-size: 1.65rem;
  }
}

/* Research cards */
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

/* Methodology timeline */
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

.timeline-step {
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

/* Callout */
.callout {
  border-radius: 16px;
  padding: 1.2rem 1.25rem;
  background: linear-gradient(135deg, #f7fbff 0%, #ffffff 100%);
  border: 1px solid rgba(26,115,232,0.18);
  box-shadow: var(--shadow2);
}

.callout strong {
  color: var(--text);
}

/* Scoped links */
.section a,
.insys-hero a {
  color: var(--blue);
  font-weight: 800;
  text-decoration: none;
}

.section a:hover,
.insys-hero a:hover {
  text-decoration: underline;
}
</style>

<div class="insys-wrap">

  <div class="insys-hero">
    <div class="insys-hero-content">
      <span class="hero-kicker">Intelligent Neural &amp; Signal Systems Laboratory</span>

      <h1>INSys Lab</h1>

      <div class="subtitle">
        Intelligent signal systems, hardware-aware machine learning, and low-power edge intelligence
      </div>

      <p>
        The Intelligent Neural &amp; Signal Systems Laboratory develops efficient, interpretable, and hardware-aware methods
        for intelligent signal processing and edge computing under strict power, latency, and memory constraints.
      </p>

      <div class="badges">
        <span class="badge">RF Signal Intelligence</span>
        <span class="badge">Hardware-Aware ML</span>
        <span class="badge">Edge AI Systems</span>
        <span class="badge">Efficiency and Interpretability</span>
      </div>

      <div class="hero-links">
        <a class="btn-link" href="/publications/">Publications</a>
        <a class="btn-link secondary" href="/scholars/">Scholars</a>
        <a class="btn-link secondary" href="/resume/">Resume</a>
        <a class="btn-link secondary" href="mailto:ssapire@illinoisstate.edu">Contact</a>
      </div>
    </div>
  </div>

  <div class="sliding-bar">
    <div class="slide-track">
      <div class="slide-item"><span>●</span> RF Signal Intelligence</div>
      <div class="slide-item"><span>●</span> Hardware-Aware ML</div>
      <div class="slide-item"><span>●</span> Edge AI Systems</div>
      <div class="slide-item"><span>●</span> Interpretable Learning</div>
      <div class="slide-item"><span>●</span> VLSI-Aware Computing</div>
      <div class="slide-item"><span>●</span> Low-Power Signal Processing</div>
      <div class="slide-item"><span>●</span> Embedded Intelligence</div>

      <div class="slide-item"><span>●</span> RF Signal Intelligence</div>
      <div class="slide-item"><span>●</span> Hardware-Aware ML</div>
      <div class="slide-item"><span>●</span> Edge AI Systems</div>
      <div class="slide-item"><span>●</span> Interpretable Learning</div>
      <div class="slide-item"><span>●</span> VLSI-Aware Computing</div>
      <div class="slide-item"><span>●</span> Low-Power Signal Processing</div>
      <div class="slide-item"><span>●</span> Embedded Intelligence</div>
    </div>
  </div>

  <div class="impact-grid">
    <div class="impact-card">
      <div class="big">RF</div>
      <div class="label">Signal Intelligence</div>
      <div class="small">Classification, sensing, and feature extraction</div>
    </div>

    <div class="impact-card">
      <div class="big">AI</div>
      <div class="label">Hardware-Aware ML</div>
      <div class="small">Efficient models for constrained systems</div>
    </div>

    <div class="impact-card">
      <div class="big">Edge</div>
      <div class="label">Low-Power Computing</div>
      <div class="small">Latency, memory, and power-aware design</div>
    </div>

    <div class="impact-card">
      <div class="big">VLSI</div>
      <div class="label">System Awareness</div>
      <div class="small">Algorithm-to-hardware perspective</div>
    </div>
  </div>

  <div class="section">
    <h2>🔎 Lab Overview</h2>
    <div class="divider"></div>

    <p>
      INSys Lab adopts a systems-level research perspective that spans algorithm design, evaluation methodology,
      and deployment-aware considerations. The lab emphasizes methods that are not only accurate, but also practical
      for embedded, edge, and cyber-physical platforms.
    </p>

    <div class="tag-cloud">
      <span class="tag">Signal Processing</span>
      <span class="tag">Machine Learning</span>
      <span class="tag">RF Systems</span>
      <span class="tag">Edge Computing</span>
      <span class="tag">Hardware-Aware Evaluation</span>
      <span class="tag">Resource-Constrained AI</span>
    </div>
  </div>

  <div class="grid-3">
    <div class="focus-card">
      <div class="focus-icon">📡</div>
      <h3>RF Signal Intelligence</h3>
      <p>
        Intelligent RF signal analysis, modulation classification, statistical feature extraction,
        and interpretable signal-domain learning.
      </p>
    </div>

    <div class="focus-card">
      <div class="focus-icon">🧠</div>
      <h3>Efficient Learning Models</h3>
      <p>
        Lightweight and hardware-aware neural, statistical, and hybrid learning models for deployment-aware AI systems.
      </p>
    </div>

    <div class="focus-card">
      <div class="focus-icon">⚙️</div>
      <h3>Edge and Hardware Systems</h3>
      <p>
        Evaluation workflows for runtime, memory, power, and latency across embedded and edge-computing platforms.
      </p>
    </div>
  </div>

  <div class="grid-2">
    <div class="section">
      <h2>🔬 Research Focus</h2>
      <div class="divider"></div>
      <ul>
        <li>Intelligent RF signal analysis and modulation classification</li>
        <li>Lightweight and hardware-aware neural and statistical learning models</li>
        <li>Signal-domain feature extraction and interpretable learning frameworks</li>
        <li>Edge intelligence for embedded and resource-constrained systems</li>
        <li>Robust and trustworthy intelligent signal processing architectures</li>
      </ul>
    </div>

    <div class="section">
      <h2>🛠️ Tools and Platforms</h2>
      <div class="divider"></div>
      <ul>
        <li>Python and MATLAB for signal analysis and algorithm development</li>
        <li>RF signal simulation and statistical feature extraction pipelines</li>
        <li>Embedded and edge AI development environments</li>
        <li>Hardware-aware evaluation workflows for runtime and resource analysis</li>
      </ul>
    </div>
  </div>

  <div class="grid-2">
    <div class="section">
      <h2>🧭 Research Methodology</h2>
      <div class="divider"></div>

      <div class="timeline">
        <div class="timeline-item">
          <div class="timeline-step">Step 1</div>
          <div class="timeline-title">Signal Capture and Modeling</div>
          <div class="timeline-text">
            Model, simulate, or collect signal data relevant to communication, sensing, and edge-intelligent systems.
          </div>
        </div>

        <div class="timeline-item">
          <div class="timeline-step">Step 2</div>
          <div class="timeline-title">Feature Engineering</div>
          <div class="timeline-text">
            Extract signal-domain, statistical, time-frequency, and interpretable features from raw or processed data.
          </div>
        </div>

        <div class="timeline-item">
          <div class="timeline-step">Step 3</div>
          <div class="timeline-title">Efficient Learning</div>
          <div class="timeline-text">
            Develop lightweight learning models and hardware-aware classification pipelines.
          </div>
        </div>

        <div class="timeline-item">
          <div class="timeline-step">Step 4</div>
          <div class="timeline-title">Deployment-Aware Evaluation</div>
          <div class="timeline-text">
            Evaluate accuracy, runtime, memory, power, latency, and system feasibility.
          </div>
        </div>
      </div>
    </div>

    <div class="section">
      <h2>📌 Research Philosophy</h2>
      <div class="divider"></div>

      <p>
        INSys Lab emphasizes principled and deployment-conscious research methodologies. Rather than relying exclusively
        on large or opaque models, the lab prioritizes approaches that balance performance, efficiency, and interpretability.
      </p>

      <ul>
        <li>Integrating signal processing insights with learning-based models</li>
        <li>Designing algorithms with explicit consideration of hardware constraints</li>
        <li>Evaluating methods using accuracy, runtime, memory, and power metrics</li>
        <li>Bridging theoretical foundations with system-level validation</li>
      </ul>
    </div>
  </div>

  <div class="grid-2">
    <div class="section">
      <h2>👨‍🎓 Student Involvement and Mentoring</h2>
      <div class="divider"></div>

      <p>
        INSys Lab provides hands-on research opportunities for undergraduate and graduate students through independent study,
        senior design projects, and directed research.
      </p>

      <div class="callout">
        <strong>Student pathways:</strong> signal processing projects, RF simulation, efficient machine learning,
        hardware-aware model evaluation, technical writing, and publication-oriented research.
      </div>

      <p>
        Details of current and previously mentored students are available on the <a href="/scholars/">Scholars</a> page.
      </p>
    </div>

    <div class="section">
      <h2>📚 Scholarly Output</h2>
      <div class="divider"></div>

      <p>
        Research conducted within INSys Lab contributes to peer-reviewed journal articles, conference publications,
        and technical reports in signal processing, machine learning, RF systems, and hardware-aware computing.
      </p>

      <div class="callout">
        <strong>Output areas:</strong> RF classification, envelope statistics, efficient AI, custom activations,
        edge systems, and hardware-conscious evaluation.
      </div>

      <p>
        A complete list of publications is available on the <a href="/publications/">Publications</a> page.
      </p>
    </div>
  </div>

  <div class="section">
    <h2>🤝 Collaboration and Engagement</h2>
    <div class="divider"></div>

    <p>
      INSys Lab welcomes collaboration with academic researchers, industry partners, and government laboratories interested
      in intelligent signal systems, RF analysis, and edge computing. Collaborative activities may include joint research projects,
      co-supervised students, prototype development, proposal preparation, or exploratory system-level studies.
    </p>

    <div class="tag-cloud">
      <span class="tag">Academic Collaboration</span>
      <span class="tag">Industry Engagement</span>
      <span class="tag">Student Research</span>
      <span class="tag">Proposal Development</span>
      <span class="tag">Prototype Studies</span>
      <span class="tag">System-Level Evaluation</span>
    </div>
  </div>

  <div class="grid-2">
    <div class="section">
      <h2>🚧 Lab Status</h2>
      <div class="divider"></div>

      <p>
        INSys Lab is currently in its establishment phase. Research activities are conducted through simulation-driven workflows
        and prototype-based experimentation, with laboratory infrastructure development ongoing.
      </p>
    </div>

    <div class="section">
      <h2>📬 Contact</h2>
      <div class="divider"></div>

      <p>
        Prospective students and collaborators are encouraged to reach out by email to discuss research interests,
        project ideas, or collaboration opportunities.
      </p>

      <div class="hero-links">
        <a class="btn-link" href="mailto:ssapire@illinoisstate.edu">Email</a>
        <a class="btn-link secondary" href="/publications/">Publications</a>
        <a class="btn-link secondary" href="/scholars/">Scholars</a>
      </div>
    </div>
  </div>


  </div>

</div>
