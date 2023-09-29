# Awesome Django Performance [![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)

> A curated list of libraries, blog articles, books, and talks to help profile and optimize your Django project.

## Contents

- [Profiling](#profiling)
- [ORM](#orm)
- [Caching](#caching)
- [Serialization](#serialization)
- [Tasks](#tasks)

## Profiling

*Tools to profile your code*

### Libraries

- [Django Silk](https://github.com/jazzband/django-silk) - Silk is a live profiling and inspection tool for the Django framework. Silk intercepts and stores HTTP requests and database queries before presenting them in a user interface for further inspection.
- [Django Debug Toolbar](https://github.com/jazzband/django-debug-toolbar) - A configurable set of panels that display various debug information about the current request/response.
- [pyinstrument](https://github.com/joerick/pyinstrument) - Call stack profiler for Python. Shows you why your code is slow!
- [cProfile](https://docs.python.org/3.11/library/profile.html) - cProfile and profile provide deterministic profiling of Python programs.

## ORM

*Tools to optimize the performance of Django's ORM*

### Libraries

- [django-perf-rec](https://github.com/adamchainz/django-perf-rec) - Django-perf-rec is like Django's assertNumQueries on steroids. It lets you track the individual queries and cache operations that occur in your code.

### Articles

- [Database access optimization](https://docs.djangoproject.com/en/4.2/topics/db/optimization/) - Outlines the steps to take when attempting to optimize your database usage.

### Books

- [The Temple of Django Database Performance](https://spellbookpress.com/books/temple-of-django-database-performance/) - By [Andrew Brookins](https://andrewbrookins.com/)

### Talks

- [Django Performance & You](https://www.stephenmwangi.com/talks/django-perf-and-you/) - Presentation on the N+1 query problem, EXPLAIN ANALYZE, scan types, covering & partial indexes, and SELECT COUNT(*) estimates.

## Caching

*"A certain woman had a very sharp consciousness but almost no memory. She remembered enough to work, and she worked hard." - Lydia Davis*

### Libraries

- [django-cacheops](https://github.com/Suor/django-cacheops) - A slick ORM cache with automatic granular event-driven invalidation.
- [django-cachalot](https://github.com/noripyt/django-cachalot) - Caches your Django ORM queries and automatically invalidates them.
- [django-cache-machine](https://github.com/django-cache-machine/django-cache-machine) - Automatic caching and invalidation for Django models through the ORM.
- [django-ormcache](https://github.com/educreations/django-ormcache) - A cache manager mixin that provides some caching of objects for the ORM.

## Serialization

*Tools to optimize Django serializers*

### Libraries

- [drf_orjson_renderer](https://github.com/brianjbuck/drf_orjson_renderer) - A JSON renderer and parser for Django Rest Framework using the orjson library. Backed by Rust, orjson is safe, correct and fast.
- [Django Compression Middleware](https://github.com/friedelwolff/django-compression-middleware) -  Django middleware to compress responses using algorithms such as Zstandard, Brotli, and gzip.
- [serpy](https://github.com/clarkduvall/serpy) - A super simple object serialization framework built for speed.
- [marshmallow](https://github.com/marshmallow-code/marshmallow) - An ORM/ODM/framework-agnostic library for converting complex datatypes, such as objects, to and from native Python datatypes.

### Articles

- [Improve Serialization Performance in Django Rest Framework](https://hakibenita.com/django-rest-framework-slow) - How we reduced serialization time by 99%!
- [Python Serialization Benchmark](https://voidfiles.github.io/python-serialization-benchmark/) - A set of benchmarks for python serialization frameworks.

## Tasks
