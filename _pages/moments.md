---
title: "Moments"
layout: single
permalink: /moments/
author_profile: true
---

<style>
:root {
  --moments-primary: #1a73e8;
  --moments-dark: #0f172a;
  --moments-muted: #64748b;
  --moments-bg: #f8fbff;
  --moments-card: #ffffff;
  --moments-border: rgba(26, 115, 232, 0.22);
}

/* Page Header */
.moments-hero {
  background: linear-gradient(135deg, #eef6ff 0%, #ffffff 50%, #f4f8ff 100%);
  border: 1px solid var(--moments-border);
  border-radius: 22px;
  padding: 2rem;
  margin: 1.5rem 0 2rem;
  box-shadow: 0 12px 30px rgba(15, 23, 42, 0.06);
  position: relative;
  overflow: hidden;
}

.moments-hero::before {
  content: "";
  position: absolute;
  top: -70px;
  right: -70px;
  width: 180px;
  height: 180px;
  background: radial-gradient(circle, rgba(26,115,232,0.18), transparent 70%);
  border-radius: 50%;
}

.moments-hero h2 {
  margin: 0 0 0.7rem;
  color: var(--moments-dark);
  font-size: 2rem;
  font-weight: 800;
}

.moments-hero p {
  margin: 0;
  color: var(--moments-muted);
  font-size: 1rem;
  line-height: 1.7;
  max-width: 850px;
}

/* Stats Strip */
.moments-strip {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
  gap: 1rem;
  margin: 1.5rem 0 2rem;
}

.moments-stat {
  background: #ffffff;
  border: 1px solid rgba(15, 23, 42, 0.08);
  border-radius: 16px;
  padding: 1rem;
  text-align: center;
  box-shadow: 0 8px 20px rgba(15, 23, 42, 0.04);
}

.moments-stat span {
  display: block;
  color: var(--moments-primary);
  font-size: 1.5rem;
  font-weight: 800;
}

.moments-stat small {
  color: var(--moments-muted);
  font-size: 0.82rem;
}

/* Grid */
.highlight-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(310px, 1fr));
  gap: 1.5rem;
  margin-top: 1.5rem;
}

/* Cards */
.highlight-card {
  background: var(--moments-card);
  border: 1px solid rgba(26, 115, 232, 0.20);
  border-radius: 20px;
  overflow: hidden;
  box-shadow: 0 10px 26px rgba(15, 23, 42, 0.07);
  transition: transform 0.25s ease, box-shadow 0.25s ease, border-color 0.25s ease;
  position: relative;
}

.highlight-card:hover {
  transform: translateY(-6px);
  box-shadow: 0 18px 38px rgba(26, 115, 232, 0.16);
  border-color: rgba(26, 115, 232, 0.45);
}

.highlight-image-wrap {
  position: relative;
  overflow: hidden;
  background: #eaf2ff;
}

.highlight-card img {
  width: 100%;
  height: 230px;
  object-fit: cover;
  display: block;
  cursor: pointer;
  transition: transform 0.35s ease, filter 0.35s ease;
  -webkit-user-drag: none;
  user-drag: none;
}

.highlight-card:hover img {
  transform: scale(1.045);
  filter: brightness(0.96);
}

.highlight-badge {
  position: absolute;
  top: 14px;
  left: 14px;
  background: rgba(26, 115, 232, 0.94);
  color: #ffffff;
  font-size: 0.72rem;
  font-weight: 700;
  padding: 0.35rem 0.65rem;
  border-radius: 999px;
  letter-spacing: 0.02em;
  box-shadow: 0 6px 16px rgba(15, 23, 42, 0.18);
}

.highlight-content {
  padding: 1.1rem 1.15rem 1.25rem;
}

.highlight-card h4 {
  margin: 0 0 0.45rem;
  color: var(--moments-dark);
  font-size: 1.05rem;
  line-height: 1.35;
}

.highlight-card p {
  margin: 0;
  color: #475569;
  font-size: 0.92rem;
  line-height: 1.65;
}

.highlight-meta {
  margin-top: 0.85rem;
  display: flex;
  flex-wrap: wrap;
  gap: 0.45rem;
}

.highlight-meta span {
  background: #eef6ff;
  color: #1a73e8;
  border: 1px solid rgba(26, 115, 232, 0.16);
  padding: 0.28rem 0.55rem;
  border-radius: 999px;
  font-size: 0.72rem;
  font-weight: 650;
}

/* Copyright Notice */
.moments-copyright {
  margin-top: 2.2rem;
  padding: 1rem 1.2rem;
  border-left: 4px solid var(--moments-primary);
  background: #f8fbff;
  border-radius: 12px;
  color: #475569;
  font-size: 0.86rem;
  line-height: 1.6;
}

