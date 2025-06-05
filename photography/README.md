---
layout: page
title: Photography
hide_description: true
sitemap: false
permalink: /photography/
---

<style>
  /* Justify paragraphs on this page */
  .layout-page p {
    text-align: justify;
  }

  /* Masonry‐style grid CSS */
  .photo-grid-js {
    width: 100%;           /* Must be 100% so Masonry computes two 45% columns */
    margin-left: -0.5rem;  /* half of the gutter */
    /* NO opacity:0 here—allow images to render immediately */
  }
  .photo-grid-js .grid-item {
    width: 45%;            /* Two columns: 45% + 45% + 16px gutter */
    padding-left: 0.5rem;  /* left‐side gutter */
    margin-bottom: 1rem;   /* vertical gutter */
  }
  .photo-grid-js .grid-item img {
    display: block;
    width: 100%;
    height: auto;
    border-radius: 4px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  }

  /* Lightbox Styles */
  #lightbox {
    position: fixed;
    top: 0; left: 0;
    width: 100%; height: 100%;
    background: rgba(0,0,0,0.85);
    display: flex;
    justify-content: center;
    align-items: center;
    z-index: 1000;
    opacity: 0;
    transform: scale(0.9);
    pointer-events: none;
    transition: opacity 0.2s ease-out,
                transform 0.2s cubic-bezier(0.33,1,0.68,1);
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

  /* Optional breakpoints if you want 2 columns under 768px or 1 column under 480px:
  @media (max-width: 768px) {
    .photo-grid-js .grid-item { width: 50%; }
  }
  @media (max-width: 480px) {
    .photo-grid-js .grid-item { width: 100%; }
  }
  */
</style>

When I am not working or doing research, I really like taking photos, especially **landscapes**, **astrophotography**, and **moon/sun alignments**. Here are a few photos that I like.

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

<div id="lightbox" onclick="closeLightbox()">
  <img id="lightbox-img" src="" alt="Expanded Image">
</div>

<!-- Load imagesLoaded & Masonry from CDN -->
<script src="https://unpkg.com/imagesloaded@4/imagesloaded.pkgd.min.js"></script>
<script src="https://unpkg.com/masonry-layout@4/dist/masonry.pkgd.min.js"></script>

<script>
  function openLightbox(img) {
    document.getElementById("lightbox-img").src = img.src;
    document.getElementById("lightbox").classList.add("show");
  }
  function closeLightbox() {
    document.getElementById("lightbox").classList.remove("show");
  }

  window.addEventListener("load", function() {
    const grid = document.querySelector('.photo-grid-js');
    if (!grid) return;

    // 1) Instantiate Masonry with initLayout: false so it won't immediately collapse everything.
    const msnry = new Masonry(grid, {
      itemSelector: '.grid-item',
      columnWidth: '.grid-item',  /* ensures Masonry uses each .grid-item’s width */
      percentPosition: true,
      gutter: 16,
      initLayout: false         /* ← do NOT do the first layout pass yet */
    });

    // 2) Wait for ALL images in “grid” to load, then trigger layout exactly once.
    imagesLoaded(grid, function() {
      msnry.layout();
    });
  });
</script>
