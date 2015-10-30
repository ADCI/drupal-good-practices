# Search

## Table of Contents

  - [Core Search](#core-search)
  - [Apache Solr Search](#apache-solr-search)
  - [Search API](#search-api)
  - [Summary](#summary)

## Core Search

Drupal core contains **Search** module for search functionality.
**Search** module provides separate search page with search form and block with search form which can be placed anywhere on the site and which leads to this single search page on submission.
The module stores indexed data in the site's database which may noticeably affect on performance, only core's entities may be indexed (without writing custom code) and output configuration is very limited.

**Search** module may fit the needs on small sites. It's not recommended for use on medium and large sites, when there are a lot of content to search through and/or several kinds of search functionality are presented.

## [Apache Solr Search](https://www.drupal.org/project/apachesolr)

This module doesn't have disadvantages that Drupal core's **Search** module does, so:

  - Search output is fully customizable.
  - There may be many search pages.
  - Faceted search via [Facet API](https://www.drupal.org/project/facetapi)
  - More entity types can be indexed (some via additional contrib modules), any other entity types can be easily made indexable by implementing a few hooks.

But of course main advantage of the module is:

  - **Indexed data IS NOT stored in database.**

**Apache Solr Search** module allows to drastically improve search performance (on small amounts of data it'll be less noticeable) and perform full-text search.

Main disadvantage is that the module is limited to [Apache Solr](http://lucene.apache.org/solr/) search platform so if it cannot be installed/used for some reason then module will not work for you as well.

## [Search API](https://www.drupal.org/project/search_api)

**Search API** is probably the best solution for search on Drupal 7.
This module is framework, it's generic, very flexible and extendable.
Module's functionality is build on top of entity metadata wrappers (provided by [Entity API](https://www.drupal.org/project/entity) module) so basically any entity can be indexed.
Search backends are implemented as separate modules, current implementations inlcudes [Database Search](https://www.drupal.org/project/search_api_db), [Solr Search](https://www.drupal.org/project/search_api_solr) and many more.

Advantages of the module:

  - (Almost) all of advantages of the **Apache Solr Search** module.
  - Outputs can be built via [Views](https://www.drupal.org/project/views), exposed filters are fully-functional in this case.
  - There may be many indexes and many search backends used at the same time.
  - For particular search index you can switch search backend to another one at any time.
  - In most of use cases UI will be 100% enough for needed functionality configuration.
  - Index data may be processed or altered using special filters.
  - Search servers, data sources, filters - all can be defined in nice way via PHP classes.

## Summary

**Search API** module is probably the best search for Drupal 7 so it's highly recommended for use on any site.
Even if database powered search is ok for your needs, with **Search API** you'll be able to easily switch to any of many other search backends if needs will change.
