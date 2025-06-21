---
title: "Moments"
layout: single
permalink: /moments/
author_profile: true
---

<style>
.highlight-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
  gap: 1.5rem;
  margin-top: 1.5rem;
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
  border-radius: 10px;
  margin-bottom: 0.5rem;
  cursor: pointer;
  transition: transform 0.2s ease-in-out;
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
</style>

## 🎉 Memorable Moments

<div class="highlight-grid">

  <div class="highlight-card">
    <img src="/images/asic_class_fall2023.png" alt="ASIC Teaching Photo">
    <h4>Instructor – ASIC Physical Design</h4>
    <p>Fall 2023: My first course as instructor. Amazing classroom energy and engagement!</p>
  </div>

  <div class="highlight-card">
    <img src="/images/rfcon_award.png" alt="Best Paper Award – RFCoN 2025">
    <h4>🏆 Best Paper Award – RFCoN 2025</h4>
    <p>Honored to receive the Best Paper Award at the 1st Intl. Conf. on RF Communication and Networks (Track 2, Session II).</p>
  </div>


  <div class="highlight-card">
    <img src="/images/sg_senator_result.png" alt="SGA Senator Re-election">
    <h4>Re-Elected: SGA Senator (SSE)</h4>
    <p>Proud to be re-elected as Student Senator for the School of Science & Engineering for 2024–2025.</p>
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
