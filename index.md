---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: shelf
title: Clarkinia Astrology
image: noun_103916_cc_horiz.gif
header: Clarkinia Astrology
subhead: straightforward intuitive guidance
author: with Regina Clarkinia
cta: Choose a reading based on what you need now.
bioheader: Regina Clarkinia
biopic: bio_pic_astrology_bw.jpg
description: Candid astrology and tarot readings designed to get your butt in gear.
bio: has been reading tarot and astrology charts for 20 years. She writes about mysticism and teaches practical meditation techniques. Her readings investigate family relationships, personality patterns and career strategy. Regina tells it like it is with candid readings designed to get your butt in gear.
---
<body>
<article class="store">
  <div class="store-items">
    <ul>
      {% for reading in site.readings %}
      <li>
        <a href="{{ reading.url }}">
        <div class="store-top-container">
        <div class="store-top">
          <div class="store-button">
            <div class="store-button-container">
              <img src="{{ site.github.url }}/assets/img/{{ reading.button }}" >
            </div>
          </div>
          <div class="store-product-name">
            <h5>{{ reading.name }}</h5>
          </div>
          <div class="store-byline">
            <h2>{{ reading.byline }}</h2>
          </div>
          <div class ="store-whatuget">
            <h3>{{ reading.content }}</h3>
          </div>
          <div class="store-cta-button">
            <h3>{{ reading.cta }}</h3>
          </div>
        </div> <!-- closes store-top -->
        </div>
        </a>
      </li>
      {% endfor %}
    </ul>
  </div><!-- closes store-items -->
</article>
</body>
