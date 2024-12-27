---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<div class="main-content">
  <div id="sort-controls">
    <button onclick="sortPublications('date')">Sort by Date</button>
    <button onclick="sortPublications('citation')">Sort by Citations</button>
  </div>

  <div id="publications">
    <div class="publication" data-year="2024" data-citations="50">
      <h3>Towards sustainable AI: a comprehensive framework for Green AI</h3>
      <p><strong>GM Iqbal Mahmud</strong>, Abdulaziz Tabbakh, Lisan Al Amin, Mahbubul Islam, Imranul Kabir Chowdhury, Md Saddam Hossain Mukta</p>
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

    <div class="publication" data-year="2024" data-citations="30">
      <h3>Application of artificial intelligence in reverse logistics: A bibliometric and network analysis</h3>
      <p>Oyshik Bhowmik, Sudipta Chowdhury, Jahid Hasan Ashik, <strong>GM Iqbal Mahmud</strong>, Md Muzahid Khan, Niamat Ullah Ibne Hossain</p>
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

function sortPublications(criteria) {
  var publications = document.querySelectorAll('.publication');
  var container = document.getElementById('publications');
  var pubsArray = Array.from(publications);

  pubsArray.sort(function(a, b) {
    if (criteria === 'date') {
      return new Date(b.querySelector('.meta span:nth-child(2)').innerText) - new Date(a.querySelector('.meta span:nth-child(2)').innerText);
    } else if (criteria === 'citation') {
      return parseInt(b.getAttribute('data-citations')) - parseInt(a.getAttribute('data-citations'));
    }
  });

  container.innerHTML = '';
  pubsArray.forEach(function(pub) {
    container.appendChild(pub);
  });
}
</script>
