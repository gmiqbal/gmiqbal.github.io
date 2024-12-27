---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<div class="sidebar">
  <h1>Your Name</h1>
  <a href="/">Home</a>
</div>

<div class="main-content">
  <div class="search-bar">
    <input type="text" id="search" placeholder="Search publications...">
    <select id="filter-year">
      <option value="">Filter by Year</option>
      <option value="2024">2024</option>
      <option value="2023">2023</option>
    </select>
    <button onclick="filterPublications()">Search</button>
  </div>

  <div id="publications">
    <div class="publication" data-year="2024">
      <h3>Towards sustainable AI: a comprehensive framework for Green AI</h3>
      <div class="meta">
        <span>Journal | Discover Sustainability</span>
        <span>15th Nov 2024</span>
      </div>
      <div class="actions">
        <a href="https://link.springer.com/article/10.1007/s43621-024-00641-4">Journal Link</a>
        <span class="abstract-toggle" onclick="toggleAbstract('abstract-1')">See Abstract</span>
      </div>
      <div id="abstract-1" class="abstract">
        <strong>Abstract:</strong> The rapid advancement of artificial intelligence (AI) has brought significant benefits across various domains, yet it has also led to increased energy consum...
      </div>
    </div>

    <div class="publication" data-year="2024">
      <h3>Application of artificial intelligence in reverse logistics: A bibliometric and network analysis</h3>
      <div class="meta">
        <span>Journal | Supply Chain Analytics</span>
        <span>September 2024</span>
      </div>
      <div class="actions">
        <a href="https://doi.org/10.1016/j.sca.2024.100076">Journal Link</a>
        <span class="abstract-toggle" onclick="toggleAbstract('abstract-2')">See Abstract</span>
      </div>
      <div id="abstract-2" class="abstract">
        <strong>Abstract:</strong> Despite abundant research on the application of artificial intelligence (AI) in reverse logistics, no comprehensive study with bibliometric and network analysis has been conducted...
      </div>
    </div>
  </div>
</div>

<script>
function toggleAbstract(id) {
  var abstract = document.getElementById(id);
  abstract.style.display = abstract.style.display === "block" ? "none" : "block";
}

function filterPublications() {
  var search = document.getElementById('search').value.toLowerCase();
  var year = document.getElementById('filter-year').value;
  var publications = document.querySelectorAll('.publication');

  publications.forEach(function(pub) {
    var title = pub.querySelector('h3').innerText.toLowerCase();
    var pubYear = pub.getAttribute('data-year');

    if ((title.includes(search) || search === '') && (year === '' || pubYear === year)) {
      pub.style.display = "block";
    } else {
      pub.style.display = "none";
    }
  });
}
</script>
