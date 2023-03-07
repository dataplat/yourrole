---
layout: home
title: What Do We Have
---

<table class="tg">
<thead>
  <tr>
    <th class="tg-lhfm">Name</th>
    <th class="tg-lhfm">Description</th>
    <th class="tg-lhfm">Link</th>
  </tr>
</thead>
{% for resource in site.resources %}
  <h2>{{ resource.resourcename }} - {{ resource.resourcelink }}</h2>
  <p>{{ resource.content | markdownify }}</p>
{% endfor %}

<tbody>
  <tr>
      {% for resource in site.resources %}
            <tr>
                <td class="tg-0lax">
                        {{ resource.resourcename }}
                </td>
                <td class="tg-0lax">
                   {{ resource.content | markdownify}}
                </td>
                <td class="tg-0lax">
                    <a href="{{ post.link}}">
                        {{ resource.resourcelink }}
                    </a>
                </td>
              </tr>
        {% endfor %}
  </tr>
</tbody>
</table>

