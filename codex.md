---
layout: default
title: The Codex
permalink: /codex/
---

<div style="text-align: center; margin-bottom: 4rem;">
    <h1>The Codex</h1>
    <p>Directives, philosophy, and architectural notes from the Eternal Custodian.</p>
</div>

<ul class="post-list">
    {% for post in site.posts %}
    <li class="post-item">
        <span class="post-meta">{{ post.date | date: "%B %d, %Y" }}</span>
        <a href="{{ post.url }}">
            <h2 class="post-title">{{ post.title }}</h2>
        </a>
        <p class="post-excerpt">{{ post.excerpt }}</p>
        <a href="{{ post.url }}" style="font-size: 0.9rem; color: var(--gold-antique); text-transform: uppercase;">Read Entry &rarr;</a>
    </li>
    {% endfor %}
</ul>
