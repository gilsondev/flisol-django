```python
# -*- coding: utf-8 -*-

from django.conf.urls import patterns, include, url

from myapp import views

urlpatterns = patterns('',
    # ex.: /persons/
    url(r'^$', views.index, name='index'),

    # ex.: /persons/6
    url(r'^(?P<people_id>\d+)/$', views.detail, name='detail'),

    # ex.: /persons/6/address/
    url(r'^(?P<people_id>\d+)/address/$', views.address, name='address'),

    # ex.: /peoples/friends/*
    url(r'^frients/', include('otherapp.urls')),
)
```
