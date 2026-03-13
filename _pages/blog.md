---
title: "Blog"
layout: single
permalink: /blog/
author_profile: true
---

<style>
:root{
  --blue:#1a73e8;
  --red:#DC143C;
  --bg:#ffffff;
  --soft:#f7fbff;
  --soft2:#fff6f7;
  --text:#121212;
  --muted:#5a6573;
  --border:#d7e6fb;
  --shadow: 0 10px 24px rgba(0,0,0,0.06);
  --radius: 14px;
}

/* Page hero */
.blog-hero{
  border: 2px solid var(--blue);
  background: linear-gradient(135deg, #ffffff 0%, #f2f8ff 55%, #ffffff 100%);
  border-radius: 18px;
  padding: 1.6rem 1.6rem 1.2rem 1.6rem;
  box-shadow: var(--shadow);
  margin-bottom: 1.4rem;
}

.blog-hero h2{
  margin: 0 0 0.4rem 0;
  color: var(--blue);
  font-size: 1.55rem;
  letter-spacing: 0.2px;
}

.blog-hero p{
  margin: 0.25rem 0 0.9rem 0;
  color: var(--muted);
  line-height: 1.55;
}

.hero-row{
  display:flex;
  gap: 1rem;
  flex-wrap: wrap;
  align-items: center;
  justify-content: space-between;
}

.hero-badges{
  display:flex;
  gap: 0.5rem;
  flex-wrap: wrap;
}

.pill{
  display:inline-flex;
  align-items:center;
  gap: 0.45rem;
  padding: 0.35rem 0.7rem;
  border-radius: 999px;
  font-weight: 700;
  font-size: 0.86rem;
  border: 1px solid var(--border);
  background: #ffffff;
  color: var(--blue);
}

.pill.red{
  border-color: #ffd0d8;
  color: var(--red);
}

.pill svg{
  width: 16px;
  height: 16px;
  opacity: 0.95;
}

.hero-cta{
  display:flex;
  gap: 0.6rem;
  flex-wrap: wrap;
}

.cta{
  display:inline-block;
  padding: 0.55rem 0.9rem;
  border-radius: 12px;
  font-weight: 800;
  text-decoration:none;
  border: 2px solid var(--blue);
  color: var(--blue);
  background: #ffffff;
  transition: 0.2s ease;
}

.cta:hover{
  transform: translateY(-1px);
  background: #eaf3ff;
}

.cta.primary{
  background: var(--blue);
  color: #fff;
}

.cta.primary:hover{
  background: #135fcd;
}

/* Layout grid */
.blog-grid{
  display:grid;
  grid-template-columns: 1.25fr 0.75fr;
  gap: 1.2rem;
}

@media (max-width: 980px){
  .blog-grid{ grid-template-columns: 1fr; }
}

/* Card styles */
.panel{
  background: var(--bg);
  border: 2px solid var(--blue);
  border-radius: var(--radius);
  box-shadow: var(--shadow);
  overflow: hidden;
}

.panel-header{
  padding: 1rem 1.1rem 0.85rem 1.1rem;
  border-bottom: 1px solid #e8f2ff;
  background: linear-gradient(180deg, #ffffff 0%, #f6fbff 100%);
}

.panel-header h3{
  margin: 0;
  font-size: 1.15rem;
  color: var(--blue);
}

.panel-header p{
  margin: 0.25rem 0 0 0;
  color: var(--muted);
  font-size: 0.95rem;
}

.panel-body{
  padding: 0.9rem 1.1rem 1.1rem 1.1rem;
}

/* Featured block */
.featured{
  border: 2px solid var(--red);
}

.featured .panel-header{
  border-bottom: 1px solid #ffe1e6;
  background: linear-gradient(180deg, #ffffff 0%, #fff5f7 100%);
}

.featured .panel-header h3{ color: var(--red); }

/* Post list */
.post-list{
  display:flex;
  flex-direction: column;
  gap: 0.75rem;
  margin-top: 0.2rem;
}

.post{
  border: 1px solid #e3efff;
  background: #ffffff;
  border-radius: 12px;
  padding: 0.85rem 0.9rem;
  transition: 0.2s ease;
}

.post:hover{
  background: #f3f9ff;
  transform: translateY(-1px);
  box-shadow: 0 8px 18px rgba(26,115,232,0.08);
}

.post-title{
  margin: 0 0 0.25rem 0;
  font-size: 1.02rem;
  font-weight: 800;
  line-height: 1.3;
}

.post-title a{
  color: var(--blue);
  text-decoration: none;
}

.post-title a:hover{ text-decoration: underline; }

.post-meta{
  display:flex;
  gap: 0.5rem;
  flex-wrap: wrap;
  align-items:center;
  margin-bottom: 0.35rem;
  color: var(--muted);
  font-size: 0.9rem;
}

.tag{
  display:inline-block;
  padding: 0.18rem 0.5rem;
  border-radius: 999px;
  background: #eef5ff;
  border: 1px solid #d7e6fb;
  color: var(--blue);
  font-weight: 800;
  font-size: 0.78rem;
}

.tag.red{
  background: #fff0f2;
  border-color: #ffd0d8;
  color: var(--red);
}

.post-desc{
  margin: 0;
  color: #2b2f36;
  line-height: 1.5;
  font-size: 0.96rem;
}

/* Sidebar cards */
.side-card{
  border: 1px solid #e3efff;
  border-radius: 14px;
  padding: 0.95rem;
  background: #ffffff;
}

.side-card h4{
  margin: 0 0 0.5rem 0;
  color: var(--blue);
  font-size: 1.02rem;
}

.side-card p, .side-card li{
  color: var(--muted);
  font-size: 0.95rem;
  line-height: 1.5;
}

.side-card ul{
  margin: 0.3rem 0 0 1.05rem;
}

.side-link{
  display:flex;
  gap: 0.6rem;
  flex-wrap: wrap;
  margin-top: 0.6rem;
}

.side-link a{
  text-decoration:none;
  font-weight: 900;
  color: var(--blue);
  border-bottom: 2px solid transparent;
}

.side-link a:hover{
  border-bottom-color: var(--blue);
}

hr.soft{
  border: none;
  border-top: 1px dashed #d7e6fb;
  margin: 0.9rem 0;
}

/* Small helper line */
.note{
  margin-top: 0.7rem;
  font-size: 0.92rem;
  color: var(--muted);
}
</style>

<div class="blog-hero">
  <div class="hero-row">
    <div>
      <h2>Writing & Technical Notes</h2>
      <p>
        Short, practical write-ups on hardware-aware AI, VLSI workflows, timing/power analysis, and signal processing.
        All posts are hosted on Medium for now.
      </p>

      <div class="hero-badges">
        <span class="pill">
          <!-- icon -->
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
          Featured: VLSI / AI Tools
        </span>
      </div>
    </div>

    <div class="hero-cta">
      <a class="cta primary" href="https://medium.com/@srsapireddy" target="_blank" rel="noopener">Visit Medium</a>
      <a class="cta" href="https://srsapireddy.medium.com/" target="_blank" rel="noopener">Latest Posts</a>
    </div>
  </div>

<div class="blog-grid">

  <!-- LEFT: Posts -->
  <div>

    <div class="panel featured">
      <div class="panel-header">
        <h3>Featured Posts</h3>
        <p>High-signal tutorials and practical workflows.</p>
      </div>
      <div class="panel-body">
        <div class="post-list">

          <div class="post">
            <div class="post-meta">
              <span class="tag red">LLMs</span>
              <span>April 23, 2025</span>
            </div>
            <h4 class="post-title">
              <a href="https://srsapireddy.medium.com/run-large-language-models-in-minutes-on-windows-using-ollama-8ba98d74fdcd" target="_blank" rel="noopener">
                Run LLMs on Windows Using Ollama
              </a>
            </h4>
            <p class="post-desc">Run ChatGPT-style models locally on Windows using Ollama—no cloud dependency.</p>
          </div>

          <div class="post">
            <div class="post-meta">
              <span class="tag red">CUDA</span>
              <span>January 2, 2025</span>
            </div>
            <h4 class="post-title">
              <a href="https://srsapireddy.medium.com/setting-up-an-nvidia-gpu-for-deep-learning-59bff57b9bd9" target="_blank" rel="noopener">
                Setting Up an NVIDIA GPU for Deep Learning
              </a>
            </h4>
            <p class="post-desc">Complete guide to installing CUDA/cuDNN and frameworks for deep learning workflows.</p>
          </div>

          <div class="post">
            <div class="post-meta">
              <span class="tag red">STA</span>
              <span>September 8, 2024</span>
            </div>
            <h4 class="post-title">
              <a href="https://srsapireddy.medium.com/understanding-delay-calculation-and-static-timing-analysis-using-opensta-a-comprehensive-tutorial-cf01feaa6170" target="_blank" rel="noopener">
                Delay Calculation & Static Timing Analysis (OpenSTA)
              </a>
            </h4>
            <p class="post-desc">STA theory + real reporting workflows using OpenSTA for chip design.</p>
          </div>

        </div>
      </div>
    </div>

    <div class="panel" style="margin-top:1.2rem;">
      <div class="panel-header">
        <h3>All Posts</h3>
        <p>Chronological list of Medium articles.</p>
      </div>
      <div class="panel-body">
        <div class="post-list">

          <div class="post">
            <div class="post-meta">
              <span class="tag">AI Tools</span>
              <span>December 22, 2024</span>
            </div>
            <h4 class="post-title">
              <a href="https://srsapireddy.medium.com/how-to-create-a-proof-of-concept-poc-for-your-ai-project-as-a-manager-fc0e64751bde" target="_blank" rel="noopener">
                Create an AI PoC as a Manager
              </a>
            </h4>
            <p class="post-desc">Strategy + execution steps for building proof-of-concepts aligned to business goals.</p>
          </div>

          <div class="post">
            <div class="post-meta">
              <span class="tag">Transformers</span>
              <span>December 22, 2024</span>
            </div>
            <h4 class="post-title">
              <a href="https://srsapireddy.medium.com/understanding-self-attention-and-multi-head-attention-in-transformers-05463bb4f095" target="_blank" rel="noopener">
                Understanding Self-Attention in Transformers
              </a>
            </h4>
            <p class="post-desc">A clean explanation of attention and multi-head attention for quick intuition.</p>
          </div>

          <div class="post">
            <div class="post-meta">
              <span class="tag">OpenSTA</span>
              <span>September 15, 2024</span>
            </div>
            <h4 class="post-title">
              <a href="https://srsapireddy.medium.com/hands-on-power-analysis-with-opensta-a-comprehensive-guide-18c3350ef6ea" target="_blank" rel="noopener">
                Hands-On Power Analysis with OpenSTA
              </a>
            </h4>
            <p class="post-desc">Power + delay analysis workflow with practical examples and reporting structure.</p>
          </div>

          <div class="post">
            <div class="post-meta">
              <span class="tag">Docker</span>
              <span>September 1, 2024</span>
            </div>
            <h4 class="post-title">
              <a href="https://srsapireddy.medium.com/a-step-by-step-guide-to-installing-and-running-opensta-in-a-docker-environment-9a2d4b2fbfcd" target="_blank" rel="noopener">
                Running OpenSTA in Docker
              </a>
            </h4>
            <p class="post-desc">Spin up OpenSTA quickly via Docker for repeatable, clean timing runs.</p>
          </div>

          <div class="post">
            <div class="post-meta">
              <span class="tag">Yosys</span>
              <span>August 21, 2024</span>
            </div>
            <h4 class="post-title">
              <a href="https://srsapireddy.medium.com/enhancing-vlsi-designs-with-logic-optimization-using-yosys-8g0h2i3j4k5l" target="_blank" rel="noopener">
                Logic Optimization with Yosys
              </a>
            </h4>
            <p class="post-desc">Use Yosys passes to optimize RTL and improve downstream synthesis quality.</p>
          </div>

          <div class="post">
            <div class="post-meta">
              <span class="tag">Synthesis</span>
              <span>August 11, 2024</span>
            </div>
            <h4 class="post-title">
              <a href="https://srsapireddy.medium.com/enhancing-vlsi-designs-with-logic-optimization-using-yosys-83502d9f7cf5" target="_blank" rel="noopener">
                Logic Synthesis Tutorial with Yosys
              </a>
            </h4>
            <p class="post-desc">Start-to-finish introduction to synthesis using an open-source flow.</p>
          </div>

          <div class="post">
            <div class="post-meta">
              <span class="tag">Verilog</span>
              <span>August 9, 2024</span>
            </div>
            <h4 class="post-title">
              <a href="https://medium.com/@srsapireddy/simulation-based-verification-using-icarus-designing-and-simulating-a-4-bit-synchronous-counter-e3633dbfd76a" target="_blank" rel="noopener">
                Verilog Simulation with Icarus
              </a>
            </h4>
            <p class="post-desc">Design + verify a synchronous counter using Icarus Verilog and waveforms.</p>
          </div>

        </div>


      </div>
    </div>

  </div>

  <!-- RIGHT: Sidebar -->
  <div>
    <div class="panel">
      <div class="panel-header">
        <h3>Quick Links</h3>
        <p>Profiles and primary writing hub.</p>
      </div>
      <div class="panel-body">
        <div class="side-card">
          <h4>Medium</h4>
          <p>All long-form posts are published on Medium.</p>
          <div class="side-link">
            <a href="https://medium.com/@srsapireddy" target="_blank" rel="noopener">Open Medium →</a>
            <a href="https://srsapireddy.medium.com/" target="_blank" rel="noopener">Latest →</a>
          </div>
        </div>

        <hr class="soft">

        <div class="side-card">
          <h4>Topics</h4>
          <ul>
            <li>Hardware-aware AI and efficient inference</li>
            <li>VLSI: timing, power, synthesis, verification</li>
            <li>Signal processing and RF workflows</li>
            <li>Practical tooling (Docker, OpenSTA, Yosys)</li>
          </ul>
        </div>

  
  </div>

</div>
