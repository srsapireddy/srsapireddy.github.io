---
title: "Presentations & Talks"
layout: single
permalink: /presentations/
author_profile: true
---

<style>
:root {
  --pres-primary: #1a73e8;
  --pres-primary-dark: #0b4db3;
  --pres-accent: #00bcd4;
  --pres-dark: #0f172a;
  --pres-muted: #64748b;
  --pres-soft: #f8fbff;
  --pres-card: rgba(255, 255, 255, 0.88);
  --pres-border: rgba(26, 115, 232, 0.20);
}

/* Page Wrapper */
.presentations-page {
  position: relative;
  overflow: hidden;
  padding-bottom: 2rem;
}

.presentations-page::before,
.presentations-page::after {
  content: "";
  position: absolute;
  border-radius: 50%;
  z-index: -1;
}

.presentations-page::before {
  width: 360px;
  height: 360px;
  top: 40px;
  right: -140px;
  background: radial-gradient(circle, rgba(26,115,232,0.18), transparent 70%);
}

.presentations-page::after {
  width: 280px;
  height: 280px;
  bottom: 180px;
  left: -130px;
  background: radial-gradient(circle, rgba(0,188,212,0.15), transparent 70%);
}

/* Hero */
.presentations-hero {
  position: relative;
  padding: 2.5rem 2rem;
  margin: 1.5rem 0 2rem;
  border-radius: 30px;
  background:
    linear-gradient(135deg, rgba(26,115,232,0.13), rgba(255,255,255,0.96)),
    linear-gradient(45deg, rgba(0,188,212,0.10), rgba(255,255,255,0.94));
  border: 1px solid var(--pres-border);
  box-shadow: 0 20px 48px rgba(15, 23, 42, 0.08);
  overflow: hidden;
}

.presentations-hero::before {
  content: "Talks • Seminars • Posters • Demos";
  position: absolute;
  top: 24px;
  right: -34px;
  transform: rotate(12deg);
  font-size: 0.72rem;
  font-weight: 850;
  letter-spacing: 0.16em;
  text-transform: uppercase;
  color: rgba(26,115,232,0.28);
}

.pres-kicker {
  display: inline-block;
  margin-bottom: 0.8rem;
  padding: 0.4rem 0.85rem;
  border-radius: 999px;
  background: rgba(26,115,232,0.12);
  color: var(--pres-primary);
  font-size: 0.78rem;
  font-weight: 850;
  letter-spacing: 0.05em;
  text-transform: uppercase;
}

.presentations-hero h2 {
  margin: 0 0 0.75rem;
  color: var(--pres-dark);
  font-size: 2.35rem;
  line-height: 1.12;
  font-weight: 850;
}

.presentations-hero p {
  margin: 0;
  max-width: 880px;
  color: var(--pres-muted);
  font-size: 1rem;
  line-height: 1.75;
}

/* Summary Strip */
.pres-summary {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(165px, 1fr));
  gap: 1rem;
  margin: 1.5rem 0 2.4rem;
}

.pres-summary-card {
  position: relative;
  padding: 1.1rem;
  border-radius: 20px;
  background: var(--pres-card);
  border: 1px solid rgba(15,23,42,0.08);
  box-shadow: 0 12px 28px rgba(15,23,42,0.06);
  backdrop-filter: blur(10px);
  overflow: hidden;
  transition: 0.25s ease;
}

.pres-summary-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 18px 36px rgba(26,115,232,0.13);
}

.pres-summary-card::after {
  content: "";
  position: absolute;
  right: -30px;
  bottom: -30px;
  width: 86px;
  height: 86px;
  border-radius: 50%;
  background: rgba(26,115,232,0.09);
}

.pres-summary-card span {
  display: block;
  color: var(--pres-primary);
  font-size: 1.35rem;
  font-weight: 850;
}

.pres-summary-card small {
  color: var(--pres-muted);
  font-size: 0.82rem;
}

/* Section Header */
.pres-section {
  margin-top: 2.4rem;
}

