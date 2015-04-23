```python
# -*- coding: utf-8 -*-

from django.views.generic import ListView

from myapp.models import Person


class PersonList(ListView):
    model = Person
    # Convention over Configuration:
    #
    # template_name: 'myapp/person_list.html'
```
