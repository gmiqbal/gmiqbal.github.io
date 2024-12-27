---
layout: archive
title: "Academics"
permalink: /academics/
author_profile: true
---

<div class="main-content">
  <!-- <h2 style="text-align: left; font-size: 18px; font-weight: bold;">ACADEMICS</h2> -->

  <div class="education" data-year="2022">
    <p style="font-size: 15px; text-align: justify;">🏫 <strong><a href="https://kuet.ac.bd/" target="_blank">Khulna University of Engineering & Technology</a></strong> | Khulna, Bangladesh<br>📅 <strong>Feb 2017 – Apr 2022</strong><br>🎓 Bachelor of Science in Industrial & Production Engineering (IPE)<br>🎯 <strong>CGPA:</strong> 3.65/4.00 (3.78 in last four semesters)</p>
    
    <!-- Sliding Photo Gallery -->
    <div class="photo-gallery" style="margin-top: 20px; text-align: center;">
      <div class="slider-container" style="position: relative; width: 80%; aspect-ratio: 16 / 9; margin: 0 auto; overflow: hidden; border-radius: 10px; background-color: #f4f4f4;">
        <div class="slider" style="display: flex; transition: transform 0.5s ease-in-out; height: 100%;">
          <div class="slide" style="min-width: 100%; display: flex; align-items: center; justify-content: center;">
            <img src="/files/uni/single.jpeg" alt="Image 1" style="max-width: 100%; max-height: 100%; object-fit: contain; cursor: pointer;" onclick="enlargeImage('/files/uni/single.jpeg')">
          </div>
          <div class="slide" style="min-width: 100%; display: flex; align-items: center; justify-content: center;">
            <img src="/files/uni/last_lab.jpeg" alt="Image 2" style="max-width: 100%; max-height: 100%; object-fit: contain; cursor: pointer;" onclick="enlargeImage('/files/uni/last_lab.jpeg')">
          </div>
          <div class="slide" style="min-width: 100%; display: flex; align-items: center; justify-content: center;">
            <img src="/files/uni/discussion.jpeg" alt="Image 3" style="max-width: 100%; max-height: 100%; object-fit: contain; cursor: pointer;" onclick="enlargeImage('/files/uni/discussion.jpeg')">
          </div>
        </div>
      </div>
      <div style="font-size: 14px; margin-top: 10px;"> 
        <span id="slide-caption">At graduation day</span>
      </div>
      <div class="slider-controls" style="margin-top: 10px; display: flex; align-items: center; justify-content: center;">
        <button onclick="moveSlide(-1)" style="background: none; border: none; font-size: 18px; cursor: pointer; margin-right: 10px;">⬅️</button>
        <span id="slide-counter" style="font-size: 16px;">1/3</span>
        <button onclick="moveSlide(1)" style="background: none; border: none; font-size: 18px; cursor: pointer; margin-left: 10px;">➡️</button>
      </div>
    </div>

    <ul style="font-size: 15px; text-align: justify; padding-left: 24px;">
      <li> <strong> Key <a href="https://www.kuet.ac.bd/dept/iem/academic/ugcurriculum" target="_blank">Courses</a> 📖: </strong> Operations Management, Operations Research, Logistics & Supply Chain Management, Management Information System Analysis and Design, Computer Integrated Manufacturing, Quality Management, Production Systems Design, Computer Aided Design.</li>
    </ul>
    <div style="padding-left: 24px; font-size: 15px; text-align: justify;">
      🏅 <strong><a href="https://kuet.ac.bd/office/dean/me" target="_blank">Dean’s List Honoree</a></strong> | Faculty of Mechanical Engineering, Khulna University of Engineering & Technology | 📅 <strong>Mar 2019</strong><br>

      🏅 <strong><a href="https://1drv.ms/i/s!AjAC4dHJ0YrPokAv2B2wFEiaJWYp?e=jZlxUM" target="_blank">1st Runner Up at SolidWorks Workshop’18</a></strong> | IEM Robotics & CAD Club | 📅 <strong>Oct 2018</strong><br>

      🏅 <strong><a href="https://www.kuet.ac.bd/" target="_blank">Technical Scholarship</a></strong> | Khulna University of Engineering & Technology | 📅 <strong>Four consecutive academic years</strong><br>

      🏅 <strong><a href="https://iscea-bangladesh.com/ptakprize/" target="_blank">ISCEA PTAK Prize Case Competition - 60% Scholarship</a></strong> | International Supply Chain Education Alliance Bangladesh | 📅 <strong>Jul 2021</strong><br>

      🏅 <strong><a href="https://www.linkedin.com/company/supplychainalliancebangladesh/posts/?feedView=all" target="_blank">Top 10 Finalists of ‘SCA Upstream’ Inter-University Case Competition</a></strong> | Supply Chain Alliance, Dhaka University - Faculty of Business Studies | 📅 <strong>Oct 2020</strong>
    </div>
  </div>

  <hr>

  <div class="education" data-year="2016">
    <p style="font-size: 15px; text-align: justify;">🏫 <strong><a href="#" target="_blank">Chittagong College</a></strong><br>📅 <strong>2014 – 2016</strong><br>🎓 Higher Secondary Certificate (HSC)<br>🎯 <strong>GPA:</strong> 5.00 / 5.00</p>
  </div>

  <hr>

  <div class="education" data-year="2014">
    <p style="font-size: 15px; text-align: justify;">🏫 <strong><a href="#" target="_blank">Govt. Muslim High School, Chittagong</a></strong><br>📅 <strong>2012 – 2014</strong><br>🎓 Secondary School Certificate (SSC)<br>🎯 <strong>GPA:</strong> 5.00 / 5.00</p>
  </div>
</div>

<div id="imageModal" style="display: none; position: fixed; top: 0; left: 0; width: 100%; height: 100%; background-color: rgba(0, 0, 0, 0.8); z-index: 1000; align-items: center; justify-content: center;">
  <span style="position: absolute; top: 20px; right: 30px; font-size: 30px; color: white; cursor: pointer;" onclick="closeModal()">&times;</span>
  <img id="modalImage" src="" style="max-width: 90%; max-height: 90%; border-radius: 10px;">
</div>

<script>
let currentSlide = 0;
const totalSlides = document.querySelectorAll('.slide').length;
const captions = ["At graduation day", "Last lab at university", "Post central viva discussion"];
const counterElement = document.getElementById('slide-counter');
const captionElement = document.getElementById('slide-caption');

function moveSlide(direction) {
  const slider = document.querySelector('.slider');
  currentSlide = (currentSlide + direction + totalSlides) % totalSlides;
  slider.style.transform = `translateX(-${currentSlide * 100}%)`;
  counterElement.textContent = `${currentSlide + 1}/${totalSlides}`;
  captionElement.textContent = captions[currentSlide];
}

// Auto-slide every 2 seconds
setInterval(() => {
  moveSlide(1);
}, 2000);

function enlargeImage(src) {
  const modal = document.getElementById('imageModal');
  const modalImage = document.getElementById('modalImage');
  modal.style.display = 'flex';
  modalImage.src = src;
}

function closeModal() {
  const modal = document.getElementById('imageModal');
  modal.style.display = 'none';
}
</script>
