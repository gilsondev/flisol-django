```python
>>> from myapp.models import Person

>>> carlos = Person.objects.create(
        first_name="Carlos",
        last_name="Santos"
    )

>>> carlos.first_name
"Carlos"

>>> carlos.last_name = "Silva"

>>> carlos.save()

>>> carlos.delete()
```
