---
title: "Gallery"
layout: single
permalink: /gallery/
author_profile: true
---

Welcome to my personal gallery — moments from my academic journey, graduation, research labs, and team milestones.

<style>
.gallery-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1rem;
  margin-top: 2rem;
}
.gallery-grid img {
  width: 100%;
  height: auto;
  border-radius: 10px;
  cursor: pointer;
  transition: transform 0.2s ease;
  border: 2px solid #ccc;
}
.gallery-grid img:hover {
  transform: scale(1.03);
  border-color: #1a73e8;
}
</style>

<!-- Lightbox Fullscreen Script -->
<script>
document.addEventListener("DOMContentLoaded", function () {
  const imgs = document.querySelectorAll(".gallery-grid img");
  imgs.forEach(img => {
    img.addEventListener("click", () => {
      const src = img.getAttribute("src");
      const overlay = document.createElement("div");
      overlay.style.position = "fixed";
      overlay.style.top = 0;
      overlay.style.left = 0;
      overlay.style.width = "100vw";
      overlay.style.height = "100vh";
      overlay.style.backgroundColor = "rgba(0, 0, 0, 0.9)";
      overlay.style.display = "flex";
      overlay.style.alignItems = "center";
      overlay.style.justifyContent = "center";
      overlay.style.zIndex = 1000;
      overlay.innerHTML = `<img src="${src}" style="max-width: 90vw; max-height: 90vh; border-radius: 12px;">`;
      overlay.addEventListener("click", () => overlay.remove());
      document.body.appendChild(overlay);
    });
  });
});
</script>

<div class="gallery-grid">
  <img src="/assets/images/gallery/grad1.jpg" alt="Graduation Ceremony">
  <img src="/assets/images/gallery/grad2.jpg" alt="Graduation Ceremony">
  <img src="/assets/images/gallery/grad3.jpg" alt="Graduation Ceremony">
  <img src="/assets/images/gallery/grad4.jpg" alt="Graduation Ceremony">
  <img src="/assets/images/gallery/grad5.jpg" alt="Graduation Ceremony">
</div>
