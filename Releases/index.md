---

---
<html>
    <body>
{% assign doclist = site.pages | sort: 'url'  %}
<ul>
   {% for doc in doclist %}
        {% if doc.include == true %}
            <li><a href="{{ site.baseurl }}{{ doc.url }}">{{doc.version}}</a> {{ doc.date }} - {{doc.summary}} </li>
        {% endif %}
    {% endfor %}
</ul>

</body>
</html>