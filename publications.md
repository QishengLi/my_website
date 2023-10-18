---
layout: page
permalink: /publications/
title: Publications
class: pubs
---

<!-- {:.hidden} -->
# All Publications


{% assign pubyears = site.data.publications | group_by:"year" %}
{% for year in pubyears %}
### {{ year.name }}
{:#y{{ year.name }} .year}
{% for pub in year.items %}
    {% include publications.html pub=pub %}
{% endfor %}
{% endfor %}

<!-- <script src="https://cdn.jsdelivr.net/npm/itemsjs@1.0.40/dist/itemsjs.min.js"></script> -->
<script>
  {% include itemsjs.min.js %}
  {% include pubfilter.js %}
</script>