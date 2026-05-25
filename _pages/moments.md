---
title: "Moments"
layout: single
permalink: /moments/
author_profile: true
---

<style>
:root {
  --primary: #1a73e8;
  --primary-dark: #0b4db3;
  --accent: #00bcd4;
  --dark: #0f172a;
  --muted: #64748b;
  --light: #f8fbff;
  --card: rgba(255, 255, 255, 0.86);
  --border: rgba(26, 115, 232, 0.20);
}

/* Main Wrapper */
.moments-page {
  position: relative;
  overflow: hidden;
  padding-bottom: 2rem;
}

/* Floating Background */
.moments-page::before,
.moments-page::after {
  content: "";
  position: absolute;
  border-radius: 50%;
  z-index: -1;
}

.moments-page::before {
  width: 320px;
  height: 320px;
  top: 40px;
  right: -120px;
  background: radial-gradient(circle, rgba(26,115,232,0.18), transparent 70%);
}

.moments-page::after {
  width: 260px;
  height: 260px;
  bottom: 120px;
  left: -120px;
  background: radial-gradient(circle, rgba(0,188,212,0.16), transparent 70%);
}

/* Hero Section */
.moments-hero {
  position: relative;
  padding: 2.4rem 2rem;
  margin: 1.5rem 0 2rem;
  border-radius: 28px;
  background:
    linear-gradient(135deg, rgba(26,115,232,0.12), rgba(255,255,255,0.92)),
    linear-gradient(45deg, rgba(0,188,212,0.10), rgba(255,255,255,0.95));
  border: 1px solid var(--border);
  box-shadow: 0 18px 45px rgba(15, 23, 42, 0.08);
  overflow: hidden;
}

.moments-hero::before {
  content: "Research • Teaching • Leadership • Service";
  position: absolute;
  right: -30px;
  top: 22px;
  transform: rotate(12deg);
  font-size: 0.75rem;
  letter-spacing: 0.14em;
  color: rgba(26,115,232,0.28);
  font-weight: 800;
  text-transform: uppercase;
}

.moments-kicker {
  display: inline-block;
  margin-bottom: 0.8rem;
  padding: 0.38rem 0.8rem;
  border-radius: 999px;
  background: rgba(26,115,232,0.12);
  color: var(--primary);
  font-size: 0.78rem;
  font-weight: 800;
  letter-spacing: 0.05em;
  text-transform: uppercase;
}

.moments-hero h2 {
  margin: 0 0 0.7rem;
  color: var(--dark);
  font-size: 2.25rem;
  line-height: 1.15;
  font-weight: 850;
}

.moments-hero p {
  max-width: 850px;
  margin: 0;
  color: var(--muted);
  line-height: 1.75;
  font-size: 1rem;
}

/* Summary Cards */
.moments-summary {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(165px, 1fr));
  gap: 1rem;
  margin: 1.5rem 0 2.2rem;
}

.summary-card {
  position: relative;
  padding: 1.1rem;
  border-radius: 20px;
  background: var(--card);
  border: 1px solid rgba(15, 23, 42, 0.08);
  box-shadow: 0 12px 28px rgba(15, 23, 42, 0.06);
  backdrop-filter: blur(10px);
  transition: 0.25s ease;
  overflow: hidden;
}

.summary-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 18px 36px rgba(26,115,232,0.13);
}

.summary-card::after {
  content: "";
  position: absolute;
  right: -28px;
  bottom: -28px;
  width: 82px;
  height: 82px;
  border-radius: 50%;
  background: rgba(26,115,232,0.09);
}

.summary-card span {
  display: block;
  color: var(--primary);
  font-size: 1.35rem;
  font-weight: 850;
}

.summary-card small {
  color: var(--muted);
  font-size: 0.82rem;
}

/* Timeline Layout */
.moments-timeline {
  position: relative;
  margin-top: 1.5rem;
}

