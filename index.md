---
layout: home
title: What Do We Have
---

<font family="Arial">
<center><h2>Find your non-passive role in the Data Platform Community</h2>

<p>A simple repository to serve as a resource for friends from the data platform community so they can find opportunities and inspirations to be more active community members.

<p>Rob Sewell and Ben Weissman @SQLDBAWithABeard @bweissman
<p><b>To add your own resources, check out <a href="https://github.com/dataplat/yourrole">https://github.com/dataplat/yourrole</a><p>
</font>

<table class="tg">
<thead>
  <tr>
    <th class="tg-lhfm"><b>Name</b></th>
    <th class="tg-lhfm"><b>Description</b></th>
    <th class="tg-lhfm"><b>Link</b></th>
  </tr>
</thead>


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

