---
layout: page
title: Zheyuan (Joann) Wu
permalink: /
research:
    - title:   "Kawa: An Abstract Language for Scalable and Variable Detection of Spectre Vulnerabilities"
      author:  "Zheyuan Wu, Haoyi Zeng, Aaron Bies"
      conference: "SRC SPLASH 2024 🥉(3rd place in the undergraduate category)"
      url:     "https://dl.acm.org/doi/10.1145/3689491.3689971"

    - title:   "Expressing and Checking Statistical Assumptions"
      author:  "Alexi Turcotte, Zheyuan Wu"
      conference: "FSE 2025"
      url:  "https://conf.researchr.org/details/fse-2025/fse-2025-research-papers/93/Expressing-and-Checking-Statistical-Assumptions"
---
{% include image.html url="myphoto/baloo_home2025.jpg" width="200px" align="right" %}

I'm currently a computer science undergraduate at [Saarland University], and I'm on a journey to discover my research passions. 
<!-- **Update :**
I'll be a CS PhD Student starting Fall 2025 at Brown University! -->

📬 (λx. λy. x00001@stud.uni-y.de) (zhwu) (saarland)
<!-- (λ<span style="color: brown;">x</span>. λ<span style="color: brown;">y</span>. <span style="color: brown;">x</span>00001@stud.uni-<span style="color: brown;">y</span>.de) (<span style="color: brown;">zhwu</span>) (<span style="color: brown;">saarland</span>) -->

**Areas of interests :** 
program analysis, 
testing and verification,
formal methods in security, 
and human factors in above technologies.

### Upcoming Events
<!-- - (will attend) SuRI@EPFL 2025!
- (will attend) FSE 2025 in Trondheim 🇳🇴
- (will attend) PLISS 2025 in Bertinoro 🇮🇹
- (attened) SPLASH 2024 -->

- SuRI@EPFL 2025!
- FSE 2025 in Trondheim 🇳🇴
- PLISS 2025 in Bertinoro 🇮🇹

<!-- ----
### Research Experence -->
### <span class="title-style"> Research Experence </span>
<hr class="title-line">


{% for pub in page.research %}
<div style="display: flex; align-items: center; margin-bottom: 20px;">
  {% if pub.image %}
    <div style="margin-right: 20px;">
      {% include image.html url=pub.image caption="" height="100px" align=thumbnail %}
    </div>
  {% endif %}
  <div>
    {% if pub.url %}
      <strong style="font-size: 0.9em;"><a href="{% if pub.internal %}{{pub.url | prepend: site.baseurl}}{% else %}{{pub.url}}{% endif %}">{{ pub.title }}</a></strong><br />
    {% else %}
      <strong style="font-size: 0.9em;">{{ pub.title }}</strong><br />
    {% endif %}
    <span style="font-size: 0.9em;">{{ pub.author }}</span><br />
    <i style="font-size: 0.9em;">{{ pub.conference }}</i><br />
    {% if pub.note %} <i style="font-size: 0.9em;">({{ pub.note }})</i> {% endif %} 
    <i style="font-size: 0.9em;">{{ pub.year }}</i>
    {% if pub.doi %} 
      <span style="font-size: 0.9em;">[[doi]({{ pub.doi }})]</span> 
    {% endif %}
    {% if pub.media %}
      <br />Media: 
      {% for article in pub.media %}
        <a href="{{ article.url }}" target="_blank" style="font-size: 0.9em;">{{ article.name }}</a>
      {% endfor %}
    {% endif %}
  </div>
</div>
{% endfor %}



<!-- ---
### Teaching -->

### <span class="title-style">Teaching</span>
<hr class="title-line">
- <span style="font-size: 0.9em;"> Teaching Assistant at Saarland University: [**Mathematics for Computer Scientists I**](https://cms.sic.saarland/mfi1_mfcs1_wise2223/) (2023)</span><br />


<!-- ---
### Teaching -->

### Misc.
<hr class="title-line">

- Need a break? Take a look at [Baloo](baloo.html) 🐈
- [More about my life](/misc/)



[Saarland University]: https://saarland-informatics-campus.de/