.moments-timeline::before {
  content: "";
  position: absolute;
  top: 0;
  left: 22px;
  width: 3px;
  height: 100%;
  background: linear-gradient(to bottom, var(--primary), var(--accent));
  border-radius: 999px;
  opacity: 0.45;
}

/* Timeline Item */
.moment-item {
  position: relative;
  margin-left: 54px;
  margin-bottom: 1.8rem;
}

.moment-dot {
  position: absolute;
  left: -43px;
  top: 28px;
  width: 18px;
  height: 18px;
  border-radius: 50%;
  background: linear-gradient(135deg, var(--primary), var(--accent));
  border: 4px solid #ffffff;
  box-shadow: 0 0 0 4px rgba(26,115,232,0.12);
  z-index: 2;
}

.moment-card {
  display: grid;
  grid-template-columns: minmax(240px, 42%) 1fr;
  gap: 0;
  border-radius: 24px;
  background: var(--card);
  border: 1px solid rgba(26,115,232,0.18);
  box-shadow: 0 14px 34px rgba(15, 23, 42, 0.08);
  overflow: hidden;
  backdrop-filter: blur(12px);
  transition: transform 0.25s ease, box-shadow 0.25s ease, border-color 0.25s ease;
}

.moment-card:hover {
  transform: translateY(-5px);
  border-color: rgba(26,115,232,0.45);
  box-shadow: 0 22px 46px rgba(26,115,232,0.16);
}

.moment-image {
  position: relative;
  min-height: 250px;
  overflow: hidden;
  background: #eaf2ff;
}

.moment-image img {
  width: 100%;
  height: 100%;
  min-height: 250px;
  object-fit: cover;
  display: block;
  cursor: pointer;
  transition: transform 0.45s ease, filter 0.3s ease;
  -webkit-user-drag: none;
  user-drag: none;
}

.moment-card:hover .moment-image img {
  transform: scale(1.06);
  filter: brightness(0.96);
}

.moment-badge {
  position: absolute;
  top: 16px;
  left: 16px;
  padding: 0.38rem 0.7rem;
  border-radius: 999px;
  background: rgba(15, 23, 42, 0.78);
  color: #ffffff;
  font-size: 0.72rem;
  font-weight: 750;
  letter-spacing: 0.03em;
  backdrop-filter: blur(8px);
}

.moment-year {
  position: absolute;
  right: 16px;
  bottom: 16px;
  padding: 0.35rem 0.7rem;
  border-radius: 999px;
  background: rgba(255,255,255,0.86);
  color: var(--primary-dark);
  font-size: 0.75rem;
  font-weight: 850;
  box-shadow: 0 8px 18px rgba(15,23,42,0.14);
}

