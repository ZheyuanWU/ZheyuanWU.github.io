---
layout: page
permalink: /misc/photos.html
title: 

completed:
    - name:
      date: June 6, 2023
      location: UDS campus
      photo: 

---

{% for r in page.completed %}
- {% if r.date %}{{ r.date | date: "%-d %B %Y"  }}: {% endif %}[{{r.name}}]({{r.track}}){% if r.location %}, *{{r.location}}* {% endif %}{% if r.notes %} ({{r.notes}}){% endif %} {% if r.url %}([More info]({{r.url}})){% endif %}{% if r.photos %}, [photo]({{r.photos}}){% endif %}{% if r.private_photos %}, [private]({{r.private_photos}})]{% endif %}<br />{% endfor %}