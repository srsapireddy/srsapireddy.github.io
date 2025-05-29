---
title: "Publications"
permalink: /publications/
---

<style>
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
</style>

<section id="publications">
  <h2>📚 Publications</h2>

  <div class="pub-grid">
    <!-- (Publication cards remain unchanged) -->
    <!-- Include all the publication <div class="pub-card"> blocks here as before -->
  </div>

  <div class="logo-row">
    <a href="https://www.ieee.org/" target="_blank" title="IEEE">
      <img src="/images/IEEE.jpeg" alt="IEEE Logo" />
    </a>
    <a href="https://www.acm.or/" target="_blank" title="ACM">
      <img src="/images/ACM.png" alt="ACM Logo" />
    </a>
    <a href="https://www.ornl.gov/" target="_blank" title="Oak Ridge National Laboratory">
      <img src="/images/Oak.jpg" alt="ORNL Logo" />
    </a>
    <a href="https://openreview.net/" target="_blank" title="OpenReview">
      <img src="/images/OPEN.jpg" alt="OpenReview Logo" />
    </a>
  </div>
</section>

<footer class="pub-footer">
  📘 <a href="https://scholar.google.com/citations?user=08fgpdIAAAAJ&hl=en" target="_blank">Google Scholar</a>
  🧬 <a href="https://orcid.org/0000-0002-9898-6810" target="_blank">ORCID</a>
  📝 <a href="https://openreview.net/profile?id=~Srinivas_Rahul_Sapireddy1" target="_blank">OpenReview</a>
</footer>
