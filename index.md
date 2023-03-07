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
<tbody>
  <tr>
      {% for post in site.pages %}
            <tr>
                <td class="tg-0lax">
                        {{ post.name}}
                </td>
                <td class="tg-0lax">
                   {{ post.description}}
                </td>
                <td class="tg-0lax">
                    <a href="{{ post.link}}">
                        {{ post.link }}
                    </a>
                </td>
              </tr>
    {% endfor %}
  </tr>
</tbody>
</table>

