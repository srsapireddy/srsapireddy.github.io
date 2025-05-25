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

.lightbox {
  position: fixed;
  top: 0; left: 0;
  width: 100vw; height: 100vh;
  background: rgba(0, 0, 0, 0.9);
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 1000;
  display: none;
}

.lightbox img {
  max-width: 90vw;
  max-height: 90vh;
  border-radius: 12px;
}

.lightbox .arrow {
  position: absolute;
  top: 50%;
  font-size: 2rem;
  color: white;
  background: rgba(0, 0, 0, 0.5);
  padding: 0.5rem 1rem;
  cursor: pointer;
  user-select: none;
  border-radius: 6px;
  transform: translateY(-50%);
}

.lightbox .arrow:hover {
  background: rgba(255, 255, 255, 0.3);
}

.lightbox .prev {
  left: 2%;
}

.lightbox .next {
  right: 2%;
}
</style>

<div class="gallery-grid" id="gallery">
  <img src="/images/grad1.jpg" alt="Graduation 1">
  <img src="/images/grad2.jpg" alt="Graduation 2">
  <img src="/images/grad3.jpg" alt="Graduation 3">
  <img src="/images/grad4.jpg" alt="Graduation 4">
  <img src="/images/grad5.jpg" alt="Graduation 5">
</div>

<div class="lightbox" id="lightbox">
  <span class="arrow prev" onclick="prevImage()">‹</span>
  <img id="lightbox-img" src="" alt="">
  <span class="arrow next" onclick="nextImage()">›</span>
</div>

<script>
  const images = Array.from(document.querySelectorAll('#gallery img'));
  const lightbox = document.getElementById('lightbox');
  const lightboxImg = document.getElementById('lightbox-img');
  let current = 0;

  images.forEach((img, i) => {
    img.addEventListener('click', () => {
      current = i;
      showImage();
    });
  });

  function showImage() {
    lightboxImg.src = images[current].src;
    lightbox.style.display = 'flex';
  }

  function prevImage() {
    current = (current - 1 + images.length) % images.length;
    showImage();
  }

  function nextImage() {
    current = (current + 1) % images.length;
    showImage();
  }

  lightbox.addEventListener('click', e => {
    if (e.target === lightbox || e.target === lightboxImg) {
      lightbox.style.display = 'none';
    }
  });

  document.addEventListener('keydown', e => {
    if (lightbox.style.display === 'flex') {
      if (e.key === 'ArrowRight') nextImage();
      if (e.key === 'ArrowLeft') prevImage();
      if (e.key === 'Escape') lightbox.style.display = 'none';
    }
  });
</script>
