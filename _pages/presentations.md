---
title: "Presentations & Talks"
layout: single
permalink: /presentations/
author_profile: true
---

<style>
:root{
  --blue:#1a73e8;
  --blue2:#0b5bd3;
  --isu:#DC143C;
  --cyan:#00bcd4;
  --bg:#ffffff;
  --soft:#f6f9ff;
  --muted:#5f6368;
  --text:#0b1f44;
  --dark:#0f172a;
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

@keyframes presZoom{
  from{transform:scale(0.94); opacity:0;}
  to{transform:scale(1); opacity:1;}
}

.presentations-page{
  animation:fadeInUp 0.85s ease-in-out;
  position:relative;
  overflow:hidden;
  padding-bottom:2rem;
}

/* Hero */
.presentations-hero{
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

.presentations-hero::before{
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

.pres-kicker{
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

.presentations-hero h1{
  margin:0;
  font-size:2.15rem;
  line-height:1.15;
  color:var(--text);
}

.presentations-hero p{
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

.hero-badge{
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

.hero-badge.red{
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

/* Summary cards */
.pres-summary{
  display:grid;
  grid-template-columns:repeat(4,1fr);
  gap:0.95rem;
  margin-bottom:1.3rem;
}

.pres-summary-card{
  padding:1.1rem 1rem;
  border-radius:16px;
  background:linear-gradient(135deg,#ffffff 0%,#f7fbff 100%);
  border:1px solid rgba(26,115,232,0.18);
  box-shadow:var(--shadow2);
  text-align:center;
  transition:0.25s ease-in-out;
}

.pres-summary-card:hover{
  transform:translateY(-3px);
  box-shadow:var(--shadow);
}

.pres-summary-card span{
  display:block;
  color:var(--isu);
  font-size:1.55rem;
  font-weight:950;
  line-height:1.1;
}

.pres-summary-card small{
  display:block;
  color:var(--muted);
  font-size:0.82rem;
  margin-top:0.28rem;
}

/* Section */
.pres-section{
  border:1px solid var(--border);
  background:var(--bg);
  padding:1.35rem 1.5rem;
  margin-bottom:1.3rem;
  border-radius:var(--radius2);
  box-shadow:var(--shadow2);
  transition:0.25s ease-in-out;
}

.pres-section:hover{
  background:#fbfdff;
  transform:translateY(-2px);
  box-shadow:var(--shadow);
}

.pres-section-header{
  margin-bottom:1rem;
}

.pres-section-header h2,
.pres-section-header h3{
  margin:0;
  color:var(--text);
  font-size:1.22rem;
  display:flex;
  align-items:center;
  gap:0.55rem;
}

.pres-section-header p{
  margin:0.55rem 0 0 0;
  color:#202124;
  line-height:1.65;
  font-size:0.95rem;
}

.divider{
  height:1px;
  background:rgba(26,115,232,0.12);
  margin:0.6rem 0 1rem 0;
}

/* Tabs */
.pres-tabs{
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

/* Presentation cards */
.presentation-grid{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(285px,1fr));
  gap:1.2rem;
}

.presentation-card{
  position:relative;
  border-radius:18px;
  background:#ffffff;
  border:1px solid rgba(26,115,232,0.18);
  box-shadow:var(--shadow2);
  overflow:hidden;
  cursor:pointer;
  transition:0.25s ease-in-out;
}

.presentation-card:hover{
  transform:translateY(-5px);
  border-color:rgba(26,115,232,0.40);
  box-shadow:var(--shadow);
}

.presentation-card::before{
  content:"";
  position:absolute;
  top:0;
  left:0;
  width:100%;
  height:5px;
  background:linear-gradient(90deg,var(--blue),var(--isu));
  z-index:2;
}

.presentation-thumb{
  position:relative;
  height:205px;
  overflow:hidden;
  background:#ffffff;
}

.presentation-thumb img{
  width:100%;
  height:100%;
  object-fit:contain;
  object-position:center;
  padding:0.35rem;
  background:#ffffff;
  display:block;
  transition:transform 0.35s ease, filter 0.25s ease;
  -webkit-user-drag:none;
  user-drag:none;
}

.presentation-card:hover .presentation-thumb img{
  transform:scale(1.025);
  filter:brightness(0.98);
}

.pres-badge{
  position:absolute;
  top:14px;
  left:14px;
  padding:0.34rem 0.68rem;
  border-radius:999px;
  background:rgba(15,23,42,0.80);
  color:#ffffff;
  font-size:0.72rem;
  font-weight:900;
  backdrop-filter:blur(8px);
}

.pres-year{
  position:absolute;
  right:14px;
  bottom:14px;
  padding:0.34rem 0.65rem;
  border-radius:999px;
  background:rgba(255,255,255,0.92);
  color:var(--blue2);
  font-size:0.72rem;
  font-weight:900;
  box-shadow:0 8px 18px rgba(15,23,42,0.14);
}

.presentation-body{
  padding:1.05rem 1.15rem 1.2rem;
}

.presentation-body h4{
  margin:0 0 0.45rem;
  color:var(--text);
  font-size:1.03rem;
  line-height:1.35;
  font-weight:950;
}

.presentation-body p{
  margin:0;
  color:#475569;
  font-size:0.9rem;
  line-height:1.6;
}

.pres-tags{
  display:flex;
  flex-wrap:wrap;
  gap:0.42rem;
  margin-top:0.85rem;
}

.pres-tags span{
  padding:0.28rem 0.55rem;
  border-radius:999px;
  background:#eef6ff;
  color:var(--blue);
  border:1px solid rgba(26,115,232,0.16);
  font-size:0.72rem;
  font-weight:850;
}

/* Poster cards */
.poster-grid{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(320px,1fr));
  gap:1.2rem;
}

.poster-card{
  display:grid;
  grid-template-columns:44% 1fr;
  border-radius:18px;
  background:#ffffff;
  border:1px solid rgba(26,115,232,0.18);
  box-shadow:var(--shadow2);
  overflow:hidden;
  transition:0.25s ease-in-out;
}

.poster-card:hover{
  transform:translateY(-5px);
  box-shadow:var(--shadow);
}

.poster-card img{
  width:100%;
  height:100%;
  min-height:230px;
  object-fit:contain;
  object-position:center;
  background:#ffffff;
  padding:0.35rem;
  -webkit-user-drag:none;
  user-drag:none;
}

.poster-content{
  padding:1.2rem;
  display:flex;
  flex-direction:column;
  justify-content:center;
}

.poster-content h4{
  margin:0 0 0.45rem;
  color:var(--text);
  font-size:1.05rem;
  line-height:1.35;
  font-weight:950;
}

.poster-content p{
  margin:0;
  color:#475569;
  font-size:0.9rem;
  line-height:1.6;
}

/* YouTube cards */
.youtube-card-grid{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(285px,1fr));
  gap:1.2rem;
}

.youtube-card{
  border-radius:18px;
  background:#ffffff;
  border:1px solid rgba(26,115,232,0.18);
  box-shadow:var(--shadow2);
  overflow:hidden;
  transition:0.25s ease-in-out;
}

.youtube-card:hover{
  transform:translateY(-5px);
  box-shadow:var(--shadow);
}

.youtube-frame{
  position:relative;
  background:#0f172a;
}

.youtube-card iframe{
  width:100%;
  height:210px;
  border:none;
  display:block;
}

.youtube-body{
  padding:1rem 1.15rem 1.2rem;
}

.youtube-body h4{
  margin:0 0 0.4rem;
  color:var(--text);
  font-size:1rem;
  font-weight:950;
}

.youtube-body p{
  margin:0;
  color:#475569;
  font-size:0.88rem;
  line-height:1.55;
}

/* Copyright */
.pres-copyright{
  margin-top:1.3rem;
  padding:1.05rem 1.2rem;
  border-left:5px solid var(--blue);
  background:#f8fbff;
  border-radius:14px;
  color:#475569;
  font-size:0.86rem;
  line-height:1.65;
  box-shadow:var(--shadow2);
}

/* Lightbox viewer */
.pres-lightbox{
  position:fixed;
  inset:0;
  display:none;
  align-items:center;
  justify-content:center;
  background:rgba(2,6,23,0.94);
  z-index:9999;
  padding:1rem;
}

.pres-lightbox-content{
  width:min(1100px,94vw);
  height:min(760px,90vh);
  background:#ffffff;
  border-radius:20px;
  overflow:hidden;
  box-shadow:0 0 45px rgba(255,255,255,0.18);
  position:relative;
  animation:presZoom 0.25s ease;
}

.pres-lightbox iframe{
  width:100%;
  height:100%;
  border:none;
}

.pres-lightbox-close{
  position:fixed;
  top:20px;
  right:30px;
  color:#ffffff;
  font-size:2.2rem;
  font-weight:850;
  cursor:pointer;
  opacity:0.88;
  z-index:10000;
}

.pres-lightbox-close:hover{
  opacity:1;
}

/* Basic copy deterrent */
.presentations-protected{
  -webkit-user-select:none;
  -ms-user-select:none;
  user-select:none;
}

/* Responsive */
@media (max-width:950px){
  .pres-summary{
    grid-template-columns:repeat(2,1fr);
  }
}

@media (max-width:820px){
  .poster-card{
    grid-template-columns:1fr;
  }

  .poster-card img{
    min-height:240px;
  }
}

@media (max-width:700px){
  .presentations-hero{
    padding:1.5rem 1.1rem;
  }

  .presentations-hero h1{
    font-size:1.65rem;
  }

  .pres-summary{
    grid-template-columns:1fr;
  }
}

@media (max-width:560px){
  .presentation-thumb{
    height:190px;
  }

  .youtube-card iframe{
    height:190px;
  }

  .pres-lightbox-content{
    width:94vw;
    height:82vh;
    border-radius:14px;
  }
}
</style>

<div class="presentations-page presentations-protected">

  <section class="presentations-hero">
    <div class="hero-content">
      <span class="pres-kicker">Selected Presentations</span>

      <h1>Presentations &amp; Talks</h1>

      <p>
        A curated collection of invited lectures, research presentations, conference posters,
        academic talks, project demonstrations, and professional outreach presentations.
        This page highlights work across RF systems, VLSI design, artificial intelligence,
        teaching, outreach, and applied engineering research.
      </p>

      <div class="hero-badges">
        <span class="hero-badge red">Invited Lectures</span>
        <span class="hero-badge">Conference Talks</span>
        <span class="hero-badge">Posters</span>
        <span class="hero-badge">Project Demos</span>
        <span class="hero-badge">K-12 Outreach</span>
      </div>
    </div>
  </section>

  <div class="sliding-bar">
    <div class="slide-track">
      <div class="slide-item"><span>●</span> Invited Lectures</div>
      <div class="slide-item"><span>●</span> IEEE Talks</div>
      <div class="slide-item"><span>●</span> K-12 STEM Outreach</div>
      <div class="slide-item"><span>●</span> RFCoN Presentation</div>
      <div class="slide-item"><span>●</span> GLSVLSI Poster</div>
      <div class="slide-item"><span>●</span> VLSI Design Flow</div>
      <div class="slide-item"><span>●</span> AI Project Demos</div>

      <div class="slide-item"><span>●</span> Invited Lectures</div>
      <div class="slide-item"><span>●</span> IEEE Talks</div>
      <div class="slide-item"><span>●</span> K-12 STEM Outreach</div>
      <div class="slide-item"><span>●</span> RFCoN Presentation</div>
      <div class="slide-item"><span>●</span> GLSVLSI Poster</div>
      <div class="slide-item"><span>●</span> VLSI Design Flow</div>
      <div class="slide-item"><span>●</span> AI Project Demos</div>
    </div>
  </div>

  <section class="pres-summary">
    <div class="pres-summary-card">
      <span>Invited</span>
      <small>Lectures and professional talks</small>
    </div>

    <div class="pres-summary-card">
      <span>IEEE</span>
      <small>Conference and branch presentations</small>
    </div>

    <div class="pres-summary-card">
      <span>K-12</span>
      <small>STEM outreach presentations</small>
    </div>

    <div class="pres-summary-card">
      <span>Demos</span>
      <small>Projects, hackathons, and videos</small>
    </div>
  </section>

  <section class="pres-section">
    <div class="pres-section-header">
      <h2>📚 Presentation Categories</h2>
      <p>
        Use the tabs below to view featured presentations, conference/poster presentations,
        and video demonstrations.
      </p>
    </div>

    <div class="divider"></div>

    <div class="pres-tabs">
      <button class="tab-button active" onclick="openPresTab(event, 'featured-tab')">Featured Presentations</button>
      <button class="tab-button" onclick="openPresTab(event, 'conference-tab')">Conference & Posters</button>
      <button class="tab-button" onclick="openPresTab(event, 'videos-tab')">Videos & Demos</button>
    </div>

    <div id="featured-tab" class="tab-panel active">

      <div class="presentation-grid">

        <div class="presentation-card" onclick="openPresentation('/publications/Chiddix_K12_Speaker_Demo_PPT_2026.pdf')">
          <div class="presentation-thumb">
            <img src="/images/Chiddix_K12_Speaker_Demo_2026.png" alt="Chiddix K-12 Speaker Demo Presentation 2026">
            <div class="pres-badge">K-12 Outreach</div>
            <div class="pres-year">2026</div>
          </div>
        
          <div class="presentation-body">
            <h4>K-12 Speaker Demo Outreach at Chiddix Junior High School</h4>
            <p>
              Hands-on electrical engineering outreach presentation introducing 5th and 8th grade students
              to how a simple speaker works.
            </p>
        
            <div class="pres-tags">
              <span>K-12</span>
              <span>Speaker Demo</span>
              <span>Electrical Engineering</span>
              <span>STEM Outreach</span>
            </div>
          </div>
        </div>
        
        <div class="presentation-card" onclick="openPresentation('/publications/IAB K-12 PPT Srinivas.pdf')">
          <div class="presentation-thumb">
            <img src="/images/IAB_K12_Outreach_1.png" alt="IAB K-12 STEM Outreach Presentation 2026">
            <div class="pres-badge">Outreach</div>
            <div class="pres-year">2026</div>
          </div>
          <div class="presentation-body">
            <h4>IAB Presentation on K-12 STEM Outreach</h4>
            <p>Presentation highlighting hands-on electrical engineering outreach activities for middle and high school students.</p>
            <div class="pres-tags">
              <span>K-12</span>
              <span>STEM</span>
              <span>Outreach</span>
            </div>
          </div>
        </div>

        <div class="presentation-card" onclick="openPresentation('/publications/IEEE_Invited_Lecture_Srinivas.pdf')">
          <div class="presentation-thumb">
            <img src="/images/IEEE_Lecture.png" alt="IEEE Invited Lecture 2026">
            <div class="pres-badge">Invited Talk</div>
            <div class="pres-year">2026</div>
          </div>
          <div class="presentation-body">
            <h4>IEEE Invited Lecture</h4>
            <p>Invited lecture on RTL-to-GDSII chip design flow, EDA tools, VLSI methodology, and semiconductor career pathways.</p>
            <div class="pres-tags">
              <span>IEEE</span>
              <span>VLSI</span>
              <span>RTL to GDSII</span>
            </div>
          </div>
        </div>

        <div class="presentation-card" onclick="openPresentation('/publications/rfcon.pdf')">
          <div class="presentation-thumb">
            <img src="/images/rfcon_presentation_thumbnail.png" alt="RFCoN 2025 Presentation">
            <div class="pres-badge">Conference</div>
            <div class="pres-year">2025</div>
          </div>
          <div class="presentation-body">
            <h4>RFCoN 2025 Presentation</h4>
            <p>Research presentation on RF communication, signal processing, and lightweight modulation classification methods.</p>
            <div class="pres-tags">
              <span>RFCoN</span>
              <span>RF Systems</span>
              <span>Classification</span>
            </div>
          </div>
        </div>

        <div class="presentation-card" onclick="openPresentation('/publications/UMKC_ATP_Interview_Presentation_Rahul.pdf')">
          <div class="presentation-thumb">
            <img src="/images/umkc_presentation_thumbnail.png" alt="UMKC Assistant Teaching Professor Interview Presentation">
            <div class="pres-badge">Teaching</div>
            <div class="pres-year">Academic</div>
          </div>
          <div class="presentation-body">
            <h4>UMKC Assistant Teaching Professor Interview</h4>
            <p>Academic teaching presentation focused on instructional experience, engineering education, and student engagement.</p>
            <div class="pres-tags">
              <span>Teaching</span>
              <span>Engineering</span>
              <span>Academic Talk</span>
            </div>
          </div>
        </div>

        <div class="presentation-card" onclick="openPresentation('/publications/MIDE_Dec_2022.pdf')">
          <div class="presentation-thumb">
            <img src="/images/mide_ct_thumbnail.png" alt="MIDE Capstone Talk December 2022">
            <div class="pres-badge">Capstone</div>
            <div class="pres-year">2022</div>
          </div>
          <div class="presentation-body">
            <h4>MIDE Capstone Talk</h4>
            <p>Capstone presentation delivered in December 2022, highlighting project development and applied engineering work.</p>
            <div class="pres-tags">
              <span>Capstone</span>
              <span>Project</span>
              <span>Presentation</span>
            </div>
          </div>
        </div>

        <div class="presentation-card" onclick="openPresentation('/publications/DNN_Presentation.pptx')">
          <div class="presentation-thumb">
            <img src="/images/rahul_nn_presentation.png" alt="Deep Neural Networks Presentation">
            <div class="pres-badge">AI</div>
            <div class="pres-year">Talk</div>
          </div>
          <div class="presentation-body">
            <h4>Deep Neural Networks Talk</h4>
            <p>Presentation on deep neural networks, model structure, learning concepts, and applied machine learning workflows.</p>
            <div class="pres-tags">
              <span>AI</span>
              <span>DNN</span>
              <span>Machine Learning</span>
            </div>
          </div>
        </div>

        <div class="presentation-card" onclick="openPresentation('/publications/Army_PPT.pptx')">
          <div class="presentation-thumb">
            <img src="/images/army_ppt_thumbnail.png" alt="U.S. Army Research Presentation August 2023">
            <div class="pres-badge">Research</div>
            <div class="pres-year">2023</div>
          </div>
          <div class="presentation-body">
            <h4>U.S. Army Research Presentation</h4>
            <p>Research-oriented presentation connected to applied engineering, defense-related technologies, and technical development.</p>
            <div class="pres-tags">
              <span>Research</span>
              <span>Defense</span>
              <span>Engineering</span>
            </div>
          </div>
        </div>

        <div class="presentation-card" onclick="openPresentation('/publications/Falcon.pdf')">
          <div class="presentation-thumb">
            <img src="/images/Falcon.png" alt="Falcon Labs SaaS Platform">
            <div class="pres-badge">Software</div>
            <div class="pres-year">Project</div>
          </div>
          <div class="presentation-body">
            <h4>Falcon Labs SaaS Platform</h4>
            <p>Project presentation on a SaaS-based software platform, application development, and product-oriented system design.</p>
            <div class="pres-tags">
              <span>SaaS</span>
              <span>Software</span>
              <span>Platform</span>
            </div>
          </div>
        </div>

        <div class="presentation-card" onclick="openPresentation('/publications/Lunar.pdf')">
          <div class="presentation-thumb">
            <img src="/images/Lunar.png" alt="Lunar Lander using Deep Q-Learning">
            <div class="pres-badge">Reinforcement Learning</div>
            <div class="pres-year">Project</div>
          </div>
          <div class="presentation-body">
            <h4>Lunar Lander using Deep Q-Learning</h4>
            <p>Project presentation on reinforcement learning using Deep Q-Learning for lunar lander control and decision making.</p>
            <div class="pres-tags">
              <span>DQN</span>
              <span>RL</span>
              <span>AI Project</span>
            </div>
          </div>
        </div>

      </div>
    </div>

    <div id="conference-tab" class="tab-panel">
      <div class="poster-grid">

        <div class="poster-card">
          <img src="/images/glsposter_1.png" alt="GLSVLSI 2025 Poster Presentation">
          <div class="poster-content">
            <h4>GLSVLSI 2025 - Poster Presentation</h4>
            <p>
              Poster presentation at the Great Lakes Symposium on VLSI, highlighting work related to VLSI,
              hardware-aware machine learning, and efficient computing systems.
            </p>
            <div class="pres-tags">
              <span>GLSVLSI</span>
              <span>Poster</span>
              <span>VLSI</span>
            </div>
          </div>
        </div>

        <div class="poster-card">
          <img src="/images/rfcon_presenter.png" alt="RFCoN 2025 Oral Presentation">
          <div class="poster-content">
            <h4>RFCoN 2025 - Oral Presentation</h4>
            <p>
              Oral presentation at RFCoN 2025 focused on RF communication and lightweight modulation
              classification methods for efficient signal analysis.
            </p>
            <div class="pres-tags">
              <span>RFCoN</span>
              <span>Oral Talk</span>
              <span>RF Communication</span>
            </div>
          </div>
        </div>

      </div>
    </div>

    <div id="videos-tab" class="tab-panel">
      <div class="youtube-card-grid">

        <div class="youtube-card">
          <div class="youtube-frame">
            <iframe src="https://www.youtube.com/embed/aRM4DP-gUbg" title="Hackathon Win Fall 2021" allowfullscreen></iframe>
          </div>
          <div class="youtube-body">
            <h4>Hackathon Win - Fall 2021</h4>
            <p>Video highlight from a hackathon project and award-winning technical demonstration.</p>
          </div>
        </div>

        <div class="youtube-card">
          <div class="youtube-frame">
            <iframe src="https://www.youtube.com/embed/cJ4JHmoTgas" title="Hackathon Win Fall 2022" allowfullscreen></iframe>
          </div>
          <div class="youtube-body">
            <h4>Hackathon Win - Fall 2022</h4>
            <p>Project video showcasing technical development, teamwork, and applied software engineering.</p>
          </div>
        </div>

        <div class="youtube-card">
          <div class="youtube-frame">
            <iframe src="https://www.youtube.com/embed/E9ItHVkHuy8" title="Internship Project Demo" allowfullscreen></iframe>
          </div>
          <div class="youtube-body">
            <h4>Internship Project Demo</h4>
            <p>Demonstration video from internship work, highlighting project implementation and applied technical learning.</p>
          </div>
        </div>

      </div>
    </div>

  </section>

  <div class="pres-copyright">
    © 2026 Srinivas Rahul S. All rights reserved. The text, images, slide previews, layout, design elements,
    and presentation descriptions on this page may not be copied, reproduced, republished, modified,
    or redistributed without prior written permission.
  </div>

</div>

<!-- Presentation Lightbox Viewer -->
<div class="pres-lightbox" id="presentation-lightbox">
  <span class="pres-lightbox-close" id="presentation-lightbox-close">&times;</span>
  <div class="pres-lightbox-content">
    <iframe id="presentation-frame" src=""></iframe>
  </div>
</div>

<script>
function openPresTab(event, panelId) {
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

function openPresentation(url) {
  const baseUrl = "https://srsapireddy.github.io";
  const encodedUrl = encodeURIComponent(baseUrl + url);
  const viewerUrl = "https://docs.google.com/gview?url=" + encodedUrl + "&embedded=true";

  document.getElementById("presentation-frame").src = viewerUrl;
  document.getElementById("presentation-lightbox").style.display = "flex";
}

document.addEventListener("DOMContentLoaded", function () {
  const lightbox = document.getElementById("presentation-lightbox");
  const closeBtn = document.getElementById("presentation-lightbox-close");
  const frame = document.getElementById("presentation-frame");

  function closePresentation() {
    lightbox.style.display = "none";
    frame.src = "";
  }

  closeBtn.addEventListener("click", closePresentation);

  lightbox.addEventListener("click", function(e) {
    if (e.target === lightbox) {
      closePresentation();
    }
  });

  document.addEventListener("keydown", function(e) {
    if (e.key === "Escape") {
      closePresentation();
    }
  });

  document.addEventListener("contextmenu", function(e) {
    if (e.target.closest(".presentations-protected")) {
      e.preventDefault();
    }
  });

  document.addEventListener("keydown", function(e) {
    const blockedKeys = ["c", "u", "s", "a"];

    if ((e.ctrlKey || e.metaKey) && blockedKeys.includes(e.key.toLowerCase())) {
      if (document.activeElement.closest(".presentations-protected")) {
        e.preventDefault();
      }
    }
  });
});
</script>
