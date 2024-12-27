<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Publications</title>
<style>
/* General Styling */
body {
  font-family: 'Arial', sans-serif;
  color: #333;
  margin: 0;
  padding: 0;
  line-height: 1.6;
  display: flex;
}

/* Sidebar */
.sidebar {
  width: 250px;
  background-color: #2C3E50;
  color: #ecf0f1;
  position: fixed;
  height: 100%;
  padding: 20px;
  box-shadow: 2px 0 5px rgba(0, 0, 0, 0.1);
}
.sidebar h1 {
  margin-top: 0;
  font-size: 24px;
  text-transform: uppercase;
  letter-spacing: 2px;
}
.sidebar a {
  color: #ecf0f1;
  text-decoration: none;
}
.sidebar a:hover {
  text-decoration: underline;
}

/* Main Content */
.main-content {
  margin-left: 270px;
  padding: 20px;
  width: calc(100% - 270px);
}

/* Search Bar */
.search-bar {
  display: flex;
  margin-bottom: 20px;
  gap: 10px;
}
.search-bar input, .search-bar select {
  padding: 10px;
  font-size: 14px;
  border: 1px solid #ddd;
  border-radius: 5px;
}
.search-bar button {
  padding: 10px 15px;
  font-size: 14px;
  background-color: #3498db;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}
.search-bar button:hover {
  background-color: #2980b9;
}

/* Publications */
.publication {
  display: flex;
  flex-direction: column;
  gap: 15px;
  padding: 20px;
  background-color: #f9f9f9;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  border-radius: 10px;
  margin-bottom: 20px;
}
.publication h3 {
  margin: 0;
  font-size: 18px;
  color: #222;
}
.publication .meta {
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-size: 14px;
  color: #555;
}
.publication .actions {
  margin-top: 10px;
  display: flex;
  gap: 10px;
}
.publication .actions a {
  padding: 8px 12px;
  font-size: 13px;
  text-decoration: none;
  background-color: #4CAF50;
  color: white;
  border-radius: 5px;
  text-align: center;
}
.publication .actions a:hover {
  background-color: #45a049;
}
.publication .abstract-toggle {
  color: #0073e6;
  cursor: pointer;
  font-size: 14px;
  text-decoration: underline;
  display: inline-block;
}
.publication .abstract {
  display: none;
  padding: 10px;
  background-color: #fdfdfd;
  border-left: 4px solid #0073e6;
  border-radius: 5px;
  margin-top: 10px;
}

/* Responsive Design */
@media (max-width: 768px) {
  .main-content {
    margin-left: 0;
    width: 100%;
  }
  .sidebar {
    display: none;
  }
}
</style>
</head>
<body>
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
</body>
</html>
