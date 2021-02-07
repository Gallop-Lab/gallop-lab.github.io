---
layout: page
title:  "Research"
header: |
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/2.0.2/jquery.min.js"></script>
  <script type="text/javascript" src="//cdn.jsdelivr.net/gh/kenwheeler/slick@1.8.1/slick/slick.min.js"></script>
  <link rel="stylesheet" type="text/css" href="//cdn.jsdelivr.net/gh/kenwheeler/slick@1.8.1/slick/slick.css"/>
  <link rel="stylesheet" type="text/css" href="//cdn.jsdelivr.net/gh/kenwheeler/slick@1.8.1/slick/slick-theme.css"/>
  <style>
  .carousel div {
  width: auto;
  height: 300px;
  background-color: black;
  background-size: 100% auto;
  background-position: 0% 50%;
  }
  </style>
  
carousel:
  - image: /images/2_research_gallery/05.png
  - image: /images/2_research_gallery/10.png
  - image: /images/2_research_gallery/07.png
  - image: /images/2_research_gallery/09.png
  - image: /images/2_research_gallery/03.png
---

{% if page.carousel %}
<div class='carousel'>
  {% for slides in page.carousel %}
  <div style="background-image: url({{ slides.image }});"></div>
  {% endfor %}
</div>
<script type="text/javascript">
    $(document).ready(function(){
      $('.carousel').slick({
        slidesToShow: 1,
	autoplay: true,
	autoplaySpeed: 5000,
	fade: true,
	cssEase: 'linear',
        dots: true,
        arrows: false,
      });
    });
</script>
{% endif %}

We are interested in how filopodia form and in understanding how to intervene in actin assembly therapeutically. Our current questions include:

* What happens when filopodia initiate and extend?
* What determines the length and lifetime of filopodia, and related in vitro filopodia-like structures?
* How do cells orchestrate filopodia during axon guidance, synaptogenesis and cancer metastasis?

To answer these questions we are using a combination of biochemistry and quantitative imaging in a variety of cells. We enjoy a diverse range of external collaborations as well as collaborating with each other within the lab, and pursuing our own individual projects. We aim to be highly innovative in our approaches, use cutting-edge technologies and support everyone's ambitions.
