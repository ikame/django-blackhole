Django-Blackhole
================

Django application that let's you work in your templates apart from having or not the corresponding views created.

Features
--------

* Design your template without having the corresponding view created.
* Pass data to your template via the url.

Example
-------

In your urls.py:

```python
if settings.DEBUG:
    urlpatterns += patterns('', ('^_blackhole/', include('blackhole.urls'))
```

With that in place you should be able to access the url: `/_blackhole/templates/<template name>/?<template data>`

Installation
------------

To install, simply:

```
$ pip install django-blackhole
```

Or, directly from the main repository:

```
$ pip install -e git+http://github.com/ikame/django-blackhole.git#egg=blackhole
```
