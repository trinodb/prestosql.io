---
layout: default
pretitle: Trino Community Broadcast
title: Episodes
show_hero: true
---

<link rel="stylesheet" href="{{ '/assets/episode/main.css' | relative_url }}">

<div class="container container__broadcast">

  <div class="row spacer-60">
    {% for episode in site.episodes reversed %}
    <div class="post-entry card">
      <h3><a class="post-link" href="{{ episode.url | relative_url }}">{{ episode.title | escape }}</a></h3>
      <span class="post-meta">{{ episode.date | date: "%b %-d, %Y" }}
      </span>
      <ul>
            {% for section in episode.sections limit: 5 %}
            <li>
                <a href="https://www.youtube.com/watch?v={{ episode.youtube_id}}&t={{ section.time }}s" target="_blank">
                {{section.title}}: {{ section.desc }} ({{ section.time }}s)
                </a>
            </li>
            {% endfor %}
        </ul>
        <span><a href="https://www.youtube.com/watch?v={{ episode.youtube_id}}">Watch the full episode</a> | <a href="{{ site.baseurl }}{{ episode.url }}">Listen to the episode or read the show notes</a></span>
    </div>
    {% endfor %}
    <p class="rss-subscribe">
      <a href="{{ '/broadcast/feed.xml' | relative_url }}">subscribe via RSS</a>
      <svg class="svg-icon"><use xlink:href="{{ '/assets/blog/social-icons.svg#rss' | relative_url }}"></use></svg>
    </p>
  </div>
</div>
