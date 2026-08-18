---
title: ""
layout: single
permalink: /teaching/
toc: false
---

<style>
:root {
  --blue: #1a73e8;
  --blue2: #0b5bd3;
  --isu: #DC143C;
  --umkc: #0096d6;
  --green: #1a7f3d;
  --bg: #ffffff;
  --soft: #f6f9ff;
  --muted: #5f6368;
  --text: #0b1f44;
  --hover: #e9f3ff;
  --shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
  --shadow2: 0 2px 10px rgba(0, 0, 0, 0.05);
  --radius: 18px;
  --radius2: 14px;
  --border: rgba(26,115,232,0.18);
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

.teaching-wrap {
  animation: fadeInUp 0.85s ease-in-out;
}

/* Hero */
.page-hero {
  position: relative;
  overflow: hidden;
  border-radius: var(--radius);
  padding: 2.25rem 2rem;
  margin-bottom: 1.3rem;
  background:
    radial-gradient(circle at top right, rgba(220,20,60,0.13), transparent 32%),
    linear-gradient(135deg, #e9f3ff 0%, #ffffff 62%);
  border: 1px solid rgba(26,115,232,0.25);
  box-shadow: var(--shadow);
}

.page-hero::before {
  content: "";
  position: absolute;
  inset: 0;
  background-image:
    linear-gradient(rgba(26,115,232,0.06) 1px, transparent 1px),
    linear-gradient(90deg, rgba(26,115,232,0.06) 1px, transparent 1px);
  background-size: 34px 34px;
  pointer-events: none;
}

.hero-content {
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
  margin-bottom: 0.85rem;
}

.page-hero h1 {
  margin: 0;
  font-size: 2.15rem;
  line-height: 1.15;
  color: var(--text);
}

.page-hero p {
  margin: 0.75rem 0 0 0;
  color: var(--muted);
  font-size: 1.04rem;
  line-height: 1.65;
  max-width: 92ch;
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

/* Sliding bar */
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
  animation: slideTrack 32s linear infinite;
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
  font-size: 0.9rem;
  color: var(--text);
  font-weight: 850;
}

.badge.isu {
  border-color: rgba(220,20,60,0.35);
  color: #7a0b1f;
  background: rgba(220,20,60,0.06);
}

.badge.umkc {
  border-color: rgba(0,150,214,0.35);
  color: #065a7d;
  background: rgba(0,150,214,0.06);
}

.badge.plan {
  border-color: rgba(26,127,61,0.28);
  color: var(--green);
  background: rgba(26,127,61,0.06);
}

/* Impact cards */
.impact-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 0.95rem;
  margin-bottom: 1.3rem;
}

.impact-card {
  padding: 1.1rem 1rem;
  border-radius: 16px;
  background: linear-gradient(135deg, #ffffff 0%, #f7fbff 100%);
  border: 1px solid rgba(26,115,232,0.18);
  box-shadow: var(--shadow2);
  text-align: center;
  transition: 0.25s ease-in-out;
}

.impact-card:hover {
  transform: translateY(-3px);
  box-shadow: var(--shadow);
}

.impact-number {
  font-size: 1.6rem;
  font-weight: 950;
  color: var(--isu);
  line-height: 1.1;
}

.impact-label {
  margin-top: 0.35rem;
  font-size: 0.92rem;
  color: var(--text);
  font-weight: 850;
}

.impact-sub {
  margin-top: 0.22rem;
  font-size: 0.82rem;
  color: var(--muted);
}

/* Section */
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
  margin-bottom: 0.42rem;
  line-height: 1.5;
}

.divider {
  height: 1px;
  background: rgba(26,115,232,0.12);
  margin: 0.6rem 0 1rem 0;
}

/* Focus cards */
.focus-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1.1rem;
  margin-bottom: 1.3rem;
}

