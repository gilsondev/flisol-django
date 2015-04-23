```python
# -*- coding: utf-8 -*-

from django.shortcuts import render

from myapp.models import Person


def index(request):

    persons = Person.objects.all().order_by('-first_name')[:5]

    context = {'persons': persons}

    return render(request, 'myapp/index.html', context)
```
