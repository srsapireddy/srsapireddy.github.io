---
title: "Publications"
permalink: /publications/
---

<style>
.logo-row {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 2rem;
  margin-top: 3rem;
  flex-wrap: wrap;
}

.logo-row img {
  height: 50px;
  max-width: 120px;
  transition: transform 0.3s ease;
  object-fit: contain;
}

.logo-row img:hover {
  transform: scale(1.1);
}

.pub-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 1.5rem;
  margin-top: 2rem;
}

.pub-entry {
  display: flex;
  align-items: stretch; /* Ensures equal height */
  gap: 1rem;
  margin-bottom: 1.5rem;
}

.pub-card,
.cite-box {
  border: 2px solid #1a73e8;
  border-radius: 12px;
  padding: 1.2rem 1.5rem;
  background: #fff;
  transition: 0.3s ease;
}


.pub-card:hover,
.cite-box:hover {
  background-color: #f0f8ff;
  transform: scale(1.03);
}

.cite-box {
  align-items: center;
  text-align: center;
  font-weight: bold;
  font-size: 1.1rem;
  cursor: pointer;
}

  
.pub-card strong {
  font-weight: 600;
  color: #111;
}

.pub-card em {
  color: #333;
}

.status {
  font-size: 0.85rem;
  font-weight: bold;
  padding: 0.2rem 0.5rem;
  border-radius: 6px;
  margin-left: 0.5rem;
}

