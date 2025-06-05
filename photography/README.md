---
layout: page
title: Photography
description: >
  Here you should be able to find everything you need to know to accomplish the most common tasks when blogging with Hydejack.
hide_description: true
sitemap: false
permalink: /photography/
---

<!--
  Always reload once on entering /photography/ by using a URL parameter.
  If “reload=1” is not present, append it and reload.
-->
<script>
  (function() {
    const params = new URLSearchParams(window.location.search);
    if (!params.has('reload')) {
      params.set('reload', '1');
      window.location.replace(window.location.pathname + '?' + params.toString());
    }
  })();
</script>

0. this unordered seed list will be replaced by toc as unordered list
  {:toc}

<style>
  /* Target only this CV page’s paragraphs and force‐justify them */
  .layout-page p {
    text-align: justify;
  }
  /* Masonry‐style grid CSS */
  /* ================================
     PHOTO GRID (MASONRY.JS, 2 COLS)
     ================================ */
  .photo-grid-js {
    margin-left: -0.5rem; /* half of the gutter to “pull back” */
    width: auto;
  }
  
  .photo-grid-js .grid-item {
    width: 45.0%;         /* two 45% columns + gutter */
    padding-left: 0.5rem; /* left‐side gutter of 0.5rem */
    margin-bottom: 1rem;  /* vertical gutter between rows */
  }
  
  .photo-grid-js .grid-item img {
    display: block;
    width: 100%;
    height: auto;
    border-radius: 4px;                          
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);     
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
    transition: opacity 0.2s ease-out, transform 0.2s cubic-bezier(0.33, 1, 0.68, 1);
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

  /* Responsive: 2 columns below 768px */
  /* @media (max-width: 768px) {
    .photo-grid-js .grid-item {
      width: 50%;
    }
  } */
  /* Responsive: 1 column below 480px */
  /* @media (max-width: 480px) {
    .photo-grid-js .grid-item {
      width: 100%;
    }
  } */
</style>

When I am not working or doing research, I really like taking photos, especially **landscapes**, **astrophotography** and **moon/sun alignments**. Here are a few photos that I like.

<!-- ======= PHOTO GRID SECTION ======= -->
<div class="photo-grid-js">
  <div class="grid-item">
    <img src="../assets/photos/Hummingbird-3.jpg" alt="Hummingbird" onclick="openLightbox(this)">
  </div>
  <div class="grid-item">
    <img src="../assets/photos/Zimapan-2.jpg" alt="Zimapan" onclick="openLightbox(this)">
  </div>
  <div class="grid-item">
    <img src="../assets/photos/Guelaguetza-1.jpg" alt="Guelaguetza" onclick="openLightbox(this)">
  </div>
  <div class="grid-item">
    <img src="../assets/photos/Xochimilco-3.jpg" alt="Xochimilco" onclick="openLightbox(this)">
  </div>
  <div class="grid-item">
    <img src="../assets/photos/Hierve-el-Agua-2.jpg" alt="Hierve-el-Agua" onclick="openLightbox(this)">
  </div>
  <div class="grid-item">
    <img src="../assets/photos/Moon-HDR.jpg" alt="Moon-HDR" onclick="openLightbox(this)">
  </div>
  <div class="grid-item">
    <img src="../assets/photos/Zimapan-1.jpg" alt="Zimapan" onclick="openLightbox(this)">
  </div>
  <div class="grid-item">
    <img src="../assets/photos/Dia-de-Muertos-1.jpg" alt="Dia-de-Muertos" onclick="openLightbox(this)">
  </div>
  <div class="grid-item">
    <img src="../assets/photos/Hummingbird-1.jpg" alt="Hummingbird" onclick="openLightbox(this)">
  </div>
  <div class="grid-item">
    <img src="../assets/photos/Camilo-1.jpg" alt="Camilo" onclick="openLightbox(this)">
  </div>
  <div class="grid-item">
    <img src="../assets/photos/Angel-de-la-Independencia-1.jpg" alt="Angel-de-la-Independencia" onclick="openLightbox(this)">
  </div>
  <div class="grid-item">
    <img src="../assets/photos/Dia-de-Muertos-2.jpg" alt="Dia-de-Muertos" onclick="openLightbox(this)">
  </div>
  <div class="grid-item">
    <img src="../assets/photos/Dia-de-Muertos-3.jpg" alt="Dia-de-Muertos" onclick="openLightbox(this)">
  </div>
  <div class="grid-item">
    <img src="../assets/photos/Hierve-el-Agua-1.jpg" alt="Hierve-el-Agua" onclick="openLightbox(this)">
  </div>
  <div class="grid-item">
    <img src="../assets/photos/Xochimilco-1.jpg" alt="Xochimilco" onclick="openLightbox(this)">
  </div>
</div>

<!-- Lightbox container -->
<div id="lightbox" onclick="closeLightbox()">
  <img id="lightbox-img" src="" alt="Expanded Image">
</div>

<!-- Include imagesLoaded + Masonry.js from CDN -->
<script src="https://unpkg.com/imagesloaded@4/imagesloaded.pkgd.min.js"></script>
<script src="https://unpkg.com/masonry-layout@4/dist/masonry.pkgd.min.js"></script>

<script>
  document.addEventListener("DOMContentLoaded", function () {
    var grid = document.querySelector('.photo-grid-js');
    imagesLoaded(grid, function() {
      new Masonry(grid, {
        itemSelector: '.grid-item',
        percentPosition: true,
        gutter: 16
      });
    });
  });

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
