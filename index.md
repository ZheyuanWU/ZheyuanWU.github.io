---
layout: page
title: Zheyuan Wu
permalink: /
pubs:
    - title:   "Expressing and Checking Statistical Assumptions"
      author:  "Alexi Turcotte, Zheyuan Wu"
      conference: "FSE"
      year: "2025"
      url: "https://dl.acm.org/doi/10.1145/3729391"
      award: "⭐ Distinguished Paper"
    - title:   "Kawa: An Abstract Language for Scalable and Variable Detection of Spectre Vulnerabilities"
      author:  "Zheyuan Wu, Haoyi Zeng, Aaron Bies"
      conference: "SRC SPLASH "
      year: "2024"
      award: "🥉 3rd place"
      url: "https://dl.acm.org/doi/10.1145/3689491.3689971"
---

<div style="overflow: hidden; margin-bottom: 1em;">
  <div style="float: right; margin-left: 1em;">
    {% include image.html url="myphoto/Zheyuan_20250511.JPG" width="120px" %}
  </div>

  <p style="font-size: 1.1rem; margin-top: 0.2em;">
    <span lang="zh">哲苑</span>
    <span style="font-family: serif;">zhé yuàn</span>
  </p>

  <div style="max-width: 600px; line-height: 1.6;">
    <p>
      Hi 👋, I'm a computer science PhD student in the 
      <a href="https://cel.cs.brown.edu">Cognitive Engineering Lab</a> at Brown University,
      advised by <a href="https://willcrichton.net/">Will Crichton</a>.
      <br />
      I'm on a journey to discover my research passions :)
      <br />
      My undergrad was at <a href="https://saarland-informatics-campus.de/">Saarland University</a>, 
      worked with <a href="https://reallytg.github.io/">Alexi Turcotte</a> at CISPA. 

    </p>
    <p style="margin-top: 0.8em;">
    📬 (λx. x@brown.edu) (zheyuan)
    </p>

    <p>
      <strong>Research interests:</strong><br />
      human factors in formal methods,
      testing and verification,
      program analysis...
    </p>
  </div>
</div>



<!-- ----
### Research Experence -->
### <span class="title-style"> Research Experence </span>
<hr class="title-line">

{% for pub in page.pubs %}
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
    <span style="font-size: 0.9em;">{{ pub.author | replace: "Zheyuan Wu", "<span style='font-weight: normal; color: #999;'>Zheyuan Wu</span>" }}</span><br />
    <span style="font-family: Georgia, serif; font-variant: small-caps; font-size: 1.2em;">
      {{ pub.conference | downcase }}
      <span style="font-size: 0.75em;"> {{ pub.year }}</span>
      {% if pub.award %}
      <span style="font-size: 0.75em; color:#802F00"> {{ pub.award | downcase}}</span>
      {% endif %}
    </span>
    {% if pub.note %} <i style="font-size: 0.9em;">({{ pub.note }})</i> {% endif %} 
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

### <span class="title-style">Teaching</span>
<hr class="title-line">
- <span style="font-size: 0.9em;"> Teaching Assistant at Saarland University: [**Mathematics for Computer Scientists I**](https://cms.sic.saarland/mfi1_mfcs1_wise2223/) (2023)</span><br />


### Misc.
<hr class="title-line">

- Need a break? Take a look at [Baloo](baloo.html) 🐈
- [More about my life](/misc/)



[Saarland University]: https://saarland-informatics-campus.de/
[Cog­ni­tive En­gi­neer­ing Lab]: https://cel.cs.brown.edu
[Will Crichton]: https://willcrichton.net/
[Alexi Turcotte]: https://reallytg.github.io/