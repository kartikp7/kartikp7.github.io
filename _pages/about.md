---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a 3rd year PhD candidate at [University of California, Davis](https://www.ucdavis.edu/) - [ECE Department](https://ece.ucdavis.edu/), advised by Prof. [Chen-Nee Chuah](https://www.ece.ucdavis.edu/~chuah/rubinet/people/chuah/bio.html). 
<!-- I received my B.S. (Computer Engineering major, Computer Science minor) from UC Davis in December 2020 and my M.S. in March 2024.  -->
I am currently an Applied Scientist intern at Amazon under [Noranart (Sol) Vesdapunt](https://noranart.com/?i=1) and [Ning Zhou](https://www.linkedin.com/in/ningzh). 

**Previously**: I interned at [Sony AI](https://ai.sony/) - PPML team in summer 2023 under the mentorship of Dr. [Lingjuan Lv](https://sites.google.com/view/lingjuan-lyu/home?authuser=0) and Dr. [Vivek Sharma](https://vivoutlaw.github.io/index.html). I also interned at [Sony](https://www.sony.com/en/) - Imaging & Sensing during summer 2022 under Mr. [Hideshi Yamada](https://www.linkedin.com/in/hideshi-yamada-3593aa101/?originalSubdomain=jp). 

**Research Interests**: Privacy-Preserving Computer Vision, Multi-Modal LLMs, Vision-Language Models, Generative AI

<!-- **Previous work**:
  - Adversarial Robustness
  - Neural Network Pruning
  - Model Extraction/Fingerprinting -->

-----

# Selected Publications

{% assign selected_pubs = site.publications | sort: 'date' | reverse | where_exp: "post", "post.selected == true" %}

{% for post in selected_pubs limit:3 %}
  {% include archive-single.html %}
{% endfor %}

### [See more...]({{ site.url }}/publications)

-----

# News

{% include base_path %}
{% capture written_year %}'None'{% endcapture %}
{% for post in site.posts  limit:3  %}
  {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
  {% include archive-single.html %}
{% endfor %}

### [See more...]({{ site.url }}/updates)
