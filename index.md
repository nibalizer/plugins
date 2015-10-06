---
layout: minimal
---
# Table of Contents
<ul>
  <li><a href="#tools">Tools</a></li>
{% assign sorted_toc_tools = site.data.plugins.tools | sort: 'name' %}
{% for tool in sorted_toc_tools %}
  {% assign link = tool.display_name | split: ' ' | join: '-' %}
  {% if tool.plugins %}<li><a href="#{{link | downcase}}">{{tool.display_name}} Plugins</a></li>{%endif%}
{% endfor %}
</ul>

# Tools
Useful tools when writing Puppet.

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
  {% if tool.url %}
  <tr>
    {% if tool.display_name %}
    {% assign display_name = tool.display_name %}
    {% else %}
    {% assign display_name = tool.name %}
    {% endif %}
    <td><a href="{{tool.url}}">{{ display_name }}</a></td>
    <td>{{tool.description}}</td>
  </tr>
  {% endif %}
  {% endfor %}
  </tbody>
</table>

{% assign sorted_tools = site.data.plugins.tools | sort: 'name' %}
{% for tool in sorted_tools %}
{% if tool.plugins %}
# {{ tool.display_name }}
{% if tool.description %}{{tool.description}}{%endif%}
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
{% endif %}
{% endfor %}