.focus-card {
  position: relative;
  overflow: hidden;
  padding: 1.25rem;
  border-radius: 16px;
  background: linear-gradient(135deg, #ffffff 0%, #f4f9ff 100%);
  border: 1px solid rgba(26,115,232,0.18);
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

/* Role progression timeline */
.role-timeline {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 0.9rem;
}

.role-card {
  position: relative;
  border-radius: 16px;
  padding: 1rem 1rem;
  background: #ffffff;
  border: 1px solid rgba(26,115,232,0.2);
  box-shadow: var(--shadow2);
  transition: 0.22s ease-in-out;
  overflow: hidden;
}

.role-card:hover {
  transform: translateY(-3px);
  box-shadow: var(--shadow);
}

.role-card::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  height: 5px;
  width: 100%;
}

.role-card.umkc::before {
  background: var(--umkc);
}

.role-card.isu::before {
  background: var(--isu);
}

.role-card strong {
  display: block;
  color: var(--text);
  font-size: 1.02rem;
  line-height: 1.3;
}

.role-card small {
  display: block;
  margin-top: 0.4rem;
  color: var(--muted);
  line-height: 1.4;
}

/* Course tabs */
.course-tabs {
  display: flex;
  flex-wrap: wrap;
  gap: 0.7rem;
  margin-bottom: 1.1rem;
}

.tab-button {
  border: 1px solid rgba(26,115,232,0.22);
  background: #ffffff;
  color: var(--blue);
  padding: 0.62rem 1rem;
  border-radius: 999px;
  cursor: pointer;
  font-weight: 900;
  box-shadow: var(--shadow2);
  transition: 0.2s ease-in-out;
}

.tab-button:hover {
  transform: translateY(-2px);
  background: #f3f8ff;
}

.tab-button.active {
  background: var(--blue);
  color: #ffffff;
  border-color: var(--blue);
}

.tab-panel {
  display: none;
  animation: fadeInUp 0.45s ease-in-out;
}

.tab-panel.active {
  display: block;
}

/* Course cards */
.course-card {
  position: relative;
  overflow: hidden;
  border-radius: 16px;
  padding: 1.15rem 1.2rem;
  margin-bottom: 1rem;
  background: #ffffff;
  border: 1px solid rgba(26,115,232,0.16);
  box-shadow: var(--shadow2);
  transition: 0.22s ease-in-out;
}

.course-card:hover {
  transform: translateY(-3px);
  box-shadow: var(--shadow);
  background: #fbfdff;
}

.course-card::before {
  content: "";
  position: absolute;
  left: 0;
  top: 1rem;
  bottom: 1rem;
  width: 5px;
  border-radius: 999px;
  background: linear-gradient(180deg, var(--blue), var(--isu));
}

.course-card.isu-course::before {
  background: linear-gradient(180deg, var(--isu), var(--blue));
}

.course-card.umkc-course::before {
  background: linear-gradient(180deg, var(--umkc), var(--blue));
}

.course-title {
  margin: 0;
  font-size: 1.08rem;
  font-weight: 950;
  color: var(--text);
  line-height: 1.38;
}

.course-meta {
  margin-top: 0.35rem;
  color: var(--muted);
  font-size: 0.92rem;
}

.course-body {
  margin-top: 0.75rem;
  color: #202124;
  line-height: 1.62;
}

.course-body strong {
  color: var(--text);
}

.course-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.45rem;
  margin-top: 0.75rem;
}

.course-tag {
  display: inline-flex;
  align-items: center;
  padding: 0.3rem 0.62rem;
  border-radius: 999px;
  background: #f3f8ff;
  border: 1px solid rgba(26,115,232,0.18);
  color: var(--blue);
  font-size: 0.84rem;
  font-weight: 850;
}

.course-tag.isu {
  background: rgba(220,20,60,0.06);
  border-color: rgba(220,20,60,0.28);
  color: #7a0b1f;
}

.course-tag.umkc {
  background: rgba(0,150,214,0.06);
  border-color: rgba(0,150,214,0.28);
  color: #065a7d;
}

/* Image */
.course-img {
  width: 100%;
  max-height: 230px;
  object-fit: cover;
  border-radius: 14px;
  box-shadow: var(--shadow2);
  border: 1px solid rgba(26,115,232,0.15);
  cursor: zoom-in;
  transition: 0.22s ease-in-out;
}

