---
layout: home
title: Opening the Door to Tamil Novels and Short Stories
---


<p class="tabs">
    {% for post in site.posts %}
        <a href="{{ post.url }}">{{ post.title }}</a>
        <span class="date">
            {{ post.date | date: "%-B" }}
            {{ post.date | date: "%-d" | plus:'0' }}, 
            {{ post.date | date: "%Y" }}
        </span>
        {% for tag in post.tags %}
            <span class="tag">#{{ tag }}</span>
        {% endfor %}
        <br>
    {% endfor %}
</p>