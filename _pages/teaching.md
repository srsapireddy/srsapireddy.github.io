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
  --bg: #ffffff;
  --muted: #5f6368;
  --hover: #e9f3ff;
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
  max-width: 75ch;
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
.badge.isu { border-color: rgba(220,20,60,0.35); color: #7a0b1f; }
.badge.umkc { border-color: rgba(0,150,214,0.35); color: #065a7d; }

/* Cards / Sections */
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

/* Divider */
.divider { height: 1px; background: rgba(26,115,232,0.12); margin: 0.3rem 0 0.9rem 0; }

/* Grid */
.grid-2 { display: grid; grid-template-columns: 1fr; gap: 1.3rem; }
@media (min-width: 900px) { .grid-2 { grid-template-columns: 1fr 1fr; } }

/* Role progression cards */
.role-grid { display: grid; grid-template-columns: 1fr; gap: 1rem; }
@media (min-width: 900px) { .role-grid { grid-template-columns: repeat(4, 1fr); } }
.role-card {
  border-radius: 14px;
  padding: 1rem 1rem;
  background: #ffffff;
  border: 1px solid rgba(26,115,232,0.2);
  box-shadow: var(--shadow2);
}
.role-card strong { display:block; color:#0b1f44; font-size:1.05rem; }
.role-card small { display:block; margin-top:0.35rem; color: var(--muted); }
.role-card.umkc { border-left: 6px solid var(--umkc); }
.role-card.isu { border-left: 6px solid var(--isu); }

/* Course header */
.course-title { margin: 0.1rem 0 0.6rem 0; font-size: 1.05rem; color:#0b1f44; }
.meta { color: var(--muted); margin: 0.2rem 0 0.7rem 0; }

/* Image */
.course-img {
  width:100%;
  max-height:170px;
  object-fit:cover;
  border-radius:12px;
  box-shadow: var(--shadow2);
  border: 1px solid rgba(26,115,232,0.15);
  cursor: zoom-in;
}
</style>

<div class="page-hero">
  <h2>Teaching &amp; Instruction</h2>
  <p>
    My teaching emphasizes rigorous foundations, hands-on design practice, and deployment-oriented thinking across digital systems,
    signal processing, and hardware-aware machine learning.
  </p>
  <div class="badges">
    <span class="badge isu">Illinois State University</span>
    <span class="badge umkc">University of Missouri–Kansas City</span>
    <span class="badge">Logic Design</span>
    <span class="badge">Engineering Computation</span>
    <span class="badge">VLSI / Physical Design</span>
  </div>
</div>

<div class="section">
  <h3>Role Progression</h3>
  <div class="divider"></div>

  <div class="role-grid">
    <div class="role-card umkc">
      <strong>Teaching Assistant</strong>
      <small>Sep 2022 – Dec 2024 · UMKC</small>
    </div>
    <div class="role-card umkc">
      <strong>Adjunct Instructor</strong>
      <small>Apr 2023 – May 2025 · UMKC</small>
    </div>
    <div class="role-card umkc">
      <strong>Instructor (Full-Time)</strong>
      <small>Sep 2025 – Dec 2025 · UMKC</small>
    </div>
    <div class="role-card isu">
      <strong>Assistant Professor</strong>
      <small>Jan 2026 – Present · ISU</small>
    </div>
  </div>
</div>

<div class="section">
  <h3>Courses Taught</h3>
  <div class="divider"></div>
  <p class="meta">
    <span class="badge isu">Assistant Professor · Illinois State University (Spring 2026 – Present)</span>
    <span class="badge umkc">Instructor · University of Missouri–Kansas City (Spring 2023 – Fall 2025)</span>
  </p>
</div>

<div class="section">
  <h3>Illinois State University</h3>
  <div class="divider"></div>

  <div class="grid-2">
    <div>
      <div class="course-title">EGR 130 – Engineering Explorations (3 Credit Hours)</div>
      <p>
        <strong>Focus:</strong> Guest instruction supporting foundational engineering concepts and course activities.<br>
        <strong>Status:</strong> Guest instruction.<br>
        <strong>Semester:</strong> <span class="badge isu">Spring 2026 · Assistant Professor · 33 students</span>
      </p>
    </div>

    <div>
      <a href="/images/ENGR130.jpeg" target="_blank" rel="noopener">
        <img src="/images/ENGR130.jpeg" alt="EGR 130 Laboratory" class="course-img">
      </a>
    </div>
  </div>

  <div class="divider"></div>

  <div class="course-title">GENED XXX – Introduction to Cybersecurity and Digital Privacy (3 Credit Hours)</div>
  <p>
    <strong>Focus:</strong> Foundations of cybersecurity and digital privacy, including personal data protection, cyber risks in everyday technologies,
    ethical responsibility, and informed digital citizenship.<br>
    <strong>Status:</strong> GenEd course proposal submitted via CourseDog; pending review and approval.<br>
    <strong>Semesters:</strong> <span class="badge isu">Submitted · Under Review</span>
  </p>

  <div class="divider"></div>

  <div class="course-title">ELE 260 – Probability &amp; Statistics for Engineers (3 Credit Hours)</div>
  <p>
    <strong>Focus:</strong> Probability theory, random variables, statistical inference, and engineering applications.<br>
    <strong>Status:</strong> Planned course assignment, subject to departmental scheduling.<br>
    <strong>Semesters:</strong> <span class="badge isu">Planned · Starting Spring 2026</span>
  </p>

  <div class="divider"></div>

  <div class="course-title">ELE 265 – Signals and Systems (3 Credit Hours)</div>
  <p>
    <strong>Focus:</strong> Continuous- and discrete-time signals, linear time-invariant systems, convolution, Fourier analysis, and system representations.<br>
    <strong>Status:</strong> Planned course assignment, subject to departmental scheduling.<br>
    <strong>Semesters:</strong> <span class="badge isu">Planned · Starting Spring 2026</span>
  </p>

  <div class="divider"></div>

  <div class="course-title">ELE 280 – Communication Systems (3 Credit Hours)</div>
  <p>
    <strong>Focus:</strong> Analog and digital communication systems, modulation techniques, noise analysis, and system performance metrics.<br>
    <strong>Status:</strong> Planned course assignment, subject to departmental scheduling.<br>
    <strong>Semesters:</strong> <span class="badge isu">Planned · Starting Spring 2026</span>
  </p>
</div>

<div class="section">
  <h3>University of Missouri–Kansas City</h3>
  <div class="divider"></div>

  <div class="course-title">ENGR E&amp;C 216 – Engineering Computation (4 Credit Hours)</div>
  <p>
    <strong>Focus:</strong> C programming for engineering (control structures, modular design, numerics).<br>
    <strong>Syllabus:</strong> Structured program development using Python and C, algorithms, and data structures.<br>
    <strong>Semesters taught:</strong><br>
    <span class="badge umkc">Spring 2025 · Adjunct Instructor · 49 students</span>
    <span class="badge umkc">Fall 2025 · Instructor (Full-Time) · 53 students</span>
  </p>

  <div class="divider"></div>

  <div class="course-title">ENGR E&amp;C 226 – Logic Design (3 Credit Hours)</div>
  <p>
    <strong>Focus:</strong> Combinational and sequential logic, FSMs, Verilog modeling, and simulation labs.<br>
    <strong>Syllabus:</strong> Logic minimization, sequential circuit design, and digital system design.<br>
    <strong>Semesters taught:</strong><br>
    <span class="badge umkc">Spring 2025 · Adjunct Instructor · 13 students</span>
    <span class="badge umkc">Fall 2025 · Instructor (Full-Time) · 47 students</span>
  </p>

  <div class="divider"></div>

  <div class="course-title">ENGR E&amp;C 443/5533 – Analog Integrated Circuit Design (3 Credit Hours)</div>
  <p>
    <strong>Focus:</strong> CMOS analog circuits including current mirrors, differential pairs, gain stages, and frequency response; Virtuoso-based labs.<br>
    <strong>Semesters taught:</strong><br>
    <span class="badge umkc">Spring 2023 · Adjunct Instructor · 13 students</span>
    <span class="badge umkc">Spring 2024 · Adjunct Instructor · 16 students</span>
  </p>

  <div class="divider"></div>

  <div class="course-title">ENGR E&amp;C 447/5547 – ASIC Physical Design and Testing (3 Credit Hours)</div>
  <p>
    <strong>Focus:</strong> RTL→GDSII flow; synthesis, place-and-route, CTS, STA, and signoff.<br>
    <strong>Syllabus:</strong> Hands-on physical design using industry tools from RTL through GDSII, including floorplanning, power planning, routing,
    timing, and ECO.<br>
    <strong>Semesters taught:</strong><br>
    <span class="badge umkc">Fall 2023 · Adjunct Instructor · 14 students</span>
    <span class="badge umkc">Fall 2024 · Adjunct Instructor · 13 students</span>
    <span class="badge umkc">Fall 2025 · Instructor (Full-Time) · 9 students</span>
  </p>
</div>

<div class="section">
  <h3>Additional Teaching (Graduate Teaching Assistant)</h3>
  <div class="divider"></div>

  <div class="course-title">ENGR E&amp;C 442/5542 – Introduction to VLSI Design (3 Credit Hours)</div>
  <p>
    <span class="badge umkc">Fall 2022 · Graduate Teaching Assistant · 25 students</span><br>
    <strong>Syllabus:</strong> Fundamentals of CMOS VLSI design and layout with exposure to commercial CAD tools.
  </p>

  <div class="divider"></div>

  <div class="course-title">ENGR E&amp;C 228 – Computer Design (3 Credit Hours)</div>
  <p>
    <span class="badge umkc">Spring 2024 · Graduate Teaching Assistant · 52 students</span><br>
    <strong>Syllabus:</strong> Computer organization, datapath and control design, memory systems, and introductory Verilog HDL.
  </p>

  <div class="divider"></div>

  <div class="course-title">ENGR E&amp;C 402/403 – Senior Design I &amp; II (6 Credit Hours)</div>
  <p>
    <span class="badge umkc">Fall 2022 · Graduate Teaching Assistant · 18 students</span>
    <span class="badge umkc">Spring 2023 · Graduate Teaching Assistant · 19 students</span><br>
    <strong>Syllabus:</strong> Capstone design emphasizing prototyping, fabrication, project management, and technical communication.
  </p>
</div>
