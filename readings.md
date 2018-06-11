---
layout: shelf
title:
header: Clarkinia Astrology
image: noun_1546369_cc.svg
subhead: straightforward intuitive guidance
author: with Regina Clarkinia
cta: Choose a reading based on what you need now.
---
<!-- bgimage: store_home_bg_1200px_bags_bags_all_type_of_bags.jpg -->
<body>
<article class="store">
  <div class="store-items">
    <ul>
      {% for reading in site.readings %}
      <li>
        <a href="{{ reading.url }}">
        <div class="store-top">
          <div class="store-button">
            <img src="{{ site.github.url }}/assets/img/{{ reading.button }}" >
          </div>
          <div class="store-byline">
            <h8>{{ reading.byline }}</h8>
          </div>
          <div class ="store-whatuget">
            <h15>{{ reading.content }}</h15>
          </div>
          <div class="store-cta-button">
            <h15>{{ reading.cta }}</h15>
          </div>
          <div class="store-testimonial">
            <h15>"{{ reading.testimonial }}" —{{ reading.testimonial-auth}}</h15>
          </div>
        </div> <!-- closes store-top -->
        </a>
      </li>
      {% endfor %}
    </ul>
  </div><!-- closes store-items -->
</article>
</body>
