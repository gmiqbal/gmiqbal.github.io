---
layout: archive
title: "News & <br> Updates"
permalink: /news/
author_profile: true
---

<div class="main-content">
  <div id="news">
    <h2 style="text-align: left; font-size: 18px; font-weight: bold;">News & Updates</h2>
    <p style="font-size: 15px; text-align: justify;">Stay updated with my latest achievements, experiences, and milestones. Use the filter feature below to find specific updates based on categories.</p>

    <div class="filter-section" style="margin-top: 20px;">
      <label for="filter" style="font-size: 16px;">Filter by category:</label>
      <select id="filter" style="font-size: 15px; margin-left: 10px; padding: 5px;">
        <option value="all">All</option>
        <option value="education">Education</option>
        <option value="publication">Publications</option>
        <option value="professional">Professional Experiences</option>
        <option value="award">Honors & Awards</option>
        <option value="volunteer">Volunteer Activities</option>
      </select>
    </div>

    <div id="news-list" style="margin-top: 20px;">

      <div class="news-item" data-category="education">
        <p style="font-size: 15px; text-align: justify;">🎓 <strong>Bachelor of Science in Industrial & Production Engineering</strong><br> 🏫 <a href="https://kuet.ac.bd/" target="_blank"><strong>Khulna University of Engineering & Technology</strong></a><br>📅 <strong>| Feb 2017 – Apr 2022</strong></p>
        <p style="font-size: 15px; text-align: justify;">CGPA: 3.65/4.00 (3.78 in last four semesters)</p>
      </div>

      <div class="news-item" data-category="publication">
        <p style="font-size: 15px; text-align: justify;">📚 <strong>Application of artificial intelligence in reverse logistics</strong><br> 📝 <a href="#" target="_blank">Supply Chain Analytics, Vol. 7, September 2024</a><br>Co-Author: G M Iqbal Mahmud</p>
      </div>

      <div class="news-item" data-category="professional">
        <p style="font-size: 15px; text-align: justify;">🛠 <strong>Supply Chain Planning Officer</strong><br> 🏢 <a href="https://www.unileverconsumercarebd.com/" target="_blank"><strong>Unilever Consumer Care Limited</strong></a><br>📅 <strong>| Jun 2023 - Aug 2024</strong></p>
        <p style="font-size: 15px; text-align: justify;">Led daily Master Production Schedule (MPS) meetings, coordinating a team of 20 to drive updates and actionable plans across three plants.</p>
      </div>

      <div class="news-item" data-category="award">
        <p style="font-size: 15px; text-align: justify;">🏆 <strong>Dean’s List Honoree</strong><br> 🏫 <a href="https://kuet.ac.bd/" target="_blank"><strong>Khulna University of Engineering & Technology</strong></a><br>📅 <strong>| Mar 2019</strong></p>
        <p style="font-size: 15px; text-align: justify;">Awarded in recognition of maintaining an average GPA of 3.75 or above across two regular terms in an academic year.</p>
      </div>

      <div class="news-item" data-category="volunteer">
        <p style="font-size: 15px; text-align: justify;">🌍 <strong>Level 7 Local Guide</strong><br> 🏢 <a href="https://maps.google.com" target="_blank"><strong>Google Maps</strong></a><br>📅 <strong>| Oct 2019 - Present</strong></p>
        <p style="font-size: 15px; text-align: justify;">Completed 1,319 contributions, generating 831,000+ views.</p>
      </div>

    </div>
  </div>
</div>

<script>
document.getElementById('filter').addEventListener('change', function() {
  const category = this.value;
  const newsItems = document.querySelectorAll('.news-item');

  newsItems.forEach(item => {
    if (category === 'all' || item.dataset.category === category) {
      item.style.display = 'block';
    } else {
      item.style.display = 'none';
    }
  });
});
</script>
