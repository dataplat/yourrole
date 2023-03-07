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
<h2> A Heading with words that we should have</>

This is the place where you can find stuff that is cool and will help you ta have some thigns that Rob cant write right now because his brain isnt working very well and the creativity has gone away but at least there are some words here that people can see for a moemnt so we see what it looks like
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
                    <a href="{{ resource.resourcelink }}">
                        {{ resource.resourcelink }}
                    </a>
                </td>
              </tr>
        {% endfor %}
  </tr>
</tbody>
</table>

