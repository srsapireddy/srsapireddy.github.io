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

<section id="publications">
  <h2>📚 Publications</h2>

  <div class="pub-grid">
    <div class="pub-entry">
  <div class="pub-card">
    <strong>Srinivas Rahul Sapireddy</strong>, Naznin Akther, Mostafizur Rahman<br>
    <em>“Lightweight Classification of Spread Spectrum Signals Using Cyclostationary Autocorrelation-Based Binning”</em><br>
    <a href="https://milcom.org" target="_blank">IEEE Military Communications Conference (MILCOM)</a>, October 28–30, 2025, Los Angeles, CA. 
    <span class="status pending">Submitted</span>
  </div>
  
  <div class="copy-icon" onclick="copyCitation('milcom2025')">
    📋
  </div>
  
  <!-- Hidden BibTeX -->
  <textarea id="milcom2025" style="position:absolute; left:-9999px;">
@inproceedings{sapireddy2025lightweight,
  title={Lightweight Classification of Spread Spectrum Signals Using Cyclostationary Autocorrelation-Based Binning},
  author={Sapireddy, Srinivas Rahul and Akther, Naznin and Rahman, Mostafizur},
  booktitle={MILCOM},
  year={2025}
}
  </textarea>
</div>
    <div class="pub-card">
      <strong>Srinivas Rahul Sapireddy</strong>, Naznin Akther, Mostafizur Rahman<br>
      <em>“Lightweight Classification of Spread Spectrum Signals Using Cyclostationary Autocorrelation-Based Binning”</em><br>
      <a href="https://milcom.org" target="_blank">IEEE Military Communications Conference (MILCOM)</a>, October 28–30, 2025, Los Angeles, CA. 
      <span class="status pending">Submitted</span>
    </div>
    <div class="pub-card">
      <strong>Srinivas Rahul Sapireddy</strong>, Surekha G, Hemanth Bandi<br>
      <em>“Re-Defining R: Resource-Efficient Modulation Classification Using Bin-Based Envelope Features”</em><br>
      <a href="https://ieeemapcon.org/" target="_blank">IEEE Microwaves, Antennas, and Propagation Conference (MAPCON)</a>, , December 14–18, 2025, Kerala, India. 
      <span class="status pending">Submitted</span>
    </div>
    <div class="pub-card">
      <strong>Srinivas Rahul Sapireddy</strong>, Mostafizur Rahman<br>
      <em><a href="https://dl.acm.org/doi/10.1145/3716368.3735217" target="_blank">“On the Effectiveness of Custom Activation Functions on Long-Term Short-Term Memory”</a></em><br>
      <a href="https://dl.acm.org/doi/10.1145/3716368.3735217" target="_blank">ACM Great Lakes Symposium on VLSI (GLSVLSI)</a>, 2025, New Orleans, LA. 
      <span class="status published">Published</span><br>
      <small><em>Session: VLSI for Machine Learning and Artificial Intelligence | Acceptance rate: 27%</em></small><br>
      <a href="/images/PID69.pdf" target="_blank" title="Download PDF">📥</a>
    </div>
    <div class="pub-card">
      <strong>Srinivas Rahul Sapireddy</strong>, Mostafizur Rahman<br>
      <em>
        <a href="https://arxiv.org/abs/2506.19956" target="_blank">
          “Re-Visiting R: Statistical Envelope Analysis for Lightweight Modulation Classification”
        </a>
      </em><br>
      <em>IEEE International Conference on Radio Frequency Communication and Networks (RFCoN)</em>, 2025. 
      <span class="status accepted">🏆 Best Paper Award</span><br>
      <small>
        <em>
          Track 2 | Session II | Paper ID: 718 | Acceptance rate: 12% |
          <span style="color: red; font-weight: bold;">📄 Preprint Available</span>
        </em>
      </small><br>
      <a href="/images/PID718.pdf" target="_blank" title="Download PDF">📥</a>
    </div>
    <div class="pub-card">
      Iqbal, M. A., <strong>Sapireddy, S. R.</strong>, Dasari, S., Asifuzzaman K., Rahman, M.<br>
      <em>“A Review of Crosstalk Polymorphic Circuits and Their Scalability”</em><br>
      <em>Memories – Materials, Devices, Circuits and Systems</em>, vol. 7, article 100094, 2023. 
      <a href="https://doi.org/10.1016/j.memori.2023.100094" target="_blank">[DOI]</a>
      <span class="status published">Published</span>
    </div>
    <div class="pub-card">
      Wafi Danesh, <strong>Srinivas Rahul Sapireddy</strong>, Mostafizur Rahman<br>
      <em>“Understanding and Detecting Adversarial Examples in IoT Networks: A White-Box Analysis with Autoencoders”</em><br>
      <em>MDPI Electronics</em>, 2025.
      <a href="https://doi.org/10.3390/electronics14153015" target="_blank">[DOI]</a>
      <span class="status published">Published</span>
    </div>
    <div class="pub-card">
      <strong>Srinivas Rahul Sapireddy</strong>, Asifuzzaman K., Mostafizur Rahman<br>
      <em>“Simplifying Activations with Linear Approximations in Neural Networks”</em><br>
      <em>Memories – Materials, Devices, Circuits and Systems</em>, 2024.
      <span class="status review">Minor Revision</span>
    </div>
    <div class="pub-card">
      Bhavya Teja Gurijala, <strong>Srinivas Rahul Sapireddy</strong><br>
      <em>“Automation of Patient Medical Record Dispatch System Software Application”</em><br>
      <em>International Journal of Advanced Research in Science, Engineering and Technology (IJARSET)</em>, vol. 5, issue 6, pp. 6074–6097, June 2018.
      <span class="status published">Published</span>
    </div>
    <div class="pub-card">
      <strong>Srinivas Rahul Sapireddy</strong><br>
      <em>“CAM Cell Based Memory Architecture for Extreme Searching Operations”</em><br>
      <em>International Journal of Advances in Electronics & Computer Science</em>, vol. 3, issue 8, pp. 80–83, August 2016.
      <span class="status published">Published</span>
    </div>
    <div class="pub-card">
      <strong>Sapireddy, Srinivas Rahul</strong>, P. N. Tejaswi, Y. M. Sandeep, K. Hari Krishna<br>
      <em>“Two-Stage Operational Amplifier with a Gain Boosted, Source Follower Buffer”</em><br>
      <em>International Journal of Engineering Trends and Technology (IJETT)</em>, vol. 34, no. 6, pp. 256–259, April 2016.
      <span class="status published">Published</span>
    </div>
    <div class="pub-card">
      <strong>Mostafizur Rahman, Arif Iqbal, Srinivas Rahul Sapireddy</strong><br>
      <em>“A Messaging based Intelligent Computing Approach for Machine Learning Applications”</em><br>
      <em>Accessed: Mar, Volume 20</em>, 2024.  
      <span class="status online">📄 Online Archive – computing-lab.com |</span>
    </div>
    <div class="pub-card">
      Satya Sai Siva Rama Krishna Akula, Rownak Chowdhury, <strong>Srinivas Rahul Sapireddy</strong>, Mostafizur Rahman<br>
      <em>“An Opensource Framework for Offloading Big Data and AI Tasks (OFFLOAD) to Heterogeneous Compute Units”</em><br>
      <em>IEEE Transactions on Computer-Aided Design of Integrated Circuits and Systems (TCAD)</em>, 2025.
      <span class="status review">Under Review</span>
    </div>
  </div>

  <div class="logo-row">
  <a href="https://www.ieee.org/" target="_blank" title="IEEE">
    <img src="/images/IEEE.jpg" alt="IEEE Logo" />
  </a>
  <a href="https://www.acm.org/" target="_blank" title="ACM">
    <img src="/images/ACM.png" alt="ACM Logo" />
  </a>
  <a href="https://www.ornl.gov/" target="_blank" title="Oak Ridge National Laboratory">
    <img src="/images/Oak.jpg" alt="ORNL Logo" />
  </a>
  <a href="https://openreview.net/" target="_blank" title="OpenReview">
    <img src="/images/OPEN.jpg" alt="OpenReview Logo" />
  </a>
  <a href="https://orcid.org/0009-0004-6956-0652" target="_blank" title="ORCID">
    <img src="/images/orcid.png" alt="ORCID Logo" />
  </a>
    <a href="https://arxiv.org/search/eess?searchtype=author&query=Sapireddy,+S+R" target="_blank" title="AXVIR">
    <img src="/images/axvir.jpg" alt="AXVIR Logo" />
  </a>
    <a href="https://www.researchgate.net/profile/Srinivas-Rahul-Sapireddy" target="_blank" title="Research Gate">
    <img src="/images/RG.jpg" alt="ResearchGate Logo" />
  </a>
  <a href="https://www.uis.edu/" target="_blank" title="UIS">
    <img src="/images/UIS.png" alt="UIS Logo" />
  </a>
  <a href="https://www.umkc.edu/" target="_blank" title="UMKC">
    <img src="/images/UMKC.png" alt="UMKC Logo" />
  </a>
</div>

</section>

<footer class="pub-footer">
  📘 <a href="https://scholar.google.com/citations?user=08fgpdIAAAAJ&hl=en" target="_blank">Google Scholar</a>
  📝 <a href="https://www.researchgate.net/profile/Srinivas-Rahul-Sapireddy" target="_blank">ResearchGate</a>
  🧬 <a href="https://orcid.org/0009-0004-6956-0652" target="_blank">ORCID</a>
  📝 <a href="https://openreview.net/profile?id=~Srinivas_Rahul_Sapireddy1" target="_blank">OpenReview</a>
</footer>
