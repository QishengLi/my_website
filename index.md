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
I am a 5th year PhD student at [Paul G. Allen School of Computer Science & Engineering][allen-school] at the [University of Washington][uw], advised by [Katharina Reinecke][kr-website]. During my PhD, I've interned at Adobe Research (x2), Microsoft Research and Google Research.

I am broadly interested in human-computer interaction and accessibility. My current research is twofold: I <b>develop methods</b> for studying people with disabilities <b>at scale</b>. I also use the data collected and other techniques, such as machine learning, to <b>develop systems</b> that improve the accessibility for people with disabilities; I am particularly interested in <b>cognitive disabilities</b>, such as dyslexia.

<span style='color:red'>📢I'm on the job market this year (2022) and I'm looking for industrial research positions.</span> Please feel free to contact me with any opportunities!
</div>



<div class="me" markdown="1">
<img src="{{ '/images/headshot.jpeg' | relative_url }}" alt="Image of Qisheng Li">

{:.no-list}
* liqs [at] cs.washington.edu
* <strike>Paul G. Allen Center Room 386</strike>
* Currently WFH with my [corgi puppy][puppy]
</div>
</div>

<div class="more-intro" markdown="1">
Before joining UW CSE, I received my triple bachelor's degrees in Mathematics, Computer Science and Economics from [Macalester College][macalester] in St. Paul, Minnesota. 
For more details, please check out my [CV][cv].
</div>
</div>

<!-- <div id="projects" markdown="1">
## Projects
<div class="projects" markdown="1">
<div class="grid" markdown="1">
{% for project in site.data.projects %}
  {% include projects.html project=project %}
{% endfor %}
</div>
</div>
</div> -->

<div id="publications" markdown="1">
## Selected Publications
<div class="pubs" markdown="1">
{% assign pubyears = site.data.publications | group_by:"year" %}
{% for year in pubyears %}
<!-- ### {{ year.name }} -->
<!-- {:#y{{ year.name }} .year} -->
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
[puppy]: https://www.instagram.com/sweetpotato.corgi/

