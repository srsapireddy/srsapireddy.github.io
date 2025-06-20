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
  border: 2px solid #1a73e8; /* blue border */
  border-radius: 10px;
  padding: 0.5rem;
  background: #fff;
  transition: 0.3s ease;
}

.cert-card:hover {
  transform: scale(1.02);
  border-color: #0c57c2;
  background-color: #f0f8ff;
  box-shadow: 0 4px 12px rgba(26, 115, 232, 0.15);
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

## 🌐 Certifications
<!-- Certifications -->
<div class="cert-grid lightbox-gallery">
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
</div>

---

## 🎓 Degrees & Diplomas

<div class="cert-grid lightbox-gallery">
  <div class="cert-card">
    <img src="/images/ms_cs_uis.png" alt="MS CS Degree">
    <div class="cert-title">M.S. in Computer Science – University of Illinois, Springfield</div>
  </div>
  <div class="cert-card">
    <img src="/images/ms_ee_umkc.png" alt="MS EE Degree">
    <div class="cert-title">M.S. in Electrical Engineering – UMKC</div>
  </div>
  <div class="cert-card">
    <img src="/images/advanced_ai_nielit.png" alt="AI Diploma">
    <div class="cert-title">Advanced Diploma in AI – NIELIT, India</div>
  </div>
  <div class="cert-card">
    <img src="/images/btech_ece.png" alt="B.Tech ECE">
    <div class="cert-title">B.Tech in ECE – GRIET, JNTU Hyderabad</div>
  </div>
</div>

---

## 🏅 Honors & Recognition

<div class="cert-grid lightbox-gallery">
  <div class="cert-card">
    <img src="/images/guinness_world_record.png" alt="Guinness World Record">
    <div class="cert-title">Guinness World Record – Participation Certificate</div>
  </div>
  <div class="cert-card">
    <img src="/images/ieee_hkn_certificate.jpg" alt="IEEE-HKN Membership">
    <div class="cert-title">IEEE Eta Kappa Nu (HKN) – Honor Society Member</div>
  </div>
  <div class="cert-card">
    <img src="/images/mspe_membership.png" alt="MSPE Membership">
    <div class="cert-title">Member – Missouri Society of Professional Engineers (Western Chapter)</div>
  </div>
</div>

---

## 🌐 Professional Memberships

<div class="cert-grid lightbox-gallery">
  <div class="cert-card">
    <img src="/images/ACM_Membership.png" alt="ACM Membership">
    <div class="cert-title">
      ACM Member<br>
      <small>Membership ID: 8325933</small>
    </div>
  </div>
  <div class="cert-card">
    <img src="/images/IEEE_Membership.png" alt="IEEE Membership">
    <div class="cert-title">
      IEEE Member<br>
      <small>Membership ID: 93943359</small>
    </div>
  </div>
  <div class="cert-card">
    <img src="/images/aaai_placeholder.png" alt="AAAI Membership">
    <div class="cert-title">
      AAAI Member<br>
      <small>Membership ID: 648148</small>
    </div>
  </div>
</div>

---

## 🏆 Hackathon Awards

<div class="cert-grid lightbox-gallery">
  <div class="cert-card">
    <img src="/images/hackaroo_2022.png" alt="Hack-A-Roo 2022">
    <div class="cert-title">2nd Place – Hack-A-Roo Fall 2022 (Entrepreneur Track)</div>
  </div>
  <div class="cert-card">
    <img src="/images/hackaroo_2021.png" alt="Hack-A-Roo 2021">
    <div class="cert-title">3rd Place – Hack-A-Roo Fall 2021 (CS/IT Track)</div>
  </div>
</div>

<!-- Lightbox -->
<div class="lightbox" id="lightbox">
  <img id="lightbox-img" src="" alt="">
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
    });
  });

  lightbox.addEventListener("click", () => {
    lightbox.style.display = "none";
    lightboxImg.src = "";
  });
});
</script>
