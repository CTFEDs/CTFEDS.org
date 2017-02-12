---
layout: home
title: Organisers
---

  <article class="article organisers">
    <h1 class="block-header">The CTFEDs organising team</h1>

    {% capture organisers-list %}{% include organisers-list.md %}{% endcapture %}
       {{ organisers-list | markdownify }}

  </article>
