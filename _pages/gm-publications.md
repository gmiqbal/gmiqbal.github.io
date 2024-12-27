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
  margin: 0;
  padding: 0;
  background-color: #f5f5f5;
  color: #333;
}

/* Dark Mode */
body.dark-mode {
  background-color: #121212;
  color: #f5f5f5;
}

body.dark-mode .publication-card {
  background-color: #1e1e1e;
  color: #f5f5f5;
}

body.dark-mode .abstract {
  background-color: #2b2b2b;
}

body.dark-mode .tag {
  background-color: #444;
}

/* Publication Cards */
.publication-container {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  justify-content: center;
  padding: 20px;
}

.publication-card {
  background-color: #fff;
  border-radius: 10px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  width: 100%;
  max-width: 800px;
  padding: 20px;
  display: flex;
  flex-direction: column;
  gap: 15px;
  transition: transform 0.2s;
}

.publication-card:hover {
  transform: translateY(-5px);
}

/* Publication Metadata */
.publication-type {
  font-size: 14px;
  font-weight: bold;
  color: #0073e6;
  text-transform: uppercase;
}

.publication-title {
  font-size: 18px;
  font-weight: bold;
  margin: 0;
  color: #222;
}

.publication-authors {
  font-size: 14px;
  color: #555;
  margin-top: 5px;
}

.publication-venue {
  font-size: 14px;
  font-style: italic;
  color: #555;
}

.publication-date {
  font-size: 14px;
  font-weight: bold;
  color: #666;
  text-align: right;
}

/* Abstract Section */
.abstract {
  max-height: 0;
  overflow: hidden;
  transition: max-height 0.3s ease-out;
}

.abstract.open {
  max-height: 500px; /* Adjust based on content */
}

.abstract-toggle {
  cursor: pointer;
  color: #0073e6;
  font-size: 13px;
  text-decoration: underline;
  display: inline-block;
}

/* Tags */
.publication-tags {
  margin-top: 10px;
}

.tag {
  display: inline-block;
  background-color: #0073e6;
  color: white;
  padding: 5px 10px;
  border-radius: 15px;
  font-size: 12px;
  margin-right: 5px;
}

/* Download Button */
.download-button {
  display: inline-block;
  padding: 10px 20px;
  font-size: 14px;
  background-color: #4CAF50;
  color: white;
  text-decoration: none;
  border-radius: 5px;
  font-weight: bold;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  transition: background-color 0.2s;
}

.download-button:hover {
  background-color: #45a049;
}

/* Year Header */
.year-header {
  font-size: 20px;
  font-weight: bold;
  margin: 20px 0 10px;
  color: #555;
  text-align: center;
}

/* Pagination */
.pagination-container {
  text-align: center;
  margin-top: 20px;
}

.pagination-container button {
  padding: 10px 15px;
  margin: 0 5px;
  border: none;
  background-color: #0073e6;
  color: white;
  font-size: 14px;
  cursor: pointer;
  border-radius: 5px;
  transition: background-color 0.3s;
}

.pagination-container button:hover {
  background-color: #005bb5;
}

.pagination-container button.active {
  background-color: #005bb5;
}

/* Responsive Design */
@media (max-width: 768px) {
  .publication-card {
    width: 100%;
  }

  .publication-container {
    padding: 10px;
  }
}
</style>

<!-- Search Bar -->
<input type="text" id="search-bar" placeholder="Search publications..." onkeyup="filterPublications()" style="width: 100%; padding: 10px; margin: 20px auto; border: 1px solid #ccc; border-radius: 5px; font-size: 16px; max-width: 800px;">

