---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<style>
/* General Styling */
body {
  font-family: 'Arial', sans-serif;
  background-color: #f5f5f5;
  color: #333;
  margin: 0;
  padding: 0;
}

/* Publication Cards Container */
.publications-wrapper {
  display: flex;
  flex-direction: column;
  gap: 20px;
  max-width: 900px;
  margin: auto;
  padding: 20px;
}

/* Publication Card */
.publication-card {
  background-color: #fff;
  border-radius: 8px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  padding: 15px 20px;
  display: flex;
  flex-direction: column;
  gap: 10px;
  transition: box-shadow 0.3s ease;
}

.publication-card:hover {
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.15);
}

/* Publication Metadata */
.publication-title {
  font-size: 18px;
  font-weight: bold;
  color: #0073e6;
  margin: 0;
}

.publication-authors,
.publication-venue,
.publication-date {
  font-size: 14px;
  color: #555;
}

.publication-date {
  text-align: right;
  font-weight: bold;
  color: #888;
}

/* Abstract Section */
.abstract-toggle {
  cursor: pointer;
  color: #0073e6;
  font-size: 13px;
  text-decoration: underline;
}

.abstract-content {
  display: none;
  margin-top: 10px;
  padding: 10px;
  background-color: #f9f9f9;
  border-left: 3px solid #0073e6;
  border-radius: 5px;
  font-size: 14px;
  color: #444;
}

/* Responsive Design */
@media (max-width: 768px) {
  .publication-card {
    padding: 15px;
  }

  .publications-wrapper {
    padding: 10px;
  }
}
</style>

<div class="publications-wrapper">
  <!-- Example Publication 1 -->
  <div class="publication-card">
    <div class="publication-title">Towards sustainable AI: a comprehensive framework for Green AI</div>
    <div class="publication-authors">Abdulaziz Tabbakh, Lisan Al Amin, Mahbubul Islam, <strong>GM Iqbal Mahmud</strong></div>
    <div class="publication-venue">Discover Sustainability</div>
    <div class="abstract-toggle" onclick="toggleAbstract('abstract-1')">See Abstract</div>
    <div id="abstract-1" class="abstract-content">
      <strong>Abstract:</strong> The rapid advancement of artificial intelligence (AI) has brought significant benefits across various domains, yet it has also led to increased energy consumption and environmental impact...
    </div>
    <div class="publication-date">15th Nov 2024</div>
  </div>

  <!-- Example Publication 2 -->
  <div class="publication-card">
    <div class="publication-title">Application of artificial intelligence in reverse logistics</div>
    <div class="publication-authors">Oyshik Bhowmik, Sudipta Chowdhury, Jahid Hasan Ashik, <strong>GM Iqbal Mahmud</strong></div>
    <div class="publication-venue">Supply Chain Analytics</div>
    <div class="abstract-toggle" onclick="toggleAbstract('abstract-2')">See Abstract</div>
    <div id="abstract-2" class="abstract-content">
      <strong>Abstract:</strong> This study uses bibliometric analysis to derive the prominent research statistics in AI-centric reverse logistics, considering 2929 articles...
    </div>
    <div class="publication-date">September 2024</div>
  </div>
</div>

<script>
/* Toggle Abstract Visibility */
function toggleAbstract(id) {
  const abstract = document.getElementById(id);
  abstract.style.display = abstract.style.display === "block" ? "none" : "block";
}
</script>
