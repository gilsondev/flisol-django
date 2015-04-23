```python
>>> from django.core.urlresolvers import reverse

>>> reverse('index')
'/'

>>> reverse('detail', kwargs={'people_id': 4})
'/persons/4'
```
