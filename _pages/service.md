---
title: ""
layout: single
permalink: /service/
toc: false
author_profile: true
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
  max-width:90ch;
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

/* Badges */
.badges{
  display:flex;
  flex-wrap:wrap;
  gap:0.55rem;
  margin-top:0.75rem;
}
.badge{
  display:inline-flex;
  align-items:center;
  gap:0.35rem;
  padding:0.35rem 0.7rem;
  border-radius:999px;
  background:#ffffff;
  border:1px solid rgba(26,115,232,0.22);
  box-shadow:var(--shadow2);
  font-size:0.92rem;
  color:#0b1f44;
  font-weight:800;
}
.badge.isu{
  border-color:rgba(220,20,60,0.30);
  color:#7a0b1f;
}

/* Service Grid + Cards */
.service-grid{
  display:grid;
  grid-template-columns:1fr;
  gap:1rem;
  margin-top:0.9rem;
}
@media (min-width: 900px){
  .service-grid{ grid-template-columns:repeat(2, 1fr); }
}

.service-card{
  background:#ffffff;
  border:1px solid rgba(26,115,232,0.16);
  border-radius:14px;
  padding:1.05rem 1.15rem;
  box-shadow:var(--shadow2);
  transition:0.2s ease-in-out;
  position:relative;
}
.service-card:hover{
  transform:translateY(-2px);
  box-shadow:var(--shadow);
  background:#fbfdff;
}
.service-card::before{
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
.service-card.isu::before{ background:rgba(220,20,60,0.75); }

.service-card h4{
  margin:0 0 0.5rem 0;
  font-size:1.05rem;
  color:#0b1f44;
}
.service-card p{
  margin:0.35rem 0;
  color:#202124;
  font-size:0.96rem;
}
.meta{
  color:var(--muted);
  font-size:0.95rem;
  margin:0.2rem 0 0.2rem 0;
}

/* Status pills inside cards */
.pill{
  display:inline-block;
  font-size:0.85rem;
  font-weight:900;
  padding:0.22rem 0.55rem;
  border-radius:999px;
  margin-top:0.4rem;
}
.pill.active{ color:#1a7f3d; background:#dcfce7; }
.pill.ongoing{ color:#0a539e; background:#e5f1ff; }
.pill.pending{ color:#7a5a00; background:#fff6e6; }
.pill.submitted{ color:#444; background:#f1f3f4; }

/* Scoped links */
.section a, .page-hero a{
  color:var(--blue);
  font-weight:800;
  text-decoration:none;
}
.section a:hover, .page-hero a:hover{ text-decoration:underline; }
</style>

<div class="page-hero">
  <h2>Service</h2>
  <p>
    Service activities spanning institutional roles, professional community contribution, and research-related leadership aligned with
    Illinois State University annual review categories (Teaching, Research/Creative Activity, and Service).
  </p>
  <div class="badges">
    <span class="badge isu">Assistant Professor · Illinois State University (Spring 2026 – Present)</span>
    <span class="badge">Institutional</span>
    <span class="badge">Professional</span>
    <span class="badge">Research Service</span>
  </div>
  <div class="hero-links">
    <a class="btn-link secondary" href="/resume/">Resume</a>
    <a class="btn-link secondary" href="/teaching/">Teaching</a>
    <a class="btn-link" href="/publications/">Publications</a>
  </div>
</div>

<div class="section">
  <h3>Institutional Service</h3>
  <div class="divider"></div>

  <div class="service-grid">
    
    <div class="service-card isu">
      <h4>Judge, Student Project Expo - Spring 2026</h4>
      <p class="meta"><strong>Institution:</strong> Illinois State University</p>
      <p><strong>Focus:</strong> Evaluation of student engineering design projects, feedback on technical presentations, and support for project-based learning across the College of Engineering.</p>
      <span class="pill active">Completed</span>
    </div>

    <div class="service-card isu">
      <h4>Faculty Search Committee - Spring 2026</h4>
      <p class="meta"><strong>Institution:</strong> Illinois State University</p>
      <p><strong>Focus:</strong> Faculty recruitment, candidate evaluation, and participation in departmental hiring decisions.</p>
      <span class="pill active">Completed</span>
    </div>

    <div class="service-card isu">
      <h4>University Continuity Program - Faculty Representative</h4>
      <p class="meta"><strong>Department:</strong> Electrical Engineering</p>
      <p><strong>Focus:</strong> Departmental continuity planning, preparedness initiatives, and coordination with university-level continuity efforts.</p>
      <span class="pill active">Active</span>
    </div>

    <div class="service-card isu">
      <h4>K–12 STEM Outreach and School Engagement Coordinator</h4>
      <p class="meta"><strong>Institution:</strong> Illinois State University, College of Engineering</p>
      <p><strong>Role:</strong> Lead and coordinate outreach visits to middle schools and high schools to promote engineering education, STEM awareness, and pathways into the College of Engineering.</p>
      <p><strong>Activities:</strong> Organizing and conducting school visits, coordinating faculty and student participation, and supporting the development and deployment of hands-on STEM engagement kits for interactive demonstrations.</p>
      <p><strong>Focus:</strong> Pre-college STEM exposure, recruitment pipeline development, and community engagement.</p>
      <span class="pill active">Active</span>
    </div>

    <div class="service-card isu">
      <h4>Redbird Day 2026 — Faculty Representative</h4>
      <p class="meta"><strong>Institution:</strong> Illinois State University</p>
      <p><strong>Role:</strong> Represented the Electrical Engineering Department during Redbird Day 2026.</p>
      <p><strong>Activities:</strong> Interacted with prospective students and families during the university recruitment event.</p>
      <span class="pill active">Completed</span>
    </div>

    <div class="service-card isu">
      <h4>MSEE Curriculum Development</h4>
      <p class="meta"><strong>Institution:</strong> Illinois State University</p>
      <p><strong>Focus:</strong> Proposed new courses and contributed to structuring and formatting the MSEE curriculum, with alignment toward communication systems, signal processing, and AI-related topics.</p>
      <span class="pill active">Ongoing</span>
    </div>

    <div class="service-card umkc">
      <h4>Research Lab Demonstration and Outreach</h4>
      <p class="meta"><strong>Institution:</strong> University of Missouri–Kansas City</p>
      <p><strong>Focus:</strong> Showcased research lab work during engineering open house events, engaging with prospective students and communicating technical concepts to a broader audience.</p>
      <span class="pill active">Completed</span>
    </div>

    <div class="service-card umkc">
      <h4>Senator, Student Government Association (Fall 2023 – Fall 2024)</h4>
      <p class="meta"><strong>Institution:</strong> University of Missouri–Kansas City</p>
      <p><strong>Focus:</strong> Represented graduate student interests, participated in university governance discussions, and supported student-focused academic initiatives.</p>
      <span class="pill active">Completed</span>
    </div>

  </div>
</div>

<div class="section">
  <h3>Professional Service</h3>
  <div class="divider"></div>

  <div class="service-grid">

    <div class="service-card">
    <h4>Invited Lecture — IEEE</h4>
      <p class="meta"><strong>Organization:</strong> IEEE ISU Student Branch</p>
      <p><strong>Title:</strong> From RTL to GDSII: Hardware Design Flow, EDA Toolchain, and VLSI Industry Roles</p>
      <p><strong>Venue:</strong> Williams Hall, Room 113, Illinois State University</p>
      <p><strong>Date:</strong> April 06, 2026 &nbsp;|&nbsp; <strong>Time:</strong> 1:00–2:00 PM</p>
      <span class="pill active">Active</span>
    </div>
    
    <div class="service-card">
      <h4>Technical Program Committee (TPC) Reviewer</h4>
      <p class="meta"><strong>Organization:</strong> IEEE-affiliated conference ROSE 2026</p>
      <p><strong>Focus:</strong> Peer review of technical manuscripts and evaluation of scholarly contributions.</p>
      <span class="pill ongoing">Ongoing</span>
    </div>

    <div class="service-card">
      <h4>Philanthropic Proposal Development</h4>
      <p class="meta"><strong>Unit:</strong> College of Engineering</p>
      <p><strong>Focus:</strong> Coordination and development of philanthropic proposals supporting strategic initiatives and external engagement.</p>
      <span class="pill ongoing">Completed</span>
    </div>

  </div>
</div>

<div class="section">
  <h3>Research Service and Leadership</h3>
  <div class="divider"></div>

  <div class="service-grid">

    <div class="service-card">
      <h4>Lightweight and Hardware-Aware RF Signal Classification</h4>
      <p><strong>Focus:</strong> Energy-efficient RF classification algorithms, hardware-aware design, and edge-deployable intelligence.</p>
      <span class="pill active">Active Research Service</span>
    </div>

    <div class="service-card">
      <h4>Hardware-Aware Characterization of RF Transmission Lines and Antenna Arrays</h4>
      <p class="meta"><strong>Role:</strong> Principal Investigator</p>
      <p class="meta"><strong>Sponsor:</strong> College of Engineering University Research Grant (CEG URG)</p>
      <p><strong>Focus:</strong> Analytical modeling, numerical analysis, and experimental RF measurement, emphasizing hardware-aware characterization and undergraduate research mentoring.</p>
      <span class="pill active">Proposal Approved</span>
    </div>


    <div class="service-card">
      <h4>Redbird Engineering Innovation Open Lab</h4>
      <p class="meta"><strong>Role:</strong> Co-Principal Investigator</p>
      <p class="meta"><strong>Sponsor:</strong> Illinois State University Strategic Initiative Request Fund</p>
      <p><strong>Focus:</strong> Development of an open, hands-on engineering learning environment that supports student innovation, experiential learning, interdisciplinary collaboration, and expanded access to technical resources beyond regular class and lab hours.</p>
      <span class="pill active">Proposal Submitted</span>
    </div>
    
        <div class="service-card">
          <h4>Energy and Compute-Aware Edge Systems: A Pilot Framework</h4>
          <p class="meta"><strong>Role:</strong> Lead Principal Investigator</p>
          <p class="meta"><strong>Sponsor:</strong> IIN</p>
          <p><strong>Focus:</strong> Pilot-scale research on energy and compute-aware edge systems, emphasizing lightweight intelligence, hardware-aware design, student involvement, and applied edge deployment.</p>
          <span class="pill pending">Pending Submission</span>
        </div>

  </div>
</div>
