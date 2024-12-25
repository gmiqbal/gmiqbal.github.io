---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<style>
.publication-table {
  width: 100%;
  border-collapse: collapse;
}
.publication-table td {
  vertical-align: top;
  padding: 10px 0;
}
.publication-type {
  width: 15%;
  font-size: 14px;
  color: #666;
}
.publication-details {
  width: 70%;
}
.publication-title {
  font-size: 16px;
  font-weight: bold;
}
.publication-authors {
  font-size: 14px;
  color: #333;
}
.publication-venue {
  font-size: 14px;
  font-style: italic;
}
.publication-date {
  width: 15%;
  font-size: 14px;
  text-align: right;
}
.abstract-toggle {
  cursor: pointer;
  color: #0066cc;
  font-size: 12px;
}
.abstract {
  display: none;
  font-size: 14px;
  margin-top: 10px;
  padding: 10px;
  background-color: #f9f9f9;
}
.download-button {
  display: inline-block;
  margin-top: 5px;
  padding: 3px 8px;
  font-size: 12px;
  background-color: #4CAF50;
  color: white;
  text-decoration: none;
  border-radius: 3px;
}
</style>

<table class="publication-table">
  <tr>
    <td class="publication-type">Journal Article</td>
    <td class="publication-details">
      <div class="publication-title">Title of Your First Paper</div>
      <div class="publication-authors">Author 1, Author 2, Author 3</div>
      <div class="publication-venue">Journal of Important Research</div>
      <div class="abstract-toggle" onclick="toggleAbstract('abstract-1')">See more</div>
      <div id="abstract-1" class="abstract">
        <strong>Abstract:</strong> This is the abstract of your first paper. It provides a brief summary of the research conducted and the main findings.
      </div>
      <a href="#" class="download-button">Download</a>
    </td>
    <td class="publication-date">2023-06-15</td>
  </tr>

  <tr>
    <td class="publication-type">Conference Paper</td>
    <td class="publication-details">
      <div class="publication-title">Your Second Paper Title</div>
      <div class="publication-authors">Author 2, Author 3, Author 4</div>
      <div class="publication-venue">International Conference on Innovative Technologies</div>
      <div class="abstract-toggle" onclick="toggleAbstract('abstract-2')">See more</div>
      <div id="abstract-2" class="abstract">
        <strong>Abstract:</strong> This abstract summarizes your second paper, which was presented at a conference. It highlights the key points and contributions of your research.
      </div>
      <a href="#" class="download-button">Download</a>
    </td>
    <td class="publication-date">2022-09-30</td>
  </tr>

  <tr>
    <td class="publication-type">Thesis</td>
    <td class="publication-details">
      <div class="publication-title">Your Thesis Title</div>
      <div class="publication-authors">Your Name</div>
      <div class="publication-venue">University Name</div>
      <div class="abstract-toggle" onclick="toggleAbstract('abstract-3')">See more</div>
      <div id="abstract-3" class="abstract">
        <strong>Abstract:</strong> This is a summary of your thesis work. It outlines the main research question, methodology, findings, and conclusions of your extensive research project.
      </div>
      <a href="#" class="download-button">Download</a>
    </td>
    <td class="publication-date">2021-05-20</td>
  </tr>
</table>

<script>
function toggleAbstract(id) {
  var abstract = document.getElementById(id);
  if (abstract.style.display === "none" || abstract.style.display === "") {
    abstract.style.display = "block";
  } else {
    abstract.style.display = "none";
  }
}
</script>
