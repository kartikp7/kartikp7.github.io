---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a 4th year PhD candidate at [University of California, Davis](https://www.ucdavis.edu/) - [ECE Department](https://ece.ucdavis.edu/), advised by Prof. [Chen-Nee Chuah](https://www.ece.ucdavis.edu/~chuah/rubinet/people/chuah/bio.html), focusing on Security and Privacy of Computer Vision. 
<!-- I received my B.S. (Computer Engineering major, Computer Science minor) from UC Davis in December 2020 and my M.S. in March 2024.  -->

**Previously**: 
- ***Fall 2025***:PhD ML Engineer Intern at *[Cisco AI Defense](https://www.cisco.com/site/us/en/products/security/ai-defense/index.html)* under [Prashanth Arun](https://www.linkedin.com/in/prashanth-arun-20a7181). 
- ***Spring & Summer 2025***: Applied Scientist intern at *[Amazon](https://www.amazon.com/stores/Ring/page/77B53039-540E-4816-BABB-49AA21285FCF)* Ring (Sunnyvale, CA) under [Noranart (Sol) Vesdapunt](https://noranart.com/?i=1) and [Ning Zhou](https://www.linkedin.com/in/ningzh).
- ***Summer 2023***: PhD Research Intern at *[Sony AI](https://ai.sony/)* - PPML team under the mentorship of Dr. [Lingjuan Lv](https://sites.google.com/view/lingjuan-lyu/home?authuser=0) and Dr. [Vivek Sharma](https://vivoutlaw.github.io/index.html).
- ***Summer 2022***: ML Research Engineer Intern at *[Sony](https://www.sony.com/en/)* - Imaging & Sensing under Mr. [Hideshi Yamada](https://www.linkedin.com/in/hideshi-yamada-3593aa101/?originalSubdomain=jp). 

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
{% for post in site.posts  limit:4  %}
  {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
  {% include archive-single.html %}
{% endfor %}

### [See more...]({{ site.url }}/updates)
