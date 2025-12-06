---
title: "Gallery"
layout: single
permalink: /gallery/
author_profile: true
---

<style>
.highlight-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 1.5rem;
}


.highlight-card {
  background: #f0f8ff;
  border: 2px solid #1a73e8;
  border-radius: 12px;
  padding: 1rem;
  box-shadow: 0 4px 12px rgba(0,0,0,0.05);
  transition: 0.3s ease-in-out;
}

.highlight-card:hover {
  background: #e6f0ff;
  transform: scale(1.01);
}

.highlight-card img {
  width: 100%;
  height: 180px;     /* adjust to control size */
  object-fit: cover; /* crops edges to maintain shape */
  border-radius: 10px;
  margin-bottom: 0.5rem;
}



.highlight-card h4 {
  margin: 0.5rem 0 0.3rem;
  color: #1a73e8;
}

/* Lightbox styles */
.lightbox-overlay {
  position: fixed;
  top: 0; left: 0;
  width: 100vw; height: 100vh;
  background: rgba(0, 0, 0, 0.9);
  display: none;
  align-items: center;
  justify-content: center;
  z-index: 9999;
}

.lightbox-overlay img {
  max-width: 90%;
  max-height: 90%;
  border-radius: 12px;
  box-shadow: 0 0 20px rgba(255,255,255,0.2);
  animation: zoomIn 0.3s ease;
}

@keyframes zoomIn {
  from { transform: scale(0.9); opacity: 0; }
  to { transform: scale(1); opacity: 1; }
}

/* Make cards a bit tighter on phones */
@media (max-width: 600px) {
  .highlight-grid {
    grid-template-columns: 1fr;          /* one card per row */
    gap: 1rem;
  }

  .highlight-card {
    max-width: 420px;
    margin: 0 auto;                      /* center the card */
  }

  .highlight-card img,
  .gallery-img {                         /* gallery-img if you're using it */
    width: 100%;
    height: 220px;                       /* fixed height for all images */
    object-fit: cover;                   /* crop nicely instead of stretching */
    object-position: center;             /* center the crop */
    border-radius: 12px;
  }
}
</style>

## 🎉 Memorable Moments

Welcome to my personal gallery — moments from my academic journey, graduation, research labs, and team milestones.

<div class="highlight-grid">
   
  <div class="highlight-card">
     <img src="/images/orientation1.jpeg" alt="orientation">
     <h4>Welcoming new students at UMKC Orientation, Fall 2025.</h4>
  </div>

  <div class="highlight-card">
    <img src="/images/shyu.jpeg" alt="Office">
    <h4>With Professor Shyu, UMKC</h4>
  </div>

  <div class="highlight-card">
    <img src="/images/most.jpeg" alt="Office">
    <h4>With Professor Rahman, UMKC (Ph.D. Advisor)</h4>
  </div>

  <div class="highlight-card">
    <img src="/images/masud1.jpeg" alt="Poster 1">
    <h4>With Professor Masud, UMKC (Mentor and Department Chair).</h4>
  </div>

  <div class="highlight-card">
    <img src="/images/pos1.jpeg" alt="Poster 1">
    <h4>GLSVLSI Conference 2025</h4>
  </div>

  <div class="highlight-card">
    <img src="/images/pos2.jpeg" alt="Poster 1">
    <h4>GLSVLSI Conference 2025</h4>
  </div>

  <div class="highlight-card">
    <img src="/images/grad0.jpg" alt="Graduation 1">
    <h4>UMKC Master’s Graduation</h4>
  </div>

  <div class="highlight-card">
    <img src="/images/grad1.jpg" alt="Graduation 1">
    <h4>UMKC Master’s Graduation, 2016</h4>
  </div>

  <div class="highlight-card">
    <img src="/images/grad2.jpg" alt="Graduation 1">
    <h4>UMKC Master’s Graduation, 2016</h4>
  </div>

  <div class="highlight-card">
    <img src="/images/grad3.jpg" alt="Graduation 1">
    <h4>UMKC Master’s Graduation, 2016</h4>
  </div>

  <div class="highlight-card">
    <img src="/images/grad4.jpg" alt="Graduation 1">
    <h4>UMKC Master’s Graduation, 2016</h4>
  </div>

  <div class="highlight-card">
    <img src="/images/grad5.jpg" alt="Graduation 1">
    <h4>UMKC Master’s Graduation, 2016</h4>
  </div>

  <div class="highlight-card">
    <img src="/images/grad7.jpeg" alt="Poster 3">
    <h4>UIS Master’s Graduation, 2018</h4>
  </div>

  <div class="highlight-card">
    <img src="/images/grad6.jpeg" alt="Poster 3">
    <h4>UIS Master’s Graduation, 2018</h4>
  </div>

  <div class="highlight-card">
    <img src="/images/pos3.jpeg" alt="Poster 3">
    <h4>GLSVLSI Conference</h4>
  </div>

  
</div>

<!-- Lightbox Container -->
<div class="lightbox-overlay" id="lightbox">
  <img id="lightbox-img" src="" alt="">
</div>

<script>
document.addEventListener("DOMContentLoaded", function () {
  const images = document.querySelectorAll(".highlight-card img");
  const lightbox = document.getElementById("lightbox");
  const lightboxImg = document.getElementById("lightbox-img");

  images.forEach(img => {
    img.addEventListener("click", () => {
      lightboxImg.src = img.src;
      lightbox.style.display = "flex";
    });
  });

  lightbox.addEventListener("click", () => {
    lightbox.style.display = "none";
    lightboxImg.src = "";
  });
});
</script>
