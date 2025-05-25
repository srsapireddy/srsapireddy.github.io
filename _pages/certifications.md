---
title: "Certifications"
layout: single
permalink: /certifications/
author_profile: true
---

Below is a visual showcase of my certifications. Click on any certificate to view it in fullscreen.

<style>
.cert-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 1.2rem;
  margin-top: 2rem;
}

.cert-card {
  text-align: center;
  border: 2px solid #ccc;
  border-radius: 10px;
  padding: 0.5rem;
  background: #fff;
  transition: 0.2s ease;
}

.cert-card:hover {
  transform: scale(1.02);
  border-color: #1a73e8;
}

.cert-card img {
  width: 100%;
  border-radius: 6px;
  cursor: pointer;
}

.cert-title {
  margin-top: 0.5rem;
  font-size: 0.9rem;
  font-weight: 600;
  color: #333;
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
  box-shadow: 0 0 20px rgba(255, 255, 255, 0.2);
}
</style>

<div class="cert-grid" id="certGrid">
  <div class="cert-card">
    <img src="/images/statistical_learning.png" alt="Statistical Learning">
    <div class="cert-title">Statistical Learning – Stanford University</div>
  </div>
  <div class="cert-card">
    <img src="/images/mlops_specialization.jpg" alt="MLOps Specialization">
    <div class="cert-title">MLOps Specialization</div>
  </div>
  <div class="cert-card">
    <img src="/images/product_management.png" alt="Product Management">
    <div class="cert-title">Product Management – CII</div>
  </div>
  <div class="cert-card">
    <img src="/images/mathematics_ml.png" alt="Mathematics for ML">
    <div class="cert-title">Mathematics for ML – Imperial College London</div>
  </div>
  <div class="cert-card">
    <img src="/images/device_packaging.png" alt="Device Packaging">
    <div class="cert-title">Introduction to Device and System Packaging</div>
  </div>
  <div class="cert-card">
    <img src="/images/semiconductor_basics.png" alt="Semiconductor Basics">
    <div class="cert-title">Basics of Semiconductor Device Technology</div>
  </div>
  <div class="cert-card">
    <img src="/images/network_security.jpeg" alt="Network Security">
    <div class="cert-title">Network Security Associate</div>
  </div>
  <div class="cert-card">
    <img src="/images/intel_cloud.png" alt="Intel Cloud">
    <div class="cert-title">Intel Solution Pro Cloud Business Professional</div>
  </div>
  <!-- Add more certification cards as needed -->
</div>

<!-- Lightbox -->
<div class="lightbox" id="lightbox">
  <img id="lightbox-img" src="" alt="">
</div>

<script>
document.addEventListener("DOMContentLoaded", function () {
  const images = document.querySelectorAll("#certGrid img");
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
