---
layout: archive
title: "News & <br> Updates"
permalink: /news/
author_profile: true
---

<div class="main-content">
  <div id="news">
    <!-- <h2 style="text-align: left; font-size: 18px; font-weight: bold;">News & Updates</h2> -->
    <p style="font-size: 15px; text-align: justify;">Stay updated with my latest achievements, experiences, and milestones. Use the filter feature below to find specific updates based on year or month.</p>

    <div class="filter-section" style="margin-top: 20px;">
      <label for="filter-year" style="font-size: 16px;">Filter by year:</label>
      <select id="filter-year" style="font-size: 15px; margin-left: 10px; padding: 5px;">
        <option value="all">All Years</option>
        <option value="2024">2024</option>
        <option value="2023">2023</option>
        <option value="2022">2022</option>
      </select>
      <label for="filter-month" style="font-size: 16px; margin-left: 20px;">Filter by month:</label>
      <select id="filter-month" style="font-size: 15px; margin-left: 10px; padding: 5px;">
        <option value="all">All Months</option>
        <option value="01">January</option>
        <option value="02">February</option>
        <option value="03">March</option>
        <option value="04">April</option>
        <option value="05">May</option>
        <option value="06">June</option>
        <option value="07">July</option>
        <option value="08">August</option>
        <option value="09">September</option>
        <option value="10">October</option>
        <option value="11">November</option>
        <option value="12">December</option>
      </select>
    </div>

    <div id="news-list" style="margin-top: 20px;">
      <div class="news-item" data-year="2024" data-month="11">
        <p style="font-size: 15px; text-align: justify;">11/24/2024: Awarded <strong>International Student Award</strong> from the Lions Clubs International of Norman, Oklahoma for contributions to the University of Oklahoma campus and the local community. <a href="#" target="_blank">[Link]</a></p>
      </div>

      <div class="news-item" data-year="2024" data-month="10">
        <p style="font-size: 15px; text-align: justify;">10/24/2024: Organized two research sessions titled "<strong>Towards Sustainable Resilient Communities</strong>" and two panel sessions on decision making in community resilience at the 2024 INFORMS Annual Meeting in Seattle, WA.</p>
      </div>

      <div class="news-item" data-year="2024" data-month="10">
        <p style="font-size: 15px; text-align: justify;">10/15/2024: Accepted into the <strong>Decision Sciences Institute (DSI) Doctoral Consortium</strong> at the 2024 DSI Annual Conference in Phoenix, Arizona.</p>
      </div>

      <div class="news-item" data-year="2024" data-month="09">
        <p style="font-size: 15px; text-align: justify;">09/24/2024: Presented poster "<strong>AI-ML for Optimal Building Mitigation in Flood-Prone Communities</strong>" at the Gallogly College of Engineering Graduate Student Poster Fair.</p>
      </div>

      <div class="news-item" data-year="2024" data-month="08">
        <p style="font-size: 15px; text-align: justify;">08/11/2024: Attended <strong>Business Analytics Future BAProf 2024</strong> workshop organized by the University of Iowa Tippie College of Business at Iowa City, Iowa. <a href="#" target="_blank">[Link]</a></p>
      </div>
    </div>
  </div>
</div>

<script>
const yearFilter = document.getElementById('filter-year');
const monthFilter = document.getElementById('filter-month');

function filterNews() {
  const selectedYear = yearFilter.value;
  const selectedMonth = monthFilter.value;
  const newsItems = document.querySelectorAll('.news-item');

  newsItems.forEach(item => {
    const itemYear = item.getAttribute('data-year');
    const itemMonth = item.getAttribute('data-month');

    if ((selectedYear === 'all' || itemYear === selectedYear) &&
        (selectedMonth === 'all' || itemMonth === selectedMonth)) {
      item.style.display = 'block';
    } else {
      item.style.display = 'none';
    }
  });
}

yearFilter.addEventListener('change', filterNews);
monthFilter.addEventListener('change', filterNews);
</script>
