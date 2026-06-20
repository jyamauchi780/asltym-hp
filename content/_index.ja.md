+++
draft = false
paige.pages.disable_reading_time = true
paige.pages.disable_word_count = true
paige.site.disable_breadcrumbs = true
paige.pages.disable_toc = true
paige.site.description = "富山大学 自律システム研究室"
paige.pages.disable_collections = true
paige.pages.disable_pages = true
paige.pages.disable_sections = true
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
      font-size: 3.3rem !important;
  }
</style>

<div class="hero-container">
  <img id="hero-image" src="images/tateyama_road2.JPG" alt="ASL Toyama" style="width: 100%; object-fit: cover; border-radius: 1rem;">
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


<div class="text-center mt-4 d-flex justify-content-center align-items-center gap-4">
  <a href="https://bitbucket.org/asl_tym/workspace/projects/OPEN" target="_blank">
    <img src="icons/Bitbucket_attribution_dark.svg"
         alt="Bitbucket"
         style="height:38px;">
  </a>

  <a href="https://www.youtube.com/@asltym" target="_blank">
    <img src="icons/yt_icon_red_digital.png"
         alt="YouTube"
         style="height:60px;">
  </a>
</div>

<div align="center">

  ## News
  |  |  |
  |---|---|
  | 2026.09    | 第44回 日本ロボット学会学術講演会 (RSJ) で発表します |
  | 2026.07.22  | Atman先生（Univ. Turku）が来研されます |
  | 2026.07.10  | 倉科先生（東京農工大学）が来研されます |
  | 2026.06.19  | 畑中研究室（東京科学大学）を訪問しました |
  | 2026.06.09  | 研究室ホームページを公開しました |
  | 2024.04.01 | 自律システム研究室が発足しました |

</div>

