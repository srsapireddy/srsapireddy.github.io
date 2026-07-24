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
  --isu: #DC143C;
  --dark: #0f172a;
  --muted: #64748b;
  --light: #f8fbff;
  --card: rgba(255, 255, 255, 0.90);
  --border: rgba(26, 115, 232, 0.20);
  --shadow: 0 10px 30px rgba(0,0,0,0.08);
  --shadow2: 0 2px 10px rgba(0,0,0,0.05);
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

/* Main Wrapper */
.moments-page {
  position: relative;
  overflow: hidden;
  padding-bottom: 2rem;
  animation: fadeInUp 0.85s ease-in-out;
}

/* Hero Section */
.moments-hero {
  position: relative;
  padding: 2.35rem 2rem;
  margin: 1.5rem 0 1.3rem;
  border-radius: 24px;
  background:
    radial-gradient(circle at top right, rgba(220,20,60,0.13), transparent 32%),
    linear-gradient(135deg, #e9f3ff 0%, #ffffff 62%);
  border: 1px solid rgba(26,115,232,0.25);
  box-shadow: var(--shadow);
  overflow: hidden;
}

.moments-hero::before {
  content: "";
  position: absolute;
  inset: 0;
  background-image:
    linear-gradient(rgba(26,115,232,0.06) 1px, transparent 1px),
    linear-gradient(90deg, rgba(26,115,232,0.06) 1px, transparent 1px);
  background-size: 34px 34px;
  pointer-events: none;
}

.moments-hero-content {
  position: relative;
  z-index: 1;
}

.moments-kicker {
  display: inline-block;
  margin-bottom: 0.85rem;
  padding: 0.36rem 0.78rem;
  border-radius: 999px;
  background: #ffffff;
  border: 1px solid rgba(220,20,60,0.25);
  color: var(--isu);
  font-size: 0.88rem;
  font-weight: 900;
  box-shadow: var(--shadow2);
}

.moments-hero h1 {
  margin: 0;
  color: #0b1f44;
  font-size: 2.15rem;
  line-height: 1.15;
  font-weight: 900;
}

.moments-hero p {
  max-width: 880px;
  margin: 0.75rem 0 0 0;
  color: var(--muted);
  line-height: 1.7;
  font-size: 1.03rem;
}

.hero-badges {
  display: flex;
  flex-wrap: wrap;
  gap: 0.55rem;
  margin-top: 1rem;
}

.hero-badge {
  display: inline-flex;
  align-items: center;
  padding: 0.36rem 0.72rem;
  border-radius: 999px;
  background: #ffffff;
  border: 1px solid rgba(26,115,232,0.22);
  color: #0b1f44;
  box-shadow: var(--shadow2);
  font-size: 0.88rem;
  font-weight: 850;
}

.hero-badge.red {
  border-color: rgba(220,20,60,0.30);
  color: #7a0b1f;
  background: rgba(220,20,60,0.06);
}

/* Sliding Bar */
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
  animation: slideTrack 34s linear infinite;
}

.sliding-bar:hover .slide-track {
  animation-play-state: paused;
}

.slide-item {
  display: inline-flex;
  align-items: center;
  gap: 0.4rem;
  padding: 0.75rem 1.2rem;
  color: #0b1f44;
  font-weight: 900;
  white-space: nowrap;
  border-right: 1px solid rgba(26,115,232,0.10);
}

.slide-item span {
  color: var(--isu);
}

/* Summary Cards */
.moments-summary {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 0.95rem;
  margin: 1.3rem 0;
}