.status.accepted { color: #1a7f3d; background: #dcfce7; }
.status.review   { color: #c67c00; background: #fff6e6; }
.status.pending  { color: #555; background: #f0f0f0; }
.status.published { color: #0a539e; background: #e5f1ff; }

textarea.hidden-citation {
  position: absolute;
  left: -9999px;
}

.pub-footer {
  margin-top: 2rem;
  text-align: center;
  font-size: 0.95rem;
}

.pub-footer a {
  text-decoration: none;
  color: #1a73e8;
  margin: 0 1rem;
  font-weight: 600;
}

.pub-footer a:hover {
  text-decoration: underline;
}
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

<section id="publications">
  <h2>📚 Publications</h2>
  <div class="pub-grid">
    <div class="pub-entry">
      <div class="pub-card">
        <strong>Srinivas Rahul Sapireddy</strong>, Naznin Akther, Mostafizur Rahman<br>
        <em>“Lightweight Classification of Spread Spectrum Signals Using Cyclostationary Autocorrelation-Based Binning”</em><br>
        <a href="https://milcom.org" target="_blank">IEEE Military Communications Conference (MILCOM)</a>, 2025.
        <span class="status pending">Under Review</span>
      </div>
      <div class="cite-box" onclick="copyCitation('cite1')">
        📑 Cite
        <textarea id="cite1" class="hidden-citation">[1] Under Review</textarea>
      </div>
    </div>
    <div class="pub-entry">
      <div class="pub-card">
        <strong>Srinivas Rahul Sapireddy</strong>, Surekha G, Hemanth Bandi<br>
        <em>“Re-Defining R: Resource-Efficient Modulation Classification Using Bin-Based Envelope Features”</em><br>
        IEEE MAPCON 2025, Kerala, India.
        <span class="status pending">Under Review</span>
      </div>
      <div class="cite-box" onclick="copyCitation('cite2')">
        📑 Cite
        <textarea id="cite2" class="hidden-citation">[2] Under Review</textarea>
      </div>
    </div>
    <div class="pub-entry">
      <div class="pub-card">
        <strong>Srinivas Rahul Sapireddy</strong>, Mostafizur Rahman<br>
        <em><a href="https://doi.org/10.1145/3716368.3735217" target="_blank">On the Effectiveness of Piecewise Activation Approximations for Long-Term Short-Memory Networks</a></em><br>
        ACM GLSVLSI, June 2025, New Orleans, LA.
        <span class="status published">Published</span>
      </div>
      <div class="cite-box" onclick="copyCitation('cite3')">
        📑 Cite
        <textarea id="cite3" class="hidden-citation">[3] Srinivas Rahul Sapireddy and Mostafizur Rahman. 2025. On the Effectiveness of Piecewise Activation Approximations for Long-Term Short-Memory Networks. In Proceedings of the Great Lakes Symposium on VLSI 2025 (GLSVLSI '25), June 29, 2025, pp. 740–745. https://doi.org/10.1145/3716368.3735217</textarea>
      </div>
    </div>
    <div class="pub-entry">
      <div class="pub-card">
        <strong>Sapireddy, S. R.</strong>, Rahman, M.<br>
        <em><a href="https://arxiv.org/abs/2506.19956" target="_blank">Revisiting R: Statistical Envelope Analysis for Lightweight RF Modulation Classification</a></em><br>
        IEEE RFCoN 2025 – Best Paper Award
        <span class="status accepted">Accepted</span>
      </div>
      <div class="cite-box" onclick="copyCitation('cite4')">
        📑 Cite
        <textarea id="cite4" class="hidden-citation">[4] Sapireddy, S. R., & Rahman, M. (2025). Revisiting R: Statistical Envelope Analysis for Lightweight RF Modulation Classification. ArXiv. https://arxiv.org/abs/2506.19956</textarea>
      </div>
    </div>
    <div class="pub-entry">
      <div class="pub-card">
        Iqbal, M. A., <strong>Sapireddy, S. R.</strong>, Dasari, S., Asifuzzaman K., Rahman, M.<br>
        <em>A review of crosstalk polymorphic circuits and their scalability</em><br>
        Memories, vol. 7, article 100094, 2023
        <span class="status published">Published</span>
      </div>
      <div class="cite-box" onclick="copyCitation('cite5')">
        📑 Cite
        <textarea id="cite5" class="hidden-citation">[5] Iqbal, M. A., Sapireddy, S. R., Dasari, S., Asifuzzaman, K., & Rahman, M. (2024). A review of crosstalk polymorphic circuits and their scalability. Memories - Materials, Devices, Circuits and Systems, 7, 100094. https://doi.org/10.1016/j.memori.2023.100094</textarea>
      </div>
    </div>
    <div class="pub-entry">
      <div class="pub-card">
        Danesh, W., <strong>Sapireddy, S.R.</strong>, Rahman, M.<br>
        <em>Understanding and Detecting Adversarial Examples in IoT Networks: A White-Box Analysis with Autoencoders</em><br>
        MDPI Electronics, 2025
        <span class="status published">Published</span>
      </div>
      <div class="cite-box" onclick="copyCitation('cite6')">
        📑 Cite
        <textarea id="cite6" class="hidden-citation">[6] Danesh, W.; Sapireddy, S.R.; Rahman, M. Understanding and Detecting Adversarial Examples in IoT Networks: A White-Box Analysis with Autoencoders. Electronics 2025, 14, 3015. https://doi.org/10.3390/electronics14153015</textarea>
      </div>
    </div>
    <div class="pub-entry">
      <div class="pub-card">
        <strong>Srinivas Rahul Sapireddy</strong>, Asifuzzaman K., Mostafizur Rahman<br>
        <em>Simplifying Activations with Linear Approximations in Neural Networks</em><br>
        Memories, 2024
        <span class="status review">Minor Revision</span>
      </div>
      <div class="cite-box" onclick="copyCitation('cite7')">
        📑 Cite
        <textarea id="cite7" class="hidden-citation">[7] Under Review</textarea>
      </div>
    </div>
    <div class="pub-entry">
      <div class="pub-card">
        Gurijala, B. T., <strong>Sapireddy, S. R.</strong><br>
        <em>Automation of Patient Medical Record Dispatch System Software Application</em><br>
        IJARSET, vol. 5, no. 6, pp. 6074–6097, Jun. 2018
        <span class="status published">Published</span>
      </div>
      <div class="cite-box" onclick="copyCitation('cite8')">
        📑 Cite
        <textarea id="cite8" class="hidden-citation">[8] B. T. Gurijala and S. R. Sapireddy, "Automation of Patient Medical Record Dispatch System Software Application", International Journal of Advanced Research in Science, Engineering and Technology (IJARSET), vol. 5, no. 6, pp. 6074–6097, Jun. 2018.</textarea>
      </div>
    </div>
  <div class="pub-entry">
    <div class="pub-card">
      <strong>Srinivas Rahul Sapireddy</strong><br>
      <em>“CAM Cell Based Memory Architecture for Extreme Searching Operations”</em><br>
      IJAECS, vol. 3, issue 8, pp. 80–83, August 2016.
      <span class="status published">Published</span>
    </div>
    <div class="cite-box" onclick="copyCitation('pub9')">
      📑 Cite
      <textarea id="pub9" class="hidden-citation">[9] S. R. Sapireddy, "CAM Cell Based Memory Architecture for Extreme Searching Operations," IJAECS, vol. 3, no. 8, pp. 80–83, Aug. 2016.</textarea>
    </div>
  </div>

  <div class="pub-entry">
    <div class="pub-card">
      <strong>Sapireddy, Srinivas Rahul</strong>, P. N. Tejaswi, Y. M. Sandeep, K. Hari Krishna<br>
      <em>“Two-Stage Operational Amplifier with a Gain Boosted, Source Follower Buffer”</em><br>
      IJETT, vol. 34, no. 6, pp. 256–259, April 2016.
      <span class="status published">Published</span>
    </div>
    <div class="cite-box" onclick="copyCitation('pub10')">
      📑 Cite
      <textarea id="pub10" class="hidden-citation">[10] S. R. Sapireddy, P. N. Tejaswi, Y. M. Sandeep, and K. H. Krishna, "Two-Stage Operational Amplifier with a Gain Boosted, Source Follower Buffer," IJETT, vol. 34, no. 6, pp. 256–259, Apr. 2016.</textarea>
    </div>
  </div>

  <div class="pub-entry">
    <div class="pub-card">
      Mostafizur Rahman, Arif Iqbal, Srinivas Rahul Sapireddy<br>
      <em>“A Messaging based Intelligent Computing Approach for Machine Learning Applications”</em><br>
      Accessed: Mar, Volume 20, 2024.
      <span class="status online">📄 Online Archive</span>
    </div>
    <div class="cite-box" onclick="copyCitation('pub11')">
      📑 Cite
      <textarea id="pub11" class="hidden-citation">[11] M. Rahman, A. Iqbal, and S. R. Sapireddy, "A Messaging Based Intelligent Computing Approach for Machine Learning Applications," Accessed: Mar, vol. 20, 2024.</textarea>
    </div>
  </div>

  <div class="pub-entry">
    <div class="pub-card">
      Satya Sai Siva Rama Krishna Akula, Rownak Chowdhury, <strong>Srinivas Rahul Sapireddy</strong>, Mostafizur Rahman<br>
      <em>“An Opensource Framework for Offloading Big Data and AI Tasks (OFFLOAD) to Heterogeneous Compute Units”</em><br>
      IEEE TCAD, 2025.
      <span class="status review">Under Review</span>
    </div>
    <div class="cite-box" onclick="copyCitation('pub12')">
      📑 Cite
      <textarea id="pub12" class="hidden-citation">[12] Under Review</textarea>
    </div>
  </div>

  </div>

  <div class="logo-row">
    <a href="https://www.ieee.org/" target="_blank"><img src="/images/IEEE.jpg" alt="IEEE Logo" /></a>
    <a href="https://www.acm.org/" target="_blank"><img src="/images/ACM.png" alt="ACM Logo" /></a>
    <a href="https://www.ornl.gov/" target="_blank"><img src="/images/Oak.jpg" alt="ORNL Logo" /></a>
    <a href="https://openreview.net/" target="_blank"><img src="/images/OPEN.jpg" alt="OpenReview Logo" /></a>
    <a href="https://orcid.org/0009-0004-6956-0652" target="_blank"><img src="/images/orcid.png" alt="ORCID Logo" /></a>
    <a href="https://www.researchgate.net/profile/Srinivas-Rahul-Sapireddy" target="_blank"><img src="/images/RG.jpg" alt="ResearchGate Logo" /></a>
    <a href="https://www.uis.edu/" target="_blank"><img src="/images/UIS.png" alt="UIS Logo" /></a>
    <a href="https://www.umkc.edu/" target="_blank"><img src="/images/UMKC.png" alt="UMKC Logo" /></a>
  </div>
</section>

<footer class="pub-footer">
  📘 <a href="https://scholar.google.com/citations?user=08fgpdIAAAAJ&hl=en" target="_blank">Google Scholar</a>
  📝 <a href="https://www.researchgate.net/profile/Srinivas-Rahul-Sapireddy" target="_blank">ResearchGate</a>
  🧬 <a href="https://orcid.org/0009-0004-6956-0652" target="_blank">ORCID</a>
  📝 <a href="https://openreview.net/profile?id=~Srinivas_Rahul_Sapireddy1" target="_blank">OpenReview</a>
</footer>
