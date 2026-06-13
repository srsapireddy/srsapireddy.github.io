---
title: "Publications"
layout: single
permalink: /publications/
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

.pub-wrap{
  animation:fadeInUp 0.8s ease-in-out;
}

/* Hero */
.pub-hero{
  position:relative;
  overflow:hidden;
  border-radius:var(--radius);
  padding:2.25rem 2rem;
  margin-bottom:1.25rem;
  background:
    radial-gradient(circle at top right, rgba(220,20,60,0.13), transparent 32%),
    linear-gradient(135deg,#e9f3ff 0%, #ffffff 62%);
  border:1px solid rgba(26,115,232,0.25);
  box-shadow:var(--shadow);
}

.pub-hero::before{
  content:"";
  position:absolute;
  inset:0;
  background-image:
    linear-gradient(rgba(26,115,232,0.06) 1px, transparent 1px),
    linear-gradient(90deg, rgba(26,115,232,0.06) 1px, transparent 1px);
  background-size:34px 34px;
  pointer-events:none;
}

.pub-hero-content{
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

.pub-hero h1{
  margin:0;
  font-size:2.15rem;
  line-height:1.15;
  color:var(--text);
}

.pub-hero .subtitle{
  margin-top:0.55rem;
  color:#202124;
  font-size:1.08rem;
  font-weight:650;
}

.pub-hero p{
  margin:0.8rem 0 0 0;
  color:var(--muted);
  font-size:1.03rem;
  line-height:1.65;
  max-width:90ch;
}

.hero-links{
  display:flex;
  flex-wrap:wrap;
  gap:0.7rem;
  margin-top:1.15rem;
}

.btn-link{
  display:inline-flex;
  align-items:center;
  gap:0.45rem;
  padding:0.58rem 0.92rem;
  border-radius:12px;
  background:var(--blue);
  color:#ffffff !important;
  text-decoration:none !important;
  font-weight:850;
  box-shadow:var(--shadow2);
  transition:0.2s ease-in-out;
}

.btn-link:hover{
  background:var(--blue2);
  transform:translateY(-2px);
  text-decoration:none !important;
}

.btn-link.secondary{
  background:#ffffff;
  color:var(--blue) !important;
  border:1px solid rgba(26,115,232,0.25);
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
  gap:0.9rem;
  margin-bottom:1.3rem;
}

.impact-card{
  text-align:center;
  padding:1.05rem 0.9rem;
  border-radius:var(--radius2);
  background:linear-gradient(135deg,#ffffff 0%,#f7fbff 100%);
  border:1px solid var(--border);
  box-shadow:var(--shadow2);
  transition:0.22s ease-in-out;
}

.impact-card:hover{
  transform:translateY(-3px);
  box-shadow:var(--shadow);
}

.impact-card .big{
  color:var(--isu);
  font-size:1.55rem;
  font-weight:950;
  line-height:1.1;
}

.impact-card .label{
  color:var(--text);
  font-weight:850;
  margin-top:0.35rem;
  font-size:0.92rem;
}

.impact-card .small{
  color:var(--muted);
  font-size:0.8rem;
  margin-top:0.2rem;
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

/* Research focus cards */
.grid-3{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:1.1rem;
  margin-bottom:1.3rem;
}

.focus-card{
  position:relative;
  overflow:hidden;
  padding:1.25rem;
  border-radius:16px;
  background:linear-gradient(135deg,#ffffff 0%,#f4f9ff 100%);
  border:1px solid var(--border);
  box-shadow:var(--shadow2);
  transition:0.25s ease-in-out;
}

.focus-card:hover{
  transform:translateY(-4px);
  box-shadow:var(--shadow);
}

.focus-card::before{
  content:"";
  position:absolute;
  top:0;
  left:0;
  height:5px;
  width:100%;
  background:linear-gradient(90deg,var(--blue),var(--isu));
}

.focus-icon{
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

.focus-card h3{
  margin:0 0 0.55rem 0;
  font-size:1.12rem;
  color:var(--text);
}

.focus-card p{
  margin:0;
  color:#202124;
  line-height:1.55;
  font-size:0.95rem;
}

/* Tags */
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

/* Filter tabs */
.pub-tabs{
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

/* Year blocks */
.year-section{
  margin-top:1rem;
  padding-top:0.3rem;
}

.year-header{
  display:flex;
  justify-content:space-between;
  align-items:center;
  gap:1rem;
  margin:1.2rem 0 0.9rem 0;
  padding:0.9rem 1rem;
  border-radius:14px;
  background:linear-gradient(135deg,#f7fbff 0%,#ffffff 100%);
  border:1px solid rgba(26,115,232,0.18);
}

.year-title{
  display:inline-flex;
  align-items:center;
  gap:0.55rem;
  font-size:1.22rem;
  font-weight:950;
  color:var(--text);
}

.year-pill{
  display:inline-flex;
  padding:0.3rem 0.75rem;
  border-radius:999px;
  background:rgba(220,20,60,0.08);
  border:1px solid rgba(220,20,60,0.22);
  color:var(--isu);
  font-weight:900;
  font-size:0.85rem;
}

/* Publication cards */
.publication-card{
  position:relative;
  padding:1.15rem 1.15rem 1.15rem 1.35rem;
  border-radius:16px;
  background:#ffffff;
  border:1px solid var(--border);
  box-shadow:var(--shadow2);
  margin-bottom:1rem;
  transition:0.22s ease-in-out;
}

.publication-card:hover{
  transform:translateY(-3px);
  box-shadow:var(--shadow);
  background:#fbfdff;
}

.publication-card::before{
  content:"";
  position:absolute;
  left:0;
  top:1rem;
  bottom:1rem;
  width:4px;
  border-radius:99px;
  background:linear-gradient(180deg,var(--blue),var(--isu));
}

.publication-card.placeholder{
  background:linear-gradient(135deg,#ffffff 0%,#fffaf2 100%);
  border-color:rgba(122,90,0,0.20);
}

.publication-card.placeholder::before{
  background:#b7791f;
}

.pub-top{
  display:flex;
  flex-wrap:wrap;
  gap:0.55rem;
  align-items:center;
  margin-bottom:0.65rem;
}

.pub-year,
.pub-type,
.pub-award,
.pub-status{
  display:inline-flex;
  padding:0.25rem 0.58rem;
  border-radius:999px;
  font-size:0.78rem;
  font-weight:900;
}

.pub-year{
  background:#f3f8ff;
  border:1px solid rgba(26,115,232,0.18);
  color:var(--blue);
}

.pub-type{
  background:#ffffff;
  border:1px solid rgba(26,115,232,0.20);
  color:var(--text);
}

.pub-award{
  background:rgba(220,20,60,0.08);
  border:1px solid rgba(220,20,60,0.25);
  color:var(--isu);
}

.pub-status{
  background:#fff6e6;
  border:1px solid rgba(122,90,0,0.25);
  color:#7a5a00;
}

.pub-title{
  color:var(--text);
  font-size:1.05rem;
  font-weight:950;
  line-height:1.45;
  margin-bottom:0.45rem;
}

.pub-authors{
  color:#202124;
  font-size:0.94rem;
  line-height:1.5;
  margin-bottom:0.35rem;
}

.pub-venue{
  color:var(--muted);
  font-size:0.92rem;
  line-height:1.45;
}

.pub-note{
  margin-top:0.55rem;
  color:#475569;
  font-size:0.9rem;
  line-height:1.55;
}

/* Buttons */
.pub-links{
  display:flex;
  flex-direction:row;
  flex-wrap:wrap;
  gap:0.55rem;
  margin-top:0.85rem;
  align-items:center;
}

.pub-link,
.pub-button{
  display:inline-flex;
  align-items:center;
  justify-content:center;
  padding:0.36rem 0.72rem;
  border-radius:999px;
  background:#f3f8ff;
  border:1px solid rgba(26,115,232,0.18);
  color:var(--blue) !important;
  text-decoration:none !important;
  font-size:0.84rem;
  font-weight:850;
  cursor:pointer;
  line-height:1.2;
  white-space:nowrap;
}

.pub-link:hover,
.pub-button:hover{
  background:#e9f3ff;
  text-decoration:none !important;
}

.pub-button.primary{
  background:var(--blue);
  color:#ffffff !important;
  border-color:var(--blue);
}

.pub-button.primary:hover{
  background:var(--blue2);
}

.pub-link.disabled{
  opacity:0.55;
  cursor:not-allowed;
}

.citation-box{
  display:none;
  margin-top:0.8rem;
  padding:0.9rem;
  border-radius:12px;
  background:#f7fbff;
  border:1px solid rgba(26,115,232,0.18);
  color:#202124;
  font-size:0.88rem;
  line-height:1.55;
  white-space:pre-wrap;
  overflow-x:auto;
}

/* Timeline/profile grid */
.grid-2{
  display:grid;
  grid-template-columns:1fr;
  gap:1.2rem;
}

.timeline{
  position:relative;
  margin-top:0.3rem;
  padding-left:1.3rem;
}

.timeline::before{
  content:"";
  position:absolute;
  left:0.25rem;
  top:0.2rem;
  bottom:0.2rem;
  width:2px;
  background:linear-gradient(180deg,var(--blue),var(--isu));
}

.timeline-item{
  position:relative;
  margin-bottom:1rem;
  padding-left:1rem;
}

.timeline-item::before{
  content:"";
  position:absolute;
  left:-1.29rem;
  top:0.25rem;
  width:11px;
  height:11px;
  border-radius:50%;
  background:var(--isu);
  border:3px solid #ffffff;
  box-shadow:0 0 0 2px rgba(220,20,60,0.22);
}

.timeline-year{
  color:var(--isu);
  font-weight:900;
  font-size:0.88rem;
}

.timeline-title{
  color:var(--text);
  font-weight:900;
  margin-top:0.1rem;
}

.timeline-text{
  color:#202124;
  margin-top:0.15rem;
  line-height:1.5;
}

/* Filtering */
.publication-card.hide-card,
.year-section.hide-year{
  display:none;
}

/* Responsive */
@media (min-width:900px){
  .grid-2{
    grid-template-columns:1fr 1fr;
  }
}

@media (max-width:950px){
  .grid-3,
  .impact-grid{
    grid-template-columns:1fr 1fr;
  }
}

@media (max-width:600px){
  .pub-hero{
    padding:1.5rem 1.1rem;
  }

  .pub-hero h1{
    font-size:1.65rem;
  }

  .grid-3,
  .impact-grid{
    grid-template-columns:1fr;
  }

  .year-header{
    align-items:flex-start;
    flex-direction:column;
  }
}

/* Scoped links */
.section a,
.pub-hero a{
  color:var(--blue);
  font-weight:800;
  text-decoration:none;
}

.section a:hover,
.pub-hero a:hover{
  text-decoration:underline;
}

.research-map-section {
  width: 100%;
  padding: 2.5rem 1rem;
  background: linear-gradient(135deg, #ffffff 0%, #f7f9fc 100%);
  border-radius: 22px;
  overflow: hidden;
}

.research-map-header {
  text-align: center;
  margin-bottom: 1.5rem;
}

.research-map-kicker {
  display: inline-block;
  padding: 0.35rem 0.8rem;
  border-radius: 999px;
  background: #eef5ff;
  color: #0b5bd3;
  font-weight: 800;
  font-size: 0.85rem;
  margin-bottom: 0.6rem;
}

.research-map-header h2 {
  margin: 0;
  font-size: 2rem;
  color: #0b1f44;
  font-weight: 950;
}

.research-map-header p {
  margin: 0.45rem auto 0;
  color: #5f6368;
  max-width: 680px;
  line-height: 1.55;
}

/* Main canvas */
.mindmap-wrap {
  position: relative;
  width: 100%;
  max-width: 1180px;
  height: 900px;
  margin: 0 auto;
  background:
    radial-gradient(circle at center, rgba(11,31,68,0.05), transparent 34%),
    #ffffff;
  border-radius: 24px;
  box-shadow: 0 18px 45px rgba(0,0,0,0.08);
  overflow: hidden;
}

/* Center circle */
.mind-center {
  position: absolute;
  left: 50%;
  top: 50%;
  width: 220px;
  height: 220px;
  transform: translate(-50%, -50%);
  border-radius: 50%;
  background: radial-gradient(circle at 35% 30%, #173a63 0%, #06182b 75%);
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 10;
  box-shadow: 0 18px 40px rgba(0,0,0,0.28);
}

.center-title {
  color: #ffffff;
  font-size: 2rem;
  line-height: 1.15;
  font-weight: 950;
  text-align: center;
}

/* Shared cluster styles */
.cluster {
  position: absolute;
  z-index: 3;
}

.cluster::before {
  content: "";
  position: absolute;
  z-index: -1;
  filter: blur(0.1px);
}

.cluster-core,
.node {
  position: absolute;
  border-radius: 50%;
  color: #ffffff;
  text-align: center;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: 900;
  line-height: 1.18;
  box-shadow: 0 12px 30px rgba(0,0,0,0.12);
}

.cluster-core {
  width: 210px;
  height: 210px;
  font-size: 1.55rem;
  z-index: 3;
}

.node {
  width: 135px;
  height: 135px;
  font-size: 0.98rem;
  z-index: 4;
  padding: 0.45rem;
}

.node span {
  display: block;
  font-weight: 850;
  font-size: 0.88rem;
  margin-top: 0.15rem;
}

/* ================= RF cluster ================= */
.rf-cluster {
  left: 4%;
  top: 2%;
  width: 520px;
  height: 420px;
}

.rf-cluster::before {
  left: 230px;
  top: 190px;
  width: 310px;
  height: 60px;
  background: linear-gradient(90deg, #ff7a00, #06182b);
  transform: rotate(48deg);
  border-radius: 60px;
}

.rf-cluster .cluster-core,
.rf-cluster .node {
  background: linear-gradient(135deg, #ff8c00 0%, #f06a00 100%);
}

.rf-cluster .cluster-core {
  left: 205px;
  top: 150px;
}

.rf-cluster .n1 { left: 70px; top: 10px; }
.rf-cluster .n2 { left: 250px; top: 0; }
.rf-cluster .n3 { left: 390px; top: 100px; }
.rf-cluster .n4 { left: 400px; top: 250px; }
.rf-cluster .n5 { left: 25px; top: 255px; }
.rf-cluster .n6 { left: 0; top: 105px; }

/* Organic connectors for RF */
.rf-cluster .cluster-core::before,
.rf-cluster .cluster-core::after {
  content: "";
  position: absolute;
  background: #f57700;
  border-radius: 999px;
  z-index: -1;
}

.rf-cluster .cluster-core::before {
  width: 420px;
  height: 42px;
  left: -110px;
  top: 83px;
  transform: rotate(-22deg);
}

.rf-cluster .cluster-core::after {
  width: 390px;
  height: 42px;
  left: -80px;
  top: 90px;
  transform: rotate(42deg);
}

/* ================= AI cluster ================= */
.ai-cluster {
  right: 4%;
  top: 3%;
  width: 480px;
  height: 390px;
}

.ai-cluster::before {
  right: 245px;
  top: 255px;
  width: 270px;
  height: 60px;
  background: linear-gradient(90deg, #06182b, #0072ce);
  transform: rotate(-56deg);
  border-radius: 60px;
}

.ai-cluster .cluster-core,
.ai-cluster .node {
  background: linear-gradient(135deg, #0078d7 0%, #0053b8 100%);
}

.ai-cluster .cluster-core {
  left: 105px;
  top: 155px;
}

.ai-cluster .n1 { left: 220px; top: 0; }
.ai-cluster .n2 { left: 365px; top: 110px; }
.ai-cluster .n3 { left: 330px; top: 260px; }

.ai-cluster .cluster-core::before,
.ai-cluster .cluster-core::after {
  content: "";
  position: absolute;
  background: #0068c8;
  border-radius: 999px;
  z-index: -1;
}

.ai-cluster .cluster-core::before {
  width: 315px;
  height: 42px;
  left: 55px;
  top: 75px;
  transform: rotate(-25deg);
}

.ai-cluster .cluster-core::after {
  width: 310px;
  height: 42px;
  left: 75px;
  top: 95px;
  transform: rotate(34deg);
}

/* ================= Cyber cluster ================= */
.cyber-cluster {
  left: 2%;
  top: 48%;
  width: 430px;
  height: 350px;
}

.cyber-cluster::before {
  left: 285px;
  top: 75px;
  width: 255px;
  height: 60px;
  background: linear-gradient(90deg, #e11616, #06182b);
  transform: rotate(-16deg);
  border-radius: 60px;
}

.cyber-cluster .cluster-core,
.cyber-cluster .node {
  background: linear-gradient(135deg, #f51d1d 0%, #c90000 100%);
}

.cyber-cluster .cluster-core {
  left: 205px;
  top: 90px;
}

.cyber-cluster .n1 { left: 10px; top: 0; }
.cyber-cluster .n2 { left: 0; top: 180px; }

.cyber-cluster .cluster-core::before,
.cyber-cluster .cluster-core::after {
  content: "";
  position: absolute;
  background: #e11212;
  border-radius: 999px;
  z-index: -1;
}

.cyber-cluster .cluster-core::before {
  width: 260px;
  height: 42px;
  left: -150px;
  top: 55px;
  transform: rotate(22deg);
}

.cyber-cluster .cluster-core::after {
  width: 250px;
  height: 42px;
  left: -145px;
  top: 118px;
  transform: rotate(-35deg);
}

/* ================= VLSI cluster ================= */
.vlsi-cluster {
  right: 2%;
  top: 49%;
  width: 470px;
  height: 350px;
}

.vlsi-cluster::before {
  right: 290px;
  top: 75px;
  width: 255px;
  height: 60px;
  background: linear-gradient(90deg, #06182b, #5b3bb6);
  transform: rotate(18deg);
  border-radius: 60px;
}

.vlsi-cluster .cluster-core,
.vlsi-cluster .node {
  background: linear-gradient(135deg, #7251d1 0%, #4e32a3 100%);
}

.vlsi-cluster .cluster-core {
  left: 60px;
  top: 90px;
}

.vlsi-cluster .n1 { left: 330px; top: 0; }
.vlsi-cluster .n2 { left: 355px; top: 150px; }
.vlsi-cluster .n3 { left: 205px; top: 245px; }

.vlsi-cluster .cluster-core::before,
.vlsi-cluster .cluster-core::after {
  content: "";
  position: absolute;
  background: #5b3bb6;
  border-radius: 999px;
  z-index: -1;
}

.vlsi-cluster .cluster-core::before {
  width: 300px;
  height: 42px;
  left: 105px;
  top: 65px;
  transform: rotate(-18deg);
}

.vlsi-cluster .cluster-core::after {
  width: 330px;
  height: 42px;
  left: 95px;
  top: 130px;
  transform: rotate(28deg);
}

/* ================= Applied cluster ================= */
.applied-cluster {
  left: 50%;
  bottom: 2%;
  width: 480px;
  height: 330px;
  transform: translateX(-50%);
}

.applied-cluster::before {
  left: 210px;
  bottom: 250px;
  width: 60px;
  height: 220px;
  background: linear-gradient(180deg, #06182b, #008c68);
  border-radius: 60px;
}

.applied-cluster .cluster-core,
.applied-cluster .node {
  background: linear-gradient(135deg, #00a77a 0%, #007f5f 100%);
}

.applied-cluster .cluster-core {
  left: 135px;
  top: 0;
}

.applied-cluster .n1 { left: 0; top: 185px; }
.applied-cluster .n2 { left: 300px; top: 185px; }

.applied-cluster .cluster-core::before,
.applied-cluster .cluster-core::after {
  content: "";
  position: absolute;
  background: #008c68;
  border-radius: 999px;
  z-index: -1;
}

.applied-cluster .cluster-core::before {
  width: 230px;
  height: 40px;
  left: -105px;
  top: 145px;
  transform: rotate(35deg);
}

.applied-cluster .cluster-core::after {
  width: 230px;
  height: 40px;
  left: 85px;
  top: 145px;
  transform: rotate(-35deg);
}

/* ================= Responsive ================= */
@media (max-width: 950px) {
  .mindmap-wrap {
    height: auto;
    padding: 2rem 1rem;
    display: flex;
    flex-direction: column;
    gap: 1.4rem;
  }

  .mind-center,
  .cluster,
  .cluster-core,
  .node {
    position: relative;
    left: auto !important;
    right: auto !important;
    top: auto !important;
    bottom: auto !important;
    transform: none !important;
  }

  .mind-center {
    order: 0;
    margin: 0 auto;
    width: 190px;
    height: 190px;
  }

  .center-title {
    font-size: 1.65rem;
  }

  .cluster {
    width: 100%;
    height: auto;
    display: grid;
    grid-template-columns: 1fr;
    justify-items: center;
    gap: 0.75rem;
  }

  .cluster::before,
  .cluster-core::before,
  .cluster-core::after {
    display: none;
  }

  .cluster-core {
    width: 190px;
    height: 190px;
    font-size: 1.35rem;
    margin-bottom: 0.25rem;
  }

  .node {
    width: min(92%, 330px);
    height: auto;
    min-height: 70px;
    border-radius: 22px;
    font-size: 0.95rem;
  }
}
</style>

<div class="pub-wrap">

  <div class="pub-hero">
    <div class="pub-hero-content">
      <span class="hero-kicker">Research Publications · RF · AI · VLSI · Edge Systems</span>

      <h1>Publications</h1>

      <div class="subtitle">
        Selected publications and research outputs organized year by year
      </div>

      <p>
        This page presents selected journal articles, conference papers, accepted manuscripts,
        awarded research contributions, and earlier research outputs across RF signal intelligence,
        hardware-aware AI, VLSI systems, edge computing, and secure intelligent systems.
      </p>

      <div class="hero-links">
        <a class="btn-link" href="https://scholar.google.com/citations?user=08fgpdIAAAAJ" target="_blank" rel="noopener">Google Scholar</a>
        <a class="btn-link secondary" href="https://orcid.org/0000-0002-9898-6810" target="_blank" rel="noopener">ORCID</a>
        <a class="btn-link secondary" href="https://openreview.net/profile?id=~Srinivas_Rahul_Sapireddy1" target="_blank" rel="noopener">OpenReview</a>
        <a class="btn-link secondary" href="/resume/">Resume</a>
      </div>
    </div>
  </div>

  <div class="sliding-bar">
    <div class="slide-track">
      <div class="slide-item"><span>●</span> RF Modulation Classification</div>
      <div class="slide-item"><span>●</span> Hardware-Aware AI</div>
      <div class="slide-item"><span>●</span> Custom Activation Functions</div>
      <div class="slide-item"><span>●</span> GPS Spoofing Detection</div>
      <div class="slide-item"><span>●</span> IoT Security</div>
      <div class="slide-item"><span>●</span> RF Fingerprinting</div>
      <div class="slide-item"><span>●</span> VLSI and Edge Systems</div>

      <div class="slide-item"><span>●</span> RF Modulation Classification</div>
      <div class="slide-item"><span>●</span> Hardware-Aware AI</div>
      <div class="slide-item"><span>●</span> Custom Activation Functions</div>
      <div class="slide-item"><span>●</span> GPS Spoofing Detection</div>
      <div class="slide-item"><span>●</span> IoT Security</div>
      <div class="slide-item"><span>●</span> RF Fingerprinting</div>
      <div class="slide-item"><span>●</span> VLSI and Edge Systems</div>
    </div>
  </div>

  <div class="impact-grid">
    <div class="impact-card">
      <div class="big">2026</div>
      <div class="label">Published Work</div>
      <div class="small">IEEE SoutheastCon</div>
    </div>

    <div class="impact-card">
      <div class="big">2025</div>
      <div class="label">Major Output Year</div>
      <div class="small">RF, AI, Security, VLSI</div>
    </div>

    <div class="impact-card">
      <div class="big">2024</div>
      <div class="label">Journal Publications</div>
      <div class="small">Activations and circuits</div>
    </div>

    <div class="impact-card">
      <div class="big">Earlier</div>
      <div class="label">Prior Research Outputs</div>
      <div class="small">2018 and 2016 entries</div>
    </div>
  </div>

  <div class="grid-3">
    <div class="focus-card">
      <div class="focus-icon">📡</div>
      <h3>RF Signal Intelligence</h3>
      <p>
        Publications on modulation classification, envelope statistics, GPS spoofing detection,
        RF fingerprinting, and signal-processing methods.
      </p>
    </div>

    <div class="focus-card">
      <div class="focus-icon">🧠</div>
      <h3>Hardware-Aware AI</h3>
      <p>
        Research on lightweight neural networks, custom activation functions, model efficiency,
        and deployment-aware learning.
      </p>
    </div>

    <div class="focus-card">
      <div class="focus-icon">⚙️</div>
      <h3>VLSI and Edge Systems</h3>
      <p>
        Work related to hardware acceleration, physical design, VLSI-oriented systems,
        and efficient embedded intelligence.
      </p>
    </div>
  </div>

  <div class="section">
    <h2>🧭 Research Themes</h2>
    <div class="divider"></div>

    <div class="tag-cloud">
      <span class="tag">RF Modulation Classification</span>
      <span class="tag">Envelope Statistics</span>
      <span class="tag">R-Value Features</span>
      <span class="tag">CAF-Based Feature Extraction</span>
      <span class="tag">STFT-Based Analysis</span>
      <span class="tag">GPS Spoofing Detection</span>
      <span class="tag">Hardware-Aware AI</span>
      <span class="tag">Custom Activation Functions</span>
      <span class="tag">LSTM Optimization</span>
      <span class="tag">Edge AI</span>
      <span class="tag">VLSI Design</span>
      <span class="tag">IoT Security</span>
      <span class="tag">RF Fingerprinting</span>
      <span class="tag">Polymorphic Circuits</span>
    </div>
  </div>

    <!-- ================= Research Mind Map Section ================= -->
  <section class="research-map-section">
    <div class="research-map-header">
      <span class="research-map-kicker">Research Portfolio</span>
      <h2>Research Mind Map</h2>
      <p>
        A visual overview of publications grouped by research direction.
      </p>
    </div>
  
    <div class="mindmap-wrap">
  
      <!-- Center -->
      <div class="mind-center">
        <div class="center-title">S. R. Sapireddy</div>
      </div>
  
      <!-- RF Signal Intelligence -->
      <div class="cluster rf-cluster">
        <div class="cluster-core">
          RF Signal<br>Intelligence
        </div>
  
        <div class="node n1">Bin-Based R<br><span>[SoutheastCon ’26]</span></div>
        <div class="node n2">Revisiting R<br><span>[RFCoN ’25]</span></div>
        <div class="node n3">Spread Spectrum<br>Classification<br><span>[MILCOM ’26]</span></div>
        <div class="node n4">Signal Detection &<br>Classification<br><span>[AeroConf ’26]</span></div>
        <div class="node n5">R2ML: Interpretable<br>RF Classification<br><span>[COMNETSAT ’26]</span></div>
        <div class="node n6">Ph.D. Dissertation<br><span>[UMKC ’25]</span></div>
      </div>
  
      <!-- Hardware-Aware AI -->
      <div class="cluster ai-cluster">
        <div class="cluster-core">
          Hardware-<br>Aware AI
        </div>
  
        <div class="node n1">Linear Activation<br>Approximations<br><span>[Memories ’25]</span></div>
        <div class="node n2">Piecewise Activations<br>for LSTM<br><span>[GLSVLSI ’25]</span></div>
        <div class="node n3">Low-Power<br>Deep Learning<br><span>[Dissertation ’25]</span></div>
      </div>
  
      <!-- Cyber / IoT -->
      <div class="cluster cyber-cluster">
        <div class="cluster-core">
          Cyber, IoT &<br>Situational<br>Awareness
        </div>
  
        <div class="node n1">Adversarial Examples<br>in IoT Networks<br><span>[Electronics ’25]</span></div>
        <div class="node n2">CARS: Cyber<br>Situational Awareness<br><span>[AISSC ’27]</span></div>
      </div>
  
      <!-- VLSI / Circuits -->
      <div class="cluster vlsi-cluster">
        <div class="cluster-core">
          VLSI, Circuits &<br>Architectures
        </div>
  
        <div class="node n1">Crosstalk Polymorphic<br>Circuits<br><span>[Memories ’24]</span></div>
        <div class="node n2">CAM Cell Memory<br>Architecture<br><span>[IJAECS ’16]</span></div>
        <div class="node n3">Two-Stage Operational<br>Amplifier<br><span>[IJETT ’16]</span></div>
      </div>
  
      <!-- Applied Intelligent Systems -->
      <div class="cluster applied-cluster">
        <div class="cluster-core">
          Applied<br>Intelligent<br>Systems
        </div>
  
        <div class="node n1">Messaging-Based<br>Intelligent Computing<br><span>[2024]</span></div>
        <div class="node n2">Medical Record<br>Dispatch System<br><span>[IJARSET ’18]</span></div>
      </div>
  
    </div>
  </section>

  <div class="section">
    <h2>📚 Publications by Year</h2>
    <div class="divider"></div>

    <p>
      The list below is grouped by year while remaining on one continuous page. Use the filters for quick navigation.
    </p>

    <div class="pub-tabs">
      <button class="tab-button active" onclick="filterPublications(event, 'all')">All</button>
      <button class="tab-button" onclick="filterPublications(event, 'conference')">Conference</button>
      <button class="tab-button" onclick="filterPublications(event, 'journal')">Journal</button>
      <button class="tab-button" onclick="filterPublications(event, 'award')">Awarded / Recognized</button>
      <button class="tab-button" onclick="filterPublications(event, 'thesis')">Dissertation / Thesis</button>
      <button class="tab-button" onclick="filterPublications(event, 'earlier')">Earlier Work</button>
    </div>
        </div>

      <div class="year-section" data-year-section="2027">
    <div class="year-header">
      <div class="year-title">📅 2027 Publications</div>
      <div class="year-pill">To be submitted publications</div>
    </div>
              <div class="publication-card" data-type="conference">
      <div class="pub-top">
        <span class="pub-year">2027</span>
        <span class="pub-type">IEEE Conference</span>
        <span class="pub-award">To be submitted</span>
      </div>
  
      <div class="pub-title">
        CARS: From Traffic Signals to Cyber Situational Awareness
      </div>
  
      <div class="pub-authors">
        S. R. Sapireddy et al.
      </div>
  
      <div class="pub-venue">
        International Conference on Advances in Intelligence Systems, Security, and Cybernetics, 29–30 January 2027.
      </div>
  
      <div class="pub-note">
        DOI: Pending
      </div>
  
      <div class="pub-links">
        <button class="pub-button primary" onclick="toggleCitation('cite-2027-aissc-cars')">Citation</button>
        <button class="pub-button" onclick="copyCitation('cite-2027-aissc-cars')">Copy Citation</button>
        <a class="pub-link disabled" href="#" onclick="return false;">DOI pending</a>
        <a class="pub-link disabled" href="#" onclick="return false;">PDF pending</a>
      </div>
  
       <div id="cite-2027-aissc-cars" class="citation-box">Under Review</div>
    </div>
      </div>
  
    <!-- Full title: R2ML: Interpretable Machine Learning for R-Value-Based RF Modulation Classification -->

    <div class="year-section" data-year-section="2026">
      <div class="year-header">
        <div class="year-title">📅 2026 Publications</div>
        <div class="year-pill">1 publication</div>
    </div>

    <div class="publication-card" data-type="conference">
      <div class="pub-top">
        <span class="pub-year">2026</span>
        <span class="pub-type">IEEE Conference</span>
        <span class="pub-award">Under Review</span>
      </div>
    
      <div class="pub-title">
        Lightweight Methods for Spread Spectrum Signal Classification
      </div>
    
      <div class="pub-authors">
        Srinivas Rahul Sapireddy and Mostafizur Rahman
      </div>
    
      <div class="pub-venue">
        Military Communications (MILCOM), National Capital Region, USA, 12 - 16 October 2026.
      </div>
    
      <div class="pub-note">
        DOI: Pending
      </div>
    
      <div class="pub-links">
        <button class="pub-button primary" onclick="toggleCitation('cite-2026-milcom-spread-spectrum')">Citation</button>
        <button class="pub-button" onclick="copyCitation('cite-2026-milcom-spread-spectrum')">Copy Citation</button>
        <a class="pub-link disabled" href="#" onclick="return false;">DOI pending</a>
        <a class="pub-link disabled" href="#" onclick="return false;">PDF pending</a>
      </div>
    
      <div id="cite-2026-milcom-spread-spectrum" class="citation-box">Under Review</div>
    </div>
    
    <div class="publication-card" data-type="conference">
      <div class="pub-top">
        <span class="pub-year">2026</span>
        <span class="pub-type">IEEE Conference</span>
        <span class="pub-award">To be submitted</span>
      </div>
    
      <div class="pub-title">
        Signal Detection and Classification in the Presence of Interference
      </div>
    
      <div class="pub-authors">
        Marcus Butler, Donald Riead, Srinivas Rahul Sapireddy, and Mostafizur Rahman
      </div>
    
      <div class="pub-venue">
        IEEE Aerospace Conference (AeroConf), Big Sky, Montana, USA, 7 March 2026 – 14 March 2026.
      </div>
    
      <div class="pub-note">
        DOI: Pending
      </div>
    
      <div class="pub-links">
        <button class="pub-button primary" onclick="toggleCitation('cite-2026-aero-interference')">Citation</button>
        <button class="pub-button" onclick="copyCitation('cite-2026-aero-interference')">Copy Citation</button>
        <a class="pub-link disabled" href="#" onclick="return false;">DOI pending</a>
        <a class="pub-link disabled" href="#" onclick="return false;">PDF pending</a>
      </div>
    
      <div id="cite-2026-milcom-interference" class="citation-box">M. Butler, D. Riead, S. R. Sapireddy, and M. Rahman, "Signal Detection and Classification in the Presence of Interference," Military Communications (MILCOM), National Capital Region, USA, 2026.</div>
    </div>

             <div class="publication-card" data-type="conference">
      <div class="pub-top">
        <span class="pub-year">2027</span>
        <span class="pub-type">IEEE Conference</span>
        <span class="pub-award">To be submitted</span>
      </div>
  
      <div class="pub-title">
        R2ML: Interpretable RF Modulation Classification
      </div>
  
      <div class="pub-authors">
        S. R. Sapireddy et al.
      </div>
  
      <div class="pub-venue">
        IEEE International Conference on Communications, Networks, and Satellite (COMNETSAT), Manado, Indonesia, 3–5 December 2026.
      </div>
  
      <div class="pub-note">
        DOI: Pending
      </div>
  
      <div class="pub-links">
        <button class="pub-button primary" onclick="toggleCitation('cite-2026-comnetsat-r2ml')">Citation</button>
        <button class="pub-button" onclick="copyCitation('cite-2026-comnetsat-r2ml')">Copy Citation</button>
        <a class="pub-link disabled" href="#" onclick="return false;">DOI pending</a>
        <a class="pub-link disabled" href="#" onclick="return false;">PDF pending</a>
      </div>
  
      <div id="cite-2026-comnetsat-r2ml" class="citation-box">
        S. R. Sapireddy et al., "R2ML: Interpretable RF Modulation Classification," IEEE International Conference on Communications, Networks, and Satellite (COMNETSAT), Manado, Indonesia, 2026.
      </div>
    </div>
  
    <!-- Full title: CARS: From Traffic Signals to Cyber Situational Awareness -->
    
    <div class="publication-card" data-type="conference">
      <div class="pub-top">
        <span class="pub-year">2026</span>
        <span class="pub-type">IEEE Conference</span>
        <span class="pub-award">Published</span>
      </div>
    
      <div class="pub-title">
        Bin-Based R: Resource-Efficient RF Modulation Classification Using Envelope Statistics
      </div>
    
      <div class="pub-authors">
        S. R. Sapireddy, G. Surekha, and H. Bandi
      </div>
    
      <div class="pub-venue">
        SoutheastCon 2026, Huntsville, AL, USA, 2026, pp. 1-6.
      </div>
    
      <div class="pub-note">
        DOI: 10.1109/SoutheastCon63549.2026.11476603
      </div>
    
      <div class="pub-links">
        <button class="pub-button primary" onclick="toggleCitation('cite-2026-southeastcon-bin-r')">Citation</button>
        <button class="pub-button" onclick="copyCitation('cite-2026-southeastcon-bin-r')">Copy Citation</button>
        <a class="pub-link" href="https://doi.org/10.1109/SoutheastCon63549.2026.11476603" target="_blank" rel="noopener">DOI</a>
        <a class="pub-link" href="https://srsapireddy.github.io/publications/C3.pdf" target="_blank" rel="noopener">PDF</a>
      </div>
    
      <div id="cite-2026-southeastcon-bin-r" class="citation-box">S. R. Sapireddy, G. Surekha, and H. Bandi, "Bin-Based R: Resource-Efficient RF Modulation Classification Using Envelope Statistics," SoutheastCon 2026, Huntsville, AL, USA, 2026, pp. 1-6, doi: 10.1109/SoutheastCon63549.2026.11476603.</div>
    </div>

    <div class="year-section" data-year-section="2025">
      <div class="year-header">
        <div class="year-title">📅 2025 Publications</div>
        <div class="year-pill">6 publications</div>
      </div>

      <div class="publication-card" data-type="journal">
        <div class="pub-top">
          <span class="pub-year">2025</span>
          <span class="pub-type">Journal Article</span>
          <span class="pub-award">Published</span>
        </div>
      
        <div class="pub-title">
          Simplifying Activations with Linear Approximations in Neural Networks
        </div>
      
        <div class="pub-authors">
          Srinivas Rahul Sapireddy, Kazi Asifuzzaman, and Rahman Mostafizur
        </div>
      
        <div class="pub-venue">
          Memories - Materials, Devices, Circuits and Systems, Volume 11, 2025, Article 100134.
        </div>
      
        <div class="pub-note">
          ISSN: 2773-0646 | DOI: 10.1016/j.memori.2025.100134
        </div>
      
        <div class="pub-links">
          <button class="pub-button primary" onclick="toggleCitation('cite-2025-memories-linear')">Citation</button>
          <button class="pub-button" onclick="copyCitation('cite-2025-memories-linear')">Copy Citation</button>
          <a class="pub-link" href="https://doi.org/10.1016/j.memori.2025.100134" target="_blank" rel="noopener">DOI</a>
          <a class="pub-link" href="https://srsapireddy.github.io/publications/J1.pdf" target="_blank" rel="noopener">PDF</a>
        </div>
      
        <div id="cite-2025-memories-linear" class="citation-box">S. R. Sapireddy, K. Asifuzzaman, and R. Mostafizur, "Simplifying activations with linear approximations in neural networks," Memories - Materials, Devices, Circuits and Systems, vol. 11, 2025, Art. no. 100134, doi: 10.1016/j.memori.2025.100134.</div>
      </div>
      
      <div class="publication-card" data-type="journal">
        <div class="pub-top">
          <span class="pub-year">2025</span>
          <span class="pub-type">Journal Article</span>
          <span class="pub-award">Published</span>
        </div>
      
        <div class="pub-title">
          Understanding and Detecting Adversarial Examples in IoT Networks: A White-Box Analysis with Autoencoders
        </div>
      
        <div class="pub-authors">
          W. Danesh, S. R. Sapireddy, and M. Rahman
        </div>
      
        <div class="pub-venue">
          Electronics, Volume 14, Issue 15, 2025, Article 3015.
        </div>
      
        <div class="pub-note">
          DOI: 10.3390/electronics14153015
        </div>
      
        <div class="pub-links">
          <button class="pub-button primary" onclick="toggleCitation('cite-2025-electronics')">Citation</button>
          <button class="pub-button" onclick="copyCitation('cite-2025-electronics')">Copy Citation</button>
          <a class="pub-link" href="https://doi.org/10.3390/electronics14153015" target="_blank" rel="noopener">DOI</a>
          <a class="pub-link" href="https://srsapireddy.github.io/publications/J2.pdf" target="_blank" rel="noopener">PDF</a>
        </div>
      
        <div id="cite-2025-electronics" class="citation-box">W. Danesh, S. R. Sapireddy, and M. Rahman, "Understanding and Detecting Adversarial Examples in IoT Networks: A White-Box Analysis with Autoencoders," Electronics, vol. 14, no. 15, Art. no. 3015, 2025, doi: 10.3390/electronics14153015.</div>
      </div>

      <div class="publication-card" data-type="conference award">
        <div class="pub-top">
          <span class="pub-year">2025</span>
          <span class="pub-type">IEEE Conference Paper</span>
          <span class="pub-award">Best Paper Award</span>
          <span class="pub-award">Published</span>
        </div>
      
        <div class="pub-title">
          Revisiting R: Statistical Envelope Analysis for Lightweight RF Modulation Classification
        </div>
      
        <div class="pub-authors">
          S. R. Sapireddy and M. Rahman
        </div>
      
        <div class="pub-venue">
          2025 1st International Conference on Radio Frequency Communication and Networks (RFCoN), Thanjavur, India, 2025, pp. 1-6.
        </div>
      
        <div class="pub-note">
          Best Paper Award | DOI: 10.1109/RFCoN62306.2025.11085271
        </div>
      
        <div class="pub-links">
          <button class="pub-button primary" onclick="toggleCitation('cite-2025-rfcon')">Citation</button>
          <button class="pub-button" onclick="copyCitation('cite-2025-rfcon')">Copy Citation</button>
          <a class="pub-link" href="https://doi.org/10.1109/RFCoN62306.2025.11085271" target="_blank" rel="noopener">DOI</a>
          <a class="pub-link" href="https://srsapireddy.github.io/publications/C1.pdf" target="_blank" rel="noopener">PDF</a>
        </div>
      
        <div id="cite-2025-rfcon" class="citation-box">S. R. Sapireddy and M. Rahman, "Revisiting R: Statistical Envelope Analysis for Lightweight RF Modulation Classification," 2025 1st International Conference on Radio Frequency Communication and Networks (RFCoN), Thanjavur, India, 2025, pp. 1-6, doi: 10.1109/RFCoN62306.2025.11085271.</div>
      </div>

      <div class="publication-card" data-type="conference">
        <div class="pub-top">
          <span class="pub-year">2025</span>
          <span class="pub-type">ACM Conference Paper</span>
          <span class="pub-award">Published</span>
        </div>
      
        <div class="pub-title">
          On the Effectiveness of Piecewise Activation Approximations for Long-Term Short-Memory Networks
        </div>
      
        <div class="pub-authors">
          Srinivas Rahul Sapireddy and Mostafizur Rahman
        </div>
      
        <div class="pub-venue">
          Proceedings of the Great Lakes Symposium on VLSI 2025 (GLSVLSI '25), Association for Computing Machinery, New York, NY, USA, 2025, pp. 740-745.
        </div>
      
        <div class="pub-note">
          DOI: 10.1145/3716368.3735217
        </div>
      
        <div class="pub-links">
          <button class="pub-button primary" onclick="toggleCitation('cite-2025-glsvlsi')">Citation</button>
          <button class="pub-button" onclick="copyCitation('cite-2025-glsvlsi')">Copy Citation</button>
          <a class="pub-link" href="https://doi.org/10.1145/3716368.3735217" target="_blank" rel="noopener">DOI</a>
          <a class="pub-link" href="https://srsapireddy.github.io/publications/C2.pdf" target="_blank" rel="noopener">PDF</a>
        </div>
      
        <div id="cite-2025-glsvlsi" class="citation-box">S. R. Sapireddy and M. Rahman, "On the Effectiveness of Piecewise Activation Approximations for Long-Term Short-Memory Networks," in Proceedings of the Great Lakes Symposium on VLSI 2025 (GLSVLSI '25), Association for Computing Machinery, New York, NY, USA, 2025, pp. 740-745, doi: 10.1145/3716368.3735217.</div>
      </div>
      
      <div class="publication-card" data-type="thesis">
        <div class="pub-top">
          <span class="pub-year">2025</span>
          <span class="pub-type">Dissertation / Thesis</span>
          <span class="pub-award">Published</span>
        </div>
      
        <div class="pub-title">
          Hardware-Aware Deep Learning and Signal Processing for Low-Power RF Modulation Classification
        </div>
      
        <div class="pub-authors">
          Srinivas Rahul Sapireddy
        </div>
      
        <div class="pub-venue">
          Ph.D. Dissertation, University of Missouri-Kansas City, ProQuest Dissertations &amp; Theses, 2025.
        </div>
      
        <div class="pub-note">
          ProQuest Publication No. 32172775
        </div>
      
        <div class="pub-links">
          <button class="pub-button primary" onclick="toggleCitation('cite-2025-dissertation')">Citation</button>
          <button class="pub-button" onclick="copyCitation('cite-2025-dissertation')">Copy Citation</button>
          <a class="pub-link disabled" href="#" onclick="return false;">Link pending</a>
          <a class="pub-link disabled" href="#" onclick="return false;">PDF pending</a>
        </div>
      
        <div id="cite-2025-dissertation" class="citation-box">S. R. Sapireddy, "Hardware-Aware Deep Learning and Signal Processing for Low-Power RF Modulation Classification," Ph.D. dissertation, University of Missouri-Kansas City, ProQuest Dissertations &amp; Theses, 2025, Publication No. 32172775.</div>
      </div>

    <div class="year-section" data-year-section="2024">
      <div class="year-header">
        <div class="year-title">📅 2024 Publications</div>
        <div class="year-pill">2 publications</div>
      </div>

    <div class="publication-card" data-type="journal">
      <div class="pub-top">
        <span class="pub-year">2024</span>
        <span class="pub-type">Journal Article</span>
        <span class="pub-award">Published</span>
      </div>
    
      <div class="pub-title">
        A Review of Crosstalk Polymorphic Circuits and Their Scalability
      </div>
    
      <div class="pub-authors">
        Md Arif Iqbal, Srinivas Rahul Sapireddy, Sumanth Dasari, Kazi Asifuzzaman, and Mostafizur Rahman
      </div>
    
      <div class="pub-venue">
        Memories - Materials, Devices, Circuits and Systems, Volume 7, 2024, Article 100094.
      </div>
    
      <div class="pub-note">
        ISSN: 2773-0646 | DOI: 10.1016/j.memori.2023.100094
      </div>
    
      <div class="pub-links">
        <button class="pub-button primary" onclick="toggleCitation('cite-2024-crosstalk')">Citation</button>
        <button class="pub-button" onclick="copyCitation('cite-2024-crosstalk')">Copy Citation</button>
        <a class="pub-link" href="https://doi.org/10.1016/j.memori.2023.100094" target="_blank" rel="noopener">DOI</a>
        <a class="pub-link" href="https://srsapireddy.github.io/publications/J3.pdf" target="_blank" rel="noopener">PDF</a>
      </div>
    
      <div id="cite-2024-crosstalk" class="citation-box">M. A. Iqbal, S. R. Sapireddy, S. Dasari, K. Asifuzzaman, and M. Rahman, "A review of crosstalk polymorphic circuits and their scalability," Memories - Materials, Devices, Circuits and Systems, vol. 7, Art. no. 100094, 2024, doi: 10.1016/j.memori.2023.100094.</div>
    </div>

    <div class="publication-card" data-type="journal">
      <div class="pub-top">
        <span class="pub-year">2024</span>
        <span class="pub-type">Journal Article</span>
        <span class="pub-award">Published</span>
      </div>
    
      <div class="pub-title">
        A Messaging-Based Intelligent Computing Approach for Machine Learning Applications
      </div>
    
      <div class="pub-authors">
        Mostafizur Rahman, Arif Iqbal, and Srinivas Rahul
      </div>
    
      <div class="pub-venue">
        Accessed: Mar, Volume 20, 2024.
      </div>
    
      <div class="pub-note">
        Journal details, page numbers, DOI, and publisher information can be added once available.
      </div>
    
      <div class="pub-links">
        <button class="pub-button primary" onclick="toggleCitation('cite-2024-messaging-ml')">Citation</button>
        <button class="pub-button" onclick="copyCitation('cite-2024-messaging-ml')">Copy Citation</button>
        <a class="pub-link disabled" href="#" onclick="return false;">DOI pending</a>
        <a class="pub-link" href="https://srsapireddy.github.io/publications/J4.pdf" target="_blank" rel="noopener">PDF</a>
      </div>
    
      <div id="cite-2024-messaging-ml" class="citation-box">M. Rahman, A. Iqbal, and S. Rahul, "A Messaging-Based Intelligent Computing Approach for Machine Learning Applications," Accessed: Mar, vol. 20, 2024.</div>
    </div>

    

    <div class="year-section" data-year-section="2018">
      <div class="year-header">
        <div class="year-title">📅 2018 Publications</div>
      </div>

     <div class="publication-card" data-type="journal earlier">
      <div class="pub-top">
        <span class="pub-year">2018</span>
        <span class="pub-type">Journal Article</span>
        <span class="pub-award">Published</span>
      </div>
    
      <div class="pub-title">
        Automation of Patient Medical Record Dispatch System Software Application
      </div>
    
      <div class="pub-authors">
        Bhavya Teja Gurijala and Srinivas Rahul Sapireddy
      </div>
    
      <div class="pub-venue">
        International Journal of Advanced Research in Science, Engineering and Technology (IJARSET), Volume 5, Issue 6, 2018, pp. 6074-6079.
      </div>
    
      <div class="pub-note">
        Publication date: June 2018.
      </div>
    
      <div class="pub-links">
        <button class="pub-button primary" onclick="toggleCitation('cite-2018-medical-record-dispatch')">Citation</button>
        <button class="pub-button" onclick="copyCitation('cite-2018-medical-record-dispatch')">Copy Citation</button>
        <a class="pub-link disabled" href="#" onclick="return false;">DOI pending</a>
        <a class="pub-link" href="https://srsapireddy.github.io/publications/J5.pdf" target="_blank" rel="noopener">PDF</a>
      </div>
    
      <div id="cite-2018-medical-record-dispatch" class="citation-box">B. T. Gurijala and S. R. Sapireddy, "Automation of Patient Medical Record Dispatch System Software Application," International Journal of Advanced Research in Science, Engineering and Technology (IJARSET), vol. 5, no. 6, pp. 6074-6079, Jun. 2018.</div>
    </div>
        <div class="year-section" data-year-section="2016">
          <div class="year-header">
            <div class="year-title">📅 2016 Publications</div>
          </div>

     <div class="publication-card" data-type="journal earlier">
      <div class="pub-top">
        <span class="pub-year">2016</span>
        <span class="pub-type">Journal Article</span>
        <span class="pub-award">Published</span>
      </div>
    
      <div class="pub-title">
        CAM Cell Based Memory Architecture for Extreme Searching Operations
      </div>
    
      <div class="pub-authors">
        Srinivas Rahul Sapireddy
      </div>
    
      <div class="pub-venue">
        International Journal of Advances in Electronics and Computer Science, Volume 8, Issue 3, 2016, pp. 80-83.
      </div>
    
      <div class="pub-note">
        Publication date: September 15, 2016 | ISSN: 2393-2835
      </div>
    
      <div class="pub-links">
        <button class="pub-button primary" onclick="toggleCitation('cite-2016-cam-memory')">Citation</button>
        <button class="pub-button" onclick="copyCitation('cite-2016-cam-memory')">Copy Citation</button>
        <a class="pub-link" href="https://iraj.doionline.org/dx/IJAECS-IRAJ-DOIONLINE-5387" onclick="return false;">DOI pending</a>
        <a class="pub-link" href="https://srsapireddy.github.io/publications/J6.pdf" target="_blank" rel="noopener">PDF</a>
      </div>
    
      <div id="cite-2016-cam-memory" class="citation-box">S. R. Sapireddy, "CAM Cell Based Memory Architecture for Extreme Searching Operations," International Journal of Advances in Electronics and Computer Science, vol. 8, no. 3, pp. 80-83, Sep. 15, 2016. ISSN: 2393-2835.</div>
    </div>

     <div class="publication-card" data-type="journal earlier">
        <div class="pub-top">
          <span class="pub-year">2016</span>
          <span class="pub-type">Journal Article</span>
          <span class="pub-award">Published</span>
        </div>
      
        <div class="pub-title">
          Two Stage Operational Amplifier with a Gain Boosted, Source Follower Buffer
        </div>
      
        <div class="pub-authors">
          S. Srinivas Rahul, P. Naga Tejaswi, Y. Mohan Sandeep, and K. Hari Krishna
        </div>
      
        <div class="pub-venue">
          International Journal of Engineering Trends and Technology (IJETT), Volume 34, Issue 2, 2016, pp. 256-259.
        </div>
      
        <div class="pub-note">
          DOI: 10.14445/22315381/IJETT-V34P252
        </div>
      
        <div class="pub-links">
          <button class="pub-button primary" onclick="toggleCitation('cite-2016-opamp-buffer')">Citation</button>
          <button class="pub-button" onclick="copyCitation('cite-2016-opamp-buffer')">Copy Citation</button>
          <a class="pub-link" href="https://doi.org/10.14445/22315381/IJETT-V34P252" target="_blank" rel="noopener">DOI</a>
          <a class="pub-link" href="https://srsapireddy.github.io/publications/J7.pdf" target="_blank" rel="noopener">PDF</a>
        </div>
      
        <div id="cite-2016-opamp-buffer" class="citation-box">S. Srinivas Rahul, P. Naga Tejaswi, Y. Mohan Sandeep, and K. Hari Krishna, "Two Stage Operational Amplifier with a Gain Boosted, Source Follower Buffer," International Journal of Engineering Trends and Technology (IJETT), vol. 34, no. 2, pp. 256-259, 2016, doi: 10.14445/22315381/IJETT-V34P252.</div>
      </div>

  </div>

  <div class="grid-2">
    <div class="section">
      <h2>📍 Publication Timeline</h2>
      <div class="divider"></div>

      <div class="timeline">
        <div class="timeline-item">
          <div class="timeline-year">2026</div>
          <div class="timeline-title">IEEE SoutheastCon</div>
          <div class="timeline-text">
            Bin-Based R framework for resource-efficient RF modulation classification using envelope statistics.
          </div>
        </div>

        <div class="timeline-item">
          <div class="timeline-year">2025</div>
          <div class="timeline-title">RF, AI, Security, and VLSI Publications</div>
          <div class="timeline-text">
            Work across RFCoN, GLSVLSI, ICMLA, IEEE CARS, Electronics, and Memories.
          </div>
        </div>

        <div class="timeline-item">
          <div class="timeline-year">2024</div>
          <div class="timeline-title">Activation Functions and Circuit Design</div>
          <div class="timeline-text">
            Journal work on piecewise activation approximation and polymorphic circuit design.
          </div>
        </div>

        <div class="timeline-item">
          <div class="timeline-year">2018 / 2016</div>
          <div class="timeline-title">Earlier Research Outputs</div>
          <div class="timeline-text">
            Replace the placeholder cards above with exact title, author, venue, DOI, and PDF details.
          </div>
        </div>
      </div>
    </div>

    <div class="section">
      <h2>🌐 Publication Profiles</h2>
      <div class="divider"></div>

      <p>
        For updated indexing, citation counts, and official metadata, please visit my public scholarly profiles.
      </p>

      <div class="pub-links">
        <a class="pub-link" href="https://scholar.google.com/citations?user=08fgpdIAAAAJ" target="_blank" rel="noopener">Google Scholar</a>
        <a class="pub-link" href="https://orcid.org/0000-0002-9898-6810" target="_blank" rel="noopener">ORCID</a>
        <a class="pub-link" href="https://openreview.net/profile?id=~Srinivas_Rahul_Sapireddy1" target="_blank" rel="noopener">OpenReview</a>
        <a class="pub-link" href="/resume/">Resume</a>
      </div>
    </div>
  </div>

</div>

<script>
function toggleCitation(id) {
  const box = document.getElementById(id);
  if (!box) return;

  if (box.style.display === "block") {
    box.style.display = "none";
  } else {
    box.style.display = "block";
  }
}

function copyCitation(id) {
  const box = document.getElementById(id);
  if (!box) return;

  const text = box.innerText;

  if (navigator.clipboard) {
    navigator.clipboard.writeText(text).then(function () {
      alert("Citation copied to clipboard.");
    }).catch(function () {
      alert("Unable to copy automatically. Please copy the citation manually.");
    });
  } else {
    alert("Clipboard not supported. Please copy the citation manually.");
  }
}

function filterPublications(event, filterType) {
  const buttons = document.querySelectorAll(".tab-button");
  const cards = document.querySelectorAll(".publication-card");
  const yearSections = document.querySelectorAll(".year-section");

  buttons.forEach(function(button) {
    button.classList.remove("active");
  });

  if (event && event.currentTarget) {
    event.currentTarget.classList.add("active");
  }

  cards.forEach(function(card) {
    const type = card.getAttribute("data-type") || "";

    if (filterType === "all" || type.includes(filterType)) {
      card.classList.remove("hide-card");
    } else {
      card.classList.add("hide-card");
    }
  });

  yearSections.forEach(function(section) {
    const visibleCards = section.querySelectorAll(".publication-card:not(.hide-card)");
    if (visibleCards.length === 0) {
      section.classList.add("hide-year");
    } else {
      section.classList.remove("hide-year");
    }
  });
}
</script>