.summary-card {
  position: relative;
  padding: 1.1rem 1rem;
  border-radius: 16px;
  background: linear-gradient(135deg, #ffffff 0%, #f7fbff 100%);
  border: 1px solid rgba(26,115,232,0.18);
  box-shadow: var(--shadow2);
  text-align: center;
  transition: 0.25s ease-in-out;
  overflow: hidden;
}

.summary-card:hover {
  transform: translateY(-3px);
  box-shadow: var(--shadow);
}

.summary-card span {
  display: block;
  color: var(--isu);
  font-size: 1.5rem;
  font-weight: 950;
  line-height: 1.1;
}

.summary-card small {
  display: block;
  color: var(--muted);
  font-size: 0.82rem;
  margin-top: 0.28rem;
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
  background: linear-gradient(to bottom, var(--primary), var(--isu));
  border-radius: 999px;
  opacity: 0.45;
}

/* Timeline Item */
.moment-item {
  position: relative;
  margin-left: 54px;
  margin-bottom: 1.35rem;
}

.moment-dot {
  position: absolute;
  left: -43px;
  top: 28px;
  width: 18px;
  height: 18px;
  border-radius: 50%;
  background: linear-gradient(135deg, var(--primary), var(--isu));
  border: 4px solid #ffffff;
  box-shadow: 0 0 0 4px rgba(26,115,232,0.12);
  z-index: 2;
}

.moment-card {
  display: grid;
  grid-template-columns: minmax(260px, 42%) 1fr;
  gap: 0;
  border-radius: 20px;
  background: var(--card);
  border: 1px solid rgba(26,115,232,0.18);
  box-shadow: var(--shadow2);
  overflow: hidden;
  transition: 0.25s ease-in-out;
}

.moment-card:hover {
  transform: translateY(-5px);
  border-color: rgba(26,115,232,0.40);
  box-shadow: var(--shadow);
}

.moment-image {
  position: relative;
  min-height: 280px;
  overflow: hidden;
  background: #ffffff;
}

/* IMPORTANT FIX: contain prevents image 1 and image 4 from being cut */
.moment-image img {
  width: 100%;
  height: 100%;
  min-height: 280px;
  object-fit: contain;
  object-position: center;
  display: block;
  cursor: pointer;
  transition: transform 0.35s ease, filter 0.25s ease;
  -webkit-user-drag: none;
  user-drag: none;
  background: #ffffff;
  padding: 0.35rem;
}

.moment-card:hover .moment-image img {
  transform: scale(1.025);
  filter: brightness(0.98);
}

.moment-badge {
  position: absolute;
  top: 16px;
  left: 16px;
  padding: 0.36rem 0.7rem;
  border-radius: 999px;
  background: rgba(15,23,42,0.80);
  color: #ffffff;
  font-size: 0.72rem;
  font-weight: 850;
  letter-spacing: 0.03em;
  backdrop-filter: blur(8px);
}

.moment-year {
  position: absolute;
  right: 16px;
  bottom: 16px;
  padding: 0.35rem 0.7rem;
  border-radius: 999px;
  background: rgba(255,255,255,0.92);
  color: var(--primary-dark);
  font-size: 0.75rem;
  font-weight: 900;
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
  color: #0b1f44;
  font-size: 1.2rem;
  line-height: 1.35;
  font-weight: 950;
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
  font-weight: 800;
}

/* Copyright */
.moments-copyright {
  margin-top: 2rem;
  padding: 1.05rem 1.2rem;
  border-left: 5px solid var(--primary);
  background: rgba(248,251,255,0.92);
  border-radius: 14px;
  color: #475569;
  font-size: 0.86rem;
  line-height: 1.65;
  box-shadow: var(--shadow2);
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
  object-fit: contain;
  border-radius: 18px;
  box-shadow: 0 0 42px rgba(255,255,255,0.20);
  animation: zoomIn 0.25s ease;
  -webkit-user-drag: none;
  user-drag: none;
  background: #ffffff;
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

/* Copy Deterrent */
.moments-protected {
  -webkit-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

/* Responsive */
@media (max-width: 950px) {
  .moments-summary {
    grid-template-columns: repeat(2, 1fr);
  }

  .moment-card {
    grid-template-columns: 1fr;
  }

  .moment-image,
  .moment-image img {
    min-height: 300px;
  }
}

@media (max-width: 700px) {
  .moments-hero {
    padding: 1.5rem 1.1rem;
  }

  .moments-hero h1 {
    font-size: 1.65rem;
  }

  .moments-summary {
    grid-template-columns: 1fr;
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

  .moment-image,
  .moment-image img {
    min-height: 260px;
  }
}
</style>

<div class="moments-page moments-protected">

  <section class="moments-hero">
    <div class="moments-hero-content">
      <span class="moments-kicker">Selected Highlights</span>

      <h1>Memorable Moments</h1>

      <p>
        A visual timeline of selected academic, research, teaching, leadership, and professional milestones.
        These highlights represent conference participation, research recognition, classroom engagement,
        and service contributions across my academic journey.
      </p>

      <div class="hero-badges">
        <span class="hero-badge red">Research Recognition</span>
        <span class="hero-badge">Conference Presentation</span>
        <span class="hero-badge">Leadership</span>
        <span class="hero-badge">Teaching</span>
      </div>
    </div>
  </section>

  <div class="sliding-bar">
    <div class="slide-track">
      <div class="slide-item"><span>●</span> GLSVLSI 2025 Poster Presentation</div>
      <div class="slide-item"><span>●</span> RFCoN 2025 Best Paper Award</div>
      <div class="slide-item"><span>●</span> SGA Senator Leadership</div>
      <div class="slide-item"><span>●</span> ASIC Physical Design Teaching</div>

      <div class="slide-item"><span>●</span> GLSVLSI 2025 Poster Presentation</div>
      <div class="slide-item"><span>●</span> RFCoN 2025 Best Paper Award</div>
      <div class="slide-item"><span>●</span> SGA Senator Leadership</div>
      <div class="slide-item"><span>●</span> ASIC Physical Design Teaching</div>
    </div>
  </div>

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
      <img
        src="/images/engineering-building-interview.jpg"
        alt="The Pantagraph coverage of Illinois State University College of Engineering"
      >

        <div class="moment-badge">Media Coverage</div>
        <div class="moment-year">2026</div>
        </div>
    
        <div class="moment-content">
          <h3>Featured in The Pantagraph</h3>
    
          <p>
            Featured in The Pantagraph’s coverage of Illinois State University’s
            new College of Engineering building. Discussed the Digital and
            Microcontrollers Laboratory and the role of hands-on learning in
            electrical engineering education.
          </p>
    
          <div class="moment-tags">
            <span>The Pantagraph</span>
            <span>Media Coverage</span>
            <span>Engineering Education</span>
          </div>
    
          <a
            href="https://pantagraph.com/news/local/video_4dd9fcd5-99bd-548a-af33-ed2bc76f7506.html"
            class="moment-link"
            target="_blank"
            rel="noopener noreferrer"
          >
            View Media Coverage →
          </a>
        </div>
      </article>
    </div>

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
          <h3>Best Paper Award - RFCoN 2025</h3>
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
          <div class="moment-year">2024-2025</div>
        </div>

        <div class="moment-content">
          <h3>Re-Elected as SGA Senator</h3>
          <p>
            Re-elected as Student Government Association Senator for the School of Science and Engineering
            for the 2024-2025 academic year, continuing service through student representation,
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
          <h3>Instructor - ASIC Physical Design</h3>
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

  images.forEach(function(img) {
    img.addEventListener("click", function() {
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
