```python
# -*- coding: utf-8 -*-

from django.shortcuts import render
from django.http import HttpResponseRedirect

from myapp.forms import ContactForm


def contact(request):
    if request.method == "POST":
        if form.is_valid():
            # Processa os dados com form.cleaned_data...
            return HttpResponseRedirect('/thanks/')
        else:
            form = ContactForm()

    return render(request, 'contact.html', {'form': form})
```
