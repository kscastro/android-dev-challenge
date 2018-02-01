---
layout: page
title: Articles
site_nav_category_order: 200
is_site_nav_category: true
site_nav_category: articles
---

<div class="content-grid mdl-grid">
{% for article in site.articles %}
    <div class="mdl-cell mdl-cell--6-col mdl-cell--4-col-tablet mdl-cell--4-col-phone">
        <div class="mdl-card mdl-shadow--2dp" style="width:100%;">
            <div class="mdl-card__title" style="height:200px; background:url('{{ site.baseurl }}/assets/{{article.cover}}') center / cover;">
                <h2 class="mdl-card__title-text">{{article.title}}</h2>
            </div>
            <div class="mdl-card__supporting-text">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                Mauris sagittis pellentesque lacus eleifend lacinia...
            </div>
            <div class="mdl-card__actions mdl-card--border">
                <a class="mdl-button mdl-button--colored mdl-js-button mdl-js-ripple-effect" href="#">
                    Read more
                </a>
            </div>
        </div>
    </div>
{% endfor %}
</div>