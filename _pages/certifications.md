---
title: "Certifications"
layout: single
permalink: /certifications/
author_profile: true
---

<div class="cert-hero">
  <h2>Certifications, Training, and Credentials</h2>
  <p>
    A visual showcase of certifications, workshops, professional memberships, and awards.
    Click any image to view it fullscreen.
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
        Training & Development
      </span>
      <span class="pill">
        <svg viewBox="0 0 24 24" fill="none" aria-hidden="true">
          <path d="M12 3l10 6-10 6L2 9l10-6Z" stroke="currentColor" stroke-width="2" stroke-linejoin="round"/>
          <path d="M2 9v6l10 6 10-6V9" stroke="currentColor" stroke-width="2" stroke-linejoin="round"/>
        </svg>
        Degrees & Memberships
      </span>
    </div>
    <div class="hero-actions">
      <a class="cta" href="/resume/">Resume</a>
      <a class="cta primary" href="/publications/">Publications</a>
    </div>
  </div>
</div>

<style>
:root{
  --blue:#1a73e8;
  --red:#DC143C;
  --bg:#ffffff;
  --soft:#f7fbff;
  --muted:#5a6573;
  --border:#d7e6fb;
  --shadow: 0 10px 24px rgba(0,0,0,0.06);
  --radius: 14px;
}

