---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
---

<style>
:root{
  --blue:#1a73e8;
  --blue2:#0b5bd3;
  --isu:#DC143C;
  --green:#1a7f3d;
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

.projects-wrap{
  animation:fadeInUp 0.85s ease-in-out;
}

/* Hero */
.projects-hero{
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

.projects-hero::before{
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

.projects-hero h1{
  margin:0;
  font-size:2.15rem;
  line-height:1.15;
  color:var(--text);
}

.projects-hero p{
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

/* Sliding Bar */
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

/* Impact Cards */
.project-summary{
  display:grid;
  grid-template-columns:repeat(4,1fr);
  gap:0.95rem;
  margin-bottom:1.3rem;
}

.summary-card{
  padding:1.1rem 1rem;
  border-radius:16px;
  background:linear-gradient(135deg,#ffffff 0%,#f7fbff 100%);
  border:1px solid rgba(26,115,232,0.18);
  box-shadow:var(--shadow2);
  text-align:center;
  transition:0.25s ease-in-out;
}

.summary-card:hover{
  transform:translateY(-3px);
  box-shadow:var(--shadow);
}

.summary-card span{
  display:block;
  color:var(--isu);
  font-size:1.55rem;
  font-weight:950;
  line-height:1.1;
}

.summary-card small{
  display:block;
  color:var(--muted);
  font-size:0.82rem;
  margin-top:0.28rem;
}

/* Section */
.project-section{
  border:1px solid var(--border);
  background:var(--bg);
  padding:1.35rem 1.5rem;
  margin-bottom:1.3rem;
  border-radius:var(--radius2);
  box-shadow:var(--shadow2);
  transition:0.25s ease-in-out;
}

.project-section:hover{
  background:#fbfdff;
  transform:translateY(-2px);
  box-shadow:var(--shadow);
}

.project-section h2{
  margin:0;
  color:var(--text);
  font-size:1.22rem;
  display:flex;
  align-items:center;
  gap:0.55rem;
}

.project-section p{
  color:#202124;
  line-height:1.65;
}

.divider{
  height:1px;
  background:rgba(26,115,232,0.12);
  margin:0.6rem 0 1rem 0;
}

/* Tabs */
.project-tabs{
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

/* Project Grid */
.project-grid{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(275px,1fr));
  gap:1.1rem;
}

.project-box{
  position:relative;
  overflow:hidden;
  border:1px solid rgba(26,115,232,0.18);
  padding:1.1rem 1.15rem;
  border-radius:16px;
  background:#ffffff;
  box-shadow:var(--shadow2);
  transition:0.25s ease-in-out;
}

.project-box:hover{
  transform:translateY(-4px);
  box-shadow:var(--shadow);
  background:#fbfdff;
  border-color:rgba(26,115,232,0.38);
}

.project-box::before{
  content:"";
  position:absolute;
  top:0;
  left:0;
  width:100%;
  height:5px;
  background:linear-gradient(90deg,var(--blue),var(--isu));
}

.project-icon{
  width:44px;
  height:44px;
  display:flex;
  align-items:center;
  justify-content:center;
  border-radius:14px;
  background:#e9f3ff;
  color:var(--blue);
  font-size:1.35rem;
  margin-bottom:0.8rem;
  box-shadow:0 4px 12px rgba(26,115,232,0.16);
}

.project-box a{
  font-weight:950;
  font-size:1.02rem;
  text-decoration:none;
  color:var(--text);
  line-height:1.35;
}

.project-box a:hover{
  color:var(--blue);
  text-decoration:none;
}

.project-box p{
  margin-top:0.45rem;
  font-size:0.92rem;
  color:#475569;
  line-height:1.55;
}

.project-tags{
  display:flex;
  flex-wrap:wrap;
  gap:0.42rem;
  margin-top:0.85rem;
}

.project-tags span{
  padding:0.28rem 0.55rem;
  border-radius:999px;
  background:#eef6ff;
  color:var(--blue);
  border:1px solid rgba(26,115,232,0.16);
  font-size:0.72rem;
  font-weight:850;
}

.project-actions{
  display:flex;
  flex-wrap:wrap;
  gap:0.55rem;
  margin-top:0.9rem;
}

.project-link{
  display:inline-flex;
  align-items:center;
  padding:0.36rem 0.72rem;
  border-radius:999px;
  background:var(--blue);
  color:#ffffff !important;
  text-decoration:none !important;
  font-size:0.84rem;
  font-weight:850;
}

.project-link:hover{
  background:var(--blue2);
  text-decoration:none !important;
}

/* Theme Cards */
.theme-grid{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:1.1rem;
  margin-bottom:1.3rem;
}

.theme-card{
  position:relative;
  overflow:hidden;
  padding:1.25rem;
  border-radius:16px;
  background:linear-gradient(135deg,#ffffff 0%,#f4f9ff 100%);
  border:1px solid rgba(26,115,232,0.18);
  box-shadow:var(--shadow2);
  transition:0.25s ease-in-out;
}

.theme-card:hover{
  transform:translateY(-4px);
  box-shadow:var(--shadow);
}

.theme-card::before{
  content:"";
  position:absolute;
  top:0;
  left:0;
  height:5px;
  width:100%;
  background:linear-gradient(90deg,var(--blue),var(--isu));
}

.theme-icon{
  width:46px;
  height:46px;
  border-radius:14px;
  background:#e9f3ff;
  color:var(--blue);
  display:flex;
  align-items:center;
  justify-content:center;
  font-size:1.45rem;
  margin-bottom:0.85rem;
  box-shadow:0 4px 12px rgba(26,115,232,0.16);
}

.theme-card h3{
  margin:0 0 0.55rem 0;
  font-size:1.12rem;
  color:var(--text);
}

.theme-card p{
  margin:0;
  color:#202124;
  line-height:1.55;
  font-size:0.95rem;
}

/* Skill tags */
.tag-cloud{
  display:flex;
  flex-wrap:wrap;
  gap:0.55rem;
}

.tag{
  display:inline-flex;
  padding:0.36rem 0.72rem;
  border-radius:999px;
  background:#f3f8ff;
  border:1px solid rgba(26,115,232,0.18);
  color:var(--text);
  font-size:0.88rem;
  font-weight:850;
}

/* Responsive */
@media (max-width:950px){
  .project-summary,
  .theme-grid{
    grid-template-columns:repeat(2,1fr);
  }
}

@media (max-width:700px){
  .projects-hero{
    padding:1.5rem 1.1rem;
  }

  .projects-hero h1{
    font-size:1.65rem;
  }

  .project-summary,
  .theme-grid{
    grid-template-columns:1fr;
  }
}
</style>

<div class="projects-wrap">

  <div class="projects-hero">
    <div class="hero-content">
      <span class="hero-kicker">Projects · GitHub · AI · VLSI · RF · MLOps</span>

      <h1>Projects</h1>

      <p>
        A curated portfolio of hands-on projects across hackathons, computer science,
        machine learning, MLOps, web development, VLSI design, digital verification,
        RF signal classification, and hardware-aware computing.
      </p>

      <div class="hero-badges">
        <span class="hero-badge red">Hackathon Projects</span>
        <span class="hero-badge">Computer Science</span>
        <span class="hero-badge">Machine Learning</span>
        <span class="hero-badge">VLSI and ECE</span>
        <span class="hero-badge">GitHub Portfolio</span>
      </div>
    </div>
  </div>

  <div class="sliding-bar">
    <div class="slide-track">
      <div class="slide-item"><span>●</span> Deep Q-Learning</div>
      <div class="slide-item"><span>●</span> Worker Safety IoT</div>
      <div class="slide-item"><span>●</span> MLOps CI/CD</div>
      <div class="slide-item"><span>●</span> Local RAG</div>
      <div class="slide-item"><span>●</span> RAPIDS ML</div>
      <div class="slide-item"><span>●</span> RTL-to-GDSII</div>
      <div class="slide-item"><span>●</span> UVM Verification</div>
      <div class="slide-item"><span>●</span> RF Signal Classification</div>

      <div class="slide-item"><span>●</span> Deep Q-Learning</div>
      <div class="slide-item"><span>●</span> Worker Safety IoT</div>
      <div class="slide-item"><span>●</span> MLOps CI/CD</div>
      <div class="slide-item"><span>●</span> Local RAG</div>
      <div class="slide-item"><span>●</span> RAPIDS ML</div>
      <div class="slide-item"><span>●</span> RTL-to-GDSII</div>
      <div class="slide-item"><span>●</span> UVM Verification</div>
      <div class="slide-item"><span>●</span> RF Signal Classification</div>
    </div>
  </div>

  <div class="project-summary">
    <div class="summary-card">
      <span>Hackathon</span>
      <small>AI, IoT, analytics, and application projects</small>
    </div>

    <div class="summary-card">
      <span>CS</span>
      <small>MLOps, APIs, RAG, CI/CD, and cloud projects</small>
    </div>

    <div class="summary-card">
      <span>ECE</span>
      <small>VLSI, Verilog, UVM, TCL, and RF systems</small>
    </div>

    <div class="summary-card">
      <span>GitHub</span>
      <small>Open project repositories and code artifacts</small>
    </div>
  </div>

  <div class="theme-grid">
    <div class="theme-card">
      <div class="theme-icon">🧠</div>
      <h3>AI and Machine Learning</h3>
      <p>
        Projects include deep reinforcement learning, RAPIDS GPU acceleration,
        MLOps pipelines, Hugging Face deployment, and local RAG workflows.
      </p>
    </div>

    <div class="theme-card">
      <div class="theme-icon">⚙️</div>
      <h3>VLSI and Digital Systems</h3>
      <p>
        Hands-on ECE projects cover RTL-to-GDSII flows, OpenLANE, SKY130,
        RISC-V, UVM verification, TCL automation, and Verilog design.
      </p>
    </div>

    <div class="theme-card">
      <div class="theme-icon">📡</div>
      <h3>RF and Edge Systems</h3>
      <p>
        Projects include RF signal classification, protocol simulation,
        embedded interfaces, and practical hardware-aware workflows.
      </p>
    </div>
  </div>

  <div class="project-section">
    <h2>📂 Project Categories</h2>
    <div class="divider"></div>

    <p>
      Use the tabs below to view projects by category. Each card links directly to the corresponding GitHub repository.
    </p>

    <div class="project-tabs">
      <button class="tab-button active" onclick="openProjectTab(event, 'hackathon-tab')">Hackathon Projects</button>
      <button class="tab-button" onclick="openProjectTab(event, 'cs-tab')">Computer Science Projects</button>
      <button class="tab-button" onclick="openProjectTab(event, 'ece-tab')">Electrical & Computer Engineering</button>
      <button class="tab-button" onclick="openProjectTab(event, 'all-tab')">All Projects</button>
    </div>

    <div id="hackathon-tab" class="tab-panel active">
      <div class="project-grid">

        <div class="project-box">
          <div class="project-icon">🚀</div>
          <a href="https://github.com/srsapireddy/lunar_lander_using_DQN" target="_blank" rel="noopener">Lunar Lander using DQN</a>
          <p>Deep Q-Learning based game simulation using OpenAI Gym for dynamic control.</p>
          <div class="project-tags">
            <span>DQN</span>
            <span>Reinforcement Learning</span>
            <span>OpenAI Gym</span>
          </div>
          <div class="project-actions">
            <a class="project-link" href="https://github.com/srsapireddy/lunar_lander_using_DQN" target="_blank" rel="noopener">View GitHub</a>
          </div>
        </div>

        <div class="project-box">
          <div class="project-icon">🦺</div>
          <a href="https://github.com/srsapireddy/Intelligent-Worker-Safety-System-with-Real-Time-Alerts-and-Machine-Control" target="_blank" rel="noopener">Worker Safety System</a>
          <p>IoT-based smart safety monitoring system for industrial workers with instant alerting.</p>
          <div class="project-tags">
            <span>IoT</span>
            <span>Safety</span>
            <span>Real-Time Alerts</span>
          </div>
          <div class="project-actions">
            <a class="project-link" href="https://github.com/srsapireddy/Intelligent-Worker-Safety-System-with-Real-Time-Alerts-and-Machine-Control" target="_blank" rel="noopener">View GitHub</a>
          </div>
        </div>

        <div class="project-box">
          <div class="project-icon">🏢</div>
          <a href="https://github.com/srsapireddy/Data_Centers" target="_blank" rel="noopener">Data Centers</a>
          <p>Smart data center analytics with optimized power usage and real-time monitoring dashboards.</p>
          <div class="project-tags">
            <span>Analytics</span>
            <span>Power Optimization</span>
            <span>Monitoring</span>
          </div>
          <div class="project-actions">
            <a class="project-link" href="https://github.com/srsapireddy/Data_Centers" target="_blank" rel="noopener">View GitHub</a>
          </div>
        </div>

        <div class="project-box">
          <div class="project-icon">🦅</div>
          <a href="https://github.com/srsapireddy/Falcon-Application" target="_blank" rel="noopener">Falcon Application</a>
          <p>Personal assistant app.</p>
          <div class="project-tags">
            <span>Application</span>
            <span>Assistant</span>
            <span>Software</span>
          </div>
          <div class="project-actions">
            <a class="project-link" href="https://github.com/srsapireddy/Falcon-Application" target="_blank" rel="noopener">View GitHub</a>
          </div>
        </div>

      </div>
    </div>

    <div id="cs-tab" class="tab-panel">
      <div class="project-grid">

        <div class="project-box">
          <div class="project-icon">🖥️</div>
          <a href="https://github.com/srsapireddy/Setup-NVIDIA-GPU-for-Deep-Learning" target="_blank" rel="noopener">NVIDIA GPU Setup</a>
          <p>Instructions to configure NVIDIA drivers, CUDA, cuDNN for DL workloads.</p>
          <div class="project-tags">
            <span>NVIDIA</span>
            <span>CUDA</span>
            <span>Deep Learning</span>
          </div>
          <div class="project-actions">
            <a class="project-link" href="https://github.com/srsapireddy/Setup-NVIDIA-GPU-for-Deep-Learning" target="_blank" rel="noopener">View GitHub</a>
          </div>
        </div>

        <div class="project-box">
          <div class="project-icon">🧪</div>
          <a href="https://github.com/srsapireddy/Testing-Machine-Learning-Systems-Unit-Tests" target="_blank" rel="noopener">ML Unit Testing</a>
          <p>Framework for verifying ML models using unit and integration test cases.</p>
          <div class="project-tags">
            <span>Testing</span>
            <span>ML Systems</span>
            <span>Unit Tests</span>
          </div>
          <div class="project-actions">
            <a class="project-link" href="https://github.com/srsapireddy/Testing-Machine-Learning-Systems-Unit-Tests" target="_blank" rel="noopener">View GitHub</a>
          </div>
        </div>

        <div class="project-box">
          <div class="project-icon">🌐</div>
          <a href="https://github.com/srsapireddy/MEAN-Stack-Application" target="_blank" rel="noopener">MEAN Stack App</a>
          <p>Full-stack web app using MongoDB, Express, Angular, and Node.js.</p>
          <div class="project-tags">
            <span>MongoDB</span>
            <span>Express</span>
            <span>Angular</span>
            <span>Node.js</span>
          </div>
          <div class="project-actions">
            <a class="project-link" href="https://github.com/srsapireddy/MEAN-Stack-Application" target="_blank" rel="noopener">View GitHub</a>
          </div>
        </div>

        <div class="project-box">
          <div class="project-icon">☁️</div>
          <a href="https://github.com/srsapireddy/Serverless_Deep_Learning_Code" target="_blank" rel="noopener">Serverless DL</a>
          <p>Running ML models with AWS Lambda functions and API Gateway integration.</p>
          <div class="project-tags">
            <span>AWS Lambda</span>
            <span>API Gateway</span>
            <span>Serverless</span>
          </div>
          <div class="project-actions">
            <a class="project-link" href="https://github.com/srsapireddy/Serverless_Deep_Learning_Code" target="_blank" rel="noopener">View GitHub</a>
          </div>
        </div>

        <div class="project-box">
          <div class="project-icon">🤗</div>
          <a href="https://github.com/srsapireddy/hugging-face-demo-CI-with-continuous-deployment" target="_blank" rel="noopener">HuggingFace CI/CD</a>
          <p>End-to-end NLP deployment using HuggingFace transformers with GitHub Actions.</p>
          <div class="project-tags">
            <span>HuggingFace</span>
            <span>Transformers</span>
            <span>GitHub Actions</span>
          </div>
          <div class="project-actions">
            <a class="project-link" href="https://github.com/srsapireddy/hugging-face-demo-CI-with-continuous-deployment" target="_blank" rel="noopener">View GitHub</a>
          </div>
        </div>

        <div class="project-box">
          <div class="project-icon">⚡</div>
          <a href="https://github.com/srsapireddy/fastapi-swagger-ui" target="_blank" rel="noopener">FastAPI Swagger</a>
          <p>REST APIs using FastAPI framework with auto-generated Swagger documentation.</p>
          <div class="project-tags">
            <span>FastAPI</span>
            <span>Swagger</span>
            <span>REST API</span>
          </div>
          <div class="project-actions">
            <a class="project-link" href="https://github.com/srsapireddy/fastapi-swagger-ui" target="_blank" rel="noopener">View GitHub</a>
          </div>
        </div>

        <div class="project-box">
          <div class="project-icon">🚄</div>
          <a href="https://github.com/srsapireddy/RAPIDS_Machine_Learning" target="_blank" rel="noopener">RAPIDS ML</a>
          <p>GPU-accelerated ML using NVIDIA RAPIDS for large-scale data processing.</p>
          <div class="project-tags">
            <span>RAPIDS</span>
            <span>GPU ML</span>
            <span>NVIDIA</span>
          </div>
          <div class="project-actions">
            <a class="project-link" href="https://github.com/srsapireddy/RAPIDS_Machine_Learning" target="_blank" rel="noopener">View GitHub</a>
          </div>
        </div>

        <div class="project-box">
          <div class="project-icon">🔁</div>
          <a href="https://github.com/srsapireddy/End-to-End-Machine-Learning-Pipeline-Creation-Using-DVC" target="_blank" rel="noopener">ML Pipeline (DVC)</a>
          <p>Building reproducible ML pipelines using Data Version Control.</p>
          <div class="project-tags">
            <span>DVC</span>
            <span>ML Pipeline</span>
            <span>Reproducibility</span>
          </div>
          <div class="project-actions">
            <a class="project-link" href="https://github.com/srsapireddy/End-to-End-Machine-Learning-Pipeline-Creation-Using-DVC" target="_blank" rel="noopener">View GitHub</a>
          </div>
        </div>

        <div class="project-box">
          <div class="project-icon">📚</div>
          <a href="https://github.com/srsapireddy/Local-Retrieval-augmented-generation-RAG" target="_blank" rel="noopener">RAG (Local)</a>
          <p>Retrieval Augmented Generation pipeline on local knowledge base.</p>
          <div class="project-tags">
            <span>RAG</span>
            <span>LLM</span>
            <span>Local AI</span>
          </div>
          <div class="project-actions">
            <a class="project-link" href="https://github.com/srsapireddy/Local-Retrieval-augmented-generation-RAG" target="_blank" rel="noopener">View GitHub</a>
          </div>
        </div>

        <div class="project-box">
          <div class="project-icon">🧩</div>
          <a href="https://github.com/srsapireddy/MLOps-CI-CD-Pipeline" target="_blank" rel="noopener">MLOps CI/CD</a>
          <p>CI/CD pipeline for ML models using Docker, GitHub Actions, and DVC.</p>
          <div class="project-tags">
            <span>MLOps</span>
            <span>Docker</span>
            <span>CI/CD</span>
          </div>
          <div class="project-actions">
            <a class="project-link" href="https://github.com/srsapireddy/MLOps-CI-CD-Pipeline" target="_blank" rel="noopener">View GitHub</a>
          </div>
        </div>

      </div>
    </div>

    <div id="ece-tab" class="tab-panel">
      <div class="project-grid">

        <div class="project-box">
          <div class="project-icon">🧱</div>
          <a href="https://github.com/srsapireddy/Physical_Design_Flow_Cadence_Tools" target="_blank" rel="noopener">PD Flow (Cadence)</a>
          <p>RTL to GDSII implementation using Cadence Innovus tools and custom scripts.</p>
          <div class="project-tags">
            <span>Cadence</span>
            <span>RTL-to-GDSII</span>
            <span>Physical Design</span>
          </div>
          <div class="project-actions">
            <a class="project-link" href="https://github.com/srsapireddy/Physical_Design_Flow_Cadence_Tools" target="_blank" rel="noopener">View GitHub</a>
          </div>
        </div>

        <div class="project-box">
          <div class="project-icon">🔌</div>
          <a href="https://github.com/srsapireddy/SPI-and-UART-Protocol" target="_blank" rel="noopener">SPI & UART</a>
          <p>Protocol design and simulation in Verilog for SPI and UART interfaces.</p>
          <div class="project-tags">
            <span>SPI</span>
            <span>UART</span>
            <span>Verilog</span>
          </div>
          <div class="project-actions">
            <a class="project-link" href="https://github.com/srsapireddy/SPI-and-UART-Protocol" target="_blank" rel="noopener">View GitHub</a>
          </div>
        </div>

        <div class="project-box">
          <div class="project-icon">✅</div>
          <a href="https://github.com/srsapireddy/UVM-Test-Bench-Environment-ALU" target="_blank" rel="noopener">UVM ALU Testbench</a>
          <p>UVM-based testbench for verifying an Arithmetic Logic Unit (ALU).</p>
          <div class="project-tags">
            <span>UVM</span>
            <span>ALU</span>
            <span>Verification</span>
          </div>
          <div class="project-actions">
            <a class="project-link" href="https://github.com/srsapireddy/UVM-Test-Bench-Environment-ALU" target="_blank" rel="noopener">View GitHub</a>
          </div>
        </div>

        <div class="project-box">
          <div class="project-icon">➕</div>
          <a href="https://github.com/srsapireddy/Systemverilog-Test-Bench-Environment-Half-Adder" target="_blank" rel="noopener">SV Testbench - Half Adder</a>
          <p>SystemVerilog-based modular test environment for Half Adder validation.</p>
          <div class="project-tags">
            <span>SystemVerilog</span>
            <span>Half Adder</span>
            <span>Testbench</span>
          </div>
          <div class="project-actions">
            <a class="project-link" href="https://github.com/srsapireddy/Systemverilog-Test-Bench-Environment-Half-Adder" target="_blank" rel="noopener">View GitHub</a>
          </div>
        </div>

        <div class="project-box">
          <div class="project-icon">📜</div>
          <a href="https://github.com/srsapireddy/TCL-Automation" target="_blank" rel="noopener">TCL Automation</a>
          <p>Automated VLSI flow scripting using advanced TCL techniques.</p>
          <div class="project-tags">
            <span>TCL</span>
            <span>Automation</span>
            <span>VLSI Flow</span>
          </div>
          <div class="project-actions">
            <a class="project-link" href="https://github.com/srsapireddy/TCL-Automation" target="_blank" rel="noopener">View GitHub</a>
          </div>
        </div>

        <div class="project-box">
          <div class="project-icon">🛤️</div>
          <a href="https://github.com/srsapireddy/OpenLANE_EDA" target="_blank" rel="noopener">OpenLANE EDA</a>
          <p>ASIC flow using the open-source OpenLANE and Sky130 PDK.</p>
          <div class="project-tags">
            <span>OpenLANE</span>
            <span>Sky130</span>
            <span>ASIC Flow</span>
          </div>
          <div class="project-actions">
            <a class="project-link" href="https://github.com/srsapireddy/OpenLANE_EDA" target="_blank" rel="noopener">View GitHub</a>
          </div>
        </div>

        <div class="project-box">
          <div class="project-icon">🧮</div>
          <a href="https://github.com/srsapireddy/RISC-V_ISA" target="_blank" rel="noopener">RISC-V ISA</a>
          <p>RISC-V Instruction Set Architecture design and testing in Verilog.</p>
          <div class="project-tags">
            <span>RISC-V</span>
            <span>ISA</span>
            <span>Verilog</span>
          </div>
          <div class="project-actions">
            <a class="project-link" href="https://github.com/srsapireddy/RISC-V_ISA" target="_blank" rel="noopener">View GitHub</a>
          </div>
        </div>

        <div class="project-box">
          <div class="project-icon">🔷</div>
          <a href="https://github.com/srsapireddy/RTL-Design-in-Verilog-using-SKY130-Technology" target="_blank" rel="noopener">SKY130 RTL Design</a>
          <p>RTL design and synthesis using SKY130 technology nodes.</p>
          <div class="project-tags">
            <span>RTL</span>
            <span>SKY130</span>
            <span>Synthesis</span>
          </div>
          <div class="project-actions">
            <a class="project-link" href="https://github.com/srsapireddy/RTL-Design-in-Verilog-using-SKY130-Technology" target="_blank" rel="noopener">View GitHub</a>
          </div>
        </div>

        <div class="project-box">
          <div class="project-icon">🧾</div>
          <a href="https://github.com/srsapireddy/Advanced-TCL-Scripting" target="_blank" rel="noopener">Advanced TCL</a>
          <p>Deep dive into TCL scripting with conditionals and design checks.</p>
          <div class="project-tags">
            <span>TCL</span>
            <span>Scripting</span>
            <span>Design Checks</span>
          </div>
          <div class="project-actions">
            <a class="project-link" href="https://github.com/srsapireddy/Advanced-TCL-Scripting" target="_blank" rel="noopener">View GitHub</a>
          </div>
        </div>

        <div class="project-box">
          <div class="project-icon">📡</div>
          <a href="https://github.com/srsapireddy/RF_SIGNAL_CLASSIFCATION" target="_blank" rel="noopener">RF Signal Classification</a>
          <p>Modulation classification using CAF, STFT, and custom ML models.</p>
          <div class="project-tags">
            <span>RF</span>
            <span>CAF</span>
            <span>STFT</span>
            <span>ML</span>
          </div>
          <div class="project-actions">
            <a class="project-link" href="https://github.com/srsapireddy/RF_SIGNAL_CLASSIFCATION" target="_blank" rel="noopener">View GitHub</a>
          </div>
        </div>

      </div>
    </div>

    <div id="all-tab" class="tab-panel">
      <p>
        Select the Hackathon, Computer Science, or Electrical &amp; Computer Engineering tabs above for organized project views.
      </p>

      <div class="tag-cloud">
        <span class="tag">Deep Q-Learning</span>
        <span class="tag">IoT Safety</span>
        <span class="tag">Data Center Analytics</span>
        <span class="tag">NVIDIA CUDA</span>
        <span class="tag">Machine Learning Testing</span>
        <span class="tag">MEAN Stack</span>
        <span class="tag">Serverless ML</span>
        <span class="tag">HuggingFace</span>
        <span class="tag">FastAPI</span>
        <span class="tag">RAPIDS ML</span>
        <span class="tag">DVC</span>
        <span class="tag">Local RAG</span>
        <span class="tag">MLOps</span>
        <span class="tag">Cadence Innovus</span>
        <span class="tag">SPI/UART</span>
        <span class="tag">UVM</span>
        <span class="tag">SystemVerilog</span>
        <span class="tag">TCL Automation</span>
        <span class="tag">OpenLANE</span>
        <span class="tag">RISC-V</span>
        <span class="tag">SKY130</span>
        <span class="tag">RF Signal Classification</span>
      </div>
    </div>

  </div>

</div>

<script>
function openProjectTab(event, panelId) {
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
</script>
