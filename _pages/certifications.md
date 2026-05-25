---
title: "Certifications"
layout: single
permalink: /certifications/
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
  --border:rgba(26,115,232,0.18);
  --shadow:0 10px 30px rgba(0,0,0,0.08);
  --shadow2:0 2px 10px rgba(0,0,0,0.05);
  --radius:18px;
  --radius2:14px;
}

@keyframes fadeInUp{
  from{opacity:0; transform:translateY(14px);}
  to{opacity:1; transform:translateY(0);}
}

@keyframes slideTrack{
  from{transform:translateX(0);}
  to{transform:translateX(-50%);}
}

.cert-wrap{
  animation:fadeInUp 0.85s ease-in-out;
}

/* Hero */
.cert-hero{
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

.cert-hero::before{
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

.cert-hero h1{
  margin:0;
  font-size:2.15rem;
  line-height:1.15;
  color:var(--text);
}

.cert-hero p{
  margin:0.75rem 0 0 0;
  color:var(--muted);
  font-size:1.04rem;
  line-height:1.65;
  max-width:92ch;
}

/* Hero badges and buttons */
.hero-row{
  display:flex;
  gap:1rem;
  flex-wrap:wrap;
  align-items:center;
  justify-content:space-between;
  margin-top:1.1rem;
}

.hero-badges{
  display:flex;
  gap:0.55rem;
  flex-wrap:wrap;
}

.pill{
  display:inline-flex;
  align-items:center;
  gap:0.42rem;
  padding:0.36rem 0.72rem;
  border-radius:999px;
  background:#ffffff;
  border:1px solid rgba(26,115,232,0.22);
  color:var(--text);
  box-shadow:var(--shadow2);
  font-size:0.88rem;
  font-weight:850;
}

.pill.red{
  border-color:rgba(220,20,60,0.30);
  color:#7a0b1f;
  background:rgba(220,20,60,0.06);
}

.pill.green{
  border-color:rgba(26,127,61,0.25);
  color:var(--green);
  background:rgba(26,127,61,0.06);
}

.pill svg{
  width:16px;
  height:16px;
}

.hero-actions{
  display:flex;
  gap:0.7rem;
  flex-wrap:wrap;
}

.cta{
  display:inline-flex;
  align-items:center;
  padding:0.58rem 0.92rem;
  border-radius:12px;
  background:#ffffff;
  color:var(--blue) !important;
  border:1px solid rgba(26,115,232,0.25);
  text-decoration:none !important;
  font-weight:850;
  box-shadow:var(--shadow2);
  transition:0.2s ease-in-out;
}

.cta:hover{
  transform:translateY(-2px);
  background:#f3f8ff;
  text-decoration:none !important;
}

.cta.primary{
  background:var(--blue);
  color:#ffffff !important;
  border-color:var(--blue);
}

.cta.primary:hover{
  background:var(--blue2);
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
  animation:slideTrack 34s linear infinite;
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
  font-size:1.58rem;
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

/* Tabs */
.cert-tabs{
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

/* Category heading */
.category-head{
  padding:1rem 1.1rem;
  border-radius:14px;
  background:linear-gradient(135deg,#ffffff 0%,#f7fbff 100%);
  border:1px solid rgba(26,115,232,0.18);
  box-shadow:var(--shadow2);
  margin-bottom:1rem;
}

.category-head h3{
  margin:0;
  color:var(--text);
  font-size:1.12rem;
}

.category-head p{
  margin:0.35rem 0 0 0;
  color:var(--muted);
  font-size:0.94rem;
}

/* Certificate grid */
.cert-grid{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(230px,1fr));
  gap:1.1rem;
}

.cert-card{
  background:#ffffff;
  border:1px solid rgba(26,115,232,0.16);
  border-radius:16px;
  padding:0.7rem;
  transition:0.22s ease-in-out;
  position:relative;
  box-shadow:var(--shadow2);
  overflow:hidden;
}

.cert-card:hover{
  transform:translateY(-3px);
  background:#fbfdff;
  box-shadow:var(--shadow);
  border-color:rgba(26,115,232,0.35);
}

.cert-card::before{
  content:"";
  position:absolute;
  top:0;
  left:0;
  height:5px;
  width:100%;
  background:linear-gradient(90deg,var(--blue),var(--isu));
}

.cert-card img{
  width:100%;
  border-radius:12px;
  cursor:zoom-in;
  display:block;
  background:#ffffff;
  border:1px solid rgba(26,115,232,0.08);
}

.cert-title{
  margin-top:0.65rem;
  font-size:0.93rem;
  font-weight:900;
  color:var(--text);
  line-height:1.38;
}

.cert-sub{
  margin-top:0.28rem;
  color:var(--muted);
  font-size:0.86rem;
  line-height:1.35;
}

/* Corner tags */
.corner-tag{
  position:absolute;
  top:12px;
  left:12px;
  background:rgba(26,115,232,0.92);
  color:#ffffff;
  font-weight:900;
  font-size:0.74rem;
  padding:0.22rem 0.48rem;
  border-radius:999px;
  border:1px solid rgba(255,255,255,0.3);
  z-index:2;
}

.corner-tag.red{
  background:rgba(220,20,60,0.92);
}

.corner-tag.green{
  background:rgba(26,127,61,0.92);
}

.corner-tag.gold{
  background:rgba(122,90,0,0.92);
}

/* Badge cards */
.badge-card{
  text-align:center;
  padding:1rem 0.9rem;
}

.badge-card img{
  width:165px;
  height:auto;
  margin:0.4rem auto 0.2rem auto;
  border:none;
}

/* Tags */
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

/* Lightbox */
.lightbox{
  position:fixed;
  inset:0;
  width:100vw;
  height:100vh;
  background:rgba(0,0,0,0.9);
  display:none;
  align-items:center;
  justify-content:center;
  z-index:2000;
  padding:18px;
}

.lightbox img{
  max-width:92vw;
  max-height:92vh;
  border-radius:14px;
  box-shadow:0 0 22px rgba(255,255,255,0.18);
}

.lightbox .hint{
  position:fixed;
  bottom:18px;
  left:50%;
  transform:translateX(-50%);
  color:rgba(255,255,255,0.85);
  font-weight:850;
  font-size:0.92rem;
  background:rgba(0,0,0,0.35);
  padding:0.35rem 0.7rem;
  border-radius:999px;
  border:1px solid rgba(255,255,255,0.2);
}

/* Responsive */
@media (max-width:950px){
  .impact-grid{
    grid-template-columns:1fr 1fr;
  }
}

@media (max-width:700px){
  .cert-hero{
    padding:1.5rem 1.1rem;
  }

  .cert-hero h1{
    font-size:1.65rem;
  }

  .impact-grid{
    grid-template-columns:1fr;
  }
}
</style>

<div class="cert-wrap">

  <div class="cert-hero">
    <div class="hero-content">
      <span class="hero-kicker">Certifications · Training · Credentials · Honors</span>

      <h1>Certifications, Training, and Credentials</h1>

      <p>
        A visual portfolio of certifications, professional development programs, degrees, memberships,
        awards, and credentials across management, semiconductor technology, machine learning,
        hardware systems, cloud computing, research methods, and professional societies.
      </p>

      <div class="hero-row">
        <div class="hero-badges">
          <span class="pill">
            <svg viewBox="0 0 24 24" fill="none" aria-hidden="true">
              <path d="M12 2l3 7h7l-5.5 4.2L18.5 21 12 16.9 5.5 21l2-7.8L2 9h7l3-7Z" stroke="currentColor" stroke-width="2" stroke-linejoin="round"/>
            </svg>
            Certifications
          </span>

          <span class="pill red">
            <svg viewBox="0 0 24 24" fill="none" aria-hidden="true">
              <path d="M6 7h12M6 12h12M6 17h12" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
            </svg>
            Training and Development
          </span>

          <span class="pill green">
            <svg viewBox="0 0 24 24" fill="none" aria-hidden="true">
              <path d="M12 3l10 6-10 6L2 9l10-6Z" stroke="currentColor" stroke-width="2" stroke-linejoin="round"/>
              <path d="M2 9v6l10 6 10-6V9" stroke="currentColor" stroke-width="2" stroke-linejoin="round"/>
            </svg>
            Degrees and Memberships
          </span>
        </div>

        <div class="hero-actions">
          <a class="cta" href="/resume/">Resume</a>
          <a class="cta primary" href="/publications/">Publications</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sliding-bar">
    <div class="slide-track">
      <div class="slide-item"><span>●</span> Management Certificates</div>
      <div class="slide-item"><span>●</span> Semiconductor Fabrication</div>
      <div class="slide-item"><span>●</span> Machine Learning</div>
      <div class="slide-item"><span>●</span> Cloud and MLOps</div>
      <div class="slide-item"><span>●</span> Hardware Security</div>
      <div class="slide-item"><span>●</span> Degrees and Diplomas</div>
      <div class="slide-item"><span>●</span> Professional Memberships</div>
      <div class="slide-item"><span>●</span> Honors and Awards</div>

      <div class="slide-item"><span>●</span> Management Certificates</div>
      <div class="slide-item"><span>●</span> Semiconductor Fabrication</div>
      <div class="slide-item"><span>●</span> Machine Learning</div>
      <div class="slide-item"><span>●</span> Cloud and MLOps</div>
      <div class="slide-item"><span>●</span> Hardware Security</div>
      <div class="slide-item"><span>●</span> Degrees and Diplomas</div>
      <div class="slide-item"><span>●</span> Professional Memberships</div>
      <div class="slide-item"><span>●</span> Honors and Awards</div>
    </div>
  </div>

  <div class="impact-grid">
    <div class="impact-card">
      <div class="impact-number">Mgmt</div>
      <div class="impact-label">Management Training</div>
      <div class="impact-sub">Accounting and miniMBA credentials</div>
    </div>

    <div class="impact-card">
      <div class="impact-number">AI</div>
      <div class="impact-label">Machine Learning</div>
      <div class="impact-sub">MLOps, cloud, math, and AI training</div>
    </div>

    <div class="impact-card">
      <div class="impact-number">EE</div>
      <div class="impact-label">Hardware Systems</div>
      <div class="impact-sub">Semiconductors, FPGA, embedded systems</div>
    </div>

    <div class="impact-card">
      <div class="impact-number">Prof</div>
      <div class="impact-label">Memberships and Honors</div>
      <div class="impact-sub">IEEE, ACM, AAAI, HKN, awards</div>
    </div>
  </div>

  <div class="section">
    <h2>📂 Credential Categories</h2>
    <div class="divider"></div>

    <p>
      Use the tabs below to view certifications, training records, degrees, professional memberships,
      honors, and hackathon awards. Click any certificate image to view it fullscreen.
    </p>

    <div class="cert-tabs">
      <button class="tab-button active" onclick="openCertTab(event, 'management-tab')">Management</button>
      <button class="tab-button" onclick="openCertTab(event, 'certifications-tab')">Certifications</button>
      <button class="tab-button" onclick="openCertTab(event, 'training-tab')">Training</button>
      <button class="tab-button" onclick="openCertTab(event, 'professional-tab')">Professional Credentials</button>
      <button class="tab-button" onclick="openCertTab(event, 'degrees-tab')">Degrees</button>
      <button class="tab-button" onclick="openCertTab(event, 'badges-tab')">Badges</button>
      <button class="tab-button" onclick="openCertTab(event, 'honors-tab')">Honors</button>
      <button class="tab-button" onclick="openCertTab(event, 'memberships-tab')">Memberships</button>
      <button class="tab-button" onclick="openCertTab(event, 'hackathon-tab')">Hackathons</button>
    </div>

    <div id="management-tab" class="tab-panel active">
      <div class="category-head">
        <h3>Certifications in Management</h3>
        <p>Academic and professional certificates connected to management, accounting, and business decision-making.</p>
      </div>

      <div class="cert-grid lightbox-gallery">
        <div class="cert-card">
          <span class="corner-tag">Cert</span>
          <img src="/images/UIUC_1.png" alt="Managerial Accounting Cost Behaviors Systems and Analysis">
          <div class="cert-title">Managerial Accounting: Cost Behaviors, Systems, and Analysis</div>
          <div class="cert-sub">University of Illinois Urbana-Champaign</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag">Cert</span>
          <img src="/images/UIUC_2.png" alt="Managerial Accounting Tools for Business Decisions">
          <div class="cert-title">Managerial Accounting: Tools for Facilitating and Guiding Business Decisions</div>
          <div class="cert-sub">University of Illinois Urbana-Champaign</div>
        </div>
      </div>
    </div>

    <div id="certifications-tab" class="tab-panel">
      <div class="category-head">
        <h3>Certifications</h3>
        <p>Academic and professional certificates across semiconductor technology, machine learning, research methods, cloud, programming, and hardware security.</p>
      </div>

      <div class="cert-grid lightbox-gallery">
        <div class="cert-card">
          <span class="corner-tag">Cert</span>
          <img src="/images/purdue.jpeg" alt="Semiconductor Fabrication">
          <div class="cert-title">Semiconductor Fabrication</div>
          <div class="cert-sub">Purdue University, University of Texas Austin</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag">Cert</span>
          <img src="/images/statistical_learning.png" alt="Statistical Learning">
          <div class="cert-title">Statistical Learning</div>
          <div class="cert-sub">Stanford University</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag">Cert</span>
          <img src="/images/mlops_specialization.jpg" alt="MLOps Specialization">
          <div class="cert-title">MLOps Specialization</div>
          <div class="cert-sub">Duke University</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag">Cert</span>
          <img src="/images/mathematics_ml.png" alt="Mathematics for Machine Learning">
          <div class="cert-title">Mathematics for Machine Learning</div>
          <div class="cert-sub">Imperial College London</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag">Cert</span>
          <img src="/images/device_packaging.png" alt="Device and System Packaging">
          <div class="cert-title">Introduction to Device and System Packaging</div>
          <div class="cert-sub">Georgia Tech</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag">Cert</span>
          <img src="/images/Chandigarh.png" alt="MEAN Stack Development">
          <div class="cert-title">MEAN Stack Development: Contact List CRUD</div>
          <div class="cert-sub">NIELIT Chandigarh</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag">Cert</span>
          <img src="/images/LONDON.png" alt="Understanding Research Methods">
          <div class="cert-title">Understanding Research Methods</div>
          <div class="cert-sub">University of London</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag">Cert</span>
          <img src="/images/ECOLE.png" alt="Scientific Paper Writing">
          <div class="cert-title">How to Write and Publish a Scientific Paper</div>
          <div class="cert-sub">Ecole Polytechnique, France</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag">Cert</span>
          <img src="/images/GOOGLE.png" alt="Google Cloud ML">
          <div class="cert-title">Managing ML Projects with Google Cloud</div>
          <div class="cert-sub">Google Cloud</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag">Cert</span>
          <img src="/images/LEARN.png" alt="Azure AI Applications">
          <div class="cert-title">Developing AI Applications on Azure</div>
          <div class="cert-sub">LearnQuest</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag">Cert</span>
          <img src="/images/AWS.png" alt="AWS Machine Learning">
          <div class="cert-title">Getting Started with AWS Machine Learning</div>
          <div class="cert-sub">AWS</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag">Cert</span>
          <img src="/images/CODE.png" alt="Code Yourself Programming">
          <div class="cert-title">Code Yourself! An Introduction to Programming</div>
          <div class="cert-sub">University of Edinburgh and Universidad ORT Uruguay</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag">Cert</span>
          <img src="/images/HARDWARE.png" alt="Hardware Security">
          <div class="cert-title">Hardware Security</div>
          <div class="cert-sub">University of Maryland, College Park</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag">Cert</span>
          <img src="/images/GORAKHPUR.png" alt="Embedded System Design">
          <div class="cert-title">Embedded System Design</div>
          <div class="cert-sub">NIELIT Gorakhpur</div>
        </div>
      </div>
    </div>

    <div id="training-tab" class="tab-panel">
      <div class="category-head">
        <h3>Training and Professional Development</h3>
        <p>Workshops, internships, structured programs, and applied technical training.</p>
      </div>

      <div class="cert-grid lightbox-gallery">
        <div class="cert-card">
          <span class="corner-tag red">Training</span>
          <img src="/images/FPGA.png" alt="FPGA Training">
          <div class="cert-title">Summer Internship on FPGA-Based Embedded Systems for DSP</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag red">Training</span>
          <img src="/images/NEURO.png" alt="Computational Neuroscience">
          <div class="cert-title">Internship on Hardware for Computational Neuroscience</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag red">Program</span>
          <img src="/images/product_management.png" alt="Product Management">
          <div class="cert-title">Product Management Program</div>
          <div class="cert-sub">Confederation of Indian Industry</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag red">Training</span>
          <img src="/images/semiconductor_basics.png" alt="Semiconductor Basics">
          <div class="cert-title">Basics of Semiconductor Device Technology</div>
          <div class="cert-sub">Indian Institute of Science</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag red">Training</span>
          <img src="/images/TORMP.png" alt="Manuscript Drafting and Publishing">
          <div class="cert-title">Manuscript Drafting and Publishing</div>
          <div class="cert-sub">Eudoxia Research Center</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag red">Training</span>
          <img src="/images/REGEX.png" alt="MEARN Stack Training">
          <div class="cert-title">Industrial Training: MEARN Stack Development</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag red">Workshop</span>
          <img src="/images/Automobile.png" alt="Automobile Workshop">
          <div class="cert-title">Automobile Engineering and IC Engine Workshop</div>
          <div class="cert-sub">IIT Kanpur</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag red">Workshop</span>
          <img src="/images/MADRAS.png" alt="AI and Reinforcement Learning Workshop">
          <div class="cert-title">AI and Reinforcement Learning Workshop</div>
          <div class="cert-sub">IIT Madras</div>
        </div>
      </div>
    </div>

    <div id="professional-tab" class="tab-panel">
      <div class="category-head">
        <h3>Professional Certifications</h3>
        <p>Industry-recognized and professional credentials.</p>
      </div>

      <div class="cert-grid lightbox-gallery">
        <div class="cert-card">
          <span class="corner-tag green">Pro</span>
          <img src="/images/network_security.jpeg" alt="Network Security Associate">
          <div class="cert-title">Network Security Associate</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag green">Pro</span>
          <img src="/images/intel_cloud.png" alt="Intel Cloud Business Professional">
          <div class="cert-title">Intel Solution Pro: Cloud Business Professional</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag green">Pro</span>
          <img src="/images/ccna.png" alt="Cisco Certified Network Associate">
          <div class="cert-title">Cisco Certified Network Associate (X)</div>
        </div>
      </div>
    </div>

    <div id="degrees-tab" class="tab-panel">
      <div class="category-head">
        <h3>Degrees and Diplomas</h3>
        <p>Academic degrees and formal diploma credentials.</p>
      </div>

      <div class="cert-grid lightbox-gallery">
        <div class="cert-card">
          <span class="corner-tag gold">Degree</span>
          <img src="/images/PHD.png" alt="PhD ECE Degree">
          <div class="cert-title">Ph.D. in Electrical and Computer Engineering</div>
          <div class="cert-sub">University of Missouri-Kansas City</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag gold">Degree</span>
          <img src="/images/ms_cs_uis.png" alt="MS CS Degree">
          <div class="cert-title">M.S. in Computer Science</div>
          <div class="cert-sub">University of Illinois, Springfield</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag gold">Degree</span>
          <img src="/images/ms_ee_umkc.png" alt="MS EE Degree">
          <div class="cert-title">M.S. in Electrical Engineering</div>
          <div class="cert-sub">University of Missouri-Kansas City</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag gold">Degree</span>
          <img src="/images/btech_ece.png" alt="BTech ECE">
          <div class="cert-title">B.Tech in Electronics and Communication Engineering</div>
          <div class="cert-sub">GRIET, JNTU Hyderabad</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag gold">Diploma</span>
          <img src="/images/advanced_ai_nielit.png" alt="Advanced Diploma in AI">
          <div class="cert-title">Advanced Diploma in Artificial Intelligence</div>
          <div class="cert-sub">NIELIT, India</div>
        </div>
      </div>
    </div>

    <div id="badges-tab" class="tab-panel">
      <div class="category-head">
        <h3>Certification Badges</h3>
        <p>Click each badge to open its verification link.</p>
      </div>

      <div class="cert-grid">
        <div class="cert-card badge-card">
          <a href="https://badgr.com/public/assertions/ALTQFVRfTKK09z8t39bOMQ" target="_blank" rel="noopener">
            <img src="/images/decision.png" alt="miniMBA Decision Making Badge">
          </a>
          <div class="cert-title">miniMBA: Executive Judgement and Decision-Making</div>
          <div class="cert-sub">Miami University</div>
        </div>

        <div class="cert-card badge-card">
          <a href="https://badges.parchment.com/public/assertions/CvWFqkZ3Qoiije2Sap6mPQ" target="_blank" rel="noopener">
            <img src="/images/market.png" alt="miniMBA Market Presence Badge">
          </a>
          <div class="cert-title">miniMBA: Enhancing Market Presence</div>
          <div class="cert-sub">Miami University</div>
        </div>
      </div>
    </div>

    <div id="honors-tab" class="tab-panel">
      <div class="category-head">
        <h3>Honors and Recognition</h3>
        <p>Awards, honor societies, and recognition.</p>
      </div>

      <div class="cert-grid lightbox-gallery">
        <div class="cert-card">
          <span class="corner-tag gold">Honor</span>
          <img src="/images/guinness_world_record.png" alt="Guinness World Record">
          <div class="cert-title">Guinness World Record - Participation Certificate</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag gold">Honor</span>
          <img src="/images/ieee_hkn_certificate.jpg" alt="IEEE HKN Membership">
          <div class="cert-title">IEEE Eta Kappa Nu - Honor Society Member</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag gold">Honor</span>
          <img src="/images/mspe_membership.png" alt="MSPE Membership">
          <div class="cert-title">Member - Missouri Society of Professional Engineers</div>
          <div class="cert-sub">Western Chapter</div>
        </div>
      </div>
    </div>

    <div id="memberships-tab" class="tab-panel">
      <div class="category-head">
        <h3>Professional Memberships</h3>
        <p>Membership proofs and IDs where applicable.</p>
      </div>

      <div class="cert-grid lightbox-gallery">
        <div class="cert-card">
          <span class="corner-tag green">Member</span>
          <img src="/images/ACM_Membership.png" alt="ACM Membership">
          <div class="cert-title">ACM Member</div>
          <div class="cert-sub">Membership ID: 8325933</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag green">Member</span>
          <img src="/images/IEEE_Membership.png" alt="IEEE Membership">
          <div class="cert-title">IEEE Member</div>
          <div class="cert-sub">Membership ID: 93943359</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag green">Member</span>
          <img src="/images/aaai_placeholder.png" alt="AAAI Membership">
          <div class="cert-title">AAAI Member</div>
          <div class="cert-sub">Membership ID: 648148</div>
        </div>
      </div>
    </div>

    <div id="hackathon-tab" class="tab-panel">
      <div class="category-head">
        <h3>Hackathon Awards</h3>
        <p>Selected hackathon accomplishments.</p>
      </div>

      <div class="cert-grid lightbox-gallery">
        <div class="cert-card">
          <span class="corner-tag red">Award</span>
          <img src="/images/hackaroo_2022.png" alt="Hack-A-Roo 2022">
          <div class="cert-title">2nd Place - Hack-A-Roo Fall 2022</div>
          <div class="cert-sub">Entrepreneur Track</div>
        </div>

        <div class="cert-card">
          <span class="corner-tag red">Award</span>
          <img src="/images/hackaroo_2021.png" alt="Hack-A-Roo 2021">
          <div class="cert-title">3rd Place - Hack-A-Roo Fall 2021</div>
          <div class="cert-sub">CS/IT Track</div>
        </div>
      </div>
    </div>
  </div>

  <div class="section">
    <h2>🧭 Credential Themes</h2>
    <div class="divider"></div>

    <div class="tag-cloud">
      <span class="tag">Management and Accounting</span>
      <span class="tag">Semiconductor Fabrication</span>
      <span class="tag">Machine Learning</span>
      <span class="tag">MLOps</span>
      <span class="tag">Cloud Computing</span>
      <span class="tag">Hardware Security</span>
      <span class="tag">Embedded Systems</span>
      <span class="tag">Research Methods</span>
      <span class="tag">Scientific Writing</span>
      <span class="tag">Professional Memberships</span>
      <span class="tag">Academic Degrees</span>
      <span class="tag">Honors and Awards</span>
    </div>
  </div>

</div>

<div class="lightbox" id="lightbox" aria-hidden="true">
  <img id="lightbox-img" src="" alt="">
  <div class="hint">Click anywhere to close</div>
</div>

<script>
function openCertTab(event, panelId) {
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

document.addEventListener("DOMContentLoaded", function () {
  const images = document.querySelectorAll(".lightbox-gallery img");
  const lightbox = document.getElementById("lightbox");
  const lightboxImg = document.getElementById("lightbox-img");

  images.forEach(function(img) {
    img.addEventListener("click", function() {
      lightboxImg.src = img.src;
      lightboxImg.alt = img.alt;
      lightbox.style.display = "flex";
      lightbox.setAttribute("aria-hidden", "false");
    });
  });

  lightbox.addEventListener("click", function() {
    lightbox.style.display = "none";
    lightboxImg.src = "";
    lightboxImg.alt = "";
    lightbox.setAttribute("aria-hidden", "true");
  });

  document.addEventListener("keydown", function(e) {
    if (e.key === "Escape" && lightbox.style.display === "flex") {
      lightbox.style.display = "none";
      lightboxImg.src = "";
      lightboxImg.alt = "";
      lightbox.setAttribute("aria-hidden", "true");
    }
  });
});
</script>
