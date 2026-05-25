---
title: "Blog"
layout: single
permalink: /blog/
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

.blog-wrap{
  animation:fadeInUp 0.85s ease-in-out;
}

/* Hero */
.blog-hero{
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

.blog-hero::before{
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

.blog-hero h1{
  margin:0;
  font-size:2.15rem;
  line-height:1.15;
  color:var(--text);
}

.blog-hero p{
  margin:0.75rem 0 0 0;
  color:var(--muted);
  font-size:1.04rem;
  line-height:1.65;
  max-width:92ch;
}

.hero-row{
  display:flex;
  gap:1rem;
  flex-wrap:wrap;
  align-items:center;
  justify-content:space-between;
  margin-top:1.1rem;
}

.hero-badges{
  display:flex;
  gap:0.55rem;
  flex-wrap:wrap;
}

.pill{
  display:inline-flex;
  align-items:center;
  gap:0.42rem;
  padding:0.36rem 0.72rem;
  border-radius:999px;
  background:#ffffff;
  border:1px solid rgba(26,115,232,0.22);
  color:var(--text);
  box-shadow:var(--shadow2);
  font-size:0.88rem;
  font-weight:850;
}

.pill.red{
  border-color:rgba(220,20,60,0.30);
  color:#7a0b1f;
  background:rgba(220,20,60,0.06);
}

.pill.green{
  border-color:rgba(26,127,61,0.25);
  color:var(--green);
  background:rgba(26,127,61,0.06);
}

.pill svg{
  width:16px;
  height:16px;
}

.hero-cta{
  display:flex;
  gap:0.7rem;
  flex-wrap:wrap;
}

.cta{
  display:inline-flex;
  align-items:center;
  padding:0.58rem 0.92rem;
  border-radius:12px;
  background:#ffffff;
  color:var(--blue) !important;
  border:1px solid rgba(26,115,232,0.25);
  text-decoration:none !important;
  font-weight:850;
  box-shadow:var(--shadow2);
  transition:0.2s ease-in-out;
}

.cta:hover{
  transform:translateY(-2px);
  background:#f3f8ff;
  text-decoration:none !important;
}

.cta.primary{
  background:var(--blue);
  color:#ffffff !important;
  border-color:var(--blue);
}

.cta.primary:hover{
  background:var(--blue2);
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

.section h2,
.section h3{
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

/* Topic cards */
.topic-grid{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:1.1rem;
  margin-bottom:1.3rem;
}

.topic-card{
  position:relative;
  overflow:hidden;
  padding:1.25rem;
  border-radius:16px;
  background:linear-gradient(135deg,#ffffff 0%,#f4f9ff 100%);
  border:1px solid rgba(26,115,232,0.18);
  box-shadow:var(--shadow2);
  transition:0.25s ease-in-out;
}

.topic-card:hover{
  transform:translateY(-4px);
  box-shadow:var(--shadow);
}

.topic-card::before{
  content:"";
  position:absolute;
  top:0;
  left:0;
  height:5px;
  width:100%;
  background:linear-gradient(90deg,var(--blue),var(--isu));
}

.topic-icon{
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

.topic-card h3{
  margin:0 0 0.55rem 0;
  font-size:1.12rem;
  color:var(--text);
}

.topic-card p{
  margin:0;
  color:#202124;
  line-height:1.55;
  font-size:0.95rem;
}

/* Blog tabs */
.blog-tabs{
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

/* Post cards */
.post-list{
  display:flex;
  flex-direction:column;
  gap:0.9rem;
}

.post-card{
  position:relative;
  background:#ffffff;
  border:1px solid rgba(26,115,232,0.16);
  border-radius:16px;
  padding:1.05rem 1.1rem 1.05rem 1.25rem;
  box-shadow:var(--shadow2);
  transition:0.22s ease-in-out;
  overflow:hidden;
}

.post-card:hover{
  transform:translateY(-3px);
  box-shadow:var(--shadow);
  background:#fbfdff;
}

.post-card::before{
  content:"";
  position:absolute;
  left:0;
  top:1rem;
  bottom:1rem;
  width:5px;
  border-radius:999px;
  background:linear-gradient(180deg,var(--blue),var(--isu));
}

.post-card.featured::before{
  background:var(--isu);
}

.post-meta{
  display:flex;
  flex-wrap:wrap;
  gap:0.55rem;
  align-items:center;
  margin-bottom:0.65rem;
}

.tag{
  display:inline-flex;
  padding:0.25rem 0.58rem;
  border-radius:999px;
  font-size:0.78rem;
  font-weight:900;
  background:#f3f8ff;
  border:1px solid rgba(26,115,232,0.18);
  color:var(--blue);
}

.tag.red{
  background:rgba(220,20,60,0.08);
  border:1px solid rgba(220,20,60,0.25);
  color:var(--isu);
}

.tag.green{
  background:rgba(26,127,61,0.08);
  border:1px solid rgba(26,127,61,0.25);
  color:var(--green);
}

.date{
  color:var(--muted);
  font-size:0.9rem;
  font-weight:700;
}

.post-title{
  margin:0 0 0.45rem 0;
  font-size:1.05rem;
  font-weight:950;
  line-height:1.38;
}

.post-title a{
  color:var(--text);
  text-decoration:none;
}

.post-title a:hover{
  color:var(--blue);
  text-decoration:none;
}

.post-desc{
  margin:0;
  color:#202124;
  line-height:1.55;
  font-size:0.94rem;
}

.post-actions{
  display:flex;
  flex-wrap:wrap;
  gap:0.55rem;
  margin-top:0.8rem;
}

.post-link{
  display:inline-flex;
  align-items:center;
  padding:0.36rem 0.72rem;
  border-radius:999px;
  background:#f3f8ff;
  border:1px solid rgba(26,115,232,0.18);
  color:var(--blue) !important;
  text-decoration:none !important;
  font-size:0.84rem;
  font-weight:850;
}

.post-link:hover{
  background:#e9f3ff;
  text-decoration:none !important;
}

/* Layout */
.blog-grid{
  display:grid;
  grid-template-columns:1.25fr 0.75fr;
  gap:1.2rem;
  align-items:start;
}

.side-stack{
  display:flex;
  flex-direction:column;
  gap:1rem;
}

.side-card{
  border:1px solid rgba(26,115,232,0.16);
  border-radius:16px;
  padding:1rem;
  background:#ffffff;
  box-shadow:var(--shadow2);
  transition:0.22s ease-in-out;
}

.side-card:hover{
  transform:translateY(-2px);
  box-shadow:var(--shadow);
  background:#fbfdff;
}

.side-card h3{
  margin:0 0 0.55rem 0;
  color:var(--text);
  font-size:1.05rem;
}

.side-card p,
.side-card li{
  color:#202124;
  font-size:0.94rem;
  line-height:1.55;
}

.side-card ul{
  margin:0.3rem 0 0 1.05rem;
}

.side-links{
  display:flex;
  flex-wrap:wrap;
  gap:0.55rem;
  margin-top:0.65rem;
}

.side-links a{
  display:inline-flex;
  padding:0.34rem 0.68rem;
  border-radius:999px;
  background:#f3f8ff;
  border:1px solid rgba(26,115,232,0.18);
  color:var(--blue);
  font-weight:850;
  text-decoration:none;
  font-size:0.84rem;
}

.side-links a:hover{
  background:#e9f3ff;
  text-decoration:none;
}

/* Tag cloud */
.tag-cloud{
  display:flex;
  flex-wrap:wrap;
  gap:0.55rem;
}

/* Responsive */
@media (max-width:980px){
  .blog-grid{
    grid-template-columns:1fr;
  }
}

@media (max-width:950px){
  .impact-grid,
  .topic-grid{
    grid-template-columns:1fr 1fr;
  }
}

@media (max-width:700px){
  .blog-hero{
    padding:1.5rem 1.1rem;
  }

  .blog-hero h1{
    font-size:1.65rem;
  }

  .impact-grid,
  .topic-grid{
    grid-template-columns:1fr;
  }
}
</style>

<div class="blog-wrap">

  <div class="blog-hero">
    <div class="hero-content">
      <span class="hero-kicker">Writing · Technical Notes · Tutorials</span>

      <h1>Blog</h1>

      <p>
        Practical write-ups on hardware-aware artificial intelligence, VLSI workflows,
        static timing analysis, power analysis, machine learning tools, local LLMs,
        and engineering computation. Most posts are hosted on Medium.
      </p>

      <div class="hero-row">
        <div class="hero-badges">
          <span class="pill">
            <svg viewBox="0 0 24 24" fill="none" aria-hidden="true">
              <path d="M4 19V5a2 2 0 0 1 2-2h10a2 2 0 0 1 2 2v14" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
              <path d="M6 21h14a2 2 0 0 0 2-2v-2H6a2 2 0 0 0 0 4Z" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
              <path d="M8 7h8M8 11h8" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
            </svg>
            Medium Articles
          </span>

          <span class="pill red">
            <svg viewBox="0 0 24 24" fill="none" aria-hidden="true">
              <path d="M12 2l3 7h7l-5.5 4.2L18.5 21 12 16.9 5.5 21l2-7.8L2 9h7l3-7Z" stroke="currentColor" stroke-width="2" stroke-linejoin="round"/>
            </svg>
            VLSI / AI Tools
          </span>

          <span class="pill green">Tutorials and Workflows</span>
        </div>

        <div class="hero-cta">
          <a class="cta primary" href="https://medium.com/@srsapireddy" target="_blank" rel="noopener">Visit Medium</a>
          <a class="cta" href="https://srsapireddy.medium.com/" target="_blank" rel="noopener">Latest Posts</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sliding-bar">
    <div class="slide-track">
      <div class="slide-item"><span>●</span> Local LLMs</div>
      <div class="slide-item"><span>●</span> NVIDIA GPU Setup</div>
      <div class="slide-item"><span>●</span> Static Timing Analysis</div>
      <div class="slide-item"><span>●</span> OpenSTA</div>
      <div class="slide-item"><span>●</span> Yosys</div>
      <div class="slide-item"><span>●</span> Docker Workflows</div>
      <div class="slide-item"><span>●</span> Verilog Simulation</div>
      <div class="slide-item"><span>●</span> AI Project PoC</div>

      <div class="slide-item"><span>●</span> Local LLMs</div>
      <div class="slide-item"><span>●</span> NVIDIA GPU Setup</div>
      <div class="slide-item"><span>●</span> Static Timing Analysis</div>
      <div class="slide-item"><span>●</span> OpenSTA</div>
      <div class="slide-item"><span>●</span> Yosys</div>
      <div class="slide-item"><span>●</span> Docker Workflows</div>
      <div class="slide-item"><span>●</span> Verilog Simulation</div>
      <div class="slide-item"><span>●</span> AI Project PoC</div>
    </div>
  </div>

  <div class="impact-grid">
    <div class="impact-card">
      <div class="impact-number">LLM</div>
      <div class="impact-label">Local AI Tools</div>
      <div class="impact-sub">Ollama and local model workflows</div>
    </div>

    <div class="impact-card">
      <div class="impact-number">VLSI</div>
      <div class="impact-label">EDA Workflows</div>
      <div class="impact-sub">OpenSTA, Yosys, Icarus, Docker</div>
    </div>

    <div class="impact-card">
      <div class="impact-number">GPU</div>
      <div class="impact-label">Deep Learning Setup</div>
      <div class="impact-sub">CUDA and NVIDIA development</div>
    </div>

    <div class="impact-card">
      <div class="impact-number">AI</div>
      <div class="impact-label">Project Strategy</div>
      <div class="impact-sub">PoC, transformers, ML workflows</div>
    </div>
  </div>

  <div class="topic-grid">
    <div class="topic-card">
      <div class="topic-icon">⚙️</div>
      <h3>VLSI and EDA Tools</h3>
      <p>
        Tutorials on timing analysis, power analysis, synthesis, Docker-based EDA setups, and Verilog simulation.
      </p>
    </div>

    <div class="topic-card">
      <div class="topic-icon">🧠</div>
      <h3>AI and Deep Learning</h3>
      <p>
        Practical guides on local LLMs, GPU configuration, transformers, and machine learning project workflows.
      </p>
    </div>

    <div class="topic-card">
      <div class="topic-icon">📝</div>
      <h3>Practical Technical Notes</h3>
      <p>
        Short, implementation-oriented posts designed to help students and researchers reproduce technical workflows.
      </p>
    </div>
  </div>

  <div class="blog-grid">

    <div class="section">
      <h2>📚 Blog Posts</h2>
      <div class="divider"></div>

      <div class="blog-tabs">
        <button class="tab-button active" onclick="openBlogTab(event, 'featured-tab')">Featured Posts</button>
        <button class="tab-button" onclick="openBlogTab(event, 'all-tab')">All Posts</button>
        <button class="tab-button" onclick="openBlogTab(event, 'vlsi-tab')">VLSI / EDA</button>
        <button class="tab-button" onclick="openBlogTab(event, 'ai-tab')">AI / ML</button>
      </div>

      <div id="featured-tab" class="tab-panel active">
        <div class="post-list">

          <div class="post-card featured">
            <div class="post-meta">
              <span class="tag red">LLMs</span>
              <span class="date">April 23, 2025</span>
            </div>
            <h3 class="post-title">
              <a href="https://srsapireddy.medium.com/run-large-language-models-in-minutes-on-windows-using-ollama-8ba98d74fdcd" target="_blank" rel="noopener">
                Run LLMs on Windows Using Ollama
              </a>
            </h3>
            <p class="post-desc">
              Run ChatGPT-style models locally on Windows using Ollama with no cloud dependency.
            </p>
            <div class="post-actions">
              <a class="post-link" href="https://srsapireddy.medium.com/run-large-language-models-in-minutes-on-windows-using-ollama-8ba98d74fdcd" target="_blank" rel="noopener">Read on Medium</a>
            </div>
          </div>

          <div class="post-card featured">
            <div class="post-meta">
              <span class="tag red">CUDA</span>
              <span class="date">January 2, 2025</span>
            </div>
            <h3 class="post-title">
              <a href="https://srsapireddy.medium.com/setting-up-an-nvidia-gpu-for-deep-learning-59bff57b9bd9" target="_blank" rel="noopener">
                Setting Up an NVIDIA GPU for Deep Learning
              </a>
            </h3>
            <p class="post-desc">
              Complete guide to installing CUDA/cuDNN and frameworks for deep learning workflows.
            </p>
            <div class="post-actions">
              <a class="post-link" href="https://srsapireddy.medium.com/setting-up-an-nvidia-gpu-for-deep-learning-59bff57b9bd9" target="_blank" rel="noopener">Read on Medium</a>
            </div>
          </div>

          <div class="post-card featured">
            <div class="post-meta">
              <span class="tag red">STA</span>
              <span class="date">September 8, 2024</span>
            </div>
            <h3 class="post-title">
              <a href="https://srsapireddy.medium.com/understanding-delay-calculation-and-static-timing-analysis-using-opensta-a-comprehensive-tutorial-cf01feaa6170" target="_blank" rel="noopener">
                Delay Calculation and Static Timing Analysis Using OpenSTA
              </a>
            </h3>
            <p class="post-desc">
              STA theory and practical reporting workflows using OpenSTA for chip design.
            </p>
            <div class="post-actions">
              <a class="post-link" href="https://srsapireddy.medium.com/understanding-delay-calculation-and-static-timing-analysis-using-opensta-a-comprehensive-tutorial-cf01feaa6170" target="_blank" rel="noopener">Read on Medium</a>
            </div>
          </div>

        </div>
      </div>

      <div id="all-tab" class="tab-panel">
        <div class="post-list">

          <div class="post-card">
            <div class="post-meta">
              <span class="tag red">LLMs</span>
              <span class="date">April 23, 2025</span>
            </div>
            <h3 class="post-title">
              <a href="https://srsapireddy.medium.com/run-large-language-models-in-minutes-on-windows-using-ollama-8ba98d74fdcd" target="_blank" rel="noopener">Run LLMs on Windows Using Ollama</a>
            </h3>
            <p class="post-desc">Run ChatGPT-style models locally on Windows using Ollama.</p>
            <div class="post-actions">
              <a class="post-link" href="https://srsapireddy.medium.com/run-large-language-models-in-minutes-on-windows-using-ollama-8ba98d74fdcd" target="_blank" rel="noopener">Read on Medium</a>
            </div>
          </div>

          <div class="post-card">
            <div class="post-meta">
              <span class="tag red">CUDA</span>
              <span class="date">January 2, 2025</span>
            </div>
            <h3 class="post-title">
              <a href="https://srsapireddy.medium.com/setting-up-an-nvidia-gpu-for-deep-learning-59bff57b9bd9" target="_blank" rel="noopener">Setting Up an NVIDIA GPU for Deep Learning</a>
            </h3>
            <p class="post-desc">CUDA/cuDNN and deep learning framework setup for GPU workflows.</p>
            <div class="post-actions">
              <a class="post-link" href="https://srsapireddy.medium.com/setting-up-an-nvidia-gpu-for-deep-learning-59bff57b9bd9" target="_blank" rel="noopener">Read on Medium</a>
            </div>
          </div>

          <div class="post-card">
            <div class="post-meta">
              <span class="tag">AI Tools</span>
              <span class="date">December 22, 2024</span>
            </div>
            <h3 class="post-title">
              <a href="https://srsapireddy.medium.com/how-to-create-a-proof-of-concept-poc-for-your-ai-project-as-a-manager-fc0e64751bde" target="_blank" rel="noopener">Create an AI PoC as a Manager</a>
            </h3>
            <p class="post-desc">Strategy and execution steps for building AI proof-of-concepts aligned to business goals.</p>
            <div class="post-actions">
              <a class="post-link" href="https://srsapireddy.medium.com/how-to-create-a-proof-of-concept-poc-for-your-ai-project-as-a-manager-fc0e64751bde" target="_blank" rel="noopener">Read on Medium</a>
            </div>
          </div>

          <div class="post-card">
            <div class="post-meta">
              <span class="tag">Transformers</span>
              <span class="date">December 22, 2024</span>
            </div>
            <h3 class="post-title">
              <a href="https://srsapireddy.medium.com/understanding-self-attention-and-multi-head-attention-in-transformers-05463bb4f095" target="_blank" rel="noopener">Understanding Self-Attention in Transformers</a>
            </h3>
            <p class="post-desc">A clean explanation of attention and multi-head attention for quick intuition.</p>
            <div class="post-actions">
              <a class="post-link" href="https://srsapireddy.medium.com/understanding-self-attention-and-multi-head-attention-in-transformers-05463bb4f095" target="_blank" rel="noopener">Read on Medium</a>
            </div>
          </div>

          <div class="post-card">
            <div class="post-meta">
              <span class="tag red">STA</span>
              <span class="date">September 8, 2024</span>
            </div>
            <h3 class="post-title">
              <a href="https://srsapireddy.medium.com/understanding-delay-calculation-and-static-timing-analysis-using-opensta-a-comprehensive-tutorial-cf01feaa6170" target="_blank" rel="noopener">Delay Calculation and Static Timing Analysis Using OpenSTA</a>
            </h3>
            <p class="post-desc">STA theory and practical reporting workflows using OpenSTA.</p>
            <div class="post-actions">
              <a class="post-link" href="https://srsapireddy.medium.com/understanding-delay-calculation-and-static-timing-analysis-using-opensta-a-comprehensive-tutorial-cf01feaa6170" target="_blank" rel="noopener">Read on Medium</a>
            </div>
          </div>

          <div class="post-card">
            <div class="post-meta">
              <span class="tag">OpenSTA</span>
              <span class="date">September 15, 2024</span>
            </div>
            <h3 class="post-title">
              <a href="https://srsapireddy.medium.com/hands-on-power-analysis-with-opensta-a-comprehensive-guide-18c3350ef6ea" target="_blank" rel="noopener">Hands-On Power Analysis with OpenSTA</a>
            </h3>
            <p class="post-desc">Power and delay analysis workflow with practical reporting structure.</p>
            <div class="post-actions">
              <a class="post-link" href="https://srsapireddy.medium.com/hands-on-power-analysis-with-opensta-a-comprehensive-guide-18c3350ef6ea" target="_blank" rel="noopener">Read on Medium</a>
            </div>
          </div>

          <div class="post-card">
            <div class="post-meta">
              <span class="tag">Docker</span>
              <span class="date">September 1, 2024</span>
            </div>
            <h3 class="post-title">
              <a href="https://srsapireddy.medium.com/a-step-by-step-guide-to-installing-and-running-opensta-in-a-docker-environment-9a2d4b2fbfcd" target="_blank" rel="noopener">Running OpenSTA in Docker</a>
            </h3>
            <p class="post-desc">Spin up OpenSTA quickly via Docker for repeatable timing runs.</p>
            <div class="post-actions">
              <a class="post-link" href="https://srsapireddy.medium.com/a-step-by-step-guide-to-installing-and-running-opensta-in-a-docker-environment-9a2d4b2fbfcd" target="_blank" rel="noopener">Read on Medium</a>
            </div>
          </div>

          <div class="post-card">
            <div class="post-meta">
              <span class="tag">Yosys</span>
              <span class="date">August 21, 2024</span>
            </div>
            <h3 class="post-title">
              <a href="https://srsapireddy.medium.com/enhancing-vlsi-designs-with-logic-optimization-using-yosys-8g0h2i3j4k5l" target="_blank" rel="noopener">Logic Optimization with Yosys</a>
            </h3>
            <p class="post-desc">Use Yosys passes to optimize RTL and improve synthesis quality.</p>
            <div class="post-actions">
              <a class="post-link" href="https://srsapireddy.medium.com/enhancing-vlsi-designs-with-logic-optimization-using-yosys-8g0h2i3j4k5l" target="_blank" rel="noopener">Read on Medium</a>
            </div>
          </div>

          <div class="post-card">
            <div class="post-meta">
              <span class="tag">Synthesis</span>
              <span class="date">August 11, 2024</span>
            </div>
            <h3 class="post-title">
              <a href="https://srsapireddy.medium.com/enhancing-vlsi-designs-with-logic-optimization-using-yosys-83502d9f7cf5" target="_blank" rel="noopener">Logic Synthesis Tutorial with Yosys</a>
            </h3>
            <p class="post-desc">Start-to-finish introduction to synthesis using an open-source flow.</p>
            <div class="post-actions">
              <a class="post-link" href="https://srsapireddy.medium.com/enhancing-vlsi-designs-with-logic-optimization-using-yosys-83502d9f7cf5" target="_blank" rel="noopener">Read on Medium</a>
            </div>
          </div>

          <div class="post-card">
            <div class="post-meta">
              <span class="tag">Verilog</span>
              <span class="date">August 9, 2024</span>
            </div>
            <h3 class="post-title">
              <a href="https://medium.com/@srsapireddy/simulation-based-verification-using-icarus-designing-and-simulating-a-4-bit-synchronous-counter-e3633dbfd76a" target="_blank" rel="noopener">Verilog Simulation with Icarus</a>
            </h3>
            <p class="post-desc">Design and verify a synchronous counter using Icarus Verilog and waveforms.</p>
            <div class="post-actions">
              <a class="post-link" href="https://medium.com/@srsapireddy/simulation-based-verification-using-icarus-designing-and-simulating-a-4-bit-synchronous-counter-e3633dbfd76a" target="_blank" rel="noopener">Read on Medium</a>
            </div>
          </div>

        </div>
      </div>

      <div id="vlsi-tab" class="tab-panel">
        <div class="post-list">

          <div class="post-card">
            <div class="post-meta">
              <span class="tag red">STA</span>
              <span class="date">September 8, 2024</span>
            </div>
            <h3 class="post-title">
              <a href="https://srsapireddy.medium.com/understanding-delay-calculation-and-static-timing-analysis-using-opensta-a-comprehensive-tutorial-cf01feaa6170" target="_blank" rel="noopener">Delay Calculation and Static Timing Analysis Using OpenSTA</a>
            </h3>
            <p class="post-desc">Static timing analysis theory and reporting workflow using OpenSTA.</p>
            <div class="post-actions">
              <a class="post-link" href="https://srsapireddy.medium.com/understanding-delay-calculation-and-static-timing-analysis-using-opensta-a-comprehensive-tutorial-cf01feaa6170" target="_blank" rel="noopener">Read on Medium</a>
            </div>
          </div>

          <div class="post-card">
            <div class="post-meta">
              <span class="tag">OpenSTA</span>
              <span class="date">September 15, 2024</span>
            </div>
            <h3 class="post-title">
              <a href="https://srsapireddy.medium.com/hands-on-power-analysis-with-opensta-a-comprehensive-guide-18c3350ef6ea" target="_blank" rel="noopener">Hands-On Power Analysis with OpenSTA</a>
            </h3>
            <p class="post-desc">Practical OpenSTA-based power and delay analysis workflow.</p>
            <div class="post-actions">
              <a class="post-link" href="https://srsapireddy.medium.com/hands-on-power-analysis-with-opensta-a-comprehensive-guide-18c3350ef6ea" target="_blank" rel="noopener">Read on Medium</a>
            </div>
          </div>

          <div class="post-card">
            <div class="post-meta">
              <span class="tag">Docker</span>
              <span class="date">September 1, 2024</span>
            </div>
            <h3 class="post-title">
              <a href="https://srsapireddy.medium.com/a-step-by-step-guide-to-installing-and-running-opensta-in-a-docker-environment-9a2d4b2fbfcd" target="_blank" rel="noopener">Running OpenSTA in Docker</a>
            </h3>
            <p class="post-desc">Docker-based OpenSTA setup for reproducible timing analysis runs.</p>
            <div class="post-actions">
              <a class="post-link" href="https://srsapireddy.medium.com/a-step-by-step-guide-to-installing-and-running-opensta-in-a-docker-environment-9a2d4b2fbfcd" target="_blank" rel="noopener">Read on Medium</a>
            </div>
          </div>

          <div class="post-card">
            <div class="post-meta">
              <span class="tag">Yosys</span>
              <span class="date">August 21, 2024</span>
            </div>
            <h3 class="post-title">
              <a href="https://srsapireddy.medium.com/enhancing-vlsi-designs-with-logic-optimization-using-yosys-8g0h2i3j4k5l" target="_blank" rel="noopener">Logic Optimization with Yosys</a>
            </h3>
            <p class="post-desc">Yosys optimization passes for improving RTL quality before synthesis.</p>
            <div class="post-actions">
              <a class="post-link" href="https://srsapireddy.medium.com/enhancing-vlsi-designs-with-logic-optimization-using-yosys-8g0h2i3j4k5l" target="_blank" rel="noopener">Read on Medium</a>
            </div>
          </div>

          <div class="post-card">
            <div class="post-meta">
              <span class="tag">Synthesis</span>
              <span class="date">August 11, 2024</span>
            </div>
            <h3 class="post-title">
              <a href="https://srsapireddy.medium.com/enhancing-vlsi-designs-with-logic-optimization-using-yosys-83502d9f7cf5" target="_blank" rel="noopener">Logic Synthesis Tutorial with Yosys</a>
            </h3>
            <p class="post-desc">Open-source synthesis workflow using Yosys.</p>
            <div class="post-actions">
              <a class="post-link" href="https://srsapireddy.medium.com/enhancing-vlsi-designs-with-logic-optimization-using-yosys-83502d9f7cf5" target="_blank" rel="noopener">Read on Medium</a>
            </div>
          </div>

          <div class="post-card">
            <div class="post-meta">
              <span class="tag">Verilog</span>
              <span class="date">August 9, 2024</span>
            </div>
            <h3 class="post-title">
              <a href="https://medium.com/@srsapireddy/simulation-based-verification-using-icarus-designing-and-simulating-a-4-bit-synchronous-counter-e3633dbfd76a" target="_blank" rel="noopener">Verilog Simulation with Icarus</a>
            </h3>
            <p class="post-desc">Counter design and waveform-based verification using Icarus Verilog.</p>
            <div class="post-actions">
              <a class="post-link" href="https://medium.com/@srsapireddy/simulation-based-verification-using-icarus-designing-and-simulating-a-4-bit-synchronous-counter-e3633dbfd76a" target="_blank" rel="noopener">Read on Medium</a>
            </div>
          </div>

        </div>
      </div>

      <div id="ai-tab" class="tab-panel">
        <div class="post-list">

          <div class="post-card">
            <div class="post-meta">
              <span class="tag red">LLMs</span>
              <span class="date">April 23, 2025</span>
            </div>
            <h3 class="post-title">
              <a href="https://srsapireddy.medium.com/run-large-language-models-in-minutes-on-windows-using-ollama-8ba98d74fdcd" target="_blank" rel="noopener">Run LLMs on Windows Using Ollama</a>
            </h3>
            <p class="post-desc">Local large-language-model workflow using Ollama on Windows.</p>
            <div class="post-actions">
              <a class="post-link" href="https://srsapireddy.medium.com/run-large-language-models-in-minutes-on-windows-using-ollama-8ba98d74fdcd" target="_blank" rel="noopener">Read on Medium</a>
            </div>
          </div>

          <div class="post-card">
            <div class="post-meta">
              <span class="tag red">CUDA</span>
              <span class="date">January 2, 2025</span>
            </div>
            <h3 class="post-title">
              <a href="https://srsapireddy.medium.com/setting-up-an-nvidia-gpu-for-deep-learning-59bff57b9bd9" target="_blank" rel="noopener">Setting Up an NVIDIA GPU for Deep Learning</a>
            </h3>
            <p class="post-desc">CUDA, cuDNN, and framework setup for NVIDIA-based deep learning.</p>
            <div class="post-actions">
              <a class="post-link" href="https://srsapireddy.medium.com/setting-up-an-nvidia-gpu-for-deep-learning-59bff57b9bd9" target="_blank" rel="noopener">Read on Medium</a>
            </div>
          </div>

          <div class="post-card">
            <div class="post-meta">
              <span class="tag">AI Tools</span>
              <span class="date">December 22, 2024</span>
            </div>
            <h3 class="post-title">
              <a href="https://srsapireddy.medium.com/how-to-create-a-proof-of-concept-poc-for-your-ai-project-as-a-manager-fc0e64751bde" target="_blank" rel="noopener">Create an AI PoC as a Manager</a>
            </h3>
            <p class="post-desc">Execution steps for planning and validating AI proof-of-concept projects.</p>
            <div class="post-actions">
              <a class="post-link" href="https://srsapireddy.medium.com/how-to-create-a-proof-of-concept-poc-for-your-ai-project-as-a-manager-fc0e64751bde" target="_blank" rel="noopener">Read on Medium</a>
            </div>
          </div>

          <div class="post-card">
            <div class="post-meta">
              <span class="tag">Transformers</span>
              <span class="date">December 22, 2024</span>
            </div>
            <h3 class="post-title">
              <a href="https://srsapireddy.medium.com/understanding-self-attention-and-multi-head-attention-in-transformers-05463bb4f095" target="_blank" rel="noopener">Understanding Self-Attention in Transformers</a>
            </h3>
            <p class="post-desc">A quick, intuitive explanation of self-attention and multi-head attention.</p>
            <div class="post-actions">
              <a class="post-link" href="https://srsapireddy.medium.com/understanding-self-attention-and-multi-head-attention-in-transformers-05463bb4f095" target="_blank" rel="noopener">Read on Medium</a>
            </div>
          </div>

        </div>
      </div>
    </div>

    <div class="side-stack">

      <div class="side-card">
        <h3>🌐 Writing Hub</h3>
        <p>
          All long-form technical articles are currently hosted on Medium.
        </p>
        <div class="side-links">
          <a href="https://medium.com/@srsapireddy" target="_blank" rel="noopener">Medium</a>
          <a href="https://srsapireddy.medium.com/" target="_blank" rel="noopener">Latest</a>
        </div>
      </div>

      <div class="side-card">
        <h3>🏷️ Main Topics</h3>
        <ul>
          <li>Hardware-aware AI and efficient inference</li>
          <li>VLSI timing, power, synthesis, and verification</li>
          <li>EDA workflows with OpenSTA, Yosys, Docker, and Icarus</li>
          <li>AI tools, local LLMs, CUDA, and transformer concepts</li>
        </ul>
      </div>

      <div class="side-card">
        <h3>📌 Related Pages</h3>
        <div class="side-links">
          <a href="/publications/">Publications</a>
          <a href="/insys-lab/">INSys Lab</a>
          <a href="/teaching/">Teaching</a>
          <a href="/resume/">Resume</a>
        </div>
      </div>

      <div class="side-card">
        <h3>🧭 Blog Themes</h3>
        <div class="tag-cloud">
          <span class="tag">OpenSTA</span>
          <span class="tag">Yosys</span>
          <span class="tag">Docker</span>
          <span class="tag">Verilog</span>
          <span class="tag">CUDA</span>
          <span class="tag">LLMs</span>
          <span class="tag">Transformers</span>
          <span class="tag">AI PoC</span>
        </div>
      </div>

    </div>

  </div>

</div>

<script>
function openBlogTab(event, panelId) {
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