.pres-section-header {
  margin-bottom: 1.2rem;
}

.pres-section-header h3 {
  margin: 0 0 0.35rem;
  color: var(--pres-dark);
  font-size: 1.45rem;
  font-weight: 850;
}

.pres-section-header p {
  margin: 0;
  color: var(--pres-muted);
  font-size: 0.94rem;
  line-height: 1.6;
}

/* Presentation Grid */
.presentation-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(285px, 1fr));
  gap: 1.4rem;
}

/* Presentation Card */
.presentation-card {
  position: relative;
  border-radius: 24px;
  background: var(--pres-card);
  border: 1px solid rgba(26,115,232,0.18);
  box-shadow: 0 14px 34px rgba(15,23,42,0.08);
  overflow: hidden;
  backdrop-filter: blur(12px);
  cursor: pointer;
  transition: transform 0.25s ease, box-shadow 0.25s ease, border-color 0.25s ease;
}

.presentation-card:hover {
  transform: translateY(-6px);
  border-color: rgba(26,115,232,0.46);
  box-shadow: 0 24px 48px rgba(26,115,232,0.16);
}

.presentation-thumb {
  position: relative;
  height: 205px;
  overflow: hidden;
  background: #eaf2ff;
}

.presentation-thumb img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.45s ease, filter 0.35s ease;
  display: block;
  -webkit-user-drag: none;
  user-drag: none;
}

.presentation-card:hover .presentation-thumb img {
  transform: scale(1.06);
  filter: brightness(0.95);
}

.pres-badge {
  position: absolute;
  top: 14px;
  left: 14px;
  padding: 0.36rem 0.7rem;
  border-radius: 999px;
  background: rgba(15,23,42,0.78);
  color: #ffffff;
  font-size: 0.7rem;
  font-weight: 800;
  letter-spacing: 0.03em;
  backdrop-filter: blur(8px);
}

.pres-year {
  position: absolute;
  right: 14px;
  bottom: 14px;
  padding: 0.34rem 0.65rem;
  border-radius: 999px;
  background: rgba(255,255,255,0.88);
  color: var(--pres-primary-dark);
  font-size: 0.72rem;
  font-weight: 850;
  box-shadow: 0 8px 18px rgba(15,23,42,0.14);
}

.presentation-body {
  padding: 1.1rem 1.15rem 1.25rem;
}

.presentation-body h4 {
  margin: 0 0 0.45rem;
  color: var(--pres-dark);
  font-size: 1.03rem;
  line-height: 1.35;
  font-weight: 850;
}

.presentation-body p {
  margin: 0;
  color: #475569;
  font-size: 0.88rem;
  line-height: 1.6;
}

.pres-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.42rem;
  margin-top: 0.85rem;
}

.pres-tags span {
  padding: 0.28rem 0.55rem;
  border-radius: 999px;
  background: #eef6ff;
  color: var(--pres-primary);
  border: 1px solid rgba(26,115,232,0.16);
  font-size: 0.68rem;
  font-weight: 750;
}

/* Poster Cards */
.poster-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
  gap: 1.4rem;
}

.poster-card {
  display: grid;
  grid-template-columns: 44% 1fr;
  border-radius: 24px;
  background: var(--pres-card);
  border: 1px solid rgba(26,115,232,0.18);
  box-shadow: 0 14px 34px rgba(15,23,42,0.08);
  overflow: hidden;
  backdrop-filter: blur(12px);
  transition: 0.25s ease;
}

.poster-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 22px 44px rgba(26,115,232,0.15);
}

.poster-card img {
  width: 100%;
  height: 100%;
  min-height: 220px;
  object-fit: cover;
  -webkit-user-drag: none;
  user-drag: none;
}

.poster-content {
  padding: 1.2rem;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.poster-content h4 {
  margin: 0 0 0.45rem;
  color: var(--pres-dark);
  font-size: 1.05rem;
  line-height: 1.35;
  font-weight: 850;
}

.poster-content p {
  margin: 0;
  color: #475569;
  font-size: 0.88rem;
  line-height: 1.6;
}

/* YouTube Cards */
.youtube-card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(285px, 1fr));
  gap: 1.4rem;
}

