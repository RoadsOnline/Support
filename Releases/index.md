---

---
<html>
    <body>
    <h1>All Releases</h1>
{% assign doclist = site.pages | sort: 'releaseDate' | reverse  %}
<ul>
   {% for doc in doclist %}
        {% if doc.isReleaseDetails == true %}
            <li><a href="{{ site.baseurl }}{{ doc.url }}">{{doc.version}}</a> {{ doc.releaseDate | date: "%-d %B %Y" }} - {{doc.summary}} </li>
        {% endif %}
    {% endfor %}
</ul>

</body>
</html>
