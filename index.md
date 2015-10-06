---
layout: minimal
---
## Table of Contents
<ul>
  <li><a href="#tools">Tools</a></li>
{% for tool in site.data.plugins.plugins | sort: tool[0] %}
  {% assign link = tool[0] | split: ' ' | join: '-' %}
  <li><a href="#{{link | downcase}}">{{tool[0]}} Plugins</a></li>
{% endfor %}
</ul>

## Tools
<table>
  <thead>
  <tr>
    <th>Tool Link</th>
    <th>Description</th>
  </tr>
  </thead>
  <tbody>
  {% for tool in site.data.plugins.tools | sort: 'name' %}
  <tr>
    <td><a href="{{tool.url}}">{{tool.name}}</a></td>
    <td>{{tool.description}}</td>
  </tr>
  {% endfor %}
  </tbody>
</table>

{% for tool in site.data.plugins.plugins | sort: tool[0] %}
## {{ tool[0] }}
<table>
  <thead>
  <tr>
    <th>Plugin Link</th>
    <th>Description</th>
  </tr>
  </thead>
  <tbody>
  {% for plugin in tool[1] | sort: 'name' %}
  <tr>
    <td><a href="{{plugin.url}}">{{plugin.name}}</a></td>
    <td>{{plugin.description}}</td>
  </tr>
  {% endfor %}
  </tbody>
</table>
{% endfor %}
