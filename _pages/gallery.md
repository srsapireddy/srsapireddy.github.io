---
title: "Gallery"
layout: single
permalink: /gallery/
author_profile: true
---

<style>
:root{
  --blue:#1a73e8;
  --blue2:#0b5bd3;
  --isu:#DC143C;
  --bg:#ffffff;
  --soft:#f6f9ff;
  --muted:#5f6368;
  --text:#0b1f44;
  --border:rgba(26,115,232,0.18);
  --shadow:0 10px 30px rgba(0,0,0,0.08);
  --shadow2:0 2px 10px rgba(0,0,0,0.05);
  --radius:18px;
  --radius2:14px;
}

@keyframes fadeInUp{
  from{opacity:0; transform:translateY(14px);}
  to{opacity:1; transform:translateY(0);}
}

@keyframes slideTrack{
  from{transform:translateX(0);}
  to{transform:translateX(-50%);}
}

@keyframes zoomIn{
  from{transform:scale(0.92); opacity:0;}
  to{transform:scale(1); opacity:1;}
}

.gallery-wrap{
  animation:fadeInUp 0.85s ease-in-out;
}

/* Hero */
.gallery-hero{
  position:relative;
  overflow:hidden;
  border-radius:var(--radius);
  padding:2.25rem 2rem;
  margin-bottom:1.3rem;
  background:
    radial-gradient(circle at top right, rgba(220,20,60,0.13), transparent 32%),
    linear-gradient(135deg,#e9f3ff 0%, #ffffff 62%);
  border:1px solid rgba(26,115,232,0.25);
  box-shadow:var(--shadow);
}

.gallery-hero::before{
  content:"";
  position:absolute;
  inset:0;
  background-image:
    linear-gradient(rgba(26,115,232,0.06) 1px, transparent 1px),
    linear-gradient(90deg, rgba(26,115,232,0.06) 1px, transparent 1px);
  background-size:34px 34px;
  pointer-events:none;
}

.hero-content{
  position:relative;
  z-index:1;
}

.hero-kicker{
  display:inline-block;
  padding:0.35rem 0.75rem;
  border-radius:999px;
  background:#ffffff;
  border:1px solid rgba(220,20,60,0.25);
  color:var(--isu);
  font-weight:900;
  font-size:0.88rem;
  box-shadow:var(--shadow2);
  margin-bottom:0.85rem;
}

.gallery-hero h1{
  margin:0;
  font-size:2.15rem;
  line-height:1.15;
  color:var(--text);
}

.gallery-hero p{
  margin:0.75rem 0 0 0;
  color:var(--muted);
  font-size:1.04rem;
  line-height:1.65;
  max-width:92ch;
}

.hero-badges{
  display:flex;
  flex-wrap:wrap;
  gap:0.55rem;
  margin-top:1rem;
}

.badge{
  display:inline-flex;
  align-items:center;
  padding:0.36rem 0.72rem;
  border-radius:999px;
  background:#ffffff;
  border:1px solid rgba(26,115,232,0.22);
  color:var(--text);
  box-shadow:var(--shadow2);
  font-size:0.88rem;
  font-weight:850;
}

.badge.red{
  border-color:rgba(220,20,60,0.30);
  color:#7a0b1f;
  background:rgba(220,20,60,0.06);
}

/* Sliding bar */
.sliding-bar{
  overflow:hidden;
  border-radius:16px;
  border:1px solid rgba(26,115,232,0.18);
  background:#ffffff;
  box-shadow:var(--shadow2);
  margin-bottom:1.3rem;
}

.slide-track{
  display:flex;
  width:max-content;
  animation:slideTrack 34s linear infinite;
}

.sliding-bar:hover .slide-track{
  animation-play-state:paused;
}

.slide-item{
  display:inline-flex;
  align-items:center;
  gap:0.4rem;
  padding:0.75rem 1.2rem;
  color:var(--text);
  font-weight:900;
  white-space:nowrap;
  border-right:1px solid rgba(26,115,232,0.10);
}

.slide-item span{
  color:var(--isu);
}

/* Impact cards */
.impact-grid{
  display:grid;
  grid-template-columns:repeat(4,1fr);
  gap:0.95rem;
  margin-bottom:1.3rem;
}

.impact-card{
  padding:1.1rem 1rem;
  border-radius:16px;
  background:linear-gradient(135deg,#ffffff 0%,#f7fbff 100%);
  border:1px solid rgba(26,115,232,0.18);
  box-shadow:var(--shadow2);
  text-align:center;
  transition:0.25s ease-in-out;
}

.impact-card:hover{
  transform:translateY(-3px);
  box-shadow:var(--shadow);
}

.impact-number{
  font-size:1.58rem;
  font-weight:950;
  color:var(--isu);
  line-height:1.1;
}

.impact-label{
  margin-top:0.35rem;
  font-size:0.92rem;
  color:var(--text);
  font-weight:850;
}

.impact-sub{
  margin-top:0.22rem;
  font-size:0.82rem;
  color:var(--muted);
}

/* Section */
.section{
  border:1px solid var(--border);
  background:var(--bg);
  padding:1.35rem 1.5rem;
  margin-bottom:1.3rem;
  border-radius:var(--radius2);
  box-shadow:var(--shadow2);
  transition:0.25s ease-in-out;
}

.section:hover{
  background:#fbfdff;
  transform:translateY(-2px);
  box-shadow:var(--shadow);
}

.section h2{
  margin:0;
  color:var(--text);
  font-size:1.22rem;
  display:flex;
  align-items:center;
  gap:0.55rem;
}

.section p{
  color:#202124;
  line-height:1.65;
}

.divider{
  height:1px;
  background:rgba(26,115,232,0.12);
  margin:0.6rem 0 1rem 0;
}

/* Tabs */
.gallery-tabs{
  display:flex;
  flex-wrap:wrap;
  gap:0.7rem;
  margin-bottom:1.1rem;
}

.tab-button{
  border:1px solid rgba(26,115,232,0.22);
  background:#ffffff;
  color:var(--blue);
  padding:0.62rem 1rem;
  border-radius:999px;
  cursor:pointer;
  font-weight:900;
  box-shadow:var(--shadow2);
  transition:0.2s ease-in-out;
}

.tab-button:hover{
  transform:translateY(-2px);
  background:#f3f8ff;
}

.tab-button.active{
  background:var(--blue);
  color:#ffffff;
  border-color:var(--blue);
}

.tab-panel{
  display:none;
  animation:fadeInUp 0.45s ease-in-out;
}

.tab-panel.active{
  display:block;
}

/* Gallery grid */
.highlight-grid{
  display:grid;
  grid-template-columns:repeat(4,1fr);
  gap:1.2rem;
}

.highlight-card{
  position:relative;
  overflow:hidden;
  background:#ffffff;
  border:1px solid rgba(26,115,232,0.18);
  border-radius:16px;
  padding:0.75rem;
  box-shadow:var(--shadow2);
  transition:0.25s ease-in-out;
}

.highlight-card:hover{
  background:#fbfdff;
  transform:translateY(-4px);
  box-shadow:var(--shadow);
  border-color:rgba(26,115,232,0.35);
}

.highlight-card::before{
  content:"";
  position:absolute;
  top:0;
  left:0;
  width:100%;
  height:5px;
  background:linear-gradient(90deg,var(--blue),var(--isu));
}

.highlight-card img{
  width:100%;
  height:190px;
  object-fit:cover;
  object-position:center;
  border-radius:12px;
  display:block;
  background:#ffffff;
  cursor:zoom-in;
  border:1px solid rgba(26,115,232,0.08);
}

.highlight-card h4{
  margin:0.7rem 0 0.25rem 0;
  color:var(--text);
  font-size:0.95rem;
  line-height:1.4;
  font-weight:900;
}

.gallery-tag{
  position:absolute;
  top:12px;
  left:12px;
  z-index:2;
  display:inline-flex;
  padding:0.22rem 0.5rem;
  border-radius:999px;
  background:rgba(26,115,232,0.92);
  color:#ffffff;
  font-size:0.72rem;
  font-weight:900;
  border:1px solid rgba(255,255,255,0.25);
}

.gallery-tag.red{
  background:rgba(220,20,60,0.92);
}

.gallery-tag.green{
  background:rgba(26,127,61,0.92);
}

/* Lightbox */
.lightbox-overlay{
  position:fixed;
  inset:0;
  width:100vw;
  height:100vh;
  background:rgba(0,0,0,0.92);
  display:none;
  align-items:center;
  justify-content:center;
  z-index:9999;
  padding:18px;
}

.lightbox-overlay img{
  max-width:92vw;
  max-height:88vh;
  border-radius:14px;
  box-shadow:0 0 24px rgba(255,255,255,0.18);
  animation:zoomIn 0.25s ease;
}

.lightbox-caption{
  position:fixed;
  bottom:18px;
  left:50%;
  transform:translateX(-50%);
  color:rgba(255,255,255,0.92);
  font-weight:850;
  font-size:0.92rem;
  background:rgba(0,0,0,0.38);
  padding:0.45rem 0.8rem;
  border-radius:999px;
  border:1px solid rgba(255,255,255,0.2);
  text-align:center;
  max-width:90vw;
}

/* Responsive */
@media (max-width:1100px){
  .highlight-grid{
    grid-template-columns:repeat(3,1fr);
  }
}

@media (max-width:900px){
  .impact-grid{
    grid-template-columns:repeat(2,1fr);
  }

  .highlight-grid{
    grid-template-columns:repeat(2,1fr);
  }
}

@media (max-width:700px){
  .gallery-hero{
    padding:1.5rem 1.1rem;
  }

  .gallery-hero h1{
    font-size:1.65rem;
  }

  .impact-grid,
  .highlight-grid{
    grid-template-columns:1fr;
  }

  .highlight-card{
    max-width:430px;
    margin:0 auto;
  }

  .highlight-card img{
    height:230px;
  }
}
</style>

<div class="gallery-wrap">

  <div class="gallery-hero">
    <div class="hero-content">
      <span class="hero-kicker">Gallery · Academic Journey · Research · Milestones</span>

      <h1>Gallery</h1>

      <p>
        A visual collection of memorable moments from my academic journey, campus visits,
        graduations, research activities, conferences, mentorship, and professional milestones.
      </p>

      <div class="hero-badges">
        <span class="badge red">Academic Milestones</span>
        <span class="badge">Graduations</span>
        <span class="badge">Research and Conferences</span>
        <span class="badge">Mentors and Collaborators</span>
      </div>
    </div>
  </div>

  <div class="sliding-bar">
    <div class="slide-track">
      <div class="slide-item"><span>●</span> UMKC Graduation</div>
      <div class="slide-item"><span>●</span> UIS Graduation</div>
      <div class="slide-item"><span>●</span> GLSVLSI Conference</div>
      <div class="slide-item"><span>●</span> Research Mentors</div>
      <div class="slide-item"><span>●</span> UIUC Visit</div>
      <div class="slide-item"><span>●</span> UMKC Orientation</div>

      <div class="slide-item"><span>●</span> UMKC Graduation</div>
      <div class="slide-item"><span>●</span> UIS Graduation</div>
      <div class="slide-item"><span>●</span> GLSVLSI Conference</div>
      <div class="slide-item"><span>●</span> Research Mentors</div>
      <div class="slide-item"><span>●</span> UIUC Visit</div>
      <div class="slide-item"><span>●</span> UMKC Orientation</div>
    </div>
  </div>

  <div class="impact-grid">
    <div class="impact-card">
      <div class="impact-number">UIUC</div>
      <div class="impact-label">Campus Visit</div>
      <div class="impact-sub">Academic and professional engagement</div>
    </div>


    <div class="impact-card">
      <div class="impact-number">UMKC</div>
      <div class="impact-label">Graduate Journey</div>
      <div class="impact-sub">Mentors, orientation, and graduation</div>
    </div>

    <div class="impact-card">
      <div class="impact-number">UIS</div>
      <div class="impact-label">Master's Graduation</div>
      <div class="impact-sub">Academic milestone</div>
    </div>

    <div class="impact-card">
      <div class="impact-number">GLSVLSI</div>
      <div class="impact-label">Conference</div>
      <div class="impact-sub">Research presentation and networking</div>
    </div>
  </div>

  <div class="section">
    <h2>🎉 Memorable Moments</h2>
    <div class="divider"></div>

    <p>
      Use the tabs below to view images by category. Click any image to open it in a larger view.
    </p>

    <div class="gallery-tabs">
      <button class="tab-button active" onclick="openGalleryTab(event, 'all-tab')">All Moments</button>
      <button class="tab-button" onclick="openGalleryTab(event, 'campus-tab')">Campus and Orientation</button>
      <button class="tab-button" onclick="openGalleryTab(event, 'mentors-tab')">Mentors</button>
      <button class="tab-button" onclick="openGalleryTab(event, 'conference-tab')">Conferences</button>
      <button class="tab-button" onclick="openGalleryTab(event, 'graduation-tab')">Graduations</button>
    </div>

    <div id="all-tab" class="tab-panel active">
      <div class="highlight-grid">

        <div class="highlight-card">
          <span class="gallery-tag">School Visit</span>
          <img src="/images/Fair_1.jpeg" alt="Academic Department & Student Services Fair">
          <h4>School visit for K-12 STEM outreach.</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag">School Visit</span>
          <img src="/images/school.jpeg" alt="School visit for K-12 STEM outreach.">
          <h4>School visit for K-12 STEM outreach.</h4>
        </div>
        
        <div class="highlight-card">
          <span class="gallery-tag">Campus</span>
          <img src="/images/Gies.jpeg" alt="Campus visit to University of Illinois Urbana-Champaign.">
          <h4>Campus visit to University of Illinois Urbana-Champaign.</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag">Orientation</span>
          <img src="/images/orientation1.jpeg" alt="Welcoming new students at UMKC Orientation, Fall 2025.">
          <h4>Welcoming new students at UMKC Orientation, Fall 2025.</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag red">Mentor</span>
          <img src="/images/shyu.jpeg" alt="With Professor Shyu, UMKC">
          <h4>With Professor Shyu, UMKC</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag red">Advisor</span>
          <img src="/images/most.jpeg" alt="With Professor Rahman, UMKC Ph.D. Advisor">
          <h4>With Professor Rahman, UMKC (Ph.D. Advisor)</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag red">Mentor</span>
          <img src="/images/masud1.jpeg" alt="With Professor Masud, UMKC Mentor and Department Chair">
          <h4>With Professor Masud, UMKC (Mentor and Department Chair).</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag green">Conference</span>
          <img src="/images/pos1.jpeg" alt="GLSVLSI Conference 2025">
          <h4>GLSVLSI Conference 2025</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag green">Conference</span>
          <img src="/images/pos2.jpeg" alt="GLSVLSI Conference 2025">
          <h4>GLSVLSI Conference 2025</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag">Graduation</span>
          <img src="/images/grad0.jpg" alt="UMKC Master’s Graduation">
          <h4>UMKC Master’s Graduation</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag">Graduation</span>
          <img src="/images/grad1.jpg" alt="UMKC Master’s Graduation, 2016">
          <h4>UMKC Master’s Graduation, 2016</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag">Graduation</span>
          <img src="/images/grad2.jpg" alt="UMKC Master’s Graduation, 2016">
          <h4>UMKC Master’s Graduation, 2016</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag">Graduation</span>
          <img src="/images/grad3.jpg" alt="UMKC Master’s Graduation, 2016">
          <h4>UMKC Master’s Graduation, 2016</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag">Graduation</span>
          <img src="/images/grad4.jpg" alt="UMKC Master’s Graduation, 2016">
          <h4>UMKC Master’s Graduation, 2016</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag">Graduation</span>
          <img src="/images/grad5.jpg" alt="UMKC Master’s Graduation, 2016">
          <h4>UMKC Master’s Graduation, 2016</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag">Graduation</span>
          <img src="/images/grad7.jpeg" alt="UIS Master’s Graduation, 2018">
          <h4>UIS Master’s Graduation, 2018</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag">Graduation</span>
          <img src="/images/grad6.jpeg" alt="UIS Master’s Graduation, 2018">
          <h4>UIS Master’s Graduation, 2018</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag green">Conference</span>
          <img src="/images/pos3.jpeg" alt="GLSVLSI Conference">
          <h4>GLSVLSI Conference</h4>
        </div>

      </div>
    </div>

    <div id="campus-tab" class="tab-panel">
      <div class="highlight-grid">

        <div class="highlight-card">
          <span class="gallery-tag">Campus</span>
          <img src="/images/Gies.jpeg" alt="Campus visit to University of Illinois Urbana-Champaign.">
          <h4>Campus visit to University of Illinois Urbana-Champaign.</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag">Orientation</span>
          <img src="/images/orientation1.jpeg" alt="Welcoming new students at UMKC Orientation, Fall 2025.">
          <h4>Welcoming new students at UMKC Orientation, Fall 2025.</h4>
        </div>

      </div>
    </div>

    <div id="mentors-tab" class="tab-panel">
      <div class="highlight-grid">

        <div class="highlight-card">
          <span class="gallery-tag red">Mentor</span>
          <img src="/images/shyu.jpeg" alt="With Professor Shyu, UMKC">
          <h4>With Professor Shyu, UMKC</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag red">Advisor</span>
          <img src="/images/most.jpeg" alt="With Professor Rahman, UMKC Ph.D. Advisor">
          <h4>With Professor Rahman, UMKC (Ph.D. Advisor)</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag red">Mentor</span>
          <img src="/images/masud1.jpeg" alt="With Professor Masud, UMKC Mentor and Department Chair">
          <h4>With Professor Masud, UMKC (Mentor and Department Chair).</h4>
        </div>

      </div>
    </div>

    <div id="conference-tab" class="tab-panel">
      <div class="highlight-grid">

        <div class="highlight-card">
          <span class="gallery-tag green">Conference</span>
          <img src="/images/pos1.jpeg" alt="GLSVLSI Conference 2025">
          <h4>GLSVLSI Conference 2025</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag green">Conference</span>
          <img src="/images/pos2.jpeg" alt="GLSVLSI Conference 2025">
          <h4>GLSVLSI Conference 2025</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag green">Conference</span>
          <img src="/images/pos3.jpeg" alt="GLSVLSI Conference">
          <h4>GLSVLSI Conference</h4>
        </div>

      </div>
    </div>

    <div id="graduation-tab" class="tab-panel">
      <div class="highlight-grid">

        <div class="highlight-card">
          <span class="gallery-tag">Graduation</span>
          <img src="/images/grad0.jpg" alt="UMKC Master’s Graduation">
          <h4>UMKC Master’s Graduation</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag">Graduation</span>
          <img src="/images/grad1.jpg" alt="UMKC Master’s Graduation, 2016">
          <h4>UMKC Master’s Graduation, 2016</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag">Graduation</span>
          <img src="/images/grad2.jpg" alt="UMKC Master’s Graduation, 2016">
          <h4>UMKC Master’s Graduation, 2016</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag">Graduation</span>
          <img src="/images/grad3.jpg" alt="UMKC Master’s Graduation, 2016">
          <h4>UMKC Master’s Graduation, 2016</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag">Graduation</span>
          <img src="/images/grad4.jpg" alt="UMKC Master’s Graduation, 2016">
          <h4>UMKC Master’s Graduation, 2016</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag">Graduation</span>
          <img src="/images/grad5.jpg" alt="UMKC Master’s Graduation, 2016">
          <h4>UMKC Master’s Graduation, 2016</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag">Graduation</span>
          <img src="/images/grad7.jpeg" alt="UIS Master’s Graduation, 2018">
          <h4>UIS Master’s Graduation, 2018</h4>
        </div>

        <div class="highlight-card">
          <span class="gallery-tag">Graduation</span>
          <img src="/images/grad6.jpeg" alt="UIS Master’s Graduation, 2018">
          <h4>UIS Master’s Graduation, 2018</h4>
        </div>

      </div>
    </div>

  </div>

</div>

<div class="lightbox-overlay" id="lightbox">
  <img id="lightbox-img" src="" alt="">
  <div class="lightbox-caption" id="lightbox-caption">Click anywhere to close</div>
</div>

<script>
function openGalleryTab(event, panelId) {
  const panels = document.querySelectorAll(".tab-panel");
  const buttons = document.querySelectorAll(".tab-button");

  panels.forEach(function(panel) {
    panel.classList.remove("active");
  });

  buttons.forEach(function(button) {
    button.classList.remove("active");
  });

  const selectedPanel = document.getElementById(panelId);
  if (selectedPanel) {
    selectedPanel.classList.add("active");
  }

  if (event && event.currentTarget) {
    event.currentTarget.classList.add("active");
  }
}

document.addEventListener("DOMContentLoaded", function () {
  const images = document.querySelectorAll(".highlight-card img");
  const lightbox = document.getElementById("lightbox");
  const lightboxImg = document.getElementById("lightbox-img");
  const lightboxCaption = document.getElementById("lightbox-caption");

  images.forEach(function(img) {
    img.addEventListener("click", function() {
      lightboxImg.src = img.src;
      lightboxImg.alt = img.alt;
      lightboxCaption.textContent = img.alt || "Click anywhere to close";
      lightbox.style.display = "flex";
    });
  });

  lightbox.addEventListener("click", function() {
    lightbox.style.display = "none";
    lightboxImg.src = "";
    lightboxImg.alt = "";
    lightboxCaption.textContent = "Click anywhere to close";
  });

  document.addEventListener("keydown", function(e) {
    if (e.key === "Escape" && lightbox.style.display === "flex") {
      lightbox.style.display = "none";
      lightboxImg.src = "";
      lightboxImg.alt = "";
      lightboxCaption.textContent = "Click anywhere to close";
    }
  });
});
</script>
