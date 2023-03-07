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
<center><h2>Find your non-passive role in the Data Platform Community</h2>

<p>A simple repository to serve as a resource for friends from the data platform community so they can find opportunities and inspirations to be more active community members.

<p>Rob Sewell and Ben Weissman @SQLDBAWithABeard @bweissman
<p><b>To add your own resources, check out <a href="https://github.com/dataplat/yourrole">https://github.com/dataplat/yourrole</a><p>


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

