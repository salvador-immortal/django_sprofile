=====
Django Sprofile
=====

Based on `django-profile-middleware
<https://github.com/lavi06/django-profile-middleware>`_.

this is a package that can profile your requests and functions/lines ,, created on top of `cProfile
<https://docs.python.org/3.6/library/profile.html>`_.

Compatible with Django 1.11 and later

Python 3.x

Quick start
-----------

1. Add "django_sprofile" to your INSTALLED_APPS setting like this:

    INSTALLED_APPS = [
        ...
        'django_sprofile',
    ]

2. Add "django_sprofile.middleware.sProfilerMiddleware" to your MIDDLEWARE setting like this:

    MIDDLEWARE = [
        ...
        'django_sprofile.middleware.sProfilerMiddleware',
    ]

3. Set sProfile Config(PROFILER) to your setting:

    PROFILER = {
        'enable': True,
        'sort': 'time',
        'count': None ,
        'output': ['console','file'],             
        'file_location': 'profiling_results.txt'
    }

TODO
----
1. better logfile

2. dashboard

3. testing with django 2.2