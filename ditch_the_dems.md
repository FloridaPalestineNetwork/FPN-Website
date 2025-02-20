---
layout: page
title: Ditch The Dems
permalink: /ditch_the_dems/
menu: false
---
<p style="text-align: justify;">Born out of Florida Palestine Network’s critical advocacy and urgent mobilizations in response to the uninterrupted genocide of the Palestinian people: Ditch The Dems offers Florida voters an option outside the current 2 party system that prioritizes devastation instead of the care of its people.</p>

<div class="button-container">
    <div class="button">
    <a href="https://docs.google.com/forms/d/e/1FAIpQLSdzu9dKurutY1zavpmUYpgO3fnjwOgGRirWDj3ca4wCX-97tw/viewform" target="_blank">Ditch The Dems Newsletter</a>
    </div>
</div>

<p style="text-align: justify;">Ditch the Dems is a campaign that aims to mobilize the masses in rejecting the two-party system. We invite our Florida community members, families, and working-class people to join us as we divest from both the Florida Democratic and Republican establishments and to reimagine, re-engage, and redirect resources to mobilize for a world outside duopoly corporations.</p>


<div class="button-container">
    <div class="button">
    <a href="https://docs.google.com/forms/d/e/1FAIpQLSe2QpPLE-Mfhqt_TXJcpmWXo28TC7Wyw0HeJvi-7JksiJeRWw/viewform" target="_blank">Ditch The Dems Pledge</a>
    </div>
</div>

<div class="grid">
    {% assign articles = site.posts | where: "categories", "article" | where: "tags", "DTD" | sort: "date" | reverse %}
    {% for article in articles %}
    <div class="article">
        <p>{{ article.date | date: "%B %d, %Y" }}</p>
        <a href="{{ article.url }}">
            {% if article.cover_image %}
            <img src="{{ article.cover_image }}" alt="{{ article.title }} cover image">
            {% endif %}
        </a>
    </div>
    {% endfor %}
</div>