<div id="publications" class="publication-container">
  <!-- Year Group -->
  <div class="year-header">2024</div>
  
  <!-- Publication 1 -->
  <div class="publication-card">
    <div class="publication-type">Journal</div>
    <div class="publication-title">Towards sustainable AI: a comprehensive framework for Green AI</div>
    <div class="publication-authors">Abdulaziz Tabbakh, Lisan Al Amin, Mahbubul Islam, <strong>GM Iqbal Mahmud</strong>, Imranul Kabir Chowdhury, Md Saddam Hossain Mukta</div>
    <div class="publication-venue">Discover Sustainability</div>
    <div class="publication-tags">
      <span class="tag">AI</span>
      <span class="tag">Sustainability</span>
    </div>
    <div class="abstract-toggle" onclick="toggleAbstract('abstract-1')">See Abstract</div>
    <div id="abstract-1" class="abstract">
      <strong>Abstract:</strong> The rapid advancement of artificial intelligence (AI) has brought significant benefits across various domains, yet it has also led to increased energy consumption and environmental impact. This paper positions Green AI as a crucial direction for future research and development.
    </div>
    <a href="https://link.springer.com/article/10.1007/s43621-024-00641-4" class="download-button">Journal Link</a>
    <div class="publication-date">15th Nov 2024</div>
  </div>
  
  <!-- Publication 2 -->
  <div class="publication-card">
    <div class="publication-type">Journal</div>
    <div class="publication-title">Application of artificial intelligence in reverse logistics</div>
    <div class="publication-authors">Oyshik Bhowmik, Sudipta Chowdhury, Jahid Hasan Ashik, <strong>GM Iqbal Mahmud</strong></div>
    <div class="publication-venue">Supply Chain Analytics</div>
    <div class="publication-tags">
      <span class="tag">Logistics</span>
      <span class="tag">AI</span>
    </div>
    <div class="abstract-toggle" onclick="toggleAbstract('abstract-2')">See Abstract</div>
    <div id="abstract-2" class="abstract">
      <strong>Abstract:</strong> This study uses bibliometric analysis to derive the prominent research statistics in AI-centric reverse logistics, considering 2929 articles from the last three decades.
    </div>
    <a href="https://doi.org/10.1016/j.sca.2024.100076" class="download-button">Journal Link</a>
    <div class="publication-date">September 2024</div>
  </div>

  <!-- Publication 3 -->
  <div class="publication-card">
    <div class="publication-type">Thesis</div>
    <div class="publication-title">Solving a Capacitated Vehicle Routing Problem (CVRP)</div>
    <div class="publication-authors">G M Iqbal Mahmud <strong>Supervisor:</strong> Md. Habibur Rahman</div>
    <div class="publication-venue">Khulna University of Engineering & Technology</div>
    <div class="publication-tags">
      <span class="tag">Optimization</span>
      <span class="tag">Routing</span>
    </div>
    <div class="abstract-toggle" onclick="toggleAbstract('abstract-3')">See Abstract</div>
    <div id="abstract-3" class="abstract">
      <strong>Abstract:</strong> This thesis aims to solve the poor vehicle routing and underutilization of vehicles by finding optimal routes for distribution using Google OR-Tools.
    </div>
    <div class="publication-date">10th Apr 2022</div>
  </div>
</div>

<div class="pagination-container" id="pagination-container"></div>

<!-- Dark Mode Toggle -->
<button onclick="toggleTheme()" style="position: fixed; top: 20px; right: 20px; padding: 10px;">Toggle Theme</button>

<script>
/* Toggle Abstract */
function toggleAbstract(id) {
  const abstract = document.getElementById(id);
  abstract.classList.toggle("open");
}

/* Filter Publications */
function filterPublications() {
  const input = document.getElementById("search-bar").value.toLowerCase();
  const cards = document.querySelectorAll(".publication-card");
  cards.forEach(card => {
    const textContent = card.textContent.toLowerCase();
    card.style.display = textContent.includes(input) ? "block" : "none";
  });
}

/* Dark Mode Toggle */
function toggleTheme() {
  document.body.classList.toggle("dark-mode");
}

/* Pagination */
const itemsPerPage = 2;
const publications = document.querySelectorAll(".publication-card");
const paginationContainer = document.getElementById("pagination-container");

function showPage(page) {
  publications.forEach((card, index) => {
    card.style.display = index >= (page - 1) * itemsPerPage && index < page * itemsPerPage ? "block" : "none";
  });
  updatePagination(page);
}

function updatePagination(currentPage) {
  paginationContainer.innerHTML = "";
  const totalPages = Math.ceil(publications.length / itemsPerPage);
  for (let i = 1; i <= totalPages; i++) {
    const button = document.createElement("button");
    button.textContent = i;
    button.classList.add(i === currentPage ? "active" : "");
    button.onclick = () => showPage(i);
    paginationContainer.appendChild(button);
  }
}

showPage(1);
</script>
