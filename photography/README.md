---
layout: page
title: Photography
description: >
  Here you should be able to find everything you need to know to accomplish the most common tasks when blogging with Hydejack.
hide_description: true
sitemap: false
permalink: /photography/
---

0. this unordered seed list will be replaced by toc as unordered list
{:toc}

<style>
  /* Target only this CV page’s paragraphs and force‐justify them */
  .layout-page p {
    text-align: justify;
  }
</style>

When I am not working or doing research, I really like taking photos, especially landscapes and astrophotography. Here are a few photos that I like.

<div class="photo-grid">
  <img src="../assets/photos/Hummingbird-3.jpg" alt="Photo 1" onclick="openLightbox(this)">
  <img src="../assets/photos/Camilo-1.jpg" alt="Photo 2" onclick="openLightbox(this)">
  <img src="../assets/photos/Zimapan-2.jpg" alt="Photo 3" onclick="openLightbox(this)">
  <img src="../assets/photos/Guelaguetza-1.jpg" alt="Photo 4" onclick="openLightbox(this)">
  <img src="../assets/photos/Hierve-el-Agua-2.jpg" alt="Photo 5" onclick="openLightbox(this)">
  <img src="../assets/photos/Moon-HDR.jpg" alt="Photo 6" onclick="openLightbox(this)">
</div>

<!-- Lightbox container -->
<div id="lightbox" onclick="closeLightbox()">
  <img id="lightbox-img" src="" alt="Expanded Image">
</div>

<style>
.photo-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 1rem;
  margin-top: 1rem;
}
.photo-grid img {
  width: 100%;
  height: auto;
  object-fit: cover;
  border-radius: 0.5rem;
  cursor: pointer;
  transition: transform 0.2s ease;
}
.photo-grid img:hover {
  transform: scale(1.03);
}

/* Lightbox styles */
#lightbox {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0,0,0,0.85);
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 1000;
  opacity: 0;
  transform: scale(0.9);
  pointer-events: none;
  transition: opacity 0.2s ease-out, transform 0.2s cubic-bezier(0.33, 1, 0.68, 1); /* snap easing */
}
#lightbox.show {
  opacity: 1;
  transform: scale(1);
  pointer-events: auto;
}

#lightbox img {
  max-width: 90%;
  max-height: 90%;
  border-radius: 0.5rem;
  transition: transform 0.3s ease;
}
</style>

<script>
function openLightbox(img) {
  const lightbox = document.getElementById("lightbox");
  const lightboxImg = document.getElementById("lightbox-img");
  lightboxImg.src = img.src;
  lightbox.classList.add("show");
}
function closeLightbox() {
  const lightbox = document.getElementById("lightbox");
  lightbox.classList.remove("show");
}
</script>