/* Lightbox */
.lightbox-overlay {
  position: fixed;
  inset: 0;
  width: 100vw;
  height: 100vh;
  background: rgba(2, 6, 23, 0.92);
  display: none;
  align-items: center;
  justify-content: center;
  z-index: 9999;
  padding: 1rem;
}

.lightbox-overlay img {
  max-width: 92%;
  max-height: 86%;
  border-radius: 16px;
  box-shadow: 0 0 34px rgba(255,255,255,0.18);
  animation: zoomIn 0.25s ease;
  -webkit-user-drag: none;
  user-drag: none;
}

.lightbox-close {
  position: fixed;
  top: 22px;
  right: 28px;
  color: #ffffff;
  font-size: 2rem;
  font-weight: 700;
  cursor: pointer;
  line-height: 1;
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

/* Light copy deterrent */
.moments-protected {
  -webkit-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

/* Mobile */
@media (max-width: 640px) {
  .moments-hero {
    padding: 1.3rem;
  }

  .moments-hero h2 {
    font-size: 1.55rem;
  }

  .highlight-card img {
    height: 200px;
  }
}
</style>

<div class="moments-protected">

<div class="moments-hero">
  <h2>Memorable Moments</h2>
  <p>
    A collection of selected academic, research, teaching, leadership, and professional milestones.
    These moments reflect conference participation, recognition, classroom engagement, and service contributions.
  </p>
</div>

<div class="moments-strip">
  <div class="moments-stat">
    <span>2025</span>
    <small>Conference Highlights</small>
  </div>

  <div class="moments-stat">
    <span>IEEE</span>
    <small>Research Recognition</small>
  </div>

  <div class="moments-stat">
    <span>SGA</span>
    <small>Leadership and Service</small>
  </div>

  <div class="moments-stat">
    <span>ASIC</span>
    <small>Teaching Experience</small>
  </div>
</div>

<div class="highlight-grid">

  <div class="highlight-card">
    <div class="highlight-image-wrap">
      <img src="/images/glsvlsi.jpeg" alt="Poster Presentation at GLSVLSI 2025">
      <div class="highlight-badge">Conference</div>
    </div>
    <div class="highlight-content">
      <h4>Poster Presentation at GLSVLSI 2025</h4>
      <p>
        Poster presentation at the Great Lakes Symposium on VLSI, held from June 30 to July 2, 2025,
        in New Orleans, Louisiana, USA.
      </p>
      <div class="highlight-meta">
        <span>GLSVLSI 2025</span>
        <span>VLSI</span>
        <span>Poster</span>
      </div>
    </div>
  </div>

  <div class="highlight-card">
    <div class="highlight-image-wrap">
      <img src="/images/rfcon_award.png" alt="Best Paper Award at RFCoN 2025">
      <div class="highlight-badge">Award</div>
    </div>
    <div class="highlight-content">
      <h4>Best Paper Award – RFCoN 2025</h4>
      <p>
        Honored to receive the Best Paper Award at the IEEE International Conference on RF Communication
        and Networks, Track 2, Session II.
      </p>
      <div class="highlight-meta">
        <span>IEEE</span>
        <span>RFCoN 2025</span>
        <span>Best Paper</span>
      </div>
    </div>
  </div>

  <div class="highlight-card">
    <div class="highlight-image-wrap">
      <img src="/images/sg_senator_result.png" alt="SGA Senator Re-election">
      <div class="highlight-badge">Leadership</div>
    </div>
    <div class="highlight-content">
      <h4>Re-Elected as SGA Senator</h4>
      <p>
        Re-elected as Student Government Association Senator for the School of Science and Engineering
        for the 2024–2025 academic year.
      </p>
      <div class="highlight-meta">
        <span>SGA</span>
        <span>Service</span>
        <span>Leadership</span>
      </div>
    </div>
  </div>

  <div class="highlight-card">
    <div class="highlight-image-wrap">
      <img src="/images/asic_class_fall2023.png" alt="ASIC Physical Design Teaching">
      <div class="highlight-badge">Teaching</div>
    </div>
    <div class="highlight-content">
      <h4>Instructor – ASIC Physical Design</h4>
      <p>
        Fall 2023 marked my first course as instructor, with strong classroom engagement and active
        student participation in ASIC physical design concepts.
      </p>
      <div class="highlight-meta">
        <span>Teaching</span>
        <span>ASIC</span>
        <span>Physical Design</span>
      </div>
    </div>
  </div>

</div>

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
  const images = document.querySelectorAll(".highlight-card img");
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
