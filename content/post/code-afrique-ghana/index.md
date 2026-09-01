---
title: 'Taught Python and data science with Code Afrique 2025 in Accra, Ghana'
summary: "Served as a teaching assistant, mentor, and teacher at Code Afrique 2025 in Accra, Ghana, teaching Python and data science to K-12 students."
date: 2026-08-13

authors:
  - admin

tags:
  - Outreach
---

Traveled to Accra, Ghana, to serve as a teaching assistant, mentor, and teacher at Code Afrique 2025, a coding bootcamp hosted at Academic City University by [Code Afrique](https://codeafrique.org/), a nonprofit that gives African science students a window into computer science. Taught Python and data science to K-12 students, August 10-13, 2026.

Students worked hands-on in Python, using pandas and matplotlib to load, clean, and plot real World Bank population data, and we also walked through how large language models work, mapping the ideas back to the regression and modeling concepts from earlier in the week. The cohort worked alongside volunteers and mentors from Cornell Bowers CIS, Meta, LinkedIn, and IEEE.

<div class="slide-carousel" id="code-afrique-carousel">
  <div class="slide-carousel-viewport">
    <img src="photos/photo-01-shirt.jpg" class="slide-carousel-img active" alt="Wearing a Code Afrique t-shirt reading 'Reimagining Learning for Global Impact in AI + Data Science' on the Academic City University campus">
    <img src="photos/photo-02-lab-session.jpg" class="slide-carousel-img" alt="Teaching a computer lab session on pandas and plotting population data">
    <img src="photos/photo-03-llm-lecture.jpg" class="slide-carousel-img" alt="Leading a lesson on how large language models work">
    <img src="photos/photo-04-group.jpg" class="slide-carousel-img" alt="Group photo of the Code Afrique 2025 cohort in orange t-shirts on campus">
    <img src="photos/photo-05-campus-evening.jpg" class="slide-carousel-img" alt="Academic City University campus in the evening">
    <button class="slide-carousel-prev" aria-label="Previous slide">&#8249;</button>
    <button class="slide-carousel-next" aria-label="Next slide">&#8250;</button>
  </div>
  <div class="slide-carousel-counter">1 / 5</div>
</div>

<style>
  .slide-carousel { max-width: 800px; margin: 0 auto; }
  .slide-carousel-viewport { position: relative; width: 100%; aspect-ratio: 4 / 3; background: #000; border-radius: 0.5rem; overflow: hidden; }
  .slide-carousel-img { position: absolute; inset: 0; width: 100%; height: 100%; object-fit: contain; opacity: 0; transition: opacity 0.4s ease; }
  .slide-carousel-img.active { opacity: 1; }
  .slide-carousel-prev, .slide-carousel-next { position: absolute; top: 50%; transform: translateY(-50%); background: rgba(0,0,0,0.5); color: #fff; border: none; width: 2.5rem; height: 2.5rem; border-radius: 9999px; cursor: pointer; font-size: 1.5rem; line-height: 1; z-index: 2; }
  .slide-carousel-prev { left: 0.75rem; }
  .slide-carousel-next { right: 0.75rem; }
  .slide-carousel-prev:hover, .slide-carousel-next:hover { background: rgba(0,0,0,0.75); }
  .slide-carousel-counter { text-align: center; margin-top: 0.5rem; font-size: 0.875rem; color: #6b7280; }
</style>

<script>
(function () {
  var root = document.getElementById('code-afrique-carousel');
  if (!root) return;
  var imgs = root.querySelectorAll('.slide-carousel-img');
  var counter = root.querySelector('.slide-carousel-counter');
  var total = imgs.length;
  var current = 0;
  var intervalMs = 4000;
  var timer;

  function show(i) {
    imgs[current].classList.remove('active');
    current = (i + total) % total;
    imgs[current].classList.add('active');
    counter.textContent = (current + 1) + ' / ' + total;
  }

  function next() { show(current + 1); }
  function prev() { show(current - 1); }

  function resetTimer() {
    clearInterval(timer);
    timer = setInterval(next, intervalMs);
  }

  root.querySelector('.slide-carousel-next').addEventListener('click', function () { next(); resetTimer(); });
  root.querySelector('.slide-carousel-prev').addEventListener('click', function () { prev(); resetTimer(); });

  resetTimer();
})();
</script>
