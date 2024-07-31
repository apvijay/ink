---
layout: home
title: Opinions on Tamil Novels and Short Stories
---

{{ site.email }}


<p class="tabs">
    {% for post in site.posts %}
        <a href="{{ post.url }}">{{ post.title }}</a>
        <span class="date">
            {{ post.date | date: "%-d" }}
            {{ post.date | date: "%-m" }}
            {{ post.date | date: "%Y" }}
        </span>
        {% for tag in post.tags %}
            <span class="tag">#{{ tag }}</span>
        {% endfor %}
        <br>
    {% endfor %}
</p>