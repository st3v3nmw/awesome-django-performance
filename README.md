# Awesome Django Performance [![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)

> A curated list of libraries, tools, blog articles, and books to help profile and optimize your Django project.

## Contents

- [Profiling](#profiling)
- [Database](#database)
- [Caching](#caching)
- [Serialization](#serialization)
- [Tasks](#tasks)
- [Testing](#testing)
- [Monitoring](#monitoring)
- [Servers](#servers)
- [Books](#books)

## Profiling

### Tools

- [Django Silk](https://github.com/jazzband/django-silk) - Silk is a live profiling and inspection tool for the Django framework. Silk intercepts and stores HTTP requests and database queries before presenting them in a user interface for further inspection.
- [Django Debug Toolbar](https://github.com/jazzband/django-debug-toolbar) - A configurable set of panels that display various debug information about the current request/response.
- [pyinstrument](https://github.com/joerick/pyinstrument) - Call stack profiler for Python. Shows you why your code is slow!
- [cProfile](https://docs.python.org/3.11/library/profile.html) - cProfile and profile provide deterministic profiling of Python programs.

## Database

### Tools

- [django-auto-prefetching](https://github.com/GeeWee/django-auto-prefetching) - Never worry about n+1 performance problems again (DRF views level).
- [djangorestframework-queryfields](https://github.com/wimglenn/djangorestframework-queryfields) - Allows clients to control which fields will be sent in the API response.
- [django-perf-rec](https://github.com/adamchainz/django-perf-rec) - Django-perf-rec is like Django's assertNumQueries on steroids. It lets you track the individual queries and cache operations that occur in your code.
- [django-auto-prefetch](https://github.com/tolomea/django-auto-prefetch) - Automatically prefetch foreign key values as needed (ORM level).
- [django-zen-queries](https://github.com/dabapps/django-zen-queries) - Explicit control over database query execution in Django applications.
- [nplusone](https://github.com/jmcarp/nplusone) - Auto-detecting the n+1 queries problem in Python.
- [django-pickling](https://github.com/Suor/django-pickling) - Efficient pickling for Django models.
- [django-test-query-counter](https://github.com/sophilabs/django-test-query-counter/) - A Django toolkit for controlling query count when testing.
- [PgBouncer](https://www.pgbouncer.org/) - Lightweight connection pooler for PostgreSQL.

### Articles

- [Database access optimization](https://docs.djangoproject.com/en/dev/topics/db/optimization/) - Outlines the steps to take when attempting to optimize your database usage.
- [Django Performance Improvements - Part 1: Database Optimizations](https://blog.sentry.io/django-performance-improvements-part-1-database-optimizations/)
- [Automating Performance Testing in Django](https://testdriven.io/blog/django-performance-testing/)
- [Performing raw SQL queries](https://docs.djangoproject.com/en/dev/topics/db/sql/#performing-raw-sql-queries)

## Caching

### Tools

- [django-cacheback](https://github.com/codeinthehole/django-cacheback) - Smart caching for Django using Celery to refresh cached items asynchronously.
- [django-memoize](https://github.com/tdr-autosync/mi-lib-django_memoize) - A cache for function or method results.
- [django_model_cached_property](https://github.com/Legotckoi/django_model_cached_property) - Useful for caching of property results for more time than lifetime of object during the request.
- [django-cacheops](https://github.com/Suor/django-cacheops) - A slick ORM cache with automatic granular event-driven invalidation.
- [django-cachalot](https://github.com/noripyt/django-cachalot) - Caches your Django ORM queries and automatically invalidates them.
- [django-cache-machine](https://github.com/django-cache-machine/django-cache-machine) - Automatic caching and invalidation for Django models through the ORM.
- [django-ormcache](https://github.com/educreations/django-ormcache) - A cache manager mixin that provides some caching of objects for the ORM.
- [PolyScale.ai](https://www.polyscale.ai/) - A high performance Data Delivery Network (DDN) that accelerates databases. Using smart caching, it improves query performance, lowers latency and makes data access and scale engineering a breeze, both on premise and at the edge.

### Articles

- [Django's cache framework](https://docs.djangoproject.com/en/dev/topics/cache/)

## Serialization

### Tools

- [drf_orjson_renderer](https://github.com/brianjbuck/drf_orjson_renderer) - A JSON renderer and parser for Django Rest Framework using the orjson library. Backed by Rust, orjson is safe, correct and fast.
- [Django Compression Middleware](https://github.com/friedelwolff/django-compression-middleware) -  Django middleware to compress responses using algorithms such as Zstandard, Brotli, and gzip.
- [serpy](https://github.com/clarkduvall/serpy) - A super simple object serialization framework built for speed.
- [django-rest-marshmallow](https://github.com/marshmallow-code/django-rest-marshmallow) - Marshmallow schemas for Django REST framework.
- [marshmallow](https://github.com/marshmallow-code/marshmallow) - An ORM/ODM/framework-agnostic library for converting complex datatypes, such as objects, to and from native Python datatypes.

### Articles

- [Improve Serialization Performance in Django Rest Framework](https://hakibenita.com/django-rest-framework-slow) - How we reduced serialization time by 99%!
- [Python Serialization Benchmark](https://voidfiles.github.io/python-serialization-benchmark/) - A set of benchmarks for Python serialization frameworks.

## Tasks

### Tools

- [Celery](https://github.com/celery/celery) - Distributed Task Queue.
- [Celery Flower](https://github.com/mher/flower) - Real-time monitor and web admin for Celery distributed task queue.
- [django_dramatiq](https://github.com/Bogdanp/django_dramatiq) - A Django app that integrates with Dramatiq.
- [Django-RQ](https://github.com/rq/django-rq) - A simple app that provides django integration for RQ (Redis Queue).
- [Django Q](https://github.com/Koed00/django-q) - A multiprocessing distributed task queue for Django.

## Testing

### Tools

- [Locust](https://github.com/locustio/locust) - An easy to use, scriptable and scalable performance testing tool.
- [hey](https://github.com/rakyll/hey) - HTTP load generator, ApacheBench (ab) replacement.

## Monitoring

### Tools

- [Sentry SDK](https://docs.sentry.io/platforms/python/) - The official Python SDK for Sentry.io (has an APM offering).
- [statsd](https://github.com/statsd/statsd) - Daemon for easy but powerful stats aggregation.
- [django-prometheus](https://github.com/korfuri/django-prometheus) - Export Django monitoring metrics for Prometheus.io.
- [django-postgres-metrics](https://github.com/django-postgres-metrics/django-postgres-metrics) - A Django application that exposes a bunch of PostgreSQL database metrics.
- [Grafana](https://grafana.com/) - Operational dashboards for your data here, there, or anywhere.
- [apm-agent-python](https://github.com/elastic/apm-agent-python) -  Official Python agent for Elastic APM.
- [New Relic Python Agent](https://github.com/newrelic/newrelic-python-agent) - Instruments your application for performance monitoring and advanced performance analytics with New Relic.

## Servers

### Tools

- [Varnish Cache](https://varnish-cache.org/intro/index.html#intro) - A web application accelerator also known as a caching HTTP reverse proxy.

### Articles

- [Is Django too slow?](https://mattsegal.dev/is-django-too-slow.html)

## Books

- [The Temple of Django Database Performance](https://spellbookpress.com/books/temple-of-django-database-performance/) - By [Andrew Brookins](https://andrewbrookins.com/).
- [High Performance Django](https://lincolnloop.com/high-performance-django/index.html) - By Peter Baumgartner and Yann Malet.