.course-img:hover {
  transform: scale(1.01);
  box-shadow: var(--shadow);
}

.course-feature-grid {
  display: grid;
  grid-template-columns: 1.25fr 0.75fr;
  gap: 1.2rem;
  align-items: start;
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
  font-weight: 850;
}

/* Teaching method cards */
.method-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1rem;
}

/* Scoped links */
.section a,
.page-hero a {
  color: var(--blue);
  font-weight: 850;
  text-decoration: none;
}

.section a:hover,
.page-hero a:hover {
  text-decoration: underline;
}

/* Responsive */
@media (max-width: 1050px) {
  .role-timeline,
  .method-grid {
    grid-template-columns: repeat(2, 1fr);
  }

  .course-feature-grid {
    grid-template-columns: 1fr;
  }
}

@media (max-width: 950px) {
  .impact-grid,
  .focus-grid {
    grid-template-columns: 1fr 1fr;
  }
}

@media (max-width: 700px) {
  .page-hero {
    padding: 1.5rem 1.1rem;
  }

  .page-hero h1 {
    font-size: 1.65rem;
  }

  .impact-grid,
  .focus-grid,
  .role-timeline,
  .method-grid {
    grid-template-columns: 1fr;
  }
}
</style>

<div class="teaching-wrap">

  <div class="page-hero">
    <div class="hero-content">
      <span class="hero-kicker">Teaching Portfolio · Engineering Education · Hands-On Learning</span>

      <h1>Teaching &amp; Instruction</h1>

      <p>
        My teaching emphasizes rigorous foundations, hands-on design practice, and deployment-oriented thinking across
        digital systems, programming, signal processing, communication systems, VLSI, and hardware-aware machine learning.
      </p>

      <div class="badges">
        <span class="badge isu">Illinois State University</span>
        <span class="badge umkc">University of Missouri–Kansas City</span>
        <span class="badge">Logic Design</span>
        <span class="badge">Engineering Computation</span>
        <span class="badge">Signals and Systems</span>
        <span class="badge">VLSI / Physical Design</span>
      </div>

      <div class="hero-links">
        <a class="btn-link" href="/resume/">Resume</a>
        <a class="btn-link secondary" href="/insys-lab/">INSys Lab</a>
        <a class="btn-link secondary" href="/scholars/">Scholars</a>
        <a class="btn-link secondary" href="/publications/">Publications</a>
      </div>
    </div>
  </div>

  <div class="sliding-bar">
    <div class="slide-track">
      <div class="slide-item"><span>●</span> Engineering Computation</div>
      <div class="slide-item"><span>●</span> Logic Design</div>
      <div class="slide-item"><span>●</span> Signals and Systems</div>
      <div class="slide-item"><span>●</span> Communication Systems</div>
      <div class="slide-item"><span>●</span> ASIC Physical Design</div>
      <div class="slide-item"><span>●</span> Analog IC Design</div>
      <div class="slide-item"><span>●</span> VLSI Design</div>
      <div class="slide-item"><span>●</span> Senior Design</div>

      <div class="slide-item"><span>●</span> Engineering Computation</div>
      <div class="slide-item"><span>●</span> Logic Design</div>
      <div class="slide-item"><span>●</span> Signals and Systems</div>
      <div class="slide-item"><span>●</span> Communication Systems</div>
      <div class="slide-item"><span>●</span> ASIC Physical Design</div>
      <div class="slide-item"><span>●</span> Analog IC Design</div>
      <div class="slide-item"><span>●</span> VLSI Design</div>
      <div class="slide-item"><span>●</span> Senior Design</div>
    </div>
  </div>

  <div class="impact-grid">
    <div class="impact-card">
      <div class="impact-number">ISU</div>
      <div class="impact-label">Assistant Professor</div>
      <div class="impact-sub">Spring 2026 - Present</div>
    </div>

    <div class="impact-card">
      <div class="impact-number">UMKC</div>
      <div class="impact-label">Instructor Experience</div>
      <div class="impact-sub">Spring 2023 - Fall 2025</div>
    </div>

    <div class="impact-card">
      <div class="impact-number">VLSI</div>
      <div class="impact-label">Design-Centered Courses</div>
      <div class="impact-sub">ASIC, VLSI, Analog IC</div>
    </div>

    <div class="impact-card">
      <div class="impact-number">Lab</div>
      <div class="impact-label">Hands-On Learning</div>
      <div class="impact-sub">Programming, CAD, circuits, systems</div>
    </div>
  </div>

  <div class="focus-grid">
    <div class="focus-card">
      <div class="focus-icon">🧮</div>
      <h3>Foundational Engineering</h3>
      <p>
        I emphasize strong foundations in computation, probability, signals, logic, and circuit-level thinking.
      </p>
    </div>

    <div class="focus-card">
      <div class="focus-icon">🛠️</div>
      <h3>Hands-On Design</h3>
      <p>
        My courses use programming, Verilog, simulation, CAD tools, and design projects to connect theory to practice.
      </p>
    </div>

    <div class="focus-card">
      <div class="focus-icon">🚀</div>
      <h3>Deployment Mindset</h3>
      <p>
        I connect classroom concepts to real engineering constraints such as timing, power, memory, reliability, and implementation.
      </p>
    </div>
  </div>

  <div class="section">
    <h2>📍 Role Progression</h2>
    <div class="divider"></div>

    <div class="role-timeline">
      <div class="role-card umkc">
        <strong>Teaching Assistant</strong>
        <small>Sep 2022 - Dec 2024 · UMKC</small>
      </div>

      <div class="role-card umkc">
        <strong>Adjunct Instructor</strong>
        <small>Apr 2023 - May 2025 · UMKC</small>
      </div>

      <div class="role-card umkc">
        <strong>Instructor (Full-Time)</strong>
        <small>Sep 2025 - Dec 2025 · UMKC</small>
      </div>

      <div class="role-card isu">
        <strong>Assistant Professor</strong>
        <small>Jan 2026 - Present · ISU</small>
      </div>
    </div>
  </div>

  <div class="section">
    <h2>📚 Courses Taught and Planned</h2>
    <div class="divider"></div>

    <p>
      Courses are organized by institution and teaching role. Use the tabs below to view Illinois State University courses,
      UMKC instructor-led courses, and graduate teaching assistant experience.
    </p>

    <div class="course-tabs">
      <button class="tab-button active" onclick="openCourseTab(event, 'isu-courses')">Illinois State University</button>
      <button class="tab-button" onclick="openCourseTab(event, 'umkc-courses')">UMKC Instructor</button>
      <button class="tab-button" onclick="openCourseTab(event, 'ta-courses')">Graduate Teaching Assistant</button>
    </div>

    <div id="isu-courses" class="tab-panel active">

      <div class="course-card isu-course">
        <div class="course-feature-grid">
          <div>
            <div class="course-title">EGR 130 - Engineering Explorations (3 Credit Hours)</div>
            <div class="course-meta">Illinois State University · Spring 2026 · Assistant Professor · 33 students</div>

            <div class="course-body">
              <strong>Focus:</strong> Guest instruction supporting foundational engineering concepts and course activities.<br>
              <strong>Status:</strong> Guest instruction.
            </div>

            <div class="course-tags">
              <span class="course-tag isu">Spring 2026</span>
              <span class="course-tag isu">Assistant Professor</span>
              <span class="course-tag">Engineering Foundations</span>
              <span class="course-tag">33 students</span>
            </div>
          </div>

          <div>
            <a href="/images/ENGR130.jpeg" target="_blank" rel="noopener">
              <img src="/images/ENGR130.jpeg" alt="EGR 130 Laboratory" class="course-img">
            </a>
          </div>
        </div>
      </div>

      <div class="course-card isu-course">
        <div class="course-title">ELE 110 – Engineering Programming with MATLAB (3 Credit Hours)</div>
        <div class="course-meta">Illinois State University · Fall 2026 · Sections 5 and 9 · 51 Students</div>
      
        <div class="course-body">
          <strong>Focus:</strong> Introductory course on designing solutions to engineering problems using MATLAB.
        </div>
      </div>

        <div class="course-tags">
          <span class="course-tag isu">Scheduled</span>
          <span class="course-tag isu">Fall 2026</span>
          <span class="course-tag">Circuits</span>
          <span class="course-tag">Engineering</span>
        </div>
      </div>

      <div class="course-card isu-course">
        <div class="course-title">ELE 210 – Electrical Circuits I (3 Credit Hours)</div>
        <div class="course-meta">Illinois State University · Fall 2026 · Section 2 · 28 Students</div>
      
        <div class="course-body">
          <strong>Focus:</strong> Introduction to DC circuit analysis and design. Topics include basic circuit laws, resistive circuits, Kirchhoff’s laws, nodal and mesh analysis, Thevenin and Norton theorems, operational amplifiers, capacitors, inductors, and the transient and steady-state responses of first-order circuits.
        </div>
      </div>

        <div class="course-tags">
          <span class="course-tag isu">Scheduled</span>
          <span class="course-tag isu">Fall 2026</span>
          <span class="course-tag">Software</span>
          <span class="course-tag">Programming</span>
        </div>
      </div>

      <div class="course-card isu-course">
        <div class="course-title">GENED XXX - Introduction to Cybersecurity and Digital Privacy (3 Credit Hours)</div>
        <div class="course-meta">Illinois State University · Course proposal submitted · Under review</div>

        <div class="course-body">
          <strong>Focus:</strong> Foundations of cybersecurity and digital privacy, including personal data protection,
          cyber risks in everyday technologies, ethical responsibility, and informed digital citizenship.<br>
          <strong>Status:</strong> GenEd course proposal submitted via CourseDog; Approved.
        </div>

        <div class="course-tags">
          <span class="course-tag isu">Submitted</span>
          <span class="course-tag isu">Approved</span>
          <span class="course-tag">Cybersecurity</span>
          <span class="course-tag">Digital Privacy</span>
        </div>
      </div>

      <div class="course-card isu-course">
        <div class="course-title">ELE 260 - Probability &amp; Statistics for Engineers (3 Credit Hours)</div>
        <div class="course-meta">Illinois State University · Planned course assignment</div>

        <div class="course-body">
          <strong>Focus:</strong> Probability theory, random variables, statistical inference, and engineering applications.<br>
          <strong>Status:</strong> Planned course assignment, subject to departmental scheduling.
        </div>

        <div class="course-tags">
          <span class="course-tag isu">Planned</span>
          <span class="course-tag isu">Starting Spring 2026</span>
          <span class="course-tag">Probability</span>
          <span class="course-tag">Statistics</span>
        </div>
      </div>

      <div class="course-card isu-course">
        <div class="course-title">ELE 265 - Signals and Systems (3 Credit Hours)</div>
        <div class="course-meta">Illinois State University · Planned course assignment</div>

        <div class="course-body">
          <strong>Focus:</strong> Continuous- and discrete-time signals, linear time-invariant systems, convolution,
          Fourier analysis, and system representations.<br>
          <strong>Status:</strong> Planned course assignment, subject to departmental scheduling.
        </div>

        <div class="course-tags">
          <span class="course-tag isu">Planned</span>
          <span class="course-tag isu">Starting Spring 2026</span>
          <span class="course-tag">Signals</span>
          <span class="course-tag">Systems</span>
        </div>
      </div>

      <div class="course-card isu-course">
        <div class="course-title">ELE 280 - Communication Systems (3 Credit Hours)</div>
        <div class="course-meta">Illinois State University · Planned course assignment</div>

        <div class="course-body">
          <strong>Focus:</strong> Analog and digital communication systems, modulation techniques, noise analysis,
          and system performance metrics.<br>
          <strong>Status:</strong> Planned course assignment, subject to departmental scheduling.
        </div>

        <div class="course-tags">
          <span class="course-tag isu">Planned</span>
          <span class="course-tag isu">Starting Spring 2026</span>
          <span class="course-tag">Communication Systems</span>
          <span class="course-tag">Modulation</span>
        </div>
      </div>

    </div>

    <div id="umkc-courses" class="tab-panel">

      <div class="course-card umkc-course">
        <div class="course-title">ENGR E&amp;C 216 - Engineering Computation (4 Credit Hours)</div>
        <div class="course-meta">University of Missouri-Kansas City · Instructor-led course</div>

        <div class="course-body">
          <strong>Focus:</strong> C programming for engineering, including control structures, modular design, and numerical methods.<br>
          <strong>Syllabus:</strong> Structured program development using Python and C, algorithms, and data structures.
        </div>

        <div class="course-tags">
          <span class="course-tag umkc">Spring 2025 · Adjunct Instructor · 49 students</span>
          <span class="course-tag umkc">Fall 2025 · Instructor (Full-Time) · 53 students</span>
          <span class="course-tag">C Programming</span>
          <span class="course-tag">Engineering Computation</span>
        </div>
      </div>

      <div class="course-card umkc-course">
        <div class="course-title">ENGR E&amp;C 226 - Logic Design (3 Credit Hours)</div>
        <div class="course-meta">University of Missouri-Kansas City · Instructor-led course</div>

        <div class="course-body">
          <strong>Focus:</strong> Combinational and sequential logic, finite-state machines, Verilog modeling, and simulation labs.<br>
          <strong>Syllabus:</strong> Logic minimization, sequential circuit design, and digital system design.
        </div>

        <div class="course-tags">
          <span class="course-tag umkc">Spring 2025 · Adjunct Instructor · 13 students</span>
          <span class="course-tag umkc">Fall 2025 · Instructor (Full-Time) · 47 students</span>
          <span class="course-tag">Verilog</span>
          <span class="course-tag">Digital Logic</span>
        </div>
      </div>

      <div class="course-card umkc-course">
        <div class="course-title">ENGR E&amp;C 443/5533 - Analog Integrated Circuit Design (3 Credit Hours)</div>
        <div class="course-meta">University of Missouri-Kansas City · Instructor-led course</div>

        <div class="course-body">
          <strong>Focus:</strong> CMOS analog circuits including current mirrors, differential pairs, gain stages,
          and frequency response; Virtuoso-based labs.
        </div>

        <div class="course-tags">
          <span class="course-tag umkc">Spring 2023 · Adjunct Instructor · 13 students</span>
          <span class="course-tag umkc">Spring 2024 · Adjunct Instructor · 16 students</span>
          <span class="course-tag">CMOS</span>
          <span class="course-tag">Analog IC</span>
          <span class="course-tag">Cadence Virtuoso</span>
        </div>
      </div>

      <div class="course-card umkc-course">
        <div class="course-title">ENGR E&amp;C 447/5547 - ASIC Physical Design and Testing (3 Credit Hours)</div>
        <div class="course-meta">University of Missouri-Kansas City · Instructor-led course</div>

        <div class="course-body">
          <strong>Focus:</strong> RTL-to-GDSII flow; synthesis, place-and-route, clock tree synthesis, static timing analysis, and signoff.<br>
          <strong>Syllabus:</strong> Hands-on physical design using industry tools from RTL through GDSII, including floorplanning,
          power planning, routing, timing, and ECO.
        </div>

        <div class="course-tags">
          <span class="course-tag umkc">Fall 2023 · Adjunct Instructor · 14 students</span>
          <span class="course-tag umkc">Fall 2024 · Adjunct Instructor · 13 students</span>
          <span class="course-tag umkc">Fall 2025 · Instructor (Full-Time) · 9 students</span>
          <span class="course-tag">RTL-to-GDSII</span>
          <span class="course-tag">STA</span>
          <span class="course-tag">Physical Design</span>
        </div>
      </div>

    </div>

    <div id="ta-courses" class="tab-panel">

      <div class="course-card umkc-course">
        <div class="course-title">ENGR E&amp;C 442/5542 - Introduction to VLSI Design (3 Credit Hours)</div>
        <div class="course-meta">University of Missouri-Kansas City · Graduate Teaching Assistant</div>

        <div class="course-body">
          <strong>Syllabus:</strong> Fundamentals of CMOS VLSI design and layout with exposure to commercial CAD tools.
        </div>

        <div class="course-tags">
          <span class="course-tag umkc">Fall 2022 · Graduate Teaching Assistant · 25 students</span>
          <span class="course-tag">VLSI</span>
          <span class="course-tag">CMOS Layout</span>
        </div>
      </div>

      <div class="course-card umkc-course">
        <div class="course-title">ENGR E&amp;C 228 - Computer Design (3 Credit Hours)</div>
        <div class="course-meta">University of Missouri-Kansas City · Graduate Teaching Assistant</div>

        <div class="course-body">
          <strong>Syllabus:</strong> Computer organization, datapath and control design, memory systems, and introductory Verilog HDL.
        </div>

        <div class="course-tags">
          <span class="course-tag umkc">Spring 2024 · Graduate Teaching Assistant · 52 students</span>
          <span class="course-tag">Computer Organization</span>
          <span class="course-tag">Datapath</span>
          <span class="course-tag">Verilog</span>
        </div>
      </div>

      <div class="course-card umkc-course">
        <div class="course-title">ENGR E&amp;C 402/403 - Senior Design I &amp; II (6 Credit Hours)</div>
        <div class="course-meta">University of Missouri-Kansas City · Graduate Teaching Assistant</div>

        <div class="course-body">
          <strong>Syllabus:</strong> Capstone design emphasizing prototyping, fabrication, project management, and technical communication.
        </div>

        <div class="course-tags">
          <span class="course-tag umkc">Fall 2022 · Graduate Teaching Assistant · 18 students</span>
          <span class="course-tag umkc">Spring 2023 · Graduate Teaching Assistant · 19 students</span>
          <span class="course-tag">Capstone Design</span>
          <span class="course-tag">Project Management</span>
        </div>
      </div>

    </div>
  </div>

  <div class="section">
    <h2>🧭 Teaching Approach</h2>
    <div class="divider"></div>

    <div class="method-grid">
      <div class="focus-card">
        <div class="focus-icon">📘</div>
        <h3>Concept First</h3>
        <p>
          I introduce mathematical and engineering foundations before moving into simulations, implementation, and design.
        </p>
      </div>

      <div class="focus-card">
        <div class="focus-icon">💻</div>
        <h3>Build and Verify</h3>
        <p>
          Students learn by writing code, simulating designs, debugging systems, and validating results using technical evidence.
        </p>
      </div>

      <div class="focus-card">
        <div class="focus-icon">🔬</div>
        <h3>Industry-Relevant Practice</h3>
        <p>
          Course activities connect classroom topics to CAD tools, hardware workflows, communication systems, and deployment constraints.
        </p>
      </div>
    </div>
  </div>

  <div class="section">
    <h2>🛠️ Instructional Areas</h2>
    <div class="divider"></div>

    <div class="tag-cloud">
      <span class="tag">Engineering Computation</span>
      <span class="tag">C Programming</span>
      <span class="tag">Logic Design</span>
      <span class="tag">Verilog HDL</span>
      <span class="tag">Computer Design</span>
      <span class="tag">Signals and Systems</span>
      <span class="tag">Communication Systems</span>
      <span class="tag">Probability and Statistics</span>
      <span class="tag">Analog Integrated Circuits</span>
      <span class="tag">CMOS VLSI</span>
      <span class="tag">ASIC Physical Design</span>
      <span class="tag">RTL-to-GDSII Flow</span>
      <span class="tag">Static Timing Analysis</span>
      <span class="tag">Senior Design</span>
      <span class="tag">Cybersecurity and Digital Privacy</span>
    </div>
  </div>

</div>

<script>
function openCourseTab(event, panelId) {
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
