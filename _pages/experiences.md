---
layout: archive
title: "Job Experience"
permalink: /experience/
author_profile: true
---

<div class="main-content">
  <div id="experience">
    <h2 style="text-align: left; font-size: 18px; font-weight: bold;">EXPERIENCES</h2>

    <div class="experience" data-year="2023">
      <p style="font-size: 15px; text-align: justify;">🛠 <strong>Supply Chain Planning Officer – Nutrition</strong><br> 🏢 <a href="https://www.unileverconsumercarebd.com/" target="_blank"><strong>Unilever Consumer Care Limited</strong></a>, Dhaka<br>📅 <strong>Jun 2023 – Aug 2024</strong></p>

      <!-- Sliding Photo Gallery -->
      <div class="photo-gallery" style="margin-top: 10px; text-align: center;">
        <div class="slider-container" style="position: relative; width: 80%; aspect-ratio: 16 / 9; margin: 0 auto; overflow: hidden; border-radius: 10px; background-color: #f4f4f4;">
          <div class="slider" style="display: flex; transition: transform 0.5s ease-in-out; height: 100%;">
            <div class="slide" style="min-width: 100%; display: flex; align-items: center; justify-content: center;">
              <img src="/files/job/unilever1.jpeg" alt="Image 1" style="max-width: 100%; max-height: 100%; object-fit: contain;">
            </div>
            <div class="slide" style="min-width: 100%; display: flex; align-items: center; justify-content: center;">
              <img src="/files/job/unilever2.jpeg" alt="Image 2" style="max-width: 100%; max-height: 100%; object-fit: contain;">
            </div>
            <div class="slide" style="min-width: 100%; display: flex; align-items: center; justify-content: center;">
              <img src="/files/job/unilever3.jpeg" alt="Image 3" style="max-width: 100%; max-height: 100%; object-fit: contain;">
            </div>
          </div>
        </div>
        <div style="font-size: 14px; margin-top: 10px;">
          <span id="slide-caption">First image description</span>
        </div>
        <div class="slider-controls" style="margin-top: 10px; display: flex; align-items: center; justify-content: center;">
          <button onclick="moveSlide(-1)" style="background: none; border: none; font-size: 18px; cursor: pointer; margin-right: 10px;">⬅️</button>
          <span id="slide-counter" style="font-size: 16px;">1/3</span>
          <button onclick="moveSlide(1)" style="background: none; border: none; font-size: 18px; cursor: pointer; margin-left: 10px;">➡️</button>
        </div>
      </div>

      <ul style="font-size: 15px; text-align: justify; padding-left: 20px;">
        <li>Craft Master Production Schedule (MPS) considering production capacity, Overall Equipment Efficiency (OEE), resource utilization, sales achievement, and inventory strategies.</li>
        <li>Develop Material Requirement Planning (MRP) considering reordering points, MOQ, Days On Hand (DOH) coverage and assist Distribution Requirement Planning (DRP) considering inventory targets and demand dynamics.</li>
        <li>Drive & monitor Supply Planning KPIs: Dispatch Rate (DR), Service Level (OTIF), Inventory FG & RM.</li>
      </ul>
    </div>

    <hr>

    <div class="experience" data-year="2022">
      <p style="font-size: 15px; text-align: justify;">🛠 <strong>Unilever Leadership Internship Program (ULIP) Supply Chain Intern</strong><br> 🏢 <a href="https://www.unilever.com.bd/" target="_blank"><strong>Unilever Bangladesh Limited</strong></a>, Dhaka<br>📅 <strong>Sep 2022 – Dec 2022</strong></p>

      <!-- Sliding Photo Gallery -->
      <div class="photo-gallery" style="margin-top: 10px; text-align: center;">
        <div class="slider-container" style="position: relative; width: 80%; aspect-ratio: 16 / 9; margin: 0 auto; overflow: hidden; border-radius: 10px; background-color: #f4f4f4;">
          <div class="slider" style="display: flex; transition: transform 0.5s ease-in-out; height: 100%;">
            <div class="slide" style="min-width: 100%; display: flex; align-items: center; justify-content: center;">
              <img src="/files/job/intern1.jpeg" alt="Image 1" style="max-width: 100%; max-height: 100%; object-fit: contain;">
            </div>
            <div class="slide" style="min-width: 100%; display: flex; align-items: center; justify-content: center;">
              <img src="/files/job/intern2.jpeg" alt="Image 2" style="max-width: 100%; max-height: 100%; object-fit: contain;">
            </div>
            <div class="slide" style="min-width: 100%; display: flex; align-items: center; justify-content: center;">
              <img src="/files/job/intern3.jpeg" alt="Image 3" style="max-width: 100%; max-height: 100%; object-fit: contain;">
            </div>
          </div>
        </div>
        <div style="font-size: 14px; margin-top: 10px;">
          <span id="slide-caption">First image description</span>
        </div>
        <div class="slider-controls" style="margin-top: 10px; display: flex; align-items: center; justify-content: center;">
          <button onclick="moveSlide(-1)" style="background: none; border: none; font-size: 18px; cursor: pointer; margin-right: 10px;">⬅️</button>
          <span id="slide-counter" style="font-size: 16px;">1/3</span>
          <button onclick="moveSlide(1)" style="background: none; border: none; font-size: 18px; cursor: pointer; margin-left: 10px;">➡️</button>
        </div>
      </div>

      <ul style="font-size: 15px; text-align: justify; padding-left: 20px;">
        <li>Got selected for the prestigious Unilever Leadership Internship Programme (ULIP) in Supply Chain competing nationally against 4,500+ candidates through a rigorous 4-phase recruitment process.</li>
        <li>Successfully completed induction on manufacturing, warehouse, operations, and quality at MFPL, Gazipur factory, gaining a thorough understanding of the production process.</li>
      </ul>
    </div>
  </div>
</div>

<script>
let currentSlide = 0;
const totalSlides = 3; // Number of slides per gallery

function moveSlide(direction) {
  const slider = document.querySelector('.slider');
  currentSlide = (currentSlide + direction + totalSlides) % totalSlides;
  slider.style.transform = `translateX(-${currentSlide * 100}%)`;
  document.getElementById('slide-counter').textContent = `${currentSlide + 1}/${totalSlides}`;
}
</script>
