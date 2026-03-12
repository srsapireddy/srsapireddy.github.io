---
title: ""
layout: single
permalink: /resume/
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
  --border: rgba(26,115,232,0.18);
  --tableBorder: #e6eef7;
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
  margin: 0 0 0.35rem 0;
  font-size: 1.9rem;
  line-height: 1.2;
  color: #0b1f44;
}
.page-hero p {
  margin: 0.55rem 0 0 0;
  color: var(--muted);
  font-size: 1.05rem;
  max-width: 85ch;
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
.section h3 {
  margin-top: 0;
  color: #0b1f44;
  font-size: 1.15rem;
  display: flex;
  align-items: center;
  gap: 0.55rem;
}
.section p { color: #202124; }

/* Divider */
.divider { height: 1px; background: rgba(26,115,232,0.12); margin: 0.3rem 0 0.9rem 0; }

/* Tables */
.table-wrap {
  border: 1px solid rgba(26,115,232,0.20);
  border-radius: 14px;
  background: #ffffff;
  overflow-x: auto; /* enables horizontal scroll on small screens instead of cutting */
  box-shadow: var(--shadow2);
}
table.resume-table {
  width: 100%;
  border-collapse: collapse;
  min-width: 900px; /* ensures the table doesn't squeeze and "cut" columns */
}
.resume-table th,
.resume-table td {
  border-bottom: 1px solid var(--tableBorder);
  padding: 0.85rem 0.8rem;
  text-align: left;
  font-size: 0.96rem;
  vertical-align: top;
}
.resume-table th {
  background: #f3f8ff;
  color: #0b1f44;
  font-weight: 800;
  border-bottom: 1px solid rgba(26,115,232,0.18);
}
.resume-table tr:hover td { background: #fbfdff; }

/* Logos */
.logo {
  max-height: 28px;
  max-width: 70px;
  object-fit: contain;
  float: right;
  margin-left: 10px;
  opacity: 0.95;
}

/* Lists */
.resume-list {
  list-style: disc;
  padding-left: 1.2rem;
  line-height: 1.65;
  margin: 0.25rem 0 0 0;
}

/* Scoped links */
.section a, .page-hero a {
  color: var(--blue);
  font-weight: 700;
  text-decoration: none;
}
.section a:hover, .page-hero a:hover { text-decoration: underline; }
</style>

<div class="page-hero">
  <h2>Resume Overview</h2>
  <p>
    A concise overview of education, experience, teaching, and selected outputs. For publications and additional details,
    please refer to the linked pages.
  </p>
  <div class="hero-links">
    <a class="btn-link" href="/publications/">Publications</a>
    <a class="btn-link secondary" href="/teaching/">Teaching</a>
    <a class="btn-link secondary" href="/insys-lab/">INSys Lab</a>
  </div>
</div>

<div class="section">
  <h3>Education</h3>
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
          <td>University of Missouri–Kansas City <img src="/images/UMKC.png" alt="UMKC Logo" class="logo"></td>
          <td>09/2021 – 07/2025</td>
        </tr>
        <tr>
          <td>M.S. in Computer Science</td>
          <td>University of Illinois–Springfield <img src="/images/UIS.png" alt="UIS Logo" class="logo"></td>
          <td>01/2017 – 12/2018</td>
        </tr>
        <tr>
          <td>M.S. in Electrical Engineering</td>
          <td>University of Missouri–Kansas City <img src="/images/UMKC.png" alt="UMKC Logo" class="logo"></td>
          <td>01/2015 – 12/2016</td>
        </tr>
        <tr>
          <td>B.Tech. in Electronics and Communication Engineering</td>
          <td>GRIET, Jawaharlal Nehru Technological University, Hyderabad <img src="/images/GRIET.png" alt="GRIET Logo" class="logo"></td>
          <td>09/2011 – 04/2014</td>
        </tr>
      </tbody>
    </table>
  </div>
</div>

<div class="section">
  <h3>Professional Development</h3>
  <div class="divider"></div>
  <div class="table-wrap">
    <table class="resume-table">
      <thead>
        <tr>
          <th>Program</th>
          <th>Institution</th>
          <th>Status</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Mini-MBA (Farmer School of Business)</td>
          <td>Miami University <img src="/images/miami.png" alt="Miami University Logo" class="logo"></td>
          <td>December 2025</td>
        </tr>
        <tr>
          <td>Advanced Diploma in Artificial Intelligence</td>
          <td>National Institute of Electronics and Information Technology (NIELIT), Calicut <img src="/images/CALICUT.png" alt="NIELIT Logo" class="logo"></td>
          <td>09/2019 – 01/2020</td>
        </tr>
      </tbody>
    </table>
  </div>
</div>

<div class="section">
  <h3>Teaching Experience</h3>
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
          <td>Assistant Professor (Tenure-Track)</td>
          <td>Illinois State University, Normal, IL</td>
          <td>ELE 260, ELE 265, ELE 280</td>
        </tr>
        <tr>
          <td>Instructor</td>
          <td>University of Missouri–Kansas City</td>
          <td>ENGR E&amp;C 216, ENGR E&amp;C 226, ENGR E&amp;C 447/5547, ENGR E&amp;C 402/5533</td>
        </tr>
        <tr>
          <td>Teaching Assistant</td>
          <td>University of Missouri–Kansas City</td>
          <td>ENGR E&amp;C 442/5542, ENGR E&amp;C 228, ENGR E&amp;C 402/403</td>
        </tr>
      </tbody>
    </table>
  </div>
</div>

<div class="section">
  <h3>Research and Industry Experience</h3>
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
          <td>09/2021 – 07/2022</td>
        </tr>
        <tr>
          <td>AI Intern</td>
          <td>SmartBridge Pvt. Ltd.</td>
          <td>06/2020 – 07/2020</td>
        </tr>
      </tbody>
    </table>
  </div>
</div>

<div class="section">
  <h3>Research Interests</h3>
  <div class="divider"></div>
  <ul class="resume-list">
    <li>Hardware-aware and low-power machine learning for edge-intelligent systems</li>
    <li>RF signal processing and modulation classification using statistical and time–frequency methods</li>
    <li>Design of hardware-efficient neural networks, including custom and piecewise-linear activation functions</li>
    <li>VLSI system design and physical implementation for energy-efficient computing</li>
    <li>Embedded and system-on-chip (SoC) architectures for signal intelligence applications</li>
  </ul>
</div>

<div class="section">
  <h3>Selected Publications</h3>
  <div class="divider"></div>
  <div class="table-wrap">
    <table class="resume-table">
      <thead>
        <tr>
          <th>Title</th>
          <th>Venue</th>
          <th>Year / Notes</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Re-Visiting R: Statistical Envelope Analysis for RF Modulation Classification (Best Paper Award)</td>
          <td>IEEE RFCoN</td>
          <td>2025</td>
        </tr>
        <tr>
          <td>Hardware-Efficient Custom Activation Functions for LSTM Networks</td>
          <td>ACM GLSVLSI</td>
          <td>2025</td>
        </tr>
        <tr>
          <td>Piecewise Linear Approximation of Activation Functions for Neural Networks</td>
          <td>MDPI Memories</td>
          <td>2024</td>
        </tr>
        <tr>
          <td>A Review of Crosstalk-Based Polymorphic Circuit Design</td>
          <td>MDPI Memories</td>
          <td>2024</td>
        </tr>
      </tbody>
    </table>
  </div>
  <p style="margin-top:0.9rem;">
    <a href="/publications/">View complete list of publications</a>
  </p>
</div>

<div class="section">
  <h3>Awards and Honors</h3>
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
          <td>University of Missouri–Kansas City</td>
          <td>2025</td>
        </tr>
        <tr>
          <td>Dean’s International Scholar Award</td>
          <td>University of Missouri–Kansas City</td>
          <td>2015–2016</td>
        </tr>
        <tr>
          <td>IEEE–Eta Kappa Nu (HKN) Honor Society Member</td>
          <td>University of Missouri–Kansas City</td>
          <td>Inducted</td>
        </tr>
        <tr>
          <td>Second Place, UMKC Hack-A-Roo (Entrepreneur Track)</td>
          <td>University of Missouri–Kansas City</td>
          <td>Fall 2022</td>
        </tr>
        <tr>
          <td>Third Place, UMKC Hack-A-Roo (CS/IT Track)</td>
          <td>University of Missouri–Kansas City</td>
          <td>Fall 2021</td>
        </tr>
      </tbody>
    </table>
  </div>
</div>

<div class="section">
  <h3>Certifications and Training</h3>
  <div class="divider"></div>
  <div class="table-wrap">
    <table class="resume-table">
      <thead>
        <tr>
          <th>Program</th>
          <th>Institution</th>
          <th>Year</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Product Management</td>
          <td>Confederation of Indian Industry (CII)</td>
          <td>2023</td>
        </tr>
        <tr>
          <td>Accelerated Artificial Intelligence</td>
          <td>Centre for Development of Advanced Computing (CDAC)</td>
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
