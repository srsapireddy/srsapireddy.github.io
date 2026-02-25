---
title: ""
layout: single
permalink: /publications/
author_profile: true
toc: false
---

<style>
:root{
  --blue:#1a73e8;
  --blue2:#0b5bd3;
  --isu:#DC143C;
  --bg:#ffffff;
  --muted:#5f6368;
  --shadow:0 10px 30px rgba(0,0,0,0.08);
  --shadow2:0 2px 10px rgba(0,0,0,0.05);
  --radius:16px;
  --radius2:12px;
  --border:rgba(26,115,232,0.18);
}

/* Hero */
.page-hero{
  border-radius:var(--radius);
  padding:2rem 1.8rem;
  margin-bottom:1.6rem;
  background:linear-gradient(135deg,#e9f3ff 0%, #ffffff 60%);
  border:1px solid rgba(26,115,232,0.25);
  box-shadow:var(--shadow);
}
.page-hero h2{
  margin:0 0 0.35rem 0;
  font-size:1.9rem;
  line-height:1.2;
  color:#0b1f44;
}
.page-hero p{
  margin:0.55rem 0 0 0;
  color:var(--muted);
  font-size:1.05rem;
  max-width:90ch;
}

/* Buttons */
.hero-links{
  display:flex;
  flex-wrap:wrap;
  gap:0.7rem;
  margin-top:1.1rem;
}
.btn-link{
  display:inline-flex;
  align-items:center;
  gap:0.45rem;
  padding:0.55rem 0.9rem;
  border-radius:10px;
  background:var(--blue);
  color:#ffffff !important;
  text-decoration:none !important;
  font-weight:700;
  box-shadow:var(--shadow2);
  transition:0.2s ease-in-out;
}
.btn-link:hover{ background:var(--blue2); transform:translateY(-1px); }
.btn-link.secondary{
  background:#ffffff;
  color:var(--blue) !important;
  border:1px solid rgba(26,115,232,0.25);
}

/* Section Cards */
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
.section h3{
  margin-top:0;
  color:#0b1f44;
  font-size:1.15rem;
  display:flex;
  align-items:center;
  gap:0.55rem;
}
.divider{ height:1px; background:rgba(26,115,232,0.12); margin:0.3rem 0 0.9rem 0; }

/* Publication layout */
.pub-grid{
  display:grid;
  grid-template-columns:1fr;
  gap:0.85rem;
  margin-top:0.5rem;
}

/* Entry: card + cite */
.pub-entry{
  display:grid;
  grid-template-columns: 4fr 1fr;
  gap:1rem;
  align-items:stretch;
}

/* Stack on small screens */
@media (max-width: 900px){
  .pub-entry{ grid-template-columns:1fr; }
}

/* Cards */
.pub-card{
  border:1px solid rgba(26,115,232,0.22);
  border-radius:14px;
  padding:1.15rem 1.35rem;
  background:#fff;
  box-shadow:var(--shadow2);
  transition:0.25s ease-in-out;
}
.pub-card:hover{
  background:#fbfdff;
  transform:translateY(-2px);
  box-shadow:var(--shadow);
}

/* WIP (ISU red accent) */
.pub-card.wip{
  border:1px solid rgba(220,20,60,0.28);
}

/* Cite box */
.cite-box{
  display:flex;
  justify-content:center;
  align-items:center;
  min-width:120px;
  cursor:pointer;
  font-size:1rem;
  font-weight:800;
  color:var(--blue);
  border:1px solid rgba(26,115,232,0.22);
  border-radius:14px;
  background:#fff;
  box-shadow:var(--shadow2);
  transition:0.2s ease-in-out;
  position:relative;
}
.cite-box:hover{
  background:#f3f8ff;
  transform:translateY(-2px);
  box-shadow:var(--shadow);
}

/* Cite box for WIP red */
.cite-box.wip{
  color:var(--isu);
  border:1px solid rgba(220,20,60,0.28);
}
.cite-box.wip:hover{ background:#fff5f6; }

/* Inline typography */
.pub-card strong{ font-weight:800; color:#0b1f44; }
.pub-card em{ color:#202124; }
.pub-card a{ color:var(--blue); font-weight:700; text-decoration:none; }
.pub-card a:hover{ text-decoration:underline; }

/* Status pills */
.status{
  display:inline-block;
  font-size:0.85rem;
  font-weight:800;
  padding:0.22rem 0.55rem;
  border-radius:999px;
  margin-left:0.5rem;
}
.status.accepted{ color:#1a7f3d; background:#dcfce7; }
.status.review{ color:#c67c00; background:#fff6e6; }
.status.pending{ color:#555; background:#f0f0f0; }
.status.published{ color:#0a539e; background:#e5f1ff; }

.status-badge{
  display:inline-block;
  padding:0.22rem 0.55rem;
  border-radius:999px;
  font-weight:900;
  font-size:0.85rem;
  margin-left:0.5rem;
}
.best-paper{ background:#e6ffe6; color:#1a7f3d; }

/* WIP badge (orange) */
.wip-badge{
  display:inline-block;
  color:#fff;
  background:#fb8c00;
  border-radius:999px;
  font-size:0.85rem;
  font-weight:900;
  padding:0.22rem 0.55rem;
  margin-left:0.5rem;
}

/* Hidden citation textarea */
textarea.hidden-citation{
  position:absolute;
  left:-9999px;
}

/* Logo rows */
.logo-row{
  display:flex;
  justify-content:center;
  align-items:center;
  gap:2rem;
  margin-top:1.4rem;
  flex-wrap:wrap;
}
.logo-row img{
  height:52px;
  max-width:140px;
  transition:transform 0.25s ease;
  object-fit:contain;
  filter:saturate(1.05);
}
.logo-row img:hover{ transform:scale(1.07); }

/* Footer links */
.pub-footer{
  margin-top:2rem;
  text-align:center;
  font-size:0.95rem;
}
.pub-footer a{
  text-decoration:none;
  color:var(--blue);
  margin:0 0.9rem;
  font-weight:800;
}
.pub-footer a:hover{ text-decoration:underline; }
</style>

<script>
function copyCitation(id) {
  const citation = document.getElementById(id);
  citation.select();
  citation.setSelectionRange(0, 99999);
  navigator.clipboard.writeText(citation.value).then(() => {
    alert("Citation copied to clipboard!");
  });
}
</script>

<div class="page-hero">
  <h2>Publications</h2>
  <p>
    Peer-reviewed publications and manuscripts in progress. Each entry includes a one-click citation copy button for convenience.
  </p>
  <div class="hero-links">
    <a class="btn-link" href="https://scholar.google.com/citations?user=08fgpdIAAAAJ&hl=en" target="_blank" rel="noopener">Google Scholar</a>
    <a class="btn-link secondary" href="/insys-lab/">INSys Lab</a>
    <a class="btn-link secondary" href="/resume/">Resume</a>
  </div>
</div>

<div class="section">
  <h3>Published / Accepted</h3>
  <div class="divider"></div>

  <div class="pub-grid">

    <div class="pub-entry">
      <div class="pub-card">
        <strong>Srinivas Rahul Sapireddy</strong>, Mostafizur Rahman<br>
        <em>"On the Effectiveness of Custom Activation Functions on Long-Term Short-Term Memory”</em><br>
        <a href="https://dl.acm.org/doi/10.1145/3716368.3735217" target="_blank" rel="noopener">The 35th edition of ACM Great Lakes Symposium on VLSI (GLSVLSI)</a>, 2025, New Orleans, LA.
        <a href="https://doi.org/10.1145/3716368.3735217" target="_blank" rel="noopener">[DOI]</a>
        <span class="status published">Published</span><br>
        <small><em>Session: VLSI for Machine Learning and Artificial Intelligence | Acceptance rate: 27%</em></small><br>
        <a href="/images/PID69.pdf" target="_blank" rel="noopener" title="Download PDF">📥</a>
      </div>
      <div class="cite-box" onclick="copyCitation('citeP1')">
        📑 Cite
        <textarea id="citeP1" class="hidden-citation">Srinivas Rahul Sapireddy and Mostafizur Rahman. 2025. On the Effectiveness of Piecewise Activation Approximations for Long-Term Short-Memory Networks. In Proceedings of Great Lakes Symposium on VLSI 2025 (GLSVLSI '25), June 29, 2025, pp. 740–745. https://doi.org/10.1145/3716368.3735217</textarea>
      </div>
    </div>

    <div class="pub-entry">
      <div class="pub-card">
        <strong>Srinivas Rahul Sapireddy</strong>, Mostafizur Rahman<br>
        <em>“Re-Visiting R: Statistical Envelope Analysis for Lightweight Modulation Classification”</em><br>
        <a href="https://ieeexplore.ieee.org/document/11085271" target="_blank" rel="noopener"> IEEE International Conference on Radio Frequency Communication and Networks (RFCoN)</a>, 2025.
        <a href="https://doi.org/10.1109/RFCoN62306.2025.11085271" target="_blank" rel="noopener">[DOI]</a>
        <span class="status published">Published</span>
        <span class="status-badge best-paper">🏆 Best Paper Award</span><br>
        <small><em>Track 2 | Session II | Paper ID: 718 | Acceptance rate: 12%</em></small><br>
        <a href="/images/PID718.pdf" target="_blank" rel="noopener" title="Download PDF">📥</a>
      </div>
      <div class="cite-box" onclick="copyCitation('citeP2')">
        📑 Cite
        <textarea id="citeP2" class="hidden-citation">S. R. Sapireddy and M. Rahman, "Revisiting R: Statistical Envelope Analysis for Lightweight RF Modulation Classification," 2025 1st International Conference on Radio Frequency Communication and Networks (RFCoN), Thanjavur, India, 2025, pp. 1-6, doi: 10.1109/RFCoN62306.2025.11085271</textarea>
      </div>
    </div>

    <div class="pub-entry">
      <div class="pub-card">
        <strong>Srinivas Rahul Sapireddy</strong>, Asifuzzaman K., Mostafizur Rahman<br>
        <em>"Simplifying Activations with Linear Approximations in Neural Networks"</em><br>
         <a href="https://www.sciencedirect.com/science/article/pii/S2773064625000143" target="_blank" rel="noopener"> Memories - Materials, Devices, Circuits and Systems (Elsevier)</a>, 2025.
        <a href="https://www.sciencedirect.com/science/article/pii/S2773064625000143" target="_blank" rel="noopener">[DOI]</a>
        <span class="status published">Published</span><br>
        <a href="/images/Memories_3.pdf" target="_blank" rel="noopener" title="Download PDF">📥</a>
      </div>
      <div class="cite-box" onclick="copyCitation('citeP3')">
        📑 Cite
        <textarea id="citeP3" class="hidden-citation">Sapireddy, S. R., Asifuzzaman, K., & Mostafizur, R. (2025). Simplifying activations with linear approximations in neural networks. Memories - Materials, Devices, Circuits and Systems, 100134. https://doi.org/10.1016/j.memori.2025.100134</textarea>
      </div>
    </div>

    <div class="pub-entry">
      <div class="pub-card">
        <strong>Srinivas Rahul Sapireddy</strong>, G Surekha, Hemanth Bandi<br>
        <em>"Bin-Based R: Resource-Efficient RF Modulation Classification Using Envelope Statistics"</em><br>
        <a href="https://ieeesoutheastcon.org/" target="_blank" rel="noopener">IEEE SoutheastCon</a>, March 13–15, 2026, Huntsville, Alabama
        <span class="status accepted">Accepted</span>
      </div>
      <div class="cite-box" onclick="copyCitation('citeP4')">
        📑 Cite
        <textarea id="citeP4" class="hidden-citation">Accepted.</textarea>
      </div>
    </div>

    <div class="pub-entry">
      <div class="pub-card">
        Iqbal, M. A., <strong>Sapireddy, S. R.</strong>, Dasari, S., Asifuzzaman K., Rahman, M.<br>
        <em>“A Review of Crosstalk Polymorphic Circuits and Their Scalability”</em><br>
        <a href="https://www.sciencedirect.com/science/article/pii/S2773064623000713" target="_blank" rel="noopener"> Memories - Materials, Devices, Circuits and Systems (Elsevier)</a>, 2023.
        <a href="https://doi.org/10.1016/j.memori.2023.100094" target="_blank" rel="noopener">[DOI]</a>
        <span class="status published">Published</span><br>
        <a href="/images/Memories_1.pdf" target="_blank" rel="noopener" title="Download PDF">📥</a>
      </div>
      <div class="cite-box" onclick="copyCitation('citeP5')">
        📑 Cite
        <textarea id="citeP5" class="hidden-citation">Iqbal, M. A., Sapireddy, S. R., Dasari, S., Asifuzzaman, K., & Rahman, M. (2024). A review of crosstalk polymorphic circuits and their scalability. Memories - Materials, Devices, Circuits and Systems, 7, 100094. https://doi.org/10.1016/j.memori.2023.100094</textarea>
      </div>
    </div>

    <div class="pub-entry">
      <div class="pub-card">
        Wafi Danesh, <strong>Srinivas Rahul Sapireddy</strong>, Mostafizur Rahman<br>
        <em>“Understanding and Detecting Adversarial Examples in IoT Networks: A White-Box Analysis with Autoencoders”</em><br>
        <a href="https://www.mdpi.com/2079-9292/14/15/3015" target="_blank" rel="noopener">MDPI Electronics</a>, 2025.
        <a href="https://doi.org/10.3390/electronics14153015" target="_blank" rel="noopener">[DOI]</a>
        <span class="status published">Published</span><br>
        <a href="/images/MDPI_1.pdf" target="_blank" rel="noopener" title="Download PDF">📥</a>
      </div>
      <div class="cite-box" onclick="copyCitation('citeP6')">
        📑 Cite
        <textarea id="citeP6" class="hidden-citation">Danesh, W.; Sapireddy, S.R.; Rahman, M. Understanding and Detecting Adversarial Examples in IoT Networks: A White-Box Analysis with Autoencoders. Electronics 2025, 14, 3015. https://doi.org/10.3390/electronics14153015</textarea>
      </div>
    </div>

    <div class="pub-entry">
      <div class="pub-card">
        <strong>Sapireddy, Srinivas Rahul</strong>, P. N. Tejaswi, Y. M. Sandeep, K. Hari Krishna<br>
        <em>“Two-Stage Operational Amplifier with a Gain Boosted, Source Follower Buffer”</em><br>
        <a href="https://ijettjournal.org/archive/ijett-v34p252" target="_blank" rel="noopener">International Journal of Engineering Trends and Technology</a>, vol. 34, no. 6, pp. 256–259, April 2016.
        <a href="https://doi.org/10.14445/22315381/IJETT-V34P252" target="_blank" rel="noopener">[DOI]</a>
        <span class="status published">Published</span>
      </div>
      <div class="cite-box" onclick="copyCitation('citeP7')">
        📑 Cite
        <textarea id="citeP7" class="hidden-citation">S. R. Sapireddy, P. N. Tejaswi, Y. M. Sandeep, and K. H. Krishna, "Two-Stage Operational Amplifier with a Gain Boosted, Source Follower Buffer," IJETT, vol. 34, no. 6, pp. 256–259, Apr. 2016.</textarea>
      </div>
    </div>

    <div class="pub-entry">
      <div class="pub-card">
        Gurijala, B. T., <strong>Sapireddy, S. R.</strong><br>
        <em>“Automation of Patient Medical Record Dispatch System Software Application”</em><br>
        IJARSET, vol. 5, no. 6, pp. 6074–6097, Jun. 2018
        <span class="status published">Published</span>
      </div>
      <div class="cite-box" onclick="copyCitation('citeP8')">
        📑 Cite
        <textarea id="citeP8" class="hidden-citation">B. T. Gurijala and S. R. Sapireddy, "Automation of Patient Medical Record Dispatch System Software Application", International Journal of Advanced Research in Science, Engineering and Technology (IJARSET), vol. 5, no. 6, pp. 6074–6097, Jun. 2018.</textarea>
      </div>
    </div>

    <div class="pub-entry">
      <div class="pub-card">
        <strong>Srinivas Rahul Sapireddy</strong><br>
        <em>“CAM Cell Based Memory Architecture for Extreme Searching Operations”</em><br>
        IJAECS, vol. 3, issue 8, pp. 80–83, August 2016.
        <span class="status published">Published</span>
      </div>
      <div class="cite-box" onclick="copyCitation('citeP9')">
        📑 Cite
        <textarea id="citeP9" class="hidden-citation">S. R. Sapireddy, "CAM Cell Based Memory Architecture for Extreme Searching Operations," IJAECS, vol. 3, no. 8, pp. 80–83, Aug. 2016.</textarea>
      </div>
    </div>

    <div class="pub-entry">
      <div class="pub-card">
        Mostafizur Rahman, Arif Iqbal, Srinivas Rahul Sapireddy<br>
        <em>“A Messaging based Intelligent Computing Approach for Machine Learning Applications”</em><br>
        Accessed: Mar, Volume 20, 2024.
        <span class="status pending">📄 Online Archive</span>
      </div>
      <div class="cite-box" onclick="copyCitation('citeP10')">
        📑 Cite
        <textarea id="citeP10" class="hidden-citation">M. Rahman, A. Iqbal, and S. R. Sapireddy, "A Messaging Based Intelligent Computing Approach for Machine Learning Applications," Accessed: Mar, vol. 20, 2024.</textarea>
      </div>
    </div>

  </div>
</div>

<div class="section">
  <h3>📝 Manuscripts in Preparation / Under Review</h3>
  <div class="divider"></div>

  <div class="pub-grid">
    <div class="pub-entry">
      <div class="pub-card">
        <strong>Srinivas Rahul Sapireddy</strong>, Naznin Akther, Mostafizur Rahman<br>
        <em>“Lightweight Classification of Spread Spectrum Signals Using Cyclostationary Autocorrelation-Based Binning”</em><br>
        <a href="https://milcom.org" target="_blank" rel="noopener">IEEE Military Communications Conference (MILCOM)</a>, October 6–10, 2025, Los Angeles, California.
        <span class="status pending">To be Submitted</span>
      </div>
      <div class="cite-box" onclick="copyCitation('citeR1')">
        📑 Cite
        <textarea id="citeR1" class="hidden-citation">To be Submitted.</textarea>
      </div>
    </div>

    <div class="pub-entry">
      <div class="pub-card">
        <strong>Srinivas Rahul Sapireddy</strong><br>
        <em>“Refining Deep Reinforcement Learning”</em><br>
        <a href="https://icadeis.org/index.php" target="_blank" rel="noopener">International Conference on Advancement in Data Science, E-learning and Information System (ICADEIS)</a>, June 23–24, 2026, Bandung, Indonesia
        <span class="status pending">Completed Manuscripts</span>
      </div>
      <div class="cite-box" onclick="copyCitation('citeR2')">
        📑 Cite
        <textarea id="citeR2" class="hidden-citation">Completed Manuscripts.</textarea>
      </div>
    </div>

    <div class="pub-entry">
      <div class="pub-card">
        <strong>Srinivas Rahul Sapireddy</strong><br>
        <em>“From Rule-Based to Neural”</em><br>
        <a href="https://r10.ieee.org/vizagbay/icissgt-2023-2/" target="_blank" rel="noopener">IEEE International Conference on Intelligent Systems, Smart and Green Technologies</a>, February 2026.
        <span class="status pending">Archived Projects</span>
      </div>
      <div class="cite-box" onclick="copyCitation('citeR3')">
        📑 Cite
        <textarea id="citeR3" class="hidden-citation">Archived Projects.</textarea>
      </div>
    </div>
  </div>
</div>

<div class="section">
  <h3>Work In Progress</h3>
  <div class="divider"></div>

  <div class="pub-grid">
    <div class="pub-entry">
      <div class="pub-card wip">
        <strong>Srinivas Rahul Sapireddy</strong>, Hemanth Bandi<br>
        <em>“Exploratory Study on Network Behavior Analysis”</em><br>
        <a href="https://www.ieee-cars.org/" target="_blank" rel="noopener">IEEE 6th Cyber Awareness and Research Symposium (CARS'26)</a>, October 26–28, 2026, Grand Forks, ND, USA
        <span class="wip-badge">Completed Manuscripts</span>
      </div>
      <div class="cite-box wip" onclick="copyCitation('citeW1')">
        📑 Cite
        <textarea id="citeW1" class="hidden-citation">Completed Manuscripts.</textarea>
      </div>
    </div>

    <div class="pub-entry">
      <div class="pub-card wip">
        <strong>Srinivas Rahul Sapireddy</strong>, Hemanth Bandi<br>
        <em>“Edge-AI Healthcare: Quantization-Aware DNN”</em><br>
        <a href="https://zhang-informatics.github.io/ICHI2026/" target="_blank" rel="noopener">IEEE International Conference on Healthcare Informatics (ICHI)</a>, June 1–4, 2026
        <span class="wip-badge">Work in Progress</span>
      </div>
      <div class="cite-box wip" onclick="copyCitation('citeW2')">
        📑 Cite
        <textarea id="citeW2" class="hidden-citation">Work in Progress.</textarea>
      </div>
    </div>

    <div class="pub-entry">
      <div class="pub-card wip">
        <strong>Srinivas Rahul Sapireddy</strong>, …<br>
        <em>“Adaptive Regularization - Efficient Neural Networks”</em><br>
        <a href="https://ieee-isvlsi.github.io/ISVLSI_2026_Website/index.html" target="_blank" rel="noopener">IEEE Computer Society Annual Symposium on VLSI (ISVLSI)</a>, April 20–21, 2026
        <span class="wip-badge">Work in Progress</span>
      </div>
      <div class="cite-box wip" onclick="copyCitation('citeW3')">
        📑 Cite
        <textarea id="citeW3" class="hidden-citation">Work in Progress.</textarea>
      </div>
    </div>

    <div class="pub-entry">
      <div class="pub-card wip">
        <strong>Srinivas Rahul Sapireddy</strong>, …<br>
        <em>“EABS: Intelligent Signal Processing”</em><br>
        <a href="https://www.ieeewamicon.org/" target="_blank" rel="noopener">IEEE Wireless and Microwave Technology Conference (WAMICON)</a>, July 7–10, 2026
        <span class="wip-badge">Work in Progress</span>
      </div>
      <div class="cite-box wip" onclick="copyCitation('citeW4')">
        📑 Cite
        <textarea id="citeW4" class="hidden-citation">Work in Progress.</textarea>
      </div>
    </div>
  </div>
</div>

<div class="section">
  <h3>Publication Venues</h3>
  <div class="divider"></div>
  <div class="logo-row">
    <a href="https://www.ieee.org/" target="_blank" rel="noopener"><img src="/images/IEEE.jpg" alt="IEEE Logo"></a>
    <a href="https://www.acm.org/" target="_blank" rel="noopener"><img src="/images/ACM.png" alt="ACM Logo"></a>
    <a href="https://www.mdpi.com/" target="_blank" rel="noopener"><img src="/images/MDPI.png" alt="MDPI Logo"></a>
    <a href="https://www.elsevier.com/" target="_blank" rel="noopener"><img src="/images/Elsevier.png" alt="Elsevier Logo"></a>
  </div>
</div>

<div class="section">
  <h3>🔎 Profiles &amp; Identifiers</h3>
  <div class="divider"></div>
  <div class="logo-row">
    <a href="https://sciprofiles.com/profile/srsapireddy" target="_blank" rel="noopener"><img src="/images/SciProfiles.png" alt="SciProfiles Logo"></a>
    <a href="https://orcid.org/0009-0004-6956-0652" target="_blank" rel="noopener"><img src="/images/orcid.png" alt="ORCID Logo"></a>
    <a href="https://www.researchgate.net/profile/Srinivas-Rahul-Sapireddy" target="_blank" rel="noopener"><img src="/images/RG.jpg" alt="ResearchGate Logo"></a>
    <a href="https://openreview.net/" target="_blank" rel="noopener"><img src="/images/OPEN.jpg" alt="OpenReview Logo"></a>
    <a href="https://dblp.org/search?q=srinivas%20rahul%20sapireddy" target="_blank" rel="noopener"><img src="/images/dblp.png" alt="dblp Logo"></a>
  </div>
</div>

<footer class="pub-footer">
  📘 <a href="https://scholar.google.com/citations?user=08fgpdIAAAAJ&hl=en" target="_blank" rel="noopener">Google Scholar</a>
  📝 <a href="https://www.researchgate.net/profile/Srinivas-Rahul-Sapireddy" target="_blank" rel="noopener">ResearchGate</a>
  🧬 <a href="https://orcid.org/0009-0004-6956-0652" target="_blank" rel="noopener">ORCID</a>
  🧾 <a href="https://openreview.net/profile?id=~Srinivas_Rahul_Sapireddy1" target="_blank" rel="noopener">OpenReview</a>
</footer>

<div style="text-align:center; margin-top: 12px;">
  <a href="https://info.flagcounter.com/gunK" title="Flag Counter" target="_blank" rel="noopener">
    <img src="https://s05.flagcounter.com/count/gunK/bg_24BDFF/txt_000000/border_4A12CC/columns_8/maxflags_12/viewers_0/labels_1/pageviews_1/flags_0/percent_1/"
         alt="Flag Counter" border="0" width="600">
  </a>
</div>
