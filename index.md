---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
---

<ul>
  {% for file in site.static_files %}
    {% if file.path contains 'index.html' %}
      <li style="list-style: none; float: left; margin: 20px 30px;">
        <a href="{{ file.path }}">
          <object height="240px" data="{{ file.path | replace: 'index.html', 'fachada.png' }}" type="image/png">
            <img src="games/default.png" />
          </object>
        </a>
      </li>
    {% endif %}
  {% endfor %}
</ul>
