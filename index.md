---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: shelf
title:
image: noun_103916_cc_horiz.gif
header: Clarkinia Astrology
subhead: straightforward intuitive guidance
author: with Regina Clarkinia
cta: Choose a reading based on what you need now.
bioheader: Regina Clarkinia
biopic: bio_pic_astrology_bw.jpg
bio: has been reading tarot and astrology charts for 20 years. She writes about mysticism and teaches practical meditation techniques. A writer and comedian, Regina presents the truth in a humorous and lighthearted style. Her readings investigate family relationships, personality patterns and career strategy. Regina tells it like it is with candid readings designed to get your butt in gear.
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
