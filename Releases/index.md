---

---
<html>
    <body>
    <h1>All Releases</h1>

    {% assign years = site.pages | sort: 'releaseDate' | reverse
   | group_by_exp: "post", "post.releaseDate | date: '%Y'"
%}

{% for year in years %}
  <h3>{{ year.name }}</h3>

  <ul>
    {% for doc in year.items %}
      {% if doc.isReleaseDetails == true %}
            <li><a href="{{ site.baseurl }}{{ doc.url }}">{{doc.version}}</a> {{ doc.releaseDate | date: "%-d %B %Y" }} - {{doc.summary}} </li>
        {% endif %}
    {% endfor %}
  </ul>
{% endfor %} 



</body>
</html>
