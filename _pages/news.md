---
layout: archive
title: "News & Updates"
permalink: /news/
author_profile: true
---

<div class="main-content">
  <div id="news">
    <!-- <h2 style="text-align: left; font-size: 18px; font-weight: bold;">News & Updates</h2> -->
    <p style="font-size: 15px; text-align: justify;">Stay updated with my latest achievements, experiences, and milestones. Use the filter feature below to find specific updates based on year or month.</p>

    <div class="filter-section" style="margin-top: 20px; display: flex; align-items: center;">
      <div style="margin-right: 20px;">
        <label for="filter-year" style="font-size: 16px;">Filter by year:</label>
        <select id="filter-year" style="font-size: 15px; margin-left: 10px; padding: 5px;">
          <option value="all">All Years</option>
          <option value="2024">2024</option>
          <option value="2023">2023</option>
          <option value="2022">2022</option>
        </select>
      </div>
      <div>
        <label for="filter-month" style="font-size: 16px;">Filter by month:</label>
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
    </div>

    <div id="news-list" style="margin-top: 20px;">
      <div class="news-item" data-year="2024" data-month="09">
        <p style="font-size: 15px; text-align: justify;">09/30/2024: Achieved <strong>GRE score of 303</strong>, including Quantitative 157 and Verbal 146, Analytical Writing 3.5.</p>
      </div>

      <div class="news-item" data-year="2024" data-month="10">
        <p style="font-size: 15px; text-align: justify;">10/29/2024: Earned an overall band of <strong>7.0 in IELTS</strong>, with 8.0 in Listening and 7.0 in Reading and Writing.</p>
      </div>

      <div class="news-item" data-year="2024" data-month="09">
        <p style="font-size: 15px; text-align: justify;">09/15/2024: Published research on <strong>Reverse Logistics AI</strong> in Supply Chain Analytics.</p>
      </div>

      <div class="news-item" data-year="2023" data-month="06">
        <p style="font-size: 15px; text-align: justify;">06/30/2023: Joined <strong>Unilever Consumer Care Limited</strong> as a Supply Chain Planning Officer.</p>
      </div>

      <div class="news-item" data-year="2022" data-month="09">
        <p style="font-size: 15px; text-align: justify;">09/10/2022: Completed <strong>ULIP Internship</strong> at Unilever Bangladesh Limited in Supply Chain.</p>
      </div>

      <div class="news-item" data-year="2022" data-month="04">
        <p style="font-size: 15px; text-align: justify;">04/30/2022: Graduated with a <strong>Bachelor of Science in Industrial & Production Engineering</strong> from Khulna University of Engineering & Technology.</p>
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