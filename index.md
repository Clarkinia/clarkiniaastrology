---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: shelf
title: Clarkinia Astrology
image: /assets/img/store-form-career-background3.jpg
header: Clarkinia Astrology
subhead: straightforward intuitive guidance
author: with Regina Clarkinia
cta: Choose a reading based on what you need now.
bioheader: Regina Clarkinia
biopic: bio_pic_astrology_bw.jpg
description: Candid astrology and tarot readings designed to get your butt in gear.
bio: In a session I listen to my client, intuitively pointing to useful insights, keeping track of the conversation and organizing takeaways into a cohesive narrative with an action-oriented strategy. I am most influenced by a modern psychological astrology approach, however I take a little from everywhere, including hellenistic timing procedures and insights from evolutionary astrology. I have been reading tarot and astrology charts professionally since 2014. <a href="https://www.queerauntie.com">I write about mysticism </a>and teach practical meditation techniques. My readings investigate key relationships, personality patterns and vocation.
url: https://www.clarkiniaastrology.com
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
