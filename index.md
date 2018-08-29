---
layout: default
title: Home
---

{% include intro.html %}


<section class="post-list">
  <div class="container">
{% for post in site.posts %}
<article class="preview">
    <header>
        <h2 class="post-title">
            <a class="post-link" href="{{ post.url }}">  {{ post.title }} </a>
        </h2>
 
        <p class="post-date"> {{ post.date }}</p>
    </header>
    <section class="post-section">
        <p>
            {{ post.excerpt }}
        </p>
        <p class="readmore">
        
         <!--   <a href="{{ post.url }}">
                阅读全文
                <span class="glyphicon glyphicon-circle-arrow-right"></span>
-->
            </a>
        </p>
    </section>

</article>
{% endfor %}
  </div>
</section>


 
