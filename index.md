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
bio: has been reading tarot and astrology charts for 20 years. She writes about mysticism and teaches practical meditation techniques. Her readings investigate family relationships, personality patterns and career strategy. Regina tells it like it is with candid readings designed to get your butt in gear.
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

<!--
          <div class="store-testimonial">
            <h3>"{{ reading.testimonial }}" —{{ reading.testimonial-auth}}</h3>
          </div>
-->
        </div> <!-- closes store-top -->
        </a>
      </li>
      {% endfor %}
    </ul>
  </div><!-- closes store-items -->
</article>
</body>
