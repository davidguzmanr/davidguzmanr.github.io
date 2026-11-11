---
layout: page
title: Photography
description: >
  Here you should be able to find everything you need to know to accomplish the most common tasks when blogging with Hydejack.
hide_description: true
sitemap: false
permalink: /photography/
# Photos shown in the grid, in order. Each one is placed into whichever column
# is currently shorter (the same rule Masonry.js uses), so the layout is computed
# at build time and renders correctly on the very first frame, with no JavaScript.
# To add a photo, append it here with its pixel dimensions, e.g.
#   python3 -c "from PIL import Image; print(Image.open('assets/photos/NAME.jpg').size)"
photos:
  - { file: Hummingbird-3.jpg, alt: Hummingbird, width: 2048, height: 1365 }
  - { file: Zimapan-2.jpg, alt: Zimapan, width: 2048, height: 1365 }
  - { file: Hierve-el-Agua-2.jpg, alt: Hierve-el-Agua, width: 2011, height: 1454 }
  - { file: Guelaguetza-1.jpg, alt: Guelaguetza, width: 2048, height: 1128 }
  - { file: Xochimilco-3.jpg, alt: Xochimilco, width: 1201, height: 1201 }
  - { file: Tadoussac.jpg, alt: Tadoussac, width: 2048, height: 1365 }
  - { file: Moon-HDR.jpg, alt: Moon-HDR, width: 2048, height: 2048 }
  - { file: Zimapan-1.jpg, alt: Zimapan, width: 1010, height: 2048 }
  - { file: Iztaccihuatl-1.jpg, alt: Iztaccihuatl, width: 2048, height: 844 }
  - { file: Dia-de-Muertos-1.jpg, alt: Dia-de-Muertos, width: 1365, height: 2048 }
  - { file: Camilo-1.jpg, alt: Camilo, width: 2048, height: 1365 }
  - { file: Hummingbird-5.jpg, alt: Hummingbird, width: 1828, height: 1200 }
  - { file: Angel-de-la-Independencia-1.jpg, alt: Angel-de-la-Independencia, width: 1216, height: 1902 }
  - { file: Dia-de-Muertos-2.jpg, alt: Dia-de-Muertos, width: 2048, height: 1609 }
  - { file: Hummingbird-1.jpg, alt: Hummingbird, width: 1728, height: 1332 }
  - { file: Clouds-1.jpg, alt: Clouds, width: 2048, height: 1520 }
  - { file: Hierve-el-Agua-1.jpg, alt: Hierve-el-Agua, width: 2048, height: 1312 }
  - { file: Montreal-Fall-2.jpg, alt: Fall, width: 1365, height: 2048 }
  - { file: Montreal-Fall-1.jpg, alt: Fall, width: 2048, height: 1268 }
  - { file: Montreal-Fall-3.jpg, alt: Fall, width: 2048, height: 1348 }
---

0. this unordered seed list will be replaced by toc as unordered list
{:toc}

<style>
  /* Target only this page’s paragraphs and force‐justify them */
  .layout-page p {
    text-align: justify;
  }

  /* ================================
     PHOTO GRID (2 COLUMNS, STATIC)
     ================================
     Two flex columns, filled at build time (see the Liquid loop below).
     Widths and gutters mirror the previous Masonry.js layout exactly:
     45% columns, a 16px gutter between them and a 1rem gap between rows. */
  .photo-grid {
    display: flex;
    align-items: flex-start;
    gap: 16px;
    margin-left: -0.5rem; /* half of the gutter to “pull back” */
  }

  .photo-grid .photo-column {
    flex: 0 0 45%;
    width: 45%;
    min-width: 0;
  }

  .photo-grid .grid-item {
    padding-left: 0.5rem; /* left‐side gutter of 0.5rem */
    margin-bottom: 1rem;  /* vertical gutter between rows */
  }

  .photo-grid .grid-item img {
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
</style>

When I am not working or doing research, I really like taking photos, especially **landscapes**, **astrophotography** and **moon/sun alignments**. Here are a few photos that I like.

<!-- ======= PHOTO GRID SECTION =======
  Assign each photo to the currently shorter column. Heights are estimated for
  a 370px wide image plus the 16px row gap; only the ratios matter, so the
  assignment is the same at any screen width. -->
{%- assign left_photos = "" | split: "" -%}
{%- assign right_photos = "" | split: "" -%}
{%- assign left_height = 0.0 -%}
{%- assign right_height = 0.0 -%}
{%- for photo in page.photos -%}
  {%- assign item_height = photo.height | times: 370.0 | divided_by: photo.width | plus: 16 -%}
  {%- if left_height <= right_height -%}
    {%- assign left_photos = left_photos | push: photo -%}
    {%- assign left_height = left_height | plus: item_height -%}
  {%- else -%}
    {%- assign right_photos = right_photos | push: photo -%}
    {%- assign right_height = right_height | plus: item_height -%}
  {%- endif -%}
{%- endfor -%}
<div class="photo-grid">
  <div class="photo-column">
    {%- for photo in left_photos %}
    <div class="grid-item">
      <img src="../assets/photos/{{ photo.file }}" width="{{ photo.width }}" height="{{ photo.height }}" alt="{{ photo.alt }}" onclick="openLightbox(this)">
    </div>
    {%- endfor %}
  </div>
  <div class="photo-column">
    {%- for photo in right_photos %}
    <div class="grid-item">
      <img src="../assets/photos/{{ photo.file }}" width="{{ photo.width }}" height="{{ photo.height }}" alt="{{ photo.alt }}" onclick="openLightbox(this)">
    </div>
    {%- endfor %}
  </div>
</div>

<!-- Lightbox container -->
<div id="lightbox" onclick="closeLightbox()">
  <img id="lightbox-img" src="" alt="Expanded Image">
</div>

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
