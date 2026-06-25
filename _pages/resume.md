---
title: "Resume"
layout: single
permalink: /resume/
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
  --tableBorder: #e6eef7;
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

.resume-wrap {
  animation: fadeInUp 0.8s ease-in-out;
}

/* Hero */
.resume-hero {
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

.resume-hero::before {
  content: "";
  position: absolute;
  inset: 0;
  background-image:
    linear-gradient(rgba(26,115,232,0.06) 1px, transparent 1px),
    linear-gradient(90deg, rgba(26,115,232,0.06) 1px, transparent 1px);
  background-size: 34px 34px;
  pointer-events: none;
}

.resume-hero-content {
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

.resume-hero h1 {
  margin: 0;
  font-size: 2.15rem;
  line-height: 1.15;
  color: var(--text);
}

.resume-hero .subtitle {
  margin-top: 0.55rem;
  color: #202124;
  font-size: 1.08rem;
  font-weight: 650;
}

.resume-hero p {
  margin: 0.8rem 0 0 0;
  color: var(--muted);
  font-size: 1.03rem;
  line-height: 1.65;
  max-width: 86ch;
}

/* Hero buttons */
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

/* General section cards */
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

  .resume-hero {
    padding: 1.5rem 1.1rem;
  }

  .resume-hero h1 {
    font-size: 1.65rem;
  }
}

/* Focus cards */
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

/* Tables */
.table-wrap {
  border: 1px solid rgba(26,115,232,0.20);
  border-radius: 14px;
  background: #ffffff;
  overflow-x: auto;
  box-shadow: var(--shadow2);
}

table.resume-table {
  width: 100%;
  border-collapse: collapse;
  min-width: 850px;
}

.resume-table th,
.resume-table td {
  border-bottom: 1px solid var(--tableBorder);
  padding: 0.85rem 0.8rem;
  text-align: left;
  font-size: 0.95rem;
  vertical-align: top;
}

.resume-table th {
  background: #f3f8ff;
  color: var(--text);
  font-weight: 850;
  border-bottom: 1px solid rgba(26,115,232,0.18);
}

.resume-table tr:hover td {
  background: #fbfdff;
}

.resume-table tr:last-child td {
  border-bottom: none;
}

/* Logos */
.logo {
  max-height: 28px;
  max-width: 70px;
  object-fit: contain;
  float: right;
  margin-left: 10px;
  opacity: 0.95;
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

.pub-note {
  color: var(--muted);
  font-size: 0.88rem;
  margin-top: 0.35rem;
}

/* Scoped links */
.section a,
.resume-hero a {
  color: var(--blue);
  font-weight: 800;
  text-decoration: none;
}

.section a:hover,
.resume-hero a:hover {
  text-decoration: underline;
}
</style>

<div class="resume-wrap">

  <div class="resume-hero">
    <div class="resume-hero-content">
      <span class="hero-kicker">Academic Resume · Research · Teaching · Engineering</span>

      <h1>Srinivas Rahul Sapireddy, Ph.D.</h1>

      <div class="subtitle">
        Assistant Professor, Electrical Engineering · Illinois State University
      </div>

      <p>
        A structured overview of my academic background, teaching experience, research direction,
        technical expertise, publications, and recognitions. My work connects hardware-aware
        artificial intelligence, RF signal intelligence, edge computing, and VLSI system design.
      </p>

      <div class="badges">
        <span class="badge">Hardware-Aware AI</span>
        <span class="badge">RF Signal Intelligence</span>
        <span class="badge">Edge Computing</span>
        <span class="badge">VLSI Physical Design</span>
      </div>

      <div class="hero-links">
        <a class="btn-link" href="/publications/">Publications</a>
        <a class="btn-link secondary" href="/teaching/">Teaching</a>
        <a class="btn-link secondary" href="/insys-lab/">INSys Lab</a>
        <a class="btn-link secondary" href="/about/">About</a>
      </div>
    </div>
  </div>

  <div class="impact-grid">
    <div class="impact-card">
      <div class="big">Ph.D.</div>
      <div class="label">Electrical and Computer Engineering</div>
      <div class="small">University of Missouri-Kansas City</div>
    </div>

    <div class="impact-card">
      <div class="big">EE</div>
      <div class="label">Assistant Professor</div>
      <div class="small">Illinois State University</div>
    </div>

    <div class="impact-card">
      <div class="big">AI</div>
      <div class="label">Hardware-Aware ML</div>
      <div class="small">Low-power and edge systems</div>
    </div>

    <div class="impact-card">
      <div class="big">RF</div>
      <div class="label">Signal Intelligence</div>
      <div class="small">Modulation classification</div>
    </div>
  </div>

  <div class="grid-3">
    <div class="focus-card">
      <div class="focus-icon">🎓</div>
      <h3>Academic Preparation</h3>
      <p>
        Multidisciplinary training across electrical engineering, computer science,
        artificial intelligence, and hardware-oriented computing.
      </p>
    </div>

    <div class="focus-card">
      <div class="focus-icon">📚</div>
      <h3>Teaching Profile</h3>
      <p>
        Teaching experience across logic design, engineering computation, ASIC physical design,
        analog IC design, and computer design topics.
      </p>
    </div>

    <div class="focus-card">
      <div class="focus-icon">🔬</div>
      <h3>Research Direction</h3>
      <p>
        Research centered on low-power AI, RF signal processing, efficient neural networks,
        and hardware-software co-design.
      </p>
    </div>
  </div>

  <div class="grid-2">
    <div class="section">
      <h2>📍 Academic Path</h2>
      <div class="divider"></div>

      <div class="timeline">
        <div class="timeline-item">
          <div class="timeline-year">2026</div>
          <div class="timeline-title">Assistant Professor, Electrical Engineering</div>
          <div class="timeline-text">Illinois State University, College of Engineering.</div>
        </div>

        <div class="timeline-item">
          <div class="timeline-year">2021 - 2025</div>
          <div class="timeline-title">Ph.D. in Electrical and Computer Engineering</div>
          <div class="timeline-text">University of Missouri-Kansas City.</div>
        </div>

        <div class="timeline-item">
          <div class="timeline-year">2017 - 2018</div>
          <div class="timeline-title">M.S. in Computer Science</div>
          <div class="timeline-text">University of Illinois-Springfield.</div>
        </div>

        <div class="timeline-item">
          <div class="timeline-year">2015 - 2016</div>
          <div class="timeline-title">M.S. in Electrical Engineering</div>
          <div class="timeline-text">University of Missouri-Kansas City.</div>
        </div>
      </div>
    </div>

    <div class="section">
      <h2>🧭 Research Interests</h2>
      <div class="divider"></div>

      <div class="tag-cloud">
        <span class="tag">Hardware-Aware Machine Learning</span>
        <span class="tag">Low-Power Edge AI</span>
        <span class="tag">RF Modulation Classification</span>
        <span class="tag">Statistical Feature Engineering</span>
        <span class="tag">Time-Frequency Analysis</span>
        <span class="tag">Custom Activation Functions</span>
        <span class="tag">VLSI Physical Design</span>
        <span class="tag">RTL-to-GDSII Flow</span>
        <span class="tag">Embedded AI Accelerators</span>
        <span class="tag">System-on-Chip Architectures</span>
      </div>
    </div>
  </div>

  <div class="section">
    <h2>🎓 Education</h2>
    <div class="divider"></div>

    <div class="table-wrap">
      <table class="resume-table">
        <thead>
          <tr>
            <th>Degree</th>
            <th>Institution</th>
            <th>Duration</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Ph.D. in Electrical and Computer Engineering</td>
            <td>University of Missouri-Kansas City <img src="/images/UMKC.png" alt="UMKC Logo" class="logo"></td>
            <td>09/2021 - 07/2025</td>
          </tr>
          <tr>
            <td>M.S. in Computer Science</td>
            <td>University of Illinois-Springfield <img src="/images/UIS.png" alt="UIS Logo" class="logo"></td>
            <td>01/2017 - 12/2018</td>
          </tr>
          <tr>
            <td>M.S. in Electrical Engineering</td>
            <td>University of Missouri-Kansas City <img src="/images/UMKC.png" alt="UMKC Logo" class="logo"></td>
            <td>01/2015 - 12/2016</td>
          </tr>
          <tr>
            <td>B.Tech. in Electronics and Communication Engineering</td>
            <td>GRIET, Jawaharlal Nehru Technological University, Hyderabad <img src="/images/GRIET.png" alt="GRIET Logo" class="logo"></td>
            <td>09/2011 - 04/2014</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>

  <div class="grid-2">
    <div class="section">
      <h2>👨‍🏫 Teaching Experience</h2>
      <div class="divider"></div>

      <div class="table-wrap">
        <table class="resume-table">
          <thead>
            <tr>
              <th>Role</th>
              <th>Institution</th>
              <th>Courses</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Assistant Professor, Tenure-Track</td>
              <td>Illinois State University, Normal, IL</td>
              <td>ELE 260, ELE 265, ELE 280</td>
            </tr>
            <tr>
              <td>Instructor</td>
              <td>University of Missouri-Kansas City</td>
              <td>ENGR E&amp;C 216, ENGR E&amp;C 226, ENGR E&amp;C 447/5547, ENGR E&amp;C 402/5533</td>
            </tr>
            <tr>
              <td>Teaching Assistant</td>
              <td>University of Missouri-Kansas City</td>
              <td>ENGR E&amp;C 442/5542, ENGR E&amp;C 228, ENGR E&amp;C 402/403</td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>

    <div class="section">
      <h2>💼 Research and Industry Experience</h2>
      <div class="divider"></div>

      <div class="table-wrap">
        <table class="resume-table">
          <thead>
            <tr>
              <th>Role</th>
              <th>Organization</th>
              <th>Duration</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Research Assistant</td>
              <td>Missouri Institute of Defense and Energy</td>
              <td>09/2021 - 07/2022</td>
            </tr>
            <tr>
              <td>AI Intern</td>
              <td>SmartBridge Pvt. Ltd.</td>
              <td>06/2020 - 07/2020</td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </div>

  <div class="section">
    <h2>🛠️ Technical Expertise</h2>
    <div class="divider"></div>

    <div class="tag-cloud">
      <span class="tag">Python</span>
      <span class="tag">C/C++</span>
      <span class="tag">Verilog</span>
      <span class="tag">TCL</span>
      <span class="tag">SQL</span>
      <span class="tag">PyTorch</span>
      <span class="tag">TensorFlow Lite</span>
      <span class="tag">Scikit-learn</span>
      <span class="tag">Docker</span>
      <span class="tag">Yosys</span>
      <span class="tag">OpenSTA</span>
      <span class="tag">Cadence</span>
      <span class="tag">Synopsys</span>
      <span class="tag">RTL Design</span>
      <span class="tag">Physical Design</span>
      <span class="tag">Machine Learning</span>
      <span class="tag">RF Signal Processing</span>
    </div>
  </div>

  <div class="section">
    <h2>📝 Selected Publications</h2>
    <div class="divider"></div>

    <div class="grid-2">
      <div>
        <div class="pub-card">
          <span class="pub-venue">IEEE RFCoN 2025</span>
          <div class="pub-title">
            Re-Visiting R: Statistical Envelope Analysis for RF Modulation Classification
          </div>
          <div class="pub-note">Best Paper Award</div>
        </div>

        <div class="pub-card">
          <span class="pub-venue">ACM GLSVLSI 2025</span>
          <div class="pub-title">
            Hardware-Efficient Custom Activation Functions for LSTM Networks
          </div>
        </div>
      </div>

      <div>
        <div class="pub-card">
          <span class="pub-venue">Elsevier Memories 2025</span>
          <div class="pub-title">
            Piecewise Linear Approximation of Activation Functions for Neural Networks
          </div>
        </div>

        <div class="pub-card">
          <span class="pub-venue">MDPI Electronics 2024</span>
          <div class="pub-title">
            A Review of Crosstalk-Based Polymorphic Circuit Design
          </div>
        </div>
      </div>
    </div>

    <p>
      <a href="/publications/">View complete list of publications</a>
    </p>
  </div>

  <div class="grid-2">
    <div class="section">
      <h2>🏆 Awards and Honors</h2>
      <div class="divider"></div>

      <div class="table-wrap">
        <table class="resume-table">
          <thead>
            <tr>
              <th>Award</th>
              <th>Organization</th>
              <th>Year</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>CS Balaji Krithikaivasan Travel Grant</td>
              <td>University of Missouri-Kansas City</td>
              <td>2025</td>
            </tr>
            <tr>
              <td>Dean's International Scholar Award</td>
              <td>University of Missouri-Kansas City</td>
              <td>2015-2016</td>
            </tr>
            <tr>
              <td>IEEE-Eta Kappa Nu Honor Society Member</td>
              <td>University of Missouri-Kansas City</td>
              <td>Inducted</td>
            </tr>
            <tr>
              <td>Second Place, UMKC Hack-A-Roo, Entrepreneur Track</td>
              <td>University of Missouri-Kansas City</td>
              <td>Fall 2022</td>
            </tr>
            <tr>
              <td>Third Place, UMKC Hack-A-Roo, CS/IT Track</td>
              <td>University of Missouri-Kansas City</td>
              <td>Fall 2021</td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>

    <div class="section">
      <h2>📜 Certifications and Training</h2>
      <div class="divider"></div>

      <div class="table-wrap">
        <table class="resume-table">
          <thead>
            <tr>
              <th>Program</th>
              <th>Institution</th>
              <th>Year / Status</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Mini-MBA, Farmer School of Business</td>
              <td>Miami University <img src="/images/miami.png" alt="Miami University Logo" class="logo"></td>
              <td>December 2025</td>
            </tr>
            <tr>
              <td>Advanced Diploma in Artificial Intelligence</td>
              <td>NIELIT, Calicut <img src="/images/CALICUT.png" alt="NIELIT Logo" class="logo"></td>
              <td>09/2019 - 01/2020</td>
            </tr>
            <tr>
              <td>Product Management</td>
              <td>Confederation of Indian Industry</td>
              <td>2023</td>
            </tr>
            <tr>
              <td>Accelerated Artificial Intelligence</td>
              <td>Centre for Development of Advanced Computing</td>
              <td>2022</td>
            </tr>
            <tr>
              <td>Statistical Learning</td>
              <td>Stanford University</td>
              <td>2017</td>
            </tr>
            <tr>
              <td>MLOps</td>
              <td>Duke University</td>
              <td>2023</td>
            </tr>
            <tr>
              <td>Mathematics for Machine Learning</td>
              <td>Imperial College London</td>
              <td>2023</td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </div>

</div>