.moment-content {
  padding: 1.35rem 1.45rem;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.moment-content h3 {
  margin: 0 0 0.6rem;
  color: var(--dark);
  font-size: 1.22rem;
  line-height: 1.35;
  font-weight: 850;
}

.moment-content p {
  margin: 0;
  color: #475569;
  font-size: 0.94rem;
  line-height: 1.7;
}

.moment-tags {
  margin-top: 1rem;
  display: flex;
  flex-wrap: wrap;
  gap: 0.45rem;
}

.moment-tags span {
  padding: 0.3rem 0.62rem;
  border-radius: 999px;
  background: #eef6ff;
  color: var(--primary);
  border: 1px solid rgba(26,115,232,0.16);
  font-size: 0.72rem;
  font-weight: 700;
}

/* Copyright */
.moments-copyright {
  margin-top: 2.4rem;
  padding: 1.05rem 1.2rem;
  border-left: 5px solid var(--primary);
  background: rgba(248,251,255,0.92);
  border-radius: 14px;
  color: #475569;
  font-size: 0.86rem;
  line-height: 1.65;
  box-shadow: 0 8px 20px rgba(15,23,42,0.04);
}

/* Lightbox */
.lightbox-overlay {
  position: fixed;
  inset: 0;
  background: rgba(2, 6, 23, 0.94);
  display: none;
  align-items: center;
  justify-content: center;
  z-index: 9999;
  padding: 1rem;
}

.lightbox-overlay img {
  max-width: 92%;
  max-height: 86%;
  border-radius: 18px;
  box-shadow: 0 0 42px rgba(255,255,255,0.20);
  animation: zoomIn 0.25s ease;
  -webkit-user-drag: none;
  user-drag: none;
}

.lightbox-close {
  position: fixed;
  top: 22px;
  right: 30px;
  color: #ffffff;
  font-size: 2.2rem;
  font-weight: 800;
  cursor: pointer;
  opacity: 0.85;
}

.lightbox-close:hover {
  opacity: 1;
}

@keyframes zoomIn {
  from {
    transform: scale(0.92);
    opacity: 0;
  }
  to {
    transform: scale(1);
    opacity: 1;
  }
}

/* Copy Deterrent */
.moments-protected {
  -webkit-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

/* Responsive */
@media (max-width: 820px) {
  .moment-card {
    grid-template-columns: 1fr;
  }

  .moment-image {
    min-height: 230px;
  }

  .moments-hero h2 {
    font-size: 1.8rem;
  }
}

@media (max-width: 560px) {
  .moments-hero {
    padding: 1.45rem;
    border-radius: 22px;
  }

  .moments-hero h2 {
    font-size: 1.55rem;
  }

  .moments-timeline::before {
    left: 12px;
  }

  .moment-item {
    margin-left: 38px;
  }

  .moment-dot {
    left: -34px;
  }

  .moment-content {
    padding: 1.1rem;
  }

  .moment-image img {
    min-height: 205px;
  }
}
</style>

<div class="moments-page moments-protected">

  <section class="moments-hero">
    <span class="moments-kicker">Selected Highlights</span>
    <h2>Memorable Moments</h2>
    <p>
      A visual timeline of selected academic, research, teaching, leadership, and professional milestones.
      These highlights represent conference participation, research recognition, classroom engagement,
      and service contributions across my academic journey.
    </p>
  </section>

  <section class="moments-summary">
    <div class="summary-card">
      <span>2025</span>
      <small>Conference and research highlights</small>
    </div>

    <div class="summary-card">
      <span>IEEE</span>
      <small>Recognition in RF communication research</small>
    </div>

    <div class="summary-card">
      <span>SGA</span>
      <small>Leadership and student service</small>
    </div>

    <div class="summary-card">
      <span>ASIC</span>
      <small>Teaching and classroom experience</small>
    </div>
  </section>

  <section class="moments-timeline">

    <div class="moment-item">
      <div class="moment-dot"></div>
      <article class="moment-card">
        <div class="moment-image">
          <img src="/images/glsvlsi.jpeg" alt="Poster Presentation at GLSVLSI 2025">
          <div class="moment-badge">Conference</div>
          <div class="moment-year">2025</div>
        </div>
        <div class="moment-content">
          <h3>Poster Presentation at GLSVLSI 2025</h3>
          <p>
            Presented research work at the Great Lakes Symposium on VLSI, held from June 30 to July 2,
            2025, in New Orleans, Louisiana, USA. This event provided an opportunity to share work
            with the VLSI and hardware research community.
          </p>
          <div class="moment-tags">
            <span>GLSVLSI</span>
            <span>VLSI</span>
            <span>Poster Presentation</span>
          </div>
        </div>
      </article>
    </div>

    <div class="moment-item">
      <div class="moment-dot"></div>
      <article class="moment-card">
        <div class="moment-image">
          <img src="/images/rfcon_award.png" alt="Best Paper Award at RFCoN 2025">
          <div class="moment-badge">Award</div>
          <div class="moment-year">2025</div>
        </div>
        <div class="moment-content">
          <h3>Best Paper Award – RFCoN 2025</h3>
          <p>
            Received the Best Paper Award at the IEEE International Conference on RF Communication
            and Networks, Track 2, Session II. This recognition highlights the contribution of my work
            in RF communication and signal processing research.
          </p>
          <div class="moment-tags">
            <span>IEEE</span>
            <span>RFCoN 2025</span>
            <span>Best Paper Award</span>
          </div>
        </div>
      </article>
    </div>

    <div class="moment-item">
      <div class="moment-dot"></div>
      <article class="moment-card">
        <div class="moment-image">
          <img src="/images/sg_senator_result.png" alt="SGA Senator Re-election">
          <div class="moment-badge">Leadership</div>
          <div class="moment-year">2024–2025</div>
        </div>
        <div class="moment-content">
          <h3>Re-Elected as SGA Senator</h3>
          <p>
            Re-elected as Student Government Association Senator for the School of Science and Engineering
            for the 2024–2025 academic year, continuing service through student representation,
            academic engagement, and campus leadership.
          </p>
          <div class="moment-tags">
            <span>SGA</span>
            <span>Leadership</span>
            <span>Service</span>
          </div>
        </div>
      </article>
    </div>

    <div class="moment-item">
      <div class="moment-dot"></div>
      <article class="moment-card">
        <div class="moment-image">
          <img src="/images/asic_class_fall2023.png" alt="ASIC Physical Design Teaching">
          <div class="moment-badge">Teaching</div>
          <div class="moment-year">Fall 2023</div>
        </div>
        <div class="moment-content">
          <h3>Instructor – ASIC Physical Design</h3>
          <p>
            Fall 2023 marked my first course as instructor, focused on ASIC Physical Design.
            The course provided an opportunity to engage students with practical concepts in synthesis,
            floorplanning, placement, routing, timing analysis, and chip design flow.
          </p>
          <div class="moment-tags">
            <span>Teaching</span>
            <span>ASIC</span>
            <span>Physical Design</span>
          </div>
        </div>
      </article>
    </div>

  </section>

  <div class="moments-copyright">
    © 2026 Srinivas Rahul S. All rights reserved. The text, images, layout, and design elements on this page
    may not be copied, reproduced, republished, modified, or redistributed without prior written permission.
  </div>

</div>

<!-- Lightbox Container -->
<div class="lightbox-overlay" id="lightbox">
  <span class="lightbox-close" id="lightbox-close">&times;</span>
  <img id="lightbox-img" src="" alt="">
</div>

<script>
document.addEventListener("DOMContentLoaded", function () {
  const images = document.querySelectorAll(".moment-image img");
  const lightbox = document.getElementById("lightbox");
  const lightboxImg = document.getElementById("lightbox-img");
  const closeBtn = document.getElementById("lightbox-close");

  images.forEach(img => {
    img.addEventListener("click", () => {
      lightboxImg.src = img.src;
      lightboxImg.alt = img.alt;
      lightbox.style.display = "flex";
    });
  });

  function closeLightbox() {
    lightbox.style.display = "none";
    lightboxImg.src = "";
    lightboxImg.alt = "";
  }

  lightbox.addEventListener("click", function(e) {
    if (e.target === lightbox) {
      closeLightbox();
    }
  });

  closeBtn.addEventListener("click", closeLightbox);

  document.addEventListener("keydown", function(e) {
    if (e.key === "Escape") {
      closeLightbox();
    }
  });

  /* Casual copy deterrent */
  document.addEventListener("contextmenu", function(e) {
    if (e.target.closest(".moments-protected")) {
      e.preventDefault();
    }
  });

  document.addEventListener("keydown", function(e) {
    const blockedKeys = ["c", "u", "s", "a"];

    if ((e.ctrlKey || e.metaKey) && blockedKeys.includes(e.key.toLowerCase())) {
      if (document.activeElement.closest(".moments-protected")) {
        e.preventDefault();
      }
    }
  });
});
</script>
