---
layout: page
permalink: /misc/photos.html
title: 

completed:
    - name:
      date: June 6, 2023
      location: UDS campus
      photo: (images/photo_2023-06-10_17-47-06.jpg)

---

{% for r in page.completed %}
- 
{% if r.date %}{{ r.date | date: "%-d %B %Y"  }}: {% endif %}
[{{r.name}}]({{r.track}}){% if r.location %}, *{{r.location}}* {% endif %}{% if r.url %}([More info]({{r.url}})){% endif %}{% if r.photos %}, [photo]({{r.photos}}){% endif %}
<br />{% endfor %}