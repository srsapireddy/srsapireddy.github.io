---
title: "Presentations"
layout: single
permalink: /presentations/
author_profile: true
---

<style>
.presentation-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5rem;
  margin-top: 2rem;
}
.presentation-card {
  background: #f0f8ff;
  border: 2px solid #1a73e8;
  border-radius: 12px;
  padding: 1rem;
  box-shadow: 0 3px 8px rgba(0,0,0,0.05);
  transition: 0.3s ease-in-out;
  cursor: pointer;
}
.presentation-card:hover {
  background: #e6f0ff;
  transform: scale(1.01);
}
.presentation-card img {
  width: 100%;
  border-radius: 8px;
  margin-bottom: 0.5rem;
}
.presentation-card h4 {
  margin: 0;
  color: #1a73e8;
}
</style>

## 🎤 Featured Presentations

<div class="presentation-grid">
  <div class="presentation-card" onclick="openLightbox('/publications/UMKC_ATP_Interview_Presentation_Rahul.pdf')">
    <img src="/images/umkc_presentation_thumbnail.jpg" alt="UMKC Presentation">
    <h4>UMKC Assistant Teaching Professor Interview</h4>
  </div>

  <div class="presentation-card" onclick="openLightbox('/publications/MIDE_Dec_2022_CT.pptx')">
    <img src="/images/mide_ct_thumbnail.jpg" alt="MIDE Presentation">
    <h4>MIDE Capstone Talk – December 2022</h4>
  </div>

  <div class="presentation-card" onclick="openLightbox('/publications/Srinivas_Rahul_Presentation.pptx')">
    <img src="/images/rahul_nn_presentation.jpg" alt="DNN Slides">
    <h4>Presentation on Deep Neural Networks</h4>
  </div>

  <div class="presentation-card" onclick="openLightbox('/publications/Army_PPT_Presentation_Updated_Aug_2nd.pptx')">
    <img src="/images/army_ppt_thumbnail.jpg" alt="Army Presentation">
    <h4>U.S. Army Research Overview – August 2023</h4>
  </div>
</div>

<!-- Lightbox Viewer -->
<div id="lightbox" style="display:none; position:fixed; top:0; left:0; width:100vw; height:100vh; background:rgba(0,0,0,0.85); align-items:center; justify-content:center; z-index:1000;" onclick="this.style.display='none'">
  <iframe id="lightbox-iframe" src="" style="width:90vw; height:90vh; border:none; border-radius:8px;"></iframe>
</div>

<script>
function openLightbox(url) {
  document.getElementById("lightbox").style.display = "flex";
  document.getElementById("lightbox-iframe").src = "https://docs.google.com/gview?url=https://srsapireddy.github.io" + url + "&embedded=true";
}
</script>
