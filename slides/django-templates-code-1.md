```jinja
<h1>{{ person.first_name }} {{ person.last_name }}</h1>

<ul>
    <!-- Ex.: List address -->
    {% for address in person.address_set.all %}
        <li>{{ address.description }} - {{ address.street }}</li>
    {% endfor %}
</ul>
```
