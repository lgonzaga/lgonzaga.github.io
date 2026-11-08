---
permalink: /
title: "Luiz Gonzaga Jr"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% assign pubs = site.publications | sort: "date" | reverse %}

<div class="home">

<section class="home-hero">
  <p class="home-hero__role">Professor · Unisinos University · Head of Vizlab</p>
  <h2 class="home-hero__title">Visual computing, multimodal imaging and immersive technologies for strategic problems</h2>
  <p class="home-hero__lead">I lead Vizlab (Center of Excellence Geoinformatics &amp; Visual Computing) in South Brazil, where we turn applied research into innovative solutions for oil &amp; gas exploration, road safety and rare earth elements in mining.</p>
</section>

<div class="home-facts">
  <div class="home-fact"><span class="home-fact__value">2004</span><span class="home-fact__label">Professor at Unisinos since</span></div>
  <div class="home-fact"><span class="home-fact__value">{{ site.publications.size }}</span><span class="home-fact__label">Recent papers listed here</span></div>
  <div class="home-fact"><span class="home-fact__value">PhD</span><span class="home-fact__label">Computer Engineering, UNICAMP</span></div>
  <div class="home-fact"><span class="home-fact__value">Vizlab</span><span class="home-fact__label">Founder &amp; head</span></div>
</div>

<section class="home-section">
  <h2>Research</h2>
  <div class="home-cards">
    <div class="home-card">
      <span class="home-card__icon"><i class="fas fa-vr-cardboard" aria-hidden="true"></i></span>
      <h3>Immersive multimodal visualization</h3>
      <p>Virtual, mixed and x-reality environments integrating stereo 360° imagery, lidar and depth sensors.</p>
    </div>
    <div class="home-card">
      <span class="home-card__icon"><i class="fas fa-layer-group" aria-hidden="true"></i></span>
      <h3>Multimodal image analysis</h3>
      <p>Imaging sensors from ultraviolet to thermal infrared, fused with remote sensing and laboratory data.</p>
    </div>
    <div class="home-card">
      <span class="home-card__icon"><i class="fas fa-eye" aria-hidden="true"></i></span>
      <h3>Applied computer vision</h3>
      <p>Image processing, machine learning and deep learning to predict quantitative parameters and extract knowledge.</p>
    </div>
  </div>

  <div class="home-spectrum" role="img" aria-label="Spectral ranges: UV, visible, VNIR, SWIR, MWIR, LWIR">
    <span class="uv">UV</span><span class="vis">VIS</span><span class="vnir">VNIR</span><span class="swir">SWIR</span><span class="mwir">MWIR</span><span class="lwir">LWIR</span>
  </div>
  <p class="home-spectrum-caption">Spectral ranges covered by our sensors and applications.</p>
</section>

<section class="home-section">
  <h2>Application areas</h2>
  <div class="home-cards home-cards--4">
    <div class="home-card">
      <span class="home-card__icon"><i class="fas fa-oil-can" aria-hidden="true"></i></span>
      <h3>Oil &amp; gas exploration</h3>
      <p>Digital outcrops and reservoir characterization in petroleum geology.</p>
    </div>
    <div class="home-card">
      <span class="home-card__icon"><i class="fas fa-road" aria-hidden="true"></i></span>
      <h3>Road safety</h3>
      <p>Immersive simulation and visualization for road design and driver behavior.</p>
    </div>
    <div class="home-card">
      <span class="home-card__icon"><i class="fas fa-gem" aria-hidden="true"></i></span>
      <h3>Rare earth elements</h3>
      <p>Multimodal imaging applied to mineral exploration and mining.</p>
    </div>
    <div class="home-card">
      <span class="home-card__icon"><i class="fas fa-mountain" aria-hidden="true"></i></span>
      <h3>Geoscience education</h3>
      <p>Immersive virtual field experiences for teaching and learning geology.</p>
    </div>
  </div>
</section>

<section class="home-section">
  <h2>Tools I build with</h2>
  <ul class="home-chips">
    <li>C++</li><li>Python</li><li>OpenGL</li><li>OpenCV</li><li>Unreal Engine</li><li>PyTorch</li>
  </ul>
</section>

<section class="home-section">
  <h2>Latest publications</h2>
  <ul class="home-pubs">
    {% for p in pubs limit: 4 %}
    <li>
      <a href="{{ p.paperurl | default: p.url }}">{{ p.title }}</a>
      <span class="home-pubs__meta">{{ p.venue }} · {{ p.date | date: "%Y" }}</span>
    </li>
    {% endfor %}
  </ul>
  <p class="home-more"><a href="{{ '/publications/' | relative_url }}">See all publications <i class="fas fa-arrow-right" aria-hidden="true"></i></a></p>
</section>

<details class="home-bio">
  <summary>Full bio</summary>

  <p>As a Professor at Unisinos University in South Brazil, I lead the Vizlab (Center of Excellence Geoinformatics &amp; Visual Computing). My expertise lies in immersive virtual reality, x-reality, and leveraging multi-source data to tackle complex problems. At Vizlab, I've spearheaded projects focusing on technologies for different application areas, such as the petroleum geology, significantly advancing the field of immersive virtual geology.</p>

  <p>My research combines immersive multimodal visualization, multimodal image analysis and applied computer vision, with strong ties to geoinformatics and remote sensing. I work with imaging sensors across the ultraviolet (UV), visible and infrared (VNIR, SWIR, MWIR and LWIR) spectrum, and apply this framework to strategic problems in oil &amp; gas exploration, road safety and rare earth elements in mining. Our profile is to conduct applied research and turn it into innovative solutions for these areas.</p>

  <p>My current focus includes transforming the education and learning experience in geology and other application areas through immersive technologies. This involves innovative approaches to integrate data from multiple remote sensors and laboratory data, primarily using image processing, computer vision, machine learning and deep learning techniques. This work aims to predict quantitative parameters and extract knowledge, achieving enriched virtual environment and disruptive virtual experiences.</p>

  <p>I have a strong background in programming, especially in C++ and Python, and I'm adept at leveraging technologies such as OpenGL, OpenCV, Unreal Engine, and PyTorch. My expertise is frequently utilized in crafting cutting-edge applications in virtual and mixed reality environments, alongside integration with stereo 360-degree imagery, lidar and depth sensors, as well as sensors operating beyond the visible spectrum. Driven by a deep enthusiasm for these fields, I continuously seek to pioneer new developments in visual computing, playing a key role in the evolution of hyper-immersive reality technologies.</p>
</details>

</div>
