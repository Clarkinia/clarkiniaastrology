---
layout: shelf
title:
header: 
---
<body>
<article class="store">
  <div class="store-items">
    <ul>
      {% for purchase in site.purchases %}
      <li>
        <a href="{{ purchase.url }}">
        <div class="store-top">

          <div class="store-testimonial">
            <h15>"{{ purchase.testimonial }}" —{{ purchase.testimonial-auth}}</h15>
          </div>
        </div> <!-- closes store-top -->
        </a>
      </li>
      {% endfor %}
    </ul>
  </div><!-- closes store-items -->
</article>
</body>
