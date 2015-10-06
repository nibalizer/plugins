---
layout: minimal
---
## Table of Contents
<ul>
  <li><a href="#tools">Tools</a></li>
{% assign sorted_toc_tools = site.data.plugins.plugins | sort: 'tool_name' %}
{% for tool in sorted_toc_tools %}
  {% assign link = tool.tool_name | split: ' ' | join: '-' %}
  <li><a href="#{{link | downcase}}">{{tool.tool_name}} Plugins</a></li>
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
  {% assign sorted_tools = site.data.plugins.tools | sort: 'name' %}
  {% for tool in sorted_tools %}
  <tr>
    <td><a href="{{tool.url}}">{{tool.name}}</a></td>
    <td>{{tool.description}}</td>
  </tr>
  {% endfor %}
  </tbody>
</table>

{% assign sorted_tools = site.data.plugins.plugins | sort: 'tool_name' %}
{% for tool in sorted_tools %}
## {{ tool.tool_name }}
<table>
  <thead>
  <tr>
    <th>Plugin Link</th>
    <th>Description</th>
  </tr>
  </thead>
  <tbody>
  {% assign sorted_plugins = tool.plugins | sort: 'name' %}
  {% for plugin in sorted_plugins %}
  <tr>
    <td><a href="{{plugin.url}}">{{plugin.name}}</a></td>
    <td>{{plugin.description}}</td>
  </tr>
  {% endfor %}
  </tbody>
</table>
{% endfor %}
