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
  - image: /~galloplab/images/2_research_gallery/05.png
  - image: /~galloplab/images/2_research_gallery/10.png
  - image: /~galloplab/images/2_research_gallery/07.png
  - image: /~galloplab/images/2_research_gallery/09.png
  - image: /~galloplab/images/2_research_gallery/03.png
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

We are interested in how actin assembles during endocytosis and filopodia formation. There are many proteins involved in both these processes. Our current key questions ask:

* How does the membrane bend to make a vesicle or filopodium and how is this curvature change communicated to the actin assembly?
* How do phosphoinositide lipids selectively recruit and activate the proteins involved in actin regulation?
* How do cells orchestrate this cell biology to do interesting things like migrating, and forming adhesions and synapses in the right places?

To answer these questions we reconstitute the membrane-cytosol interface in vitro using artificial lipid membranes and frog egg extracts as cytosol and take away and add in components to figure out how the biochemistry works. We try to find the essential crux of the answer and then take this into cells - neurons, Drosophila embryos or cell culture depending on what we want to know. We use quantitative imaging in all our work. We believe in collaborating with each other, as well as working on our own individual projects, to achieve common goals.