.youtube-card {
  border-radius: 24px;
  background: var(--pres-card);
  border: 1px solid rgba(26,115,232,0.18);
  box-shadow: 0 14px 34px rgba(15,23,42,0.08);
  overflow: hidden;
  backdrop-filter: blur(12px);
  transition: 0.25s ease;
}

.youtube-card:hover {
  transform: translateY(-6px);
  box-shadow: 0 24px 48px rgba(26,115,232,0.16);
}

.youtube-frame {
  position: relative;
  background: #0f172a;
}

.youtube-card iframe {
  width: 100%;
  height: 210px;
  border: none;
  display: block;
}

.youtube-body {
  padding: 1rem 1.15rem 1.2rem;
}

.youtube-body h4 {
  margin: 0 0 0.4rem;
  color: var(--pres-dark);
  font-size: 1rem;
  font-weight: 850;
}

.youtube-body p {
  margin: 0;
  color: #475569;
  font-size: 0.86rem;
  line-height: 1.55;
}

/* Copyright */
.pres-copyright {
  margin-top: 2.4rem;
  padding: 1.05rem 1.2rem;
  border-left: 5px solid var(--pres-primary);
  background: rgba(248,251,255,0.92);
  border-radius: 14px;
  color: #475569;
  font-size: 0.86rem;
  line-height: 1.65;
  box-shadow: 0 8px 20px rgba(15,23,42,0.04);
}

/* Lightbox Viewer */
.pres-lightbox {
  position: fixed;
  inset: 0;
  display: none;
  align-items: center;
  justify-content: center;
  background: rgba(2, 6, 23, 0.94);
  z-index: 9999;
  padding: 1rem;
}

.pres-lightbox-content {
  width: min(1100px, 94vw);
  height: min(760px, 90vh);
  background: #ffffff;
  border-radius: 20px;
  overflow: hidden;
  box-shadow: 0 0 45px rgba(255,255,255,0.18);
  position: relative;
  animation: presZoom 0.25s ease;
}

.pres-lightbox iframe {
  width: 100%;
  height: 100%;
  border: none;
}

.pres-lightbox-close {
  position: fixed;
  top: 20px;
  right: 30px;
  color: #ffffff;
  font-size: 2.2rem;
  font-weight: 850;
  cursor: pointer;
  opacity: 0.88;
  z-index: 10000;
}

.pres-lightbox-close:hover {
  opacity: 1;
}

@keyframes presZoom {
  from {
    transform: scale(0.94);
    opacity: 0;
  }
  to {
    transform: scale(1);
    opacity: 1;
  }
}

