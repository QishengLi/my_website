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
Hello, my name is Qisheng Li. 
I'm a Research Scientist working on Human-AI/Multimodal Interaction at [Meta Reality Lab Research (RL-R)][meta-rlr]. I'm also a Research Fellow at [AImpower.org][aimpower].
My research interests span across <b>human-computer interaction</b>, <b>artificial intelligence</b>, and <b>accessibility</b>. I'm currently working on building and evaluating AR systems with AI/ML.
<!-- My current research revolves around accessibility and productivity tools with <b>multimodal LLMs</b>. I worked on ML-powered <b>AR/VR</b> applications for blind and low-vision users at Apple.  -->

Previously, I was an AI/ML resident in the Human-Centered Machine Intelligence team at [Apple][apple] from 2022-2023. I received my Ph.D. in [Computer Science & Engineering][allen-school] from the [University of Washington][uw], advised by [Katharina Reinecke][kr-website]. In my Ph.D. thesis, I employed <b>mixed methods</b> to demonstrate the feasibility of conducting large-scale online experiments with individuals with cognitive disabilities that are self-motivating, while maintaining <b>rigorous experimental designs</b>. During my PhD, I've interned at Adobe Research (x2), Microsoft Research, and Google Research.

</div>



<div class="me" markdown="1">
<img src="{{ '/images/headshot.jpeg' | relative_url }}" alt="Image of Qisheng Li">

{:.no-list}
* Contact: lqsh2013 [at] gmail.com
</div>
</div>

<div class="more-intro" markdown="1">
<span style='color:red'>📢 I'm looking for full-time industrial research positions recently.</span> Please feel free to contact me with any opportunities! For more details, please check out my [CV][cv].
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
## Selected <a href="{{ "/publications/" | relative_url }}">Publications</a>
<div class="pubs" markdown="1">
{% assign pubyears = site.data.publications | group_by:"year" %}
{% for year in pubyears %}
<!-- ### {{ year.name }} -->
<!-- {:#y{{ year.name }} .year} -->
{% for pub in year.items %}
  {% if pub.highlight %}
    {% include publications.html pub=pub %}
  {% endif %}
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

<!-- <div id="news" markdown='1'>
## News & Travel
{% for news in site.data.news %}
  {% include news.html news=news %}
{% endfor %}
</div> -->

[aimpower]: https://aimpower.org/
[meta-rlr]: https://about.meta.com/realitylabs/
[apple]: https://www.apple.com/
[allen-school]: https://www.cs.washington.edu/
[uw]: http:uw.edu
[kr-website]: https://homes.cs.washington.edu/~reinecke/index.html
[labinthewild]: https://labinthewild.org
[macalester]: http://macalester.edu
[cv]: /~liqs/files/Qisheng_Li_CV.pdf
[puppy]: https://www.instagram.com/sweetpotato.corgi/

