# Cache and performance

## Table of Contents

  - [Core cache](#core-cache)
  - [Anonymous cache](#anonymous-cache)
  - [Views cache](#views-cache)
  - [Panels cache](#panels-cache)
  - [Entity cache](#entity-cache)
  - [External cache storage](#external-cache-storage)
  - [Summary](#summary)

## Core cache

Drupal core provides just a few options for caching, but even these options enabled can noticeably improve performance.

Drupal core cache options are:

  - Blocks cache.
  - Full page cache (for anonymous visitors).

## Anonymous cache

If there are no differences in behavior on backend for different anonymous users (which is usually true) then luckily the whole pages can be cached.
Pages' caching which avoids Drupal run to build and render page's content drastically improves performance.
This cache can be made even faster by using of [external storages](#external-cache-storage) for such cache.

## Views cache

In almost (all) cases there is [Views](https://www.drupal.org/project/views) module installed on a Drupal 7 site.
Outputs built with **Views** can (and should) also be cached. Views is shipped with time-based cache so lifetime is set for cache and after passing this time cache become obsolete and rebuilt. Both raw query result and rendered output can be cached.

You'll definitely want to show relevant content on your site and show updated or new content (almost) immediately after making changes. With default **Views** cache you'll have to set small enough cache lifetimes to achieve this, but performance gain will be less than it could be (cache rebuilds may happen even if there are no updates in content) and updates will still happen not immediately.
[Views content cache](https://www.drupal.org/project/views_content_cache) module is more preferred in this case - it provides alternative **Views** cache plugin which rebuilds cache when changes happen in content.

## Panels cache

When using [Panels](https://www.drupal.org/project/panels) you can leverage caching for them as well.
**Panels** allow to cache the whole panel or parts of it.
Similar to content-based caching solution for **Views** module, there is [Panels Content Cache](https://www.drupal.org/project/panels_content_cache) module for **Panels**.

## [Entity cache](https://www.drupal.org/project/entitycache)

Most of content on Drupal 7 site is stored in different types of entities (nodes, users, taxonomy terms and other) so there are always entities loaded to build and render some content on pages.
**Entity cache** allows to put entire entity (with properties, fields and other data) to cache for load times improvements.
There is no configuration for this module, just enable it to make it working. After installation the module will make core entities (nodes, users, taxonomy terms) entire cacheable, but there are many other contrib modules which define own entity types and are integrated with the **Entity cache**.
Custom entity types can be easily integrated with the **Entity cache** as well.
Again, module gives very good improvements when [external storages](#external-cache-storage) are used to store entities cache. It can be used with default Drupal 7 cache storage (database) of course, but effect will be small enough.

## External cache storage

Database is very slow solution for storing cache and it's highly recommended to use other solutions to store cache.

### Key-value storage

[Redis](https://www.drupal.org/project/redis) and [Memcache](https://www.drupal.org/project/memcache) allows to store cache in RAM.
Use one of this if you have enough RAM - they highly increase performance, especially in combination with [Entity cache](#entity-cache).

### NoSQL storage (MongoDB and other)

It's possible to store cache for example in [MongoDB](https://www.drupal.org/project/mongodb).

### Page caching

Most effective way when dealing with caching for anonymous users is when Drupal isn't triggered at all for delivering pages content.

Most popular solutions to cache pages for anonymous users on server are:

 - [Nginx](http://nginx.org/en/) - web server, reverse proxy server as well as a load balancer and an HTTP cache.
 - [Varnish](https://www.varnish-cache.org/) - very popular HTTP accelerator with a lot of configuration options.

## @todo HTTP cache headers basics (Cache-control, etc.)

## @todo Different cache implementations for different bins configuration via settings.php. DrupalFakeCache

## @todo Nginx (and Apache?) configuration for caching of assets

## Summary

Always think about caching and leverage it, don't launch your Drupal sites without any caching enabled.
Always plan your caching strategy for both anonymous and authenticated visitors, pay attention to sensitive data (for authenticated visitors) - it may happen that data for one user will be cached and accidentally shown to another one.
