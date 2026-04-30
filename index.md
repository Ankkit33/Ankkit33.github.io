---
layout: home
title: Home
---

# My Homepage  
~ AKKI  

Welcome to my website 🚀
---
layout: home
---

<div class="slider">
  <img src="assets/img1.jpg" class="slide active">
  <img src="assets/img2.jpg" class="slide">
  <img src="assets/img3.jpg" class="slide">
</div>

<style>
.slider {
  position: relative;
  height: 400px;
  overflow: hidden;
}
.slide {
  position: absolute;
  width: 100%;
  height: 100%;
  object-fit: cover;
  opacity: 0;
  transition: 1s;
}
.slide.active {
  opacity: 1;
}
</style>

<script>
let slides = document.querySelectorAll(".slide");
let index = 0;

setInterval(() => {
  slides[index].classList.remove("active");
  index = (index + 1) % slides.length;
  slides[index].classList.add("active");
}, 3000);
</script>

<h1>My Homepage</h1>
<p>~ AKKI</p>