/* Copy Deterrent */
.presentations-protected {
  -webkit-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

/* Responsive */
@media (max-width: 820px) {
  .presentations-hero h2 {
    font-size: 1.85rem;
  }

  .poster-card {
    grid-template-columns: 1fr;
  }

  .poster-card img {
    min-height: 230px;
  }
}

@media (max-width: 560px) {
  .presentations-hero {
    padding: 1.45rem;
    border-radius: 22px;
  }

  .presentations-hero h2 {
    font-size: 1.55rem;
  }

  .presentation-thumb {
    height: 190px;
  }

  .youtube-card iframe {
    height: 190px;
  }

  .pres-lightbox-content {
    width: 94vw;
    height: 82vh;
    border-radius: 14px;
  }
}
</style>

<div class="presentations-page presentations-protected">

  <section class="presentations-hero">
    <span class="pres-kicker">Selected Presentations</span>
    <h2>Presentations & Talks</h2>
    <p>
      A curated collection of invited lectures, research presentations, conference posters,
      academic talks, project demonstrations, and professional outreach presentations.
      This page highlights my work across RF systems, VLSI design, artificial intelligence,
      teaching, outreach, and applied engineering research.
    </p>
  </section>

  <section class="pres-summary">
    <div class="pres-summary-card">
      <span>Invited</span>
      <small>Lectures and professional talks</small>
    </div>

    <div class="pres-summary-card">
      <span>IEEE</span>
      <small>Conference presentations</small>
    </div>

    <div class="pres-summary-card">
      <span>K–12</span>
      <small>STEM outreach presentations</small>
    </div>

    <div class="pres-summary-card">
      <span>Demos</span>
      <small>Projects, hackathons, and videos</small>
    </div>
  </section>

  <section class="pres-section">
    <div class="pres-section-header">
      <h3>Featured Presentations</h3>
      <p>Selected slide decks and academic presentations across outreach, research, teaching, and project development.</p>
    </div>

    <div class="presentation-grid">

      <div class="presentation-card" onclick="openPresentation('/publications/IAB K-12 PPT Srinivas.pdf')">
        <div class="presentation-thumb">
          <img src="/images/IAB_K12_Outreach_1.png" alt="IAB K-12 STEM Outreach Presentation 2026">
          <div class="pres-badge">Outreach</div>
          <div class="pres-year">2026</div>
        </div>
        <div class="presentation-body">
          <h4>IAB Presentation on K–12 STEM Outreach</h4>
          <p>Presentation highlighting hands-on electrical engineering outreach activities for middle and high school students.</p>
          <div class="pres-tags">
            <span>K–12</span>
            <span>STEM</span>
            <span>Outreach</span>
          </div>
        </div>
      </div>

      <div class="presentation-card" onclick="openPresentation('/publications/IEEE_Invited_Lecture_Srinivas.pdf')">
        <div class="presentation-thumb">
          <img src="/images/IEEE_Lecture.png" alt="IEEE Invited Lecture 2026">
          <div class="pres-badge">Invited Talk</div>
          <div class="pres-year">2026</div>
        </div>
        <div class="presentation-body">
          <h4>IEEE Invited Lecture</h4>
          <p>Invited lecture on RTL-to-GDSII chip design flow, EDA tools, VLSI methodology, and semiconductor career pathways.</p>
          <div class="pres-tags">
            <span>IEEE</span>
            <span>VLSI</span>
            <span>RTL to GDSII</span>
          </div>
        </div>
      </div>

      <div class="presentation-card" onclick="openPresentation('/publications/rfcon.pdf')">
        <div class="presentation-thumb">
          <img src="/images/rfcon_presentation_thumbnail.png" alt="RFCoN 2025 Presentation">
          <div class="pres-badge">Conference</div>
          <div class="pres-year">2025</div>
        </div>
        <div class="presentation-body">
          <h4>RFCoN 2025 Presentation</h4>
          <p>Research presentation on RF communication, signal processing, and lightweight modulation classification methods.</p>
          <div class="pres-tags">
            <span>RFCoN</span>
            <span>RF Systems</span>
            <span>Classification</span>
          </div>
        </div>
      </div>

      <div class="presentation-card" onclick="openPresentation('/publications/UMKC_ATP_Interview_Presentation_Rahul.pdf')">
        <div class="presentation-thumb">
          <img src="/images/umkc_presentation_thumbnail.png" alt="UMKC Assistant Teaching Professor Interview Presentation">
          <div class="pres-badge">Teaching</div>
          <div class="pres-year">Academic</div>
        </div>
        <div class="presentation-body">
          <h4>UMKC Assistant Teaching Professor Interview</h4>
          <p>Academic teaching presentation focused on instructional experience, engineering education, and student engagement.</p>
          <div class="pres-tags">
            <span>Teaching</span>
            <span>Engineering</span>
            <span>Academic Talk</span>
          </div>
        </div>
      </div>

      <div class="presentation-card" onclick="openPresentation('/publications/MIDE_Dec_2022.pdf')">
        <div class="presentation-thumb">
          <img src="/images/mide_ct_thumbnail.png" alt="MIDE Capstone Talk December 2022">
          <div class="pres-badge">Capstone</div>
          <div class="pres-year">2022</div>
        </div>
        <div class="presentation-body">
          <h4>MIDE Capstone Talk</h4>
          <p>Capstone presentation delivered in December 2022, highlighting project development and applied engineering work.</p>
          <div class="pres-tags">
            <span>Capstone</span>
            <span>Project</span>
            <span>Presentation</span>
          </div>
        </div>
      </div>

      <div class="presentation-card" onclick="openPresentation('/publications/DNN_Presentation.pptx')">
        <div class="presentation-thumb">
          <img src="/images/rahul_nn_presentation.png" alt="Deep Neural Networks Presentation">
          <div class="pres-badge">AI</div>
          <div class="pres-year">Talk</div>
        </div>
        <div class="presentation-body">
          <h4>Deep Neural Networks Talk</h4>
          <p>Presentation on deep neural networks, model structure, learning concepts, and applied machine learning workflows.</p>
          <div class="pres-tags">
            <span>AI</span>
            <span>DNN</span>
            <span>Machine Learning</span>
          </div>
        </div>
      </div>

      <div class="presentation-card" onclick="openPresentation('/publications/Army_PPT.pptx')">
        <div class="presentation-thumb">
          <img src="/images/army_ppt_thumbnail.png" alt="U.S. Army Research Presentation August 2023">
          <div class="pres-badge">Research</div>
          <div class="pres-year">2023</div>
        </div>
        <div class="presentation-body">
          <h4>U.S. Army Research Presentation</h4>
          <p>Research-oriented presentation connected to applied engineering, defense-related technologies, and technical development.</p>
          <div class="pres-tags">
            <span>Research</span>
            <span>Defense</span>
            <span>Engineering</span>
          </div>
        </div>
      </div>

      <div class="presentation-card" onclick="openPresentation('/publications/Falcon.pdf')">
        <div class="presentation-thumb">
          <img src="/images/Falcon.png" alt="Falcon Labs SaaS Platform">
          <div class="pres-badge">Software</div>
          <div class="pres-year">Project</div>
        </div>
        <div class="presentation-body">
          <h4>Falcon Labs SaaS Platform</h4>
          <p>Project presentation on a SaaS-based software platform, application development, and product-oriented system design.</p>
          <div class="pres-tags">
            <span>SaaS</span>
            <span>Software</span>
            <span>Platform</span>
          </div>
        </div>
      </div>

      <div class="presentation-card" onclick="openPresentation('/publications/Lunar.pdf')">
        <div class="presentation-thumb">
          <img src="/images/Lunar.png" alt="Lunar Lander using Deep Q-Learning">
          <div class="pres-badge">Reinforcement Learning</div>
          <div class="pres-year">Project</div>
        </div>
        <div class="presentation-body">
          <h4>Lunar Lander using Deep Q-Learning</h4>
          <p>Project presentation on reinforcement learning using Deep Q-Learning for lunar lander control and decision making.</p>
          <div class="pres-tags">
            <span>DQN</span>
            <span>RL</span>
            <span>AI Project</span>
          </div>
        </div>
      </div>

    </div>
  </section>

  <section class="pres-section">
    <div class="pres-section-header">
      <h3>Conference Presentations & Posters</h3>
      <p>Selected conference participation, poster presentations, and oral research presentations.</p>
    </div>

    <div class="poster-grid">

      <div class="poster-card">
        <img src="/images/glsposter_1.png" alt="GLSVLSI 2025 Poster Presentation">
        <div class="poster-content">
          <h4>GLSVLSI 2025 – Poster Presentation</h4>
          <p>
            Poster presentation at the Great Lakes Symposium on VLSI, highlighting work related to VLSI,
            hardware-aware machine learning, and efficient computing systems.
          </p>
          <div class="pres-tags">
            <span>GLSVLSI</span>
            <span>Poster</span>
            <span>VLSI</span>
          </div>
        </div>
      </div>

      <div class="poster-card">
        <img src="/images/rfcon_presenter.png" alt="RFCoN 2025 Oral Presentation">
        <div class="poster-content">
          <h4>RFCoN 2025 – Oral Presentation</h4>
          <p>
            Oral presentation at RFCoN 2025 focused on RF communication and lightweight modulation
            classification methods for efficient signal analysis.
          </p>
          <div class="pres-tags">
            <span>RFCoN</span>
            <span>Oral Talk</span>
            <span>RF Communication</span>
          </div>
        </div>
      </div>

    </div>
  </section>

  <section class="pres-section">
    <div class="pres-section-header">
      <h3>Hackathons & Internship Highlights</h3>
      <p>Video highlights from hackathon achievements, project demonstrations, and internship work.</p>
    </div>

    <div class="youtube-card-grid">

      <div class="youtube-card">
        <div class="youtube-frame">
          <iframe src="https://www.youtube.com/embed/aRM4DP-gUbg" title="Hackathon Win Fall 2021" allowfullscreen></iframe>
        </div>
        <div class="youtube-body">
          <h4>Hackathon Win – Fall 2021</h4>
          <p>Video highlight from a hackathon project and award-winning technical demonstration.</p>
        </div>
      </div>

      <div class="youtube-card">
        <div class="youtube-frame">
          <iframe src="https://www.youtube.com/embed/cJ4JHmoTgas" title="Hackathon Win Fall 2022" allowfullscreen></iframe>
        </div>
        <div class="youtube-body">
          <h4>Hackathon Win – Fall 2022</h4>
          <p>Project video showcasing technical development, teamwork, and applied software engineering.</p>
        </div>
      </div>

      <div class="youtube-card">
        <div class="youtube-frame">
          <iframe src="https://www.youtube.com/embed/E9ItHVkHuy8" title="Internship Project Demo" allowfullscreen></iframe>
        </div>
        <div class="youtube-body">
          <h4>Internship Project Demo</h4>
          <p>Demonstration video from internship work, highlighting project implementation and applied technical learning.</p>
        </div>
      </div>

    </div>
  </section>

  <div class="pres-copyright">
    © 2026 Srinivas Rahul S. All rights reserved. The text, images, slide previews, layout, design elements,
    and presentation descriptions on this page may not be copied, reproduced, republished, modified,
    or redistributed without prior written permission.
  </div>

</div>

<!-- Presentation Lightbox Viewer -->
<div class="pres-lightbox" id="presentation-lightbox">
  <span class="pres-lightbox-close" id="presentation-lightbox-close">&times;</span>
  <div class="pres-lightbox-content">
    <iframe id="presentation-frame" src=""></iframe>
  </div>
</div>

<script>
function openPresentation(url) {
  const baseUrl = "https://srsapireddy.github.io";
  const encodedUrl = encodeURIComponent(baseUrl + url);
  const viewerUrl = "https://docs.google.com/gview?url=" + encodedUrl + "&embedded=true";

  document.getElementById("presentation-frame").src = viewerUrl;
  document.getElementById("presentation-lightbox").style.display = "flex";
}

document.addEventListener("DOMContentLoaded", function () {
  const lightbox = document.getElementById("presentation-lightbox");
  const closeBtn = document.getElementById("presentation-lightbox-close");
  const frame = document.getElementById("presentation-frame");

  function closePresentation() {
    lightbox.style.display = "none";
    frame.src = "";
  }

  closeBtn.addEventListener("click", closePresentation);

  lightbox.addEventListener("click", function(e) {
    if (e.target === lightbox) {
      closePresentation();
    }
  });

  document.addEventListener("keydown", function(e) {
    if (e.key === "Escape") {
      closePresentation();
    }
  });

  /* Casual copy deterrent */
  document.addEventListener("contextmenu", function(e) {
    if (e.target.closest(".presentations-protected")) {
      e.preventDefault();
    }
  });

  document.addEventListener("keydown", function(e) {
    const blockedKeys = ["c", "u", "s", "a"];

    if ((e.ctrlKey || e.metaKey) && blockedKeys.includes(e.key.toLowerCase())) {
      if (document.activeElement.closest(".presentations-protected")) {
        e.preventDefault();
      }
    }
  });
});
</script>
