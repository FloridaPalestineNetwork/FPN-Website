---
layout: tickets
title: Tickets
permalink: /tickets/
menu: false
---

<div class="narrow">
    <main>
      <h1>{{ post.title }}</h1>
      <p>{{ post.author }} - {{ post.date | date: "%B %d, %Y" }}</p>
      
      {% if post.tags contains "ticket_sale" %}
        <div class="ticket-notice">
          <p>This post is related to a ticket.</p>
        </div>
      {% endif %}
</div>
