---
layout: default
title: Home
permalink: /
---

<section class="intro">
  <p>Welcome to my homepage. Here you can find out what I am up to, new submissions, working papers, adventures and introspections.</p>
</section>

<section class="current-position">
  <h2>Current position</h2>
  <p>I am currently a <strong>{{ site.author.position }}</strong> at the <a href="{{ site.author.affiliation_url }}" target="_blank" rel="noopener">{{ site.author.affiliation }}</a>.</p>
</section>

<section class="research-interests">
  <h2>Research interests</h2>
  <p>My statistical research is primarily centered around Bayesian statistics, Monte Carlo methods, graphical models, and causal discovery.
  Recently I have gained an interest in missing data problems.
  Apart from that, I am constantly improving the causal discovery (structure learning) platform <a href="https://benchpressdocs.readthedocs.io/en/latest/" target="_blank" rel="noopener">Benchpress</a>.</p>
</section>

{% if site.news %}
<section class="news">
  <h2>News</h2>
  <ul>
    {% for item in site.news %}
      <li><span class="news-date">{{ item.date | date: "%b %Y" }}</span>{{ item.text }}</li>
    {% endfor %}
  </ul>
</section>
{% endif %}

{% if site.reviewer_for %}
<section class="reviewer-for">
  <h2>Reviewer for</h2>
  <ul>
    {% for item in site.reviewer_for %}
      <li><a href="{{ item.url }}" target="_blank" rel="noopener">{{ item.name }}</a></li>
    {% endfor %}
  </ul>
</section>
{% endif %}

<section class="talk-embed">
 <h2>Benchpress</h2>
  <p>See the <a href="https://benchpressdocs.readthedocs.io/en/latest/" target="_blank" rel="noopener">Benchpress</a> tutorial I gave at the <a href="https://www.auai.org/uai2023/" target="_blank" rel="noopener">39th Conference on Uncertainty in Artificial Intelligence (UAI 2023)</a>, Pittsburgh, PA, July 31, 2023:</p>
  <iframe width="420" height="315" src="https://www.youtube.com/embed/tx3hIH3b9Hg" title="Benchpress tutorial at UAI 2023" frameborder="0" allowfullscreen></iframe>
</section>
