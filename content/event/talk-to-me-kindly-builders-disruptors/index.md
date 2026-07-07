---
title: 'Talk to Me Kindly: Designing AI Companions to Foster Positive Self-Talk in Young Adults'

event: Cornell Tech Builders and Disruptors in the AI Era
event_url: ''

location: Cornell Tech
address:
  city: New York
  region: NY
  country: United States

summary: A talk on designing AI companions to foster positive self-talk in young adults.

# Talk start and end times.
date: '2025-12-05T00:00:00Z'
all_day: true

# Schedule page publish date (NOT talk date).
publishDate: '2026-07-06T00:00:00Z'

authors:
  - admin

tags: []

# Is this a featured talk? (true/false)
featured: true

url_code: ''
url_pdf: ''
url_slides: 'slides.pdf'
url_video: ''

slides: ""

projects:
  - talk-to-me-kindly
---

<div class="slide-carousel" id="slide-carousel-1">
  <div class="slide-carousel-viewport">
    <img src="slides/slide-01.jpg" class="slide-carousel-img active" alt="Slide 1">
    <img src="slides/slide-02.jpg" class="slide-carousel-img" alt="Slide 2">
    <img src="slides/slide-03.jpg" class="slide-carousel-img" alt="Slide 3">
    <img src="slides/slide-04.jpg" class="slide-carousel-img" alt="Slide 4">
    <img src="slides/slide-05.jpg" class="slide-carousel-img" alt="Slide 5">
    <img src="slides/slide-06.jpg" class="slide-carousel-img" alt="Slide 6">
    <img src="slides/slide-07.jpg" class="slide-carousel-img" alt="Slide 7">
    <img src="slides/slide-08.jpg" class="slide-carousel-img" alt="Slide 8">
    <img src="slides/slide-09.jpg" class="slide-carousel-img" alt="Slide 9">
    <img src="slides/slide-10.jpg" class="slide-carousel-img" alt="Slide 10">
    <img src="slides/slide-11.jpg" class="slide-carousel-img" alt="Slide 11">
    <img src="slides/slide-12.jpg" class="slide-carousel-img" alt="Slide 12">
    <img src="slides/slide-13.jpg" class="slide-carousel-img" alt="Slide 13">
    <img src="slides/slide-14.jpg" class="slide-carousel-img" alt="Slide 14">
    <img src="slides/slide-15.jpg" class="slide-carousel-img" alt="Slide 15">
    <img src="slides/slide-16.jpg" class="slide-carousel-img" alt="Slide 16">
    <img src="slides/slide-17.jpg" class="slide-carousel-img" alt="Slide 17">
    <img src="slides/slide-18.jpg" class="slide-carousel-img" alt="Slide 18">
    <button class="slide-carousel-prev" aria-label="Previous slide">&#8249;</button>
    <button class="slide-carousel-next" aria-label="Next slide">&#8250;</button>
  </div>
  <div class="slide-carousel-counter">1 / 18</div>
</div>

<style>
  .slide-carousel { max-width: 800px; margin: 0 auto; }
  .slide-carousel-viewport { position: relative; width: 100%; aspect-ratio: 16 / 9; background: #000; border-radius: 0.5rem; overflow: hidden; }
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
  var root = document.getElementById('slide-carousel-1');
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
