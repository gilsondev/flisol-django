```python
>>> from myapp.models import Person

person = Person.objects.get(id=1)

other_person = Person.objects.get(pk=2)

vitors = Person.objects.filter(first_name="Vitor")

edus = Person.objects.raw(
    "SELECT * FROM myapp_person WHERE first_name LIKE '%edu%'"
)
```
