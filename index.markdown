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
I am currently an AI/ML resident in the Human-Centered Machine Intelligence team at [Apple][apple].
I recently received my Ph.D. in Computer Science & Engineering from [Paul G. Allen School][allen-school] at the [University of Washington][uw], advised by [Katharina Reinecke][kr-website]. During my PhD, I've interned at Adobe Research (x2), Microsoft Research and Google Research.

My research interests span across <b>human-computer interaction</b>>, <b>accessibility</b>, and <b>applied machine learning</b>. My current research revolves around the design and development of ML-powered <b>AR/VR</b> applications for blind and low-vision users. 

In my Ph.D. thesis, I employed <b>mixed methods</b> to demonstrate the feasibility of conducting large-scale online experiments with individuals with cognitive disabilities that are self-motivating, while maintaining <b>rigorous experimental designs</b>. Additionally, my experience in <b>data science</b> and machine learning has been honed through a variety of courseworks, projects and internships.

<span style='color:red'>📢 I'm looking for industrial research positions this year (2023).</span> Please feel free to contact me with any opportunities!
</div>



<div class="me" markdown="1">
<img src="{{ '/images/headshot.jpeg' | relative_url }}" alt="Image of Qisheng Li">

{:.no-list}
* Contact: lqsh2013 [at] gmail.com
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

<!-- <div id="news" markdown='1'>
## News & Travel
{% for news in site.data.news %}
  {% include news.html news=news %}
{% endfor %}
</div> -->

[apple]: https://www.apple.com/
[allen-school]: https://www.cs.washington.edu/
[uw]: http:uw.edu
[kr-website]: https://homes.cs.washington.edu/~reinecke/index.html
[labinthewild]: https://labinthewild.org
[macalester]: http://macalester.edu
[cv]: /~liqs/files/Qisheng_Li_CV.pdf
[puppy]: https://www.instagram.com/sweetpotato.corgi/