/* Hero */
.cert-hero{
  border: 2px solid var(--blue);
  background: linear-gradient(135deg, #ffffff 0%, #f2f8ff 55%, #ffffff 100%);
  border-radius: 18px;
  padding: 1.6rem 1.6rem 1.2rem 1.6rem;
  box-shadow: var(--shadow);
  margin-bottom: 1.4rem;
}
.cert-hero h2{
  margin: 0 0 0.35rem 0;
  color: var(--blue);
  font-size: 1.55rem;
}
.cert-hero p{
  margin: 0.25rem 0 0.95rem 0;
  color: var(--muted);
  line-height: 1.55;
}
.hero-row{
  display:flex;
  gap: 1rem;
  flex-wrap: wrap;
  align-items: center;
  justify-content: space-between;
}
.hero-badges{
  display:flex;
  gap: 0.5rem;
  flex-wrap: wrap;
}
.pill{
  display:inline-flex;
  align-items:center;
  gap: 0.45rem;
  padding: 0.35rem 0.7rem;
  border-radius: 999px;
  font-weight: 800;
  font-size: 0.86rem;
  border: 1px solid var(--border);
  background: #ffffff;
  color: var(--blue);
}
.pill.red{
  border-color: #ffd0d8;
  color: var(--red);
}
.pill svg{ width:16px; height:16px; opacity:0.95; }

.hero-actions{
  display:flex;
  gap: 0.6rem;
  flex-wrap: wrap;
}
.cta{
  display:inline-block;
  padding: 0.55rem 0.9rem;
  border-radius: 12px;
  font-weight: 900;
  text-decoration:none;
  border: 2px solid var(--blue);
  color: var(--blue);
  background: #ffffff;
  transition: 0.2s ease;
}
.cta:hover{ transform: translateY(-1px); background:#eaf3ff; }
.cta.primary{ background: var(--blue); color:#fff; }
.cta.primary:hover{ background:#135fcd; }

/* Section wrapper */
.section{
  border: 2px solid var(--blue);
  border-radius: 18px;
  background: #ffffff;
  box-shadow: var(--shadow);
  margin: 1.2rem 0;
  overflow: hidden;
}
.section-head{
  padding: 1rem 1.2rem 0.9rem 1.2rem;
  background: linear-gradient(180deg, #ffffff 0%, #f6fbff 100%);
  border-bottom: 1px solid #e8f2ff;
}
.section-head h3{
  margin: 0;
  color: var(--blue);
  font-size: 1.2rem;
}
.section-head p{
  margin: 0.25rem 0 0 0;
  color: var(--muted);
  font-size: 0.95rem;
}
.section-body{
  padding: 1rem 1.2rem 1.2rem 1.2rem;
}

/* Grid */
.cert-grid{
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 1.1rem;
  margin-top: 0.5rem;
}
.cert-card{
  background: #fff;
  border: 1px solid #e3efff;
  border-radius: 14px;
  padding: 0.55rem;
  transition: 0.2s ease;
  position: relative;
}
.cert-card:hover{
  transform: translateY(-2px);
  background: #f3f9ff;
  box-shadow: 0 10px 18px rgba(26,115,232,0.08);
  border-color: #cfe2ff;
}
.cert-card img{
  width: 100%;
  border-radius: 10px;
  cursor: zoom-in;
  display:block;
}
.cert-title{
  margin-top: 0.55rem;
  font-size: 0.92rem;
  font-weight: 800;
  color: #1a1a1a;
  line-height: 1.35;
}
.cert-sub{
  margin-top: 0.25rem;
  color: var(--muted);
  font-size: 0.86rem;
  line-height: 1.35;
}

/* Small tag in corner (optional) */
.corner-tag{
  position:absolute;
  top: 10px;
  left: 10px;
  background: rgba(26,115,232,0.92);
  color: #fff;
  font-weight: 900;
  font-size: 0.75rem;
  padding: 0.2rem 0.45rem;
  border-radius: 999px;
  border: 1px solid rgba(255,255,255,0.25);
}

/* Badges-only cards (for small badges) */
.badge-card img{
  width: 160px;
  height: auto;
  margin: 0.4rem auto 0.2rem auto;
}
.badge-card{
  text-align:center;
  padding: 0.9rem 0.8rem;
}

/* Lightbox */
.lightbox{
  position: fixed;
  inset: 0;
  width: 100vw;
  height: 100vh;
  background: rgba(0, 0, 0, 0.9);
  display: none;
  align-items: center;
  justify-content: center;
  z-index: 2000;
  padding: 18px;
}
.lightbox img{
  max-width: 92vw;
  max-height: 92vh;
  border-radius: 14px;
  box-shadow: 0 0 22px rgba(255, 255, 255, 0.18);
}
.lightbox .hint{
  position: fixed;
  bottom: 18px;
  left: 50%;
  transform: translateX(-50%);
  color: rgba(255,255,255,0.85);
  font-weight: 800;
  font-size: 0.92rem;
  background: rgba(0,0,0,0.35);
  padding: 0.35rem 0.7rem;
  border-radius: 999px;
  border: 1px solid rgba(255,255,255,0.2);
}
</style>

<!-- SECTION 1 -->
<div class="section">
  <div class="section-head">
    <h3>Certifications (Management)</h3>
    <p>Academic and professional certificates.</p>
  </div>
  <div class="section-body">
    <div class="cert-grid lightbox-gallery">
            <div class="cert-card">
        <span class="corner-tag">Cert</span>
        <img src="/images/UIUC_1.PNG" alt=Management">
        <div class="cert-title">Cost Behaviors, Systems, and Analysis/div>
        <div class="cert-sub">University of Illinois Urbana-Champaign</div>
      </div>
  </div>
</div>
              
<!-- SECTION 1 -->
<div class="section">
  <div class="section-head">
    <h3>Certifications</h3>
    <p>Academic and professional certificates.</p>
  </div>
  <div class="section-body">
    <div class="cert-grid lightbox-gallery">

      <div class="cert-card">
        <span class="corner-tag">Cert</span>
        <img src="/images/purdue.jpeg" alt="Semiconductor">
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
        <img src="/images/mathematics_ml.png" alt="Mathematics for ML">
        <div class="cert-title">Mathematics for Machine Learning</div>
        <div class="cert-sub">Imperial College London</div>
      </div>

      <div class="cert-card">
        <span class="corner-tag">Cert</span>
        <img src="/images/device_packaging.png" alt="Device Packaging">
        <div class="cert-title">Introduction to Device and System Packaging</div>
        <div class="cert-sub">Georgia Tech</div>
      </div>

      <div class="cert-card">
        <span class="corner-tag">Cert</span>
        <img src="/images/Chandigarh.png" alt="Chandigarh">
        <div class="cert-title">MEAN Stack Development (Project: Contact List CRUD)</div>
        <div class="cert-sub">NIELIT Chandigarh</div>
      </div>

      <div class="cert-card">
        <span class="corner-tag">Cert</span>
        <img src="/images/LONDON.png" alt="Research Methods">
        <div class="cert-title">Understanding Research Methods</div>
        <div class="cert-sub">University of London</div>
      </div>

      <div class="cert-card">
        <span class="corner-tag">Cert</span>
        <img src="/images/ECOLE.png" alt="Scientific Paper">
        <div class="cert-title">How to Write and Publish a Scientific Paper</div>
        <div class="cert-sub">École Polytechnique, France</div>
      </div>

      <div class="cert-card">
        <span class="corner-tag">Cert</span>
        <img src="/images/GOOGLE.png" alt="Google">
        <div class="cert-title">Managing ML Projects with Google Cloud</div>
        <div class="cert-sub">Google Cloud</div>
      </div>

      <div class="cert-card">
        <span class="corner-tag">Cert</span>
        <img src="/images/LEARN.png" alt="Learn">
        <div class="cert-title">Developing AI Applications on Azure</div>
        <div class="cert-sub">LearnQuest</div>
      </div>

      <div class="cert-card">
        <span class="corner-tag">Cert</span>
        <img src="/images/AWS.png" alt="AWS">
        <div class="cert-title">Getting Started with AWS Machine Learning</div>
        <div class="cert-sub">AWS</div>
      </div>

      <div class="cert-card">
        <span class="corner-tag">Cert</span>
        <img src="/images/CODE.png" alt="CODE">
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
        <img src="/images/GORAKHPUR.png" alt="GORAKHPUR">
        <div class="cert-title">Embedded System Design</div>
        <div class="cert-sub">NIELIT Gorakhpur</div>
      </div>

    </div>
  </div>
</div>

<!-- SECTION 2 -->
<div class="section">
  <div class="section-head">
    <h3>Training & Professional Development</h3>
    <p>Workshops, internships, and structured programs.</p>
  </div>
  <div class="section-body">
    <div class="cert-grid lightbox-gallery">

      <div class="cert-card">
        <span class="corner-tag">Training</span>
        <img src="/images/FPGA.png" alt="FPGA Training">
        <div class="cert-title">Summer Internship on FPGA-Based Embedded Systems for DSP</div>
      </div>

      <div class="cert-card">
        <span class="corner-tag">Training</span>
        <img src="/images/NEURO.png" alt="Computational Neuroscience">
        <div class="cert-title">Internship on Hardware for Computational Neuroscience</div>
      </div>

      <div class="cert-card">
        <span class="corner-tag">Program</span>
        <img src="/images/product_management.png" alt="Product Management">
        <div class="cert-title">Product Management Program</div>
        <div class="cert-sub">Confederation of Indian Industry (CII)</div>
      </div>

      <div class="cert-card">
        <span class="corner-tag">Training</span>
        <img src="/images/semiconductor_basics.png" alt="Semiconductor Basics">
        <div class="cert-title">Basics of Semiconductor Device Technology</div>
        <div class="cert-sub">Indian Institute of Science</div>
      </div>

      <div class="cert-card">
        <span class="corner-tag">Training</span>
        <img src="/images/TORMP.png" alt="Manuscript Drafting">
        <div class="cert-title">Manuscript Drafting and Publishing</div>
        <div class="cert-sub">Eudoxia Research Center</div>
      </div>

      <div class="cert-card">
        <span class="corner-tag">Training</span>
        <img src="/images/REGEX.png" alt="MEARN Stack">
        <div class="cert-title">Industrial Training: MEARN Stack Development</div>
      </div>

      <div class="cert-card">
        <span class="corner-tag">Workshop</span>
        <img src="/images/Automobile.png" alt="Automobile">
        <div class="cert-title">Automobile Engineering and IC Engine Workshop</div>
        <div class="cert-sub">IIT Kanpur</div>
      </div>

      <div class="cert-card">
        <span class="corner-tag">Workshop</span>
        <img src="/images/MADRAS.png" alt="IIT Madras">
        <div class="cert-title">AI & Reinforcement Learning Workshop</div>
        <div class="cert-sub">IIT Madras</div>
      </div>

    </div>
  </div>
</div>

<!-- SECTION 3 -->
<div class="section">
  <div class="section-head">
    <h3>Professional Certifications</h3>
    <p>Industry-recognized credentials.</p>
  </div>
  <div class="section-body">
    <div class="cert-grid lightbox-gallery">

      <div class="cert-card">
        <span class="corner-tag">Pro</span>
        <img src="/images/network_security.jpeg" alt="Network Security">
        <div class="cert-title">Network Security Associate</div>
      </div>

      <div class="cert-card">
        <span class="corner-tag">Pro</span>
        <img src="/images/intel_cloud.png" alt="Intel Cloud">
        <div class="cert-title">Intel Solution Pro: Cloud Business Professional</div>
      </div>

      <div class="cert-card">
        <span class="corner-tag">Pro</span>
        <img src="/images/ccna.png" alt="CCNA">
        <div class="cert-title">Cisco Certified Network Associate (X)</div>
      </div>

    </div>
  </div>
</div>

<!-- SECTION 4 -->
<div class="section">
  <div class="section-head">
    <h3>Degrees & Diplomas</h3>
    <p>Academic degrees and diplomas.</p>
  </div>
  <div class="section-body">
    <div class="cert-grid lightbox-gallery">

      <div class="cert-card">
        <span class="corner-tag">Degree</span>
        <img src="/images/PHD.png" alt="PhD ECE Degree">
        <div class="cert-title">Ph.D. in Electrical and Computer Engineering</div>
        <div class="cert-sub">University of Missouri–Kansas City</div>
      </div>

      <div class="cert-card">
        <span class="corner-tag">Degree</span>
        <img src="/images/ms_cs_uis.png" alt="MS CS Degree">
        <div class="cert-title">M.S. in Computer Science</div>
        <div class="cert-sub">University of Illinois, Springfield</div>
      </div>

      <div class="cert-card">
        <span class="corner-tag">Degree</span>
        <img src="/images/ms_ee_umkc.png" alt="MS EE Degree">
        <div class="cert-title">M.S. in Electrical Engineering</div>
        <div class="cert-sub">University of Missouri–Kansas City</div>
      </div>

      <div class="cert-card">
        <span class="corner-tag">Degree</span>
        <img src="/images/btech_ece.png" alt="B.Tech ECE">
        <div class="cert-title">B.Tech in Electronics and Communication Engineering</div>
        <div class="cert-sub">GRIET, JNTU Hyderabad</div>
      </div>

      <div class="cert-card">
        <span class="corner-tag">Diploma</span>
        <img src="/images/advanced_ai_nielit.png" alt="AI Diploma">
        <div class="cert-title">Advanced Diploma in Artificial Intelligence</div>
        <div class="cert-sub">NIELIT, India</div>
      </div>

    </div>
  </div>
</div>

<!-- SECTION 5 -->
<div class="section">
  <div class="section-head">
    <h3>Certification Badges</h3>
    <p>Click the badge to open verification links.</p>
  </div>
  <div class="section-body">
    <div class="cert-grid">

      <div class="cert-card badge-card">
        <a href="https://badgr.com/public/assertions/ALTQFVRfTKK09z8t39bOMQ" target="_blank" rel="noopener">
          <img src="/images/decision.png" alt="miniMBA Badge">
        </a>
        <div class="cert-title">miniMBA: Executive Judgement and Decision-Making</div>
        <div class="cert-sub">Miami University</div>
      </div>

      <div class="cert-card badge-card">
        <a href="https://badges.parchment.com/public/assertions/CvWFqkZ3Qoiije2Sap6mPQ" target="_blank" rel="noopener">
          <img src="/images/market.png" alt="miniMBA Badge">
        </a>
        <div class="cert-title">miniMBA: Enhancing Market Presence</div>
        <div class="cert-sub">Miami University</div>
      </div>

    </div>
  </div>
</div>

<!-- SECTION 6 -->
<div class="section">
  <div class="section-head">
    <h3>Honors & Recognition</h3>
    <p>Awards, honor societies, and recognition.</p>
  </div>
  <div class="section-body">
    <div class="cert-grid lightbox-gallery">

      <div class="cert-card">
        <span class="corner-tag">Honor</span>
        <img src="/images/guinness_world_record.png" alt="Guinness World Record">
        <div class="cert-title">Guinness World Record – Participation Certificate</div>
      </div>

      <div class="cert-card">
        <span class="corner-tag">Honor</span>
        <img src="/images/ieee_hkn_certificate.jpg" alt="IEEE-HKN Membership">
        <div class="cert-title">IEEE Eta Kappa Nu (HKN) – Honor Society Member</div>
      </div>

      <div class="cert-card">
        <span class="corner-tag">Honor</span>
        <img src="/images/mspe_membership.png" alt="MSPE Membership">
        <div class="cert-title">Member – Missouri Society of Professional Engineers</div>
        <div class="cert-sub">Western Chapter</div>
      </div>

    </div>
  </div>
</div>

<!-- SECTION 7 -->
<div class="section">
  <div class="section-head">
    <h3>Professional Memberships</h3>
    <p>Membership proofs and IDs (where applicable).</p>
  </div>
  <div class="section-body">
    <div class="cert-grid lightbox-gallery">

      <div class="cert-card">
        <span class="corner-tag">Member</span>
        <img src="/images/ACM_Membership.png" alt="ACM Membership">
        <div class="cert-title">ACM Member</div>
        <div class="cert-sub">Membership ID: 8325933</div>
      </div>

      <div class="cert-card">
        <span class="corner-tag">Member</span>
        <img src="/images/IEEE_Membership.png" alt="IEEE Membership">
        <div class="cert-title">IEEE Member</div>
        <div class="cert-sub">Membership ID: 93943359</div>
      </div>

      <div class="cert-card">
        <span class="corner-tag">Member</span>
        <img src="/images/aaai_placeholder.png" alt="AAAI Membership">
        <div class="cert-title">AAAI Member</div>
        <div class="cert-sub">Membership ID: 648148</div>
      </div>

    </div>
  </div>
</div>

<!-- SECTION 8 -->
<div class="section">
  <div class="section-head">
    <h3>Hackathon Awards</h3>
    <p>Selected hackathon accomplishments.</p>
  </div>
  <div class="section-body">
    <div class="cert-grid lightbox-gallery">

      <div class="cert-card">
        <span class="corner-tag">Award</span>
        <img src="/images/hackaroo_2022.png" alt="Hack-A-Roo 2022">
        <div class="cert-title">2nd Place – Hack-A-Roo Fall 2022</div>
        <div class="cert-sub">Entrepreneur Track</div>
      </div>

      <div class="cert-card">
        <span class="corner-tag">Award</span>
        <img src="/images/hackaroo_2021.png" alt="Hack-A-Roo 2021">
        <div class="cert-title">3rd Place – Hack-A-Roo Fall 2021</div>
        <div class="cert-sub">CS/IT Track</div>
      </div>

    </div>
  </div>
</div>

<!-- Lightbox -->
<div class="lightbox" id="lightbox" aria-hidden="true">
  <img id="lightbox-img" src="" alt="">
  <div class="hint">Click anywhere to close</div>
</div>

<script>
document.addEventListener("DOMContentLoaded", function () {
  const images = document.querySelectorAll(".lightbox-gallery img");
  const lightbox = document.getElementById("lightbox");
  const lightboxImg = document.getElementById("lightbox-img");

  images.forEach(img => {
    img.addEventListener("click", () => {
      lightboxImg.src = img.src;
      lightbox.style.display = "flex";
      lightbox.setAttribute("aria-hidden", "false");
    });
  });

  lightbox.addEventListener("click", () => {
    lightbox.style.display = "none";
    lightboxImg.src = "";
    lightbox.setAttribute("aria-hidden", "true");
  });

  document.addEventListener("keydown", (e) => {
    if (e.key === "Escape" && lightbox.style.display === "flex") {
      lightbox.style.display = "none";
      lightboxImg.src = "";
      lightbox.setAttribute("aria-hidden", "true");
    }
  });
});
</script>
