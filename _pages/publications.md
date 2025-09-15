---
title: "Publications"
permalink: /publications/
---

<style>

  .wip-badge {
    display: inline-block;
    padding: 0.25rem 0.6rem;
    font-size: 0.85rem;
    font-weight: 600;
    color: #8a4c00;            /* dark orange text */
    background: #fff4e5;       /* light orange background */
    border: 1px solid #ffa726; /* orange border */
    border-radius: 0.4rem;
    text-transform: none;
  }
  
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

.pub-card {
  border: 2px solid #1a73e8;
  border-radius: 12px;
  padding: 1.2rem 1.5rem;
  background: #fff;
  transition: 0.3s ease;
}

.pub-card:hover {
  background-color: #f0f8ff;
  transform: scale(1.01);
  box-shadow: 0 4px 12px rgba(26, 115, 232, 0.1);
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

.pub-footer {
  margin-top: 2rem;
  text-align: center;
  font-size: 0.95rem;
}

.status-badge {
  display: inline-block;
  padding: 4px 10px;
  border-radius: 12px;
  font-weight: bold;
  font-size: 14px;
}

.best-paper {
  background-color: #e6ffe6;
  color: #28a745; /* Light green text */
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
.pub-entry {
  display: grid;
  grid-template-columns: 4fr 1fr;
  gap: 1rem;
  align-items: stretch;
}


.pub-card,
.cite-box {
  border: 2px solid #1a73e8;
  border-radius: 12px;
  padding: 1.2rem 1.5rem;
  background: #fff;
  transition: 0.3s ease;
}

.cite-box {
  display: flex;
  justify-content: center;
  align-items: center;
  min-width: 100px;
  cursor: pointer;
  font-size: 1rem;
  font-weight: 600;
  color: #1a73e8;
  position: relative;
}

.cite-box:hover {
  background-color: #f0f8ff;
  transform: scale(1.03);
}

.pub-grid.tight-gap {
  gap: 0.2rem; /* Reduce only for these */
}

textarea.hidden-citation {
  position: absolute;
  left: -9999px;
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

<!-- Collaborations Section -->
<h2 style="text-align:center; margin-top: 2rem;">Collaborations</h2>
<div class="logo-row">
  <a href="https://www.ornl.gov/" target="_blank"><img src="/images/Oak.jpg" alt="ORNL Logo" /></a>
  <a href="https://www.uis.edu/" target="_blank"><img src="/images/UIS.png" alt="UIS Logo" /></a>
  <a href="https://www.umkc.edu/" target="_blank"><img src="/images/UMKC.png" alt="UMKC Logo" /></a>
  <a href="https://twin-cities.umn.edu/" target="_blank"><img src="/images/UMTC.jpeg" alt="University of Minnesota Logo" /></a>
  <a href="https://www.griet.ac.in/" target="_blank"><img src="/images/GRIET.png" alt="GRIET Logo" /></a>
</div>



<section id="publications">
  <h2>📚 Publications</h2>
    <!-- Published -->

  <h3 style="margin-top:2rem;">✅ Work In Progress</h3>
  <div class="pub-grid">
  <div class="pub-entry">
  <div class="pub-card">
    <strong>Srinivas Rahul Sapireddy</strong><br>
    <em>“Adaptive Regularization - Efficient Neural Networks”</em><br>
    <a href="https://ieee-isvlsi.github.io/ISVLSI_2026_Website/index.html" target="_blank">
      IEEE Computer Society Annual Symposium on VLSI - ISVLSI</a> , July 7-10, 2026
      <span class="wip-badge">To be Submitted</span>
  </div>
  <div class="cite-box" onclick="copyCitation('cite1')">
    📑 Cite
    <textarea id="cite1" class="hidden-citation">To be Submitted</textarea>
  </div>
</div>
</div>
  
  <h3 style="margin-top:2rem;">✅ Published</h3>
  <div class="pub-grid">
    <div class="pub-entry">
      <div class="pub-card">
      <strong>Srinivas Rahul Sapireddy</strong>, Mostafizur Rahman<br>
      <em><a href="https://dl.acm.org/doi/10.1145/3716368.3735217" target="_blank">“On the Effectiveness of Custom Activation Functions on Long-Term Short-Term Memory”</a></em><br>
      <a href="https://dl.acm.org/doi/10.1145/3716368.3735217" target="_blank">ACM Great Lakes Symposium on VLSI (GLSVLSI)</a>, 2025, New Orleans, LA. 
      <a href="10.1145/3716368.3735217" target="_blank">[DOI]</a>
        <span class="status published">Published</span><br>
      <small><em>Session: VLSI for Machine Learning and Artificial Intelligence | Acceptance rate: 27%</em></small><br>
      <a href="/images/PID69.pdf" target="_blank" title="Download PDF">📥</a>
    </div>
      <div class="cite-box" onclick="copyCitation('cite3')">
        📑 Cite
        <textarea id="cite3" class="hidden-citation">Srinivas Rahul Sapireddy and Mostafizur Rahman. 2025. On the Effectiveness of Piecewise Activation Approximations for Long-Term Short-Memory Networks. In Proceedings of the Great Lakes Symposium on VLSI 2025 (GLSVLSI '25), June 29, 2025, pp. 740–745. https://doi.org/10.1145/3716368.3735217</textarea>
      </div>
    </div>
    <div class="pub-entry">
          <div class="pub-card">
      <strong>Srinivas Rahul Sapireddy</strong>, Mostafizur Rahman<br>
      <em>
        <a href="https://ieeexplore.ieee.org/document/11085271" target="_blank">
          “Re-Visiting R: Statistical Envelope Analysis for Lightweight Modulation Classification”
        </a>
      </em><br>
      <em>IEEE International Conference on Radio Frequency Communication and Networks (RFCoN)</em>, 2025. 
      <a href="10.1109/RFCoN62306.2025.11085271" target="_blank">[DOI]</a>
            <span class="status published"> Published</span>
            <span class="status-badge best-paper">🏆 Best Paper Award</span>
      <small>
        <em>
          Track 2 | Session II | Paper ID: 718 | Acceptance rate: 12%
        </em>
      </small><br>
      <a href="/images/PID718.pdf" target="_blank" title="Download PDF">📥</a>
    </div>
      <div class="cite-box" onclick="copyCitation('cite4')">
        📑 Cite
        <textarea id="cite4" class="hidden-citation">S. R. Sapireddy and M. Rahman, "Revisiting R: Statistical Envelope Analysis for Lightweight RF Modulation Classification," 2025 1st International Conference on Radio Frequency Communication and Networks (RFCoN), Thanjavur, India, 2025, pp. 1-6, doi: 10.1109/RFCoN62306.2025.11085271</textarea>
      </div>
    </div>
    <div class="pub-entry">
      <div class="pub-card">
        <strong>Srinivas Rahul Sapireddy</strong>, G Surekha, Hemanth Bandi<br>
        <em>“Re-Defining R: Resource-Efficient Modulation Classification Using Bin-Based Envelope Features”</em><br>
        <a href="https://ieeemapcon.org/" target="_blank">Microwaves, Antennas, and Propagation Conference (MAPCON) 2025</a>, December 14–18, 2025, Kerala, India.
        <span class="status published">Accepted</span>
      </div>
      <div class="cite-box" onclick="copyCitation('cite1')">
        📑 Cite
        <textarea id="cite1" class="hidden-citation">Accepted</textarea>
      </div>
    </div>
    <div class="pub-entry">
      <div class="pub-card">
      Iqbal, M. A., <strong>Sapireddy, S. R.</strong>, Dasari, S., Asifuzzaman K., Rahman, M.<br>
        <em><a href="https://www.sciencedirect.com/science/article/pii/S2773064623000713" target="_blank">“A Review of Crosstalk Polymorphic Circuits and Their Scalability”</a></em><br>
      <em>Memories – Materials, Devices, Circuits and Systems</em>, vol. 7, article 100094, 2023. 
      <a href="https://doi.org/10.1016/j.memori.2023.100094" target="_blank">[DOI]</a>
      <span class="status published">Published</span>
    </div>
      <div class="cite-box" onclick="copyCitation('cite5')">
        📑 Cite
        <textarea id="cite5" class="hidden-citation">Iqbal, M. A., Sapireddy, S. R., Dasari, S., Asifuzzaman, K., & Rahman, M. (2024). A review of crosstalk polymorphic circuits and their scalability. Memories - Materials, Devices, Circuits and Systems, 7, 100094. https://doi.org/10.1016/j.memori.2023.100094</textarea>
      </div>
    </div>
    <div class="pub-entry">
      <div class="pub-card">
      Wafi Danesh, <strong>Srinivas Rahul Sapireddy</strong>, Mostafizur Rahman<br>
      <em><a href="https://www.mdpi.com/2079-9292/14/15/3015" target="_blank">“Understanding and Detecting Adversarial Examples in IoT Networks: A White-Box Analysis with Autoencoders”</a></em><br>
      <em>MDPI Electronics</em>, 2025.
      <a href="https://doi.org/10.3390/electronics14153015" target="_blank">[DOI]</a>
      <span class="status published">Published</span>
    </div>
      <div class="cite-box" onclick="copyCitation('cite6')">
        📑 Cite
        <textarea id="cite6" class="hidden-citation">Danesh, W.; Sapireddy, S.R.; Rahman, M. Understanding and Detecting Adversarial Examples in IoT Networks: A White-Box Analysis with Autoencoders. Electronics 2025, 14, 3015. https://doi.org/10.3390/electronics14153015</textarea>
      </div>
    </div>
  <div class="pub-entry">
    <div class="pub-card">
      <strong>Sapireddy, Srinivas Rahul</strong>, P. N. Tejaswi, Y. M. Sandeep, K. Hari Krishna<br>
      <em><a href="https://ijettjournal.org/archive/ijett-v34p252" target="_blank">“Two-Stage Operational Amplifier with a Gain Boosted, Source Follower Buffer”</a></em><br>
      IJETT, vol. 34, no. 6, pp. 256–259, April 2016.
      <a href="10.14445/22315381/IJETT-V34P252" target="_blank">[DOI]</a>
      <span class="status published">Published</span>
    </div>
    <div class="cite-box" onclick="copyCitation('pub10')">
      📑 Cite
      <textarea id="pub10" class="hidden-citation">S. R. Sapireddy, P. N. Tejaswi, Y. M. Sandeep, and K. H. Krishna, "Two-Stage Operational Amplifier with a Gain Boosted, Source Follower Buffer," IJETT, vol. 34, no. 6, pp. 256–259, Apr. 2016.</textarea>
    </div>
  </div>
    <div class="pub-entry">
      <div class="pub-card">
        Gurijala, B. T., <strong>Sapireddy, S. R.</strong><br>
        <em>“Automation of Patient Medical Record Dispatch System Software Application”</em><br>
        IJARSET, vol. 5, no. 6, pp. 6074–6097, Jun. 2018
        <span class="status published">Published</span>
      </div>
      <div class="cite-box" onclick="copyCitation('cite8')">
        📑 Cite
        <textarea id="cite8" class="hidden-citation">B. T. Gurijala and S. R. Sapireddy, "Automation of Patient Medical Record Dispatch System Software Application", International Journal of Advanced Research in Science, Engineering and Technology (IJARSET), vol. 5, no. 6, pp. 6074–6097, Jun. 2018.</textarea>
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
      <textarea id="pub9" class="hidden-citation">S. R. Sapireddy, "CAM Cell Based Memory Architecture for Extreme Searching Operations," IJAECS, vol. 3, no. 8, pp. 80–83, Aug. 2016.</textarea>
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
      <textarea id="pub11" class="hidden-citation">M. Rahman, A. Iqbal, and S. R. Sapireddy, "A Messaging Based Intelligent Computing Approach for Machine Learning Applications," Accessed: Mar, vol. 20, 2024.</textarea>
    </div>
  </div>

  <h3 style="margin-top:2rem;">📝 To be Submitted / Under Review</h3>
<div class="pub-grid">
  <div class="pub-entry">
      <div class="pub-card">
        <strong>Srinivas Rahul Sapireddy</strong>, Asifuzzaman K., Mostafizur Rahman<br>
        <em>"Simplifying Activations with Linear Approximations in Neural Networks"</em><br>
        Memories, 2024
        <span class="status review">Minor Revision</span>
      </div>
      <div class="cite-box" onclick="copyCitation('cite7')">
        📑 Cite
        <textarea id="cite7" class="hidden-citation">Under Review</textarea>
      </div>
    </div>
  <div class="pub-grid tight-gap">
    <div class="pub-entry">
      <div class="pub-card">
        <strong>Srinivas Rahul Sapireddy</strong>, Naznin Akther, Mostafizur Rahman<br>
        <em>“Lightweight Classification of Spread Spectrum Signals Using Cyclostationary Autocorrelation-Based Binning”</em>
        <a href="https://milcom.org" target="_blank">IEEE Military Communications Conference (MILCOM)</a>, October 6 - 10, 2025, Los Angeles, California.
        <span class="status pending">To be Submitted</span>
      </div>
      <div class="cite-box" onclick="copyCitation('cite1')">
        📑 Cite
        <textarea id="cite1" class="hidden-citation">To be Submitted</textarea>
      </div>
    </div>
    <div class="pub-entry">
      <div class="pub-card">
      <strong>Srinivas Rahul Sapireddy*</strong>, Jahavani*, Nimisha<br>
      <em>“From Rule-Based to Neural: Statistical Envelope Feature Classification Using Feedforward Networks”</em>
      <a href="https://www.smartcomconference.com/" target="_blank">IEEE International Conference on Intelligent Systems, Smart and Green Technologies (ICISSGT – 2025)</a>, 19-20 December 2025. <span class="status pending">To be Submitted</span>
    </div>
      <div class="cite-box" onclick="copyCitation('cite2')">
        📑 Cite
        <textarea id="cite2" class="hidden-citation">To be Submitted</textarea>
      </div>
    </div>
     <div class="pub-entry">
      <div class="pub-card">
      <strong>Srinivas Rahul Sapireddy</strong>, Hemanth Bandi<br>
      <em>“Refining Deep Reinforcement Learning with Double Estimation and Optimized Target Updates”</em><br>
      <a href="https://www.smartcomconference.com/" target="_blank">10th International Conference on Smart Trends in Computing and Communications</a>,<br> 19 - 21 January 2026. <span class="status pending">To be Submitted</span>
    </div>
      <div class="cite-box" onclick="copyCitation('cite2')">
        📑 Cite
        <textarea id="cite2" class="hidden-citation">To be Submitted</textarea>
      </div>
    </div>
    <div class="pub-entry">
      <div class="pub-card">
      Nimisha, <strong>Srinivas Rahul Sapireddy</strong>, Jahavani<br>
      <em>“Advances in Optical Nanoantenna-Based LSPR Biosensors for COVID-19 Antibody Detection: A Comprehensive Review”</em><br>
      <a href="https://www.smartcomconference.com/" target="_blank">10th International Conference on Smart Trends in Computing and Communications</a>, <br> 19 - 21 January 2026. <span class="status pending">To be Submitted</span>
    </div>
      <div class="cite-box" onclick="copyCitation('cite2')">
        📑 Cite
        <textarea id="cite2" class="hidden-citation">To be Submitted</textarea>
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
      <textarea id="pub12" class="hidden-citation">Under Review</textarea>
    </div>
  </div>

<!-- Publication Venues Section -->
<h2 style="text-align:center; margin-top: 3rem;">Publication Venues</h2>
<div class="logo-row">
  <a href="https://www.ieee.org/" target="_blank"><img src="/images/IEEE.jpg" alt="IEEE Logo" /></a>
  <a href="https://www.acm.org/" target="_blank"><img src="/images/ACM.png" alt="ACM Logo" /></a>
  <a href="https://www.mdpi.com/" target="_blank"><img src="/images/MDPI.png" alt="MDPI Logo" /></a>
  <a href="https://www.elsevier.com/" target="_blank"><img src="/images/Elsevier.png" alt="Elsevier Logo" /></a>
</div>

<!-- Profiles & Identifiers Section -->
<h2 style="text-align:center; margin-top: 3rem;">Profiles & Identifiers</h2>
<div class="logo-row">
  <a href="https://sciprofiles.com/profile/srsapireddy" target="_blank"><img src="/images/SciProfiles.png" alt="SciProfiles Logo" /></a>
  <a href="https://orcid.org/0009-0004-6956-0652" target="_blank"><img src="/images/orcid.png" alt="ORCID Logo" /></a>
  <a href="https://www.researchgate.net/profile/Srinivas-Rahul-Sapireddy" target="_blank"><img src="/images/RG.jpg" alt="ResearchGate Logo" /></a>
  <a href="https://openreview.net/" target="_blank"><img src="/images/OPEN.jpg" alt="OpenReview Logo" /></a>
</div>



<footer class="pub-footer">
  📘 <a href="https://scholar.google.com/citations?user=08fgpdIAAAAJ&hl=en" target="_blank">Google Scholar</a>
  📝 <a href="https://www.researchgate.net/profile/Srinivas-Rahul-Sapireddy" target="_blank">ResearchGate</a>
  🧬 <a href="https://orcid.org/0009-0004-6956-0652" target="_blank">ORCID</a>
  📝 <a href="https://openreview.net/profile?id=~Srinivas_Rahul_Sapireddy1" target="_blank">OpenReview</a>
</footer>

<div style="text-align: center;">
  <a href='https://mapmyvisitors.com/web/1bz4s'  title='Visit tracker'><img src='https://mapmyvisitors.com/map.png?cl=ffffff&w=600&t=tt&d=Q4nlfwgfwMR0BJuj7RyFUCNPyBsWHJRRyG14HMgJViw'/></a>
</div>



