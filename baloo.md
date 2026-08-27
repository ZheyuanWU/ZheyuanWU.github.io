---
layout: page
permalink: /baloo.html
title: Random Baloo!
---

{% assign first_baloo = site.data.baloo | first %}

<figure class="baloo-random">
  <a id="baloo-link" href="{{ first_baloo.src | prepend: site.baseurl }}">
    <img
      id="random-image"
      src="{{ first_baloo.src | prepend: site.baseurl }}"
      alt="Random Baloo photo"
      decoding="async"
      fetchpriority="high">
  </a>
</figure>

<p class="baloo-pet-link">
  If you use ChatGPT, you can
  <a
    href="https://chatgpt.com/s/sharepet_6a8f100f5a8c8191836528c0a200349d"
    target="_blank"
    rel="noopener noreferrer">
    adopt your very own e-Baloo 🐾</a>
</p>

<script>
  window.balooPhotos = [
    {% for photo in site.data.baloo %}
      {
        full: "{{ photo.src | prepend: site.baseurl }}",
        display: "{{ photo.src | prepend: site.baseurl }}"
      }{% unless forloop.last %},{% endunless %}
    {% endfor %}
  ];

  (function () {
    var image = document.getElementById("random-image");
    var link = document.getElementById("baloo-link");
    var photos = window.balooPhotos || [];

    function pickPhoto() {
      if (!photos.length) return;
      var photo = photos[Math.floor(Math.random() * photos.length)];
      image.src = photo.display;
      link.href = photo.full;
    }

    pickPhoto();
  }());
</script>
