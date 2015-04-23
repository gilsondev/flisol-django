```python
# -*- coding: utf-8 -*-

from django.shortcuts import render, get_object_or_404

from myapp.models import Person


def detail(request, person_id):

    person = get_object_or_404(Person, pk=person_id)

    return render(request, 'myapp/index.html', {'person': person})
```
