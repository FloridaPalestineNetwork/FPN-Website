---
layout: page
title: Political Education
permalink: /political_education/
menu: false
---
<p style="text-align: justify;">The Florida Palestine Network's Political Education committee is involved in writing all FPN communications and statements. Deeply rooted in theory and praxis, the PE committee strives to bring the light of truth to the darkness of ignorance.</p>

<h2>Film Night</h2>
<div class="grid">
                {% assign upcoming_events = site.posts | where: "categories", "event" | where: "tags", "film_night" %}
                {% assign current_time = site.time | date: "%Y-%m-%d" | date: "%s"%}

                {% assign sorted_upcoming_events = upcoming_events | sort: "event-date" %}

                {% for event in sorted_upcoming_events %}
                {% if event.event-date %}
                {% assign event_date = event.event-date | date: "%s" %}
                {% if event_date >= current_time %}
                <div class="event">
                    <p>{{ event.event-date | date: "%B %d, %Y" }}</p>
                    <a href="{{ event.url }}">
                        {% if event.cover_image %}
                        <img src="{{ event.cover_image }}" alt="{{ event.title }} cover image">
                        {% endif %}
                    </a>
                </div>
                {% endif %}
                {% endif %}
                {% endfor %}

            </div>