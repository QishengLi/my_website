---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
class: home
title: "Home"
---

<div class="introduction" id="introduction" markdown="1">
<div class="columns" markdown="1">
<div class="intro" markdown="1">
Hello, my name is Qisheng Li (李其声). 
I am a 3rd year PhD student at [Paul G. Allen School of Computer Science & Engineering][allen-school] at the [University of Washington][uw], advised by [Katharina Reinecke][kr-website]. Please visit our virtual lab at [Lab in the Wild][labinthewild].

I am broadly interested in human-computer interaction, accessibility and social computing. I am currently focusing on understanding how people with cognitive disabilities (e.g. autism, dyslexia) use technology, facilitating researchers to conduct controlled experiments of disability studies online at large scale, and developing personalized adaptations for end users. 
</div>

<div class="me" markdown="1">
<img src="{{ '/images/headshot.jpeg' | relative_url }}" alt="Image of Qisheng Li">

{:.no-list}
* liqs [at] cs.washington.edu
* Paul G. Allen Center Room 386
</div>
</div>

<div class="more-intro" markdown="1">
Before joining UW CSE, I received my triple bachelor's degrees in Mathematics, Computer Science and Economics from [Macalester College][macalester] in St. Paul, Minnesota. 
For more details, please check out my [CV][cv].
</div>
</div>

<div id="projects" markdown="1">
## Projects
<div class="projects" markdown="1">
<div class="grid" markdown="1">
{% for project in site.data.projects %}
  {% include projects.html project=project %}
{% endfor %}
</div>
</div>
</div>

<div id="publications" markdown="1">
## Publications
<div class="pubs" markdown="1">
{% assign pubyears = site.data.publications | group_by:"year" %}
{% for year in pubyears %}
<!-- ### {{ year.name }}
{:#y{{ year.name }} .year} -->
{% for pub in year.items %}
  {% include publications.html pub=pub %}
{% endfor %}
{% endfor %}
</div>
</div>

<div id="awards" markdown="1">
## Honors & Awards
<div class="awards" markdown="1">
{% assign awardinsts = site.data.awards | group_by:"institution" %}
{% for institution in awardinsts%}
##### {{institution.name}}
{% for award in institution.items %}
  {% include awards.html award=award %}
{% endfor %}
{% endfor %}
</div>
</div>

<div id="news" markdown='1'>
## News & Travel
{% for news in site.data.news %}
  {% include news.html news=news %}
{% endfor %}
</div>


[allen-school]: https://www.cs.washington.edu/
[uw]: http:uw.edu
[kr-website]: https://homes.cs.washington.edu/~reinecke/index.html
[labinthewild]: https://labinthewild.org
[macalester]: http://macalester.edu
[cv]: /~liqs/files/Qisheng_Li_CV.pdf

