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
  --green:#1a7f3d;
  --gold:#7a5a00;
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
  from{
    opacity:0;
    transform:translateY(14px);
  }
  to{
    opacity:1;
    transform:translateY(0);
  }
}

@keyframes slideTrack{
  from{
    transform:translateX(0);
  }
  to{
    transform:translateX(-50%);
  }
}

.service-wrap{
  animation:fadeInUp 0.85s ease-in-out;
}

/* Hero */
.page-hero{
  position:relative;
  overflow:hidden;
  border-radius:var(--radius);
  padding:2.25rem 2rem;
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
  max-width:94ch;
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

/* Badges */
.badges{
  display:flex;
  flex-wrap:wrap;
  gap:0.55rem;
  margin-top:1rem;
}

.badge{
  display:inline-flex;
  align-items:center;
  gap:0.35rem;
  padding:0.36rem 0.72rem;
  border-radius:999px;
  background:#ffffff;
  border:1px solid rgba(26,115,232,0.22);
  box-shadow:var(--shadow2);
  font-size:0.9rem;
  color:var(--text);
  font-weight:850;
}

.badge.isu{
  border-color:rgba(220,20,60,0.30);
  color:#7a0b1f;
  background:rgba(220,20,60,0.06);
}

/* Impact cards */
.impact-grid{
  display:grid;
  grid-template-columns:repeat(4,1fr);
  gap:0.95rem;
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
  font-size:1.6rem;
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
  margin-top:0.22rem;
  font-size:0.82rem;
  color:var(--muted);
}

/* Sections */
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

/* Focus cards */
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
  border:1px solid rgba(26,115,232,0.18);
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

/* Service tabs */
.service-tabs{
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

/* Service Grid + Cards */
.service-grid{
  display:grid;
  grid-template-columns:1fr;
  gap:1rem;
  margin-top:0.9rem;
}

@media (min-width:900px){
  .service-grid{
    grid-template-columns:repeat(2,1fr);
  }
}

.service-card{
  background:#ffffff;
  border:1px solid rgba(26,115,232,0.16);
  border-radius:16px;
  padding:1.1rem 1.15rem;
  box-shadow:var(--shadow2);
  transition:0.22s ease-in-out;
  position:relative;
  overflow:hidden;
}

.service-card:hover{
  transform:translateY(-3px);
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
  border-top-left-radius:16px;
  border-bottom-left-radius:16px;
  background:rgba(26,115,232,0.70);
}

.service-card.isu::before{
  background:rgba(220,20,60,0.78);
}

.service-card.umkc::before{
  background:rgba(0,150,214,0.78);
}

.service-card.research::before{
  background:linear-gradient(180deg,var(--blue),var(--isu));
}

.service-card h4{
  margin:0 0 0.55rem 0;
  font-size:1.05rem;
  color:var(--text);
  line-height:1.35;
}

.service-card p{
  margin:0.38rem 0;
  color:#202124;
  font-size:0.95rem;
  line-height:1.55;
}

.meta{
  color:var(--muted) !important;
  font-size:0.92rem !important;
  margin:0.2rem 0 0.2rem 0 !important;
}

/* Status pills */
.pill{
  display:inline-flex;
  align-items:center;
  font-size:0.84rem;
  font-weight:900;
  padding:0.28rem 0.62rem;
  border-radius:999px;
  margin-top:0.55rem;
}

.pill.active{
  color:var(--green);
  background:#dcfce7;
}

.pill.ongoing{
  color:#0a539e;
  background:#e5f1ff;
}

.pill.pending{
  color:var(--gold);
  background:#fff6e6;
}

.pill.submitted{
  color:#444;
  background:#f1f3f4;
}

.pill.completed{
  color:var(--green);
  background:#dcfce7;
}

/* Tag cloud */
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

/* Timeline */
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

/* Grid */
.grid-2{
  display:grid;
  grid-template-columns:1fr;
  gap:1.2rem;
}

@media (min-width:900px){
  .grid-2{
    grid-template-columns:1fr 1fr;
  }
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

/* Responsive */
@media (max-width:950px){
  .impact-grid,
  .focus-grid{
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
  .focus-grid{
    grid-template-columns:1fr;
  }
}
</style>

<div class="service-wrap">

  <div class="page-hero">
    <div class="hero-content">
      <span class="hero-kicker">Academic Service · Outreach · Research Leadership</span>

      <h1>Service</h1>

      <p>
        My service activities span institutional leadership, student engagement, K-12 outreach,
        professional community contribution, and research-related proposal development. These activities align with
        Illinois State University annual review categories, including teaching, research and creative activity, and service.
      </p>

      <div class="badges">
        <span class="badge isu">Assistant Professor · Illinois State University</span>
        <span class="badge">Institutional Service</span>
        <span class="badge">Professional Service</span>
        <span class="badge">Research Leadership</span>
        <span class="badge">K-12 STEM Outreach</span>
      </div>

      <div class="hero-links">
        <a class="btn-link secondary" href="/resume/">Resume</a>
        <a class="btn-link secondary" href="/teaching/">Teaching</a>
        <a class="btn-link" href="/publications/">Publications</a>
        <a class="btn-link secondary" href="/insys-lab/">INSys Lab</a>
      </div>
    </div>
  </div>

  <div class="sliding-bar">
    <div class="slide-track">
      <div class="slide-item"><span>●</span> Institutional Service</div>
      <div class="slide-item"><span>●</span> Faculty Search Committee</div>
      <div class="slide-item"><span>●</span> K-12 STEM Outreach</div>
      <div class="slide-item"><span>●</span> IEEE Invited Lecture</div>
      <div class="slide-item"><span>●</span> Proposal Development</div>
      <div class="slide-item"><span>●</span> Research Leadership</div>
      <div class="slide-item"><span>●</span> Student Project Expo</div>

      <div class="slide-item"><span>●</span> Institutional Service</div>
      <div class="slide-item"><span>●</span> Faculty Search Committee</div>
      <div class="slide-item"><span>●</span> K-12 STEM Outreach</div>
      <div class="slide-item"><span>●</span> IEEE Invited Lecture</div>
      <div class="slide-item"><span>●</span> Proposal Development</div>
      <div class="slide-item"><span>●</span> Research Leadership</div>
      <div class="slide-item"><span>●</span> Student Project Expo</div>
    </div>
  </div>

  <div class="impact-grid">
    <div class="impact-card">
      <div class="impact-number">ISU</div>
      <div class="impact-label">Institutional Service</div>
      <div class="impact-sub">Department, college, and university roles</div>
    </div>

    <div class="impact-card">
      <div class="impact-number">K-12</div>
      <div class="impact-label">STEM Outreach</div>
      <div class="impact-sub">School engagement and engineering awareness</div>
    </div>

    <div class="impact-card">
      <div class="impact-number">IEEE</div>
      <div class="impact-label">Professional Service</div>
      <div class="impact-sub">Lecture, review, and technical engagement</div>
    </div>

    <div class="impact-card">
      <div class="impact-number">PI</div>
      <div class="impact-label">Research Leadership</div>
      <div class="impact-sub">Grant and proposal development</div>
    </div>
  </div>

  <div class="focus-grid">
    <div class="focus-card">
      <div class="focus-icon">🏛️</div>
      <h3>Institutional Engagement</h3>
      <p>
        Service includes committee participation, student project evaluation, continuity planning,
        curriculum development, and university recruitment events.
      </p>
    </div>

    <div class="focus-card">
      <div class="focus-icon">🤝</div>
      <h3>Outreach and Community</h3>
      <p>
        K-12 STEM outreach supports engineering awareness, school engagement,
        pre-college recruitment, and hands-on learning activities.
      </p>
    </div>

    <div class="focus-card">
      <div class="focus-icon">🔬</div>
      <h3>Research and Proposal Service</h3>
      <p>
        Research service includes proposal development, grant leadership,
        reviewer activity, and externally engaged research planning.
      </p>
    </div>
  </div>

  <div class="section">
    <h2>📂 Service Activities</h2>
    <div class="divider"></div>

    <p>
      Service activities are organized into institutional service, professional service,
      and research service/leadership. Use the tabs below to view each category.
    </p>

    <div class="service-tabs">
      <button class="tab-button active" onclick="openServiceTab(event, 'institutional-tab')">Institutional Service</button>
      <button class="tab-button" onclick="openServiceTab(event, 'professional-tab')">Professional Service</button>
      <button class="tab-button" onclick="openServiceTab(event, 'research-tab')">Research Service and Leadership</button>
    </div>

    <div id="institutional-tab" class="tab-panel active">
      <div class="service-grid">

    
    <div class="service-card isu">
      <h4>Academic Department & Student Services Fair - Summer Open House 2026</h4>
      <p class="meta"><strong>Institution:</strong> Illinois State University</p>
      <p><strong>Location:</strong> Brown Ballroom</p>
      <p><strong>Focus:</strong> Represented the College of Engineering during the Summer Open House for prospective freshman and transfer students and their families. Engaged with attendees, provided information about Electrical Engineering programs, and supported student recruitment and admissions outreach.</p>
      <span class="pill completed">Completed</span>
    </div>

    <div class="service-card isu">
      <h4>Electric Circuits I Laboratory Manual Development</h4>
      <p class="meta"><strong>Institution:</strong> Illinois State University</p>
      <p><strong>Focus:</strong> Development of laboratory manuals, experiment procedures, data tables, safety guidelines, and instructional materials for Electric Circuits I, supporting hands-on learning in DC circuits, Ohm’s law, resistor measurements, series and parallel circuits, nodal analysis, and mesh current methods.</p>
      <span class="pill ongoing">Ongoing</span>
    </div>

        <div class="service-card isu">
          <h4>Judge, Student Project Expo - Spring 2026</h4>
          <p class="meta"><strong>Institution:</strong> Illinois State University</p>
          <p><strong>Focus:</strong> Evaluation of student engineering design projects, feedback on technical presentations, and support for project-based learning across the College of Engineering.</p>
          <span class="pill completed">Completed</span>
        </div>

        <div class="service-card isu">
          <h4>Faculty Search Committee - Spring 2026</h4>
          <p class="meta"><strong>Institution:</strong> Illinois State University</p>
          <p><strong>Focus:</strong> Faculty recruitment, candidate evaluation, and participation in departmental hiring decisions.</p>
          <span class="pill completed">Completed</span>
        </div>

        <div class="service-card isu">
          <h4>University Continuity Program - Faculty Representative</h4>
          <p class="meta"><strong>Department:</strong> Electrical Engineering</p>
          <p><strong>Focus:</strong> Departmental continuity planning, preparedness initiatives, and coordination with university-level continuity efforts.</p>
          <span class="pill active">Active</span>
        </div>

        <div class="service-card isu">
          <h4>K-12 STEM Outreach and School Engagement Coordinator</h4>
          <p class="meta"><strong>Institution:</strong> Illinois State University, College of Engineering</p>
          <p><strong>Role:</strong> Coordinate and lead K-12 outreach visits to local schools to promote engineering education, STEM awareness, and student engagement with the College of Engineering.</p>
          <p><strong>Activities:</strong> Preparing outreach materials, student handouts, presentation slides, and hands-on demonstration kits; organizing school visits; coordinating outreach activities; and conducting interactive engineering sessions for students.</p>
          <p><strong>Recent Outreach Visits:</strong> Chiddix Junior High School, Bloomington, Illinois - June 8, 2026; continuing Monday visits through June 2026.</p>
          <p><strong>Focus:</strong> Pre-college STEM exposure, electrical engineering awareness, community engagement, and student recruitment pathways.</p>
          <span class="pill active">Active</span>
        </div>

        <div class="service-card isu">
          <h4>Redbird Day 2026 - Faculty Representative</h4>
          <p class="meta"><strong>Institution:</strong> Illinois State University</p>
          <p><strong>Role:</strong> Represented the Electrical Engineering Department during Redbird Day 2026.</p>
          <p><strong>Activities:</strong> Interacted with prospective students and families during the university recruitment event.</p>
          <span class="pill completed">Completed</span>
        </div>

        <div class="service-card isu">
          <h4>MSEE Curriculum Development</h4>
          <p class="meta"><strong>Institution:</strong> Illinois State University</p>
          <p><strong>Focus:</strong> Proposed new courses and contributed to structuring and formatting the MSEE curriculum, with alignment toward communication systems, signal processing, and AI-related topics.</p>
          <span class="pill ongoing">Ongoing</span>
        </div>

        <div class="service-card isu">
          <h4>Industry Advisory Board Presentation on K-12 STEM Outreach Preparation</h4>
          <p class="meta"><strong>Role:</strong> Presenter</p>
          <p class="meta"><strong>Organization:</strong> Department of Electrical Engineering, Illinois State University</p>
          <p><strong>Contribution:</strong> Presented the preparation and planned delivery of hands-on K-12 electrical engineering outreach activities using low-cost STEM kits to support school engagement, recruitment, and College of Engineering visibility.</p>
          <span class="pill completed">Completed</span>
        </div>

        <div class="service-card umkc">
          <h4>Research Lab Demonstration and Outreach</h4>
          <p class="meta"><strong>Institution:</strong> University of Missouri-Kansas City</p>
          <p><strong>Focus:</strong> Showcased research lab work during engineering open house events, engaging with prospective students and communicating technical concepts to a broader audience.</p>
          <span class="pill completed">Completed</span>
        </div>

        <div class="service-card umkc">
          <h4>Senator, Student Government Association</h4>
          <p class="meta"><strong>Institution:</strong> University of Missouri-Kansas City</p>
          <p class="meta"><strong>Period:</strong> Fall 2023 - Fall 2024</p>
          <p><strong>Focus:</strong> Represented graduate student interests, participated in university governance discussions, and supported student-focused academic initiatives.</p>
          <span class="pill completed">Completed</span>
        </div>

      </div>
    </div>

    <div id="professional-tab" class="tab-panel">
      <div class="service-grid">

        <div class="service-card isu">
          <h4>Invited Lecture - IEEE</h4>
          <p class="meta"><strong>Organization:</strong> IEEE ISU Student Branch</p>
          <p><strong>Title:</strong> From RTL to GDSII: Hardware Design Flow, EDA Toolchain, and VLSI Industry Roles</p>
          <p><strong>Venue:</strong> Williams Hall, Room 113, Illinois State University</p>
          <p><strong>Date:</strong> April 06, 2026 &nbsp;|&nbsp; <strong>Time:</strong> 1:00-2:00 PM</p>
          <span class="pill active">Active</span>
        </div>

        <div class="service-card">
          <h4>Technical Program Committee Reviewer</h4>
          <p class="meta"><strong>Organization:</strong> IEEE-affiliated conference ROSE 2026</p>
          <p><strong>Focus:</strong> Peer review of technical manuscripts and evaluation of scholarly contributions.</p>
          <span class="pill ongoing">Ongoing</span>
        </div>

        <div class="service-card isu">
          <h4>Philanthropic Proposal Development</h4>
          <p class="meta"><strong>Unit:</strong> College of Engineering</p>
          <p><strong>Focus:</strong> Coordination and development of philanthropic proposals supporting strategic initiatives and external engagement.</p>
          <span class="pill completed">Completed</span>
        </div>

      </div>
    </div>

    <div id="research-tab" class="tab-panel">
      <div class="service-grid">

        <div class="service-card research">
          <h4>Lightweight and Hardware-Aware RF Signal Classification</h4>
          <p><strong>Focus:</strong> Energy-efficient RF classification algorithms, hardware-aware design, and edge-deployable intelligence.</p>
          <span class="pill active">Active Research Service</span>
        </div>

        <div class="service-card research">
          <h4>NVIDIA Academic Grant Proposal</h4>
          <p class="meta"><strong>Role:</strong> Principal Investigator</p>
          <p class="meta"><strong>Status:</strong> In Preparation</p>
          <p><strong>Focus:</strong> GPU-accelerated scientific simulation and adaptive computational modeling.</p>
          <span class="pill pending">Pending Submission</span>
        </div>

        <div class="service-card research">
          <h4>AI-Enhanced Undergraduate Engineering Education</h4>
          <p class="meta"><strong>Role:</strong> Lead Principal Investigator</p>
          <p class="meta"><strong>Status:</strong> Submitted</p>
          <p><strong>Sponsor:</strong> NSF IUSE Program </p>
          <p><strong>Focus:</strong> Enhancing undergraduate engineering education through innovative AI-enabled learning strategies, active learning, and computational reasoning.</p>
          <span class="pill pending">Under Review</span>
        </div>

        <div class="service-card isu research">
          <h4>Hardware-Aware Characterization of RF Transmission Lines and Antenna Arrays</h4>
          <p class="meta"><strong>Role:</strong> Principal Investigator</p>
          <p class="meta"><strong>Sponsor:</strong> College of Engineering University Research Grant (CEG URG)</p>
          <p><strong>Focus:</strong> Analytical modeling, numerical analysis, and experimental RF measurement, emphasizing hardware-aware characterization and undergraduate research mentoring.</p>
          <span class="pill active">Proposal Approved</span>
        </div>

        <div class="service-card isu research">
          <h4>Engineering Innovation Open Lab</h4>
          <p class="meta"><strong>Role:</strong> Co-Principal Investigator</p>
          <p class="meta"><strong>Sponsor:</strong> Illinois State University Strategic Initiative Request Fund</p>
          <p><strong>Focus:</strong> Development of an open, hands-on engineering learning environment that supports student innovation, experiential learning, interdisciplinary collaboration, and expanded access to technical resources beyond regular class and lab hours.</p>
          <span class="pill submitted">Proposal Submitted</span>
        </div>

        <div class="service-card research">
          <h4>Energy and Compute-Aware Edge Systems: A Pilot Framework</h4>
          <p class="meta"><strong>Role:</strong> Principal Investigator</p>
          <p class="meta"><strong>Sponsor:</strong> IIN</p>
          <p><strong>Focus:</strong> Pilot-scale research on energy and compute-aware edge systems, emphasizing lightweight intelligence, hardware-aware design, student involvement, and applied edge deployment.</p>
          <span class="pill pending">Not Funded</span>
        </div>

      </div>
    </div>

  </div>

  <div class="grid-2">
    <div class="section">
      <h2>📍 Service Timeline</h2>
      <div class="divider"></div>

      <div class="timeline">
        <div class="timeline-item">
          <div class="timeline-year">2026</div>
          <div class="timeline-title">Illinois State University Service</div>
          <div class="timeline-text">
            Faculty search committee, Student Project Expo judging, Redbird Day, continuity planning, K-12 outreach, IEEE invited lecture, and proposal development.
          </div>
        </div>

        <div class="timeline-item">
          <div class="timeline-year">2025-2026</div>
          <div class="timeline-title">Research and Proposal Leadership</div>
          <div class="timeline-text">
            Research grant proposals and strategic initiatives in RF characterization, open engineering labs, GPU-accelerated simulation, and edge systems.
          </div>
        </div>

        <div class="timeline-item">
          <div class="timeline-year">2023-2024</div>
          <div class="timeline-title">UMKC Service</div>
          <div class="timeline-text">
            Student Government Association senator role and engineering open house research demonstrations.
          </div>
        </div>
      </div>
    </div>

    <div class="section">
      <h2>🧭 Service Themes</h2>
      <div class="divider"></div>

      <div class="tag-cloud">
        <span class="tag">Institutional Service</span>
        <span class="tag">K-12 STEM Outreach</span>
        <span class="tag">Faculty Recruitment</span>
        <span class="tag">Curriculum Development</span>
        <span class="tag">Student Project Evaluation</span>
        <span class="tag">Professional Review</span>
        <span class="tag">IEEE Engagement</span>
        <span class="tag">Research Leadership</span>
        <span class="tag">Proposal Development</span>
        <span class="tag">Community Engagement</span>
      </div>
    </div>
  </div>

</div>

<script>
function openServiceTab(event, panelId) {
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
