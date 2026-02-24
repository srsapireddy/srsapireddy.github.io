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
  --bg: #ffffff;
  --muted: #5f6368;
  --hover: #e9f3ff;
  --shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
  --shadow2: 0 2px 10px rgba(0, 0, 0, 0.05);
  --radius: 16px;
  --radius2: 12px;
}

/* Hero */
.insys-hero {
  border-radius: var(--radius);
  padding: 2rem 1.8rem;
  margin-bottom: 1.8rem;
  background: linear-gradient(135deg, #e9f3ff 0%, #ffffff 60%);
  border: 1px solid rgba(26,115,232,0.25);
  box-shadow: var(--shadow);
}

.insys-hero h2 {
  margin: 0 0 0.4rem 0;
  font-size: 1.9rem;
  line-height: 1.2;
  color: #0b1f44;
}

.insys-hero p {
  margin: 0.5rem 0 1rem 0;
  color: var(--muted);
  font-size: 1.05rem;
  max-width: 70ch;
}

/* Badges */
.badges {
  display: flex;
  flex-wrap: wrap;
  gap: 0.55rem;
  margin-top: 0.8rem;
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
}

/* Buttons */
.hero-links {
  display: flex;
  flex-wrap: wrap;
  gap: 0.7rem;
  margin-top: 1rem;
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
  font-weight: 600;
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
.about-section {
  border: 1px solid rgba(26,115,232,0.18);
  background: var(--bg);
  padding: 1.35rem 1.5rem;
  margin-bottom: 1.3rem;
  border-radius: var(--radius2);
  box-shadow: var(--shadow2);
  transition: 0.25s ease-in-out;
}

.about-section:hover {
  background: #fbfdff;
  transform: translateY(-2px);
  box-shadow: var(--shadow);
}

.about-section h3 {
  margin-top: 0;
  color: #0b1f44;
  font-size: 1.15rem;
  display: flex;
  align-items: center;
  gap: 0.55rem;
}

.about-section p {
  color: #202124;
}

.about-section ul {
  padding-left: 1.2rem;
  margin-bottom: 0.4rem;
}

.about-section li {
  margin-bottom: 0.4rem;
}

/* Scoped links */
.about-section a {
  color: var(--blue);
  font-weight: 600;
  text-decoration: none;
}
.about-section a:hover { text-decoration: underline; }

/* Grid */
.grid-2 {
  display: grid;
  grid-template-columns: 1fr;
  gap: 1.3rem;
}

@media (min-width: 900px) {
  .grid-2 {
    grid-template-columns: 1fr 1fr;
  }
}

/* Subtle divider */
.divider {
  height: 1px;
  background: rgba(26,115,232,0.12);
  margin: 0.3rem 0 0.8rem 0;
}
</style>

<div class="insys-hero">
  <h2>INSys Lab</h2>
  <p>
    The Intelligent Neural &amp; Signal Systems Laboratory (INSys Lab) develops efficient, interpretable, and hardware-aware methods for
    intelligent signal processing and edge computing under strict power, latency, and memory constraints.
  </p>

  <div class="badges">
    <span class="badge">RF Signal Intelligence</span>
    <span class="badge">Hardware-Aware ML</span>
    <span class="badge">Edge AI Systems</span>
    <span class="badge">Efficiency &amp; Interpretability</span>
  </div>

  <div class="hero-links">
    <a class="btn-link" href="/publications/">Publications</a>
    <a class="btn-link secondary" href="/scholars/">Scholars</a>
    <a class="btn-link secondary" href="/contact/">Contact</a>
  </div>
</div>

<div class="about-section">
  <h3>Overview</h3>
  <div class="divider"></div>
  <p>
    INSys Lab adopts a systems-level research perspective that spans algorithm design, evaluation methodology, and deployment-aware considerations.
    The lab’s research emphasizes approaches that are not only accurate, but also practical for embedded, edge, and cyber-physical platforms.
  </p>
</div>

<div class="grid-2">
  <div class="about-section">
    <h3>Research Focus</h3>
    <div class="divider"></div>
    <ul>
      <li>Intelligent RF signal analysis and modulation classification</li>
      <li>Lightweight and hardware-aware neural and statistical learning models</li>
      <li>Signal-domain feature extraction and interpretable learning frameworks</li>
      <li>Edge intelligence for embedded and resource-constrained systems</li>
      <li>Robust and trustworthy intelligent signal processing architectures</li>
    </ul>
  </div>

  <div class="about-section">
    <h3>Tools and Platforms</h3>
    <div class="divider"></div>
    <ul>
      <li>Python and MATLAB for signal analysis and algorithm development</li>
      <li>RF signal simulation and statistical feature extraction pipelines</li>
      <li>Embedded and edge AI development environments</li>
      <li>Hardware-aware evaluation workflows for runtime and resource analysis</li>
    </ul>
  </div>
</div>

<div class="about-section">
  <h3>Research Philosophy and Methodology</h3>
  <div class="divider"></div>
  <p>
    INSys Lab emphasizes principled and deployment-conscious research methodologies. Rather than relying exclusively on large or opaque models,
    the lab prioritizes approaches that balance performance, efficiency, and interpretability.
  </p>
  <ul>
    <li>Integrating signal processing insights with learning-based models</li>
    <li>Designing algorithms with explicit consideration of hardware constraints</li>
    <li>Evaluating methods using accuracy, runtime, memory, and power metrics</li>
    <li>Bridging theoretical foundations with system-level validation</li>
  </ul>
</div>

<div class="grid-2">
  <div class="about-section">
    <h3>Student Involvement and Mentoring</h3>
    <div class="divider"></div>
    <p>
      INSys Lab provides hands-on research opportunities for undergraduate and graduate students through independent study,
      senior design projects, and directed research.
    </p>
    <p>
      Details of current and previously mentored students are available on the <a href="/scholars/">Scholars</a> page.
    </p>
  </div>

  <div class="about-section">
    <h3>Scholarly Output</h3>
    <div class="divider"></div>
    <p>
      Research conducted within INSys Lab contributes to peer-reviewed journal articles, conference publications, and technical reports
      in signal processing, machine learning, and hardware-aware systems.
    </p>
    <p>
      A complete list of publications is available on the <a href="/publications/">Publications</a> page.
    </p>
  </div>
</div>

<div class="about-section">
  <h3>Collaboration and Engagement</h3>
  <div class="divider"></div>
  <p>
    INSys Lab welcomes collaboration with academic researchers, industry partners, and government laboratories interested in intelligent signal systems,
    RF analysis, and edge computing. Collaborative activities may include joint research projects, co-supervised students, or exploratory system-level studies.
  </p>
</div>

<div class="grid-2">
  <div class="about-section">
    <h3>Lab Status</h3>
    <div class="divider"></div>
    <p>
      INSys Lab is currently in its establishment phase. Research activities are conducted through simulation-driven workflows and prototype-based
      experimentation, with laboratory infrastructure development ongoing.
    </p>
  </div>

  <div class="about-section">
    <h3>Contact</h3>
    <div class="divider"></div>
    <p>
      Prospective students and collaborators are encouraged to reach out via email.
    </p>
  </div>
</div>

<div class="about-section">
  <h3>Institutional Affiliation</h3>
  <div class="divider"></div>
  <p>
    INSys Lab is a faculty-led research group within the Department of Electrical Engineering at Illinois State University.
  </p>
</div>
