+++
draft = false
paige.pages.disable_reading_time = true
paige.pages.disable_word_count = true
paige.site.disable_breadcrumbs = true
paige.pages.disable_toc = true
+++
<style>
:root {
  --bs-body-font-family: "Hiragino Sans", "Hiragino Kaku Gothic ProN", "Yu Gothic", "Meiryo", sans-serif;
  --bs-font-sans-serif: "Hiragino Sans", "Hiragino Kaku Gothic ProN", "Yu Gothic", "Meiryo", sans-serif;
}

body,
h1, h2, h3, h4, h5, h6,
.display-1, .display-2, .display-3, .display-4, .display-5, .display-6 {
  font-family: "Hiragino Sans", "Hiragino Kaku Gothic ProN", "Yu Gothic", "Meiryo", sans-serif !important;
}
h1, h2, h3, h4, h5, h6 {
  font-weight: 500 !important;
}
h1 {
    font-size: 2.4rem;
}
h2 {
    font-size: 1.8rem;
}
h3 {
    font-size: 1.5rem;
}
#paige-site-title {
    font-size: 3.5rem !important;
}
</style>

<!-- <img src="images/tateyama_road2.JPG" alt="立山連峰（富山県）" style="width: 100%; height: 100%; object-fit: cover; border-radius: 1rem;"> -->
<div class="hero-container">

  <img id="hero-image" src="images/tateyama_road2.JPG" alt="立山連峰（富山県）" style="width: 100%; height: 100%; object-fit: cover; border-radius: 1rem;">

  <button class="hero-btn left" onclick="prevImage()">❮</button>
  <button class="hero-btn right" onclick="nextImage()">❯</button>

</div>

<style>
.hero-container {
  position: relative;
  width: 100%;
}

.hero-container img {
  width: 100%;
  height: 500px;
  object-fit: cover;
}

.hero-btn {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);

  border: none;
  background: rgba(0,0,0,0.4);
  color: white;

  width: 50px;
  height: 50px;

  cursor: pointer;
  font-size: 24px;
}

.left {
  left: 10px;
}

.right {
  right: 10px;
}
</style>

<script>
const images = [
  "images/tateyama_road2.JPG",
  "images/unazuki.JPG",
];

let current = 0;
const hero = document.getElementById("hero-image");

function showImage(i) {
  current = (i + images.length) % images.length;
  hero.src = images[current];
}

function nextImage() {
  showImage(current + 1);
}

function prevImage() {
  showImage(current - 1);
}

setInterval(nextImage, 5000);
</script>


<div style="text-align:center; margin-top:00px;">

<a href="https://bitbucket.org/asl_tym/workspace/projects/OPEN" target="_blank">
  <img src="icons/Bitbucket_attribution_dark.svg"
       width="12%"
       style="margin:10px;">
</a>

<a href="https://www.youtube.com/@asltym" target="_blank">
  <img src="icons/yt_icon_red_digital.png"
       width="7%"
       style="margin:10px;">
</a>

</div>

<div align="center">

## News
|  |  |
|---|---|
| 2026.06.9 | 研究室ホームページを公開しました．|
| 2024.04.01 | 自律システム研究室が発足しました．|
</div>

