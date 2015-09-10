# Modules

## Table of Contents

  - [Administration](#administration)
    - [Administration menu](#administration-menu)
    - [Module Filter](#module-filter)
    - [Fast Permissions Administration](#fast-permissions-administration)
    - [Features](#features)
    - [Administration Views](#administration-views)
    - [Views Bulk Operations (VBO)](#views-bulk-operations-vbo)
    - [Backup and Migrate](#backup-and-migrate)
    - [ThemeKey](#themekey)
    - [Workbench Moderation](#workbench-moderation)
    - [Schema](#schema)
    - [Flood control](#flood-control)
    - [Rabbit Hole](#rabbit-hole)
    - [jQuery Update](#jquery-update)
    - [Pathauto](#pathauto)
    - [Views data export](#views-data-export)
    - [Diff](#diff)
  - [Development](#development)
    - [Devel](#devel)
    - [Masquerade](#masquarade)
    - [Libraries API](#libraries-api)
  - [Files](#files)
    - [IMCE](#imce)
  - [Content](#content)
    - [Views](#views)

## Administration

### [Administration menu](https://www.drupal.org/project/admin_menu)

  - Fast navigation through administration pages, administration and development tools and more.
  - Looks nice with Toolbar Style.

### [Module Filter](https://www.drupal.org/project/module_filter)

  - Greatly improves modules administration page.

### [Fast Permissions Administration](https://www.drupal.org/project/fpa)

  - Greatly improves permissions administration page.

### [Features](https://www.drupal.org/project/features)

  - Try to understand meaning of the "Feature" word.
  - Start machine names of your features with **feature_** prefix.
  - Place your features to **sites/all/modules/features** or **sites/[site]/modules/features** directory.
  - Set another modules package for your features (ex "Custom Features")
  - Remember: each feature is Drupal module so you can have some custom in it.
  - For complex custom code it's preferred to place it to separate custom module and set dependency on feature instead of having a lot of custom code in the feature.

### [Administration Views](https://www.drupal.org/project/admin_views)

  - Replaces number of core's administrative overview/listing pages with views making it possible to customize, extend these pages and add more similar pages for different purposes.

### [Views Bulk Operations (VBO)](https://www.drupal.org/project/views_bulk_operations)

  - Augments [Views](#views) by allowing bulk operations to be executed on the displayed rows.
  - Extendable by code and [Rules](#rules).
  - Requirement for the [Administration Views](#administration-views).

### [Backup and Migrate](https://www.drupal.org/project/backup_migrate)

  - Excellent and easy to use backup solution for small and middle projects.
  - Do not use this module on biggest projects. CLI solutions (like the Drush) more preferred.
  - Do not save backup to public access directories.

### [ThemeKey](https://www.drupal.org/project/themekey)

  - Allows to define simple or sophisticated theme-switching rules which allow automatic selection of a theme depending on current path, taxonomy terms, language, node-type, and many, many other properties.

### [Workbench Moderation](https://www.drupal.org/project/workbench_moderation)

  - Adds arbitrary moderation states to Drupal core's "unpublished" and "published" node states, and affects the behavior of node revisions when nodes are published.

### [Schema](https://www.drupal.org/project/schema)

  - Compares the live database structure with the schema structure declared by all enabled modules, reporting on any missing or incorrect tables.
  - Provides hyperlinked display of the schema's embedded documentation explaining what each table and field is for.
  - Examines the live database and creates Schema API data structures for all tables that match the live database.

### [Flood control](https://www.drupal.org/project/flood_control)

  - Adds an administration interface for hidden flood control variables in Drupal 7, like the login attempt limiters and any future hidden variables.

### [Rabbit Hole](https://www.drupal.org/project/rabbit_hole)

  - Adds the ability to control what should happen when an entity is being viewed at its own page.
  - Useful if you have a content type that never should be displayed on its own page, like an image content type that's displayed in a carousel.

### [jQuery Update](https://www.drupal.org/project/jquery_update)

  - Set default jQuery version to at least **1.7** which is safe option for most of sites, newer is better.
  - Override default jQuery version for your admin theme - set **1.5** or even **1.4** (shipped with Drupal core). With newer versions issues in admin UI are possible.

### [Views data export](https://www.drupal.org/project/views_data_export)

  **@todo TBD**

### [Diff](https://www.drupal.org/project/diff)

  **@todo TBD**

### @todo Weight vs. Nodequeue (vs. other?)
### @todo Elysia Cron vs. Ultimate Cron

## Development

### [Devel](https://www.drupal.org/project/devel)

  - A set of development helper tools for debugging, content generation, etc.

### [Masquerade](https://www.drupal.org/project/masquerade)

  - allows site administrators to switch users and surf the site as that user (no password required).
  - Helpful for site developers when trying to determine what a client, logged in as themselves, might see when logged into the site.
  - **@todo Do not use on production?**

### [Libraries API](https://www.drupal.org/project/libraries)

  - Attach all external libraries by Libraries API.
  - Exceptions are not acceptable.

### [Pathauto](https://www.drupal.org/project/pathauto)

  - Do not use default "content" path for Node

## Content

### [Views](https://www.drupal.org/project/views)

  - Adequate machine names for your views and displays.
  - View and displays names should talk about where and how they will be used.
  - Write a little descriptions for view and displays.
  - [Content cache](https://www.drupal.org/project/views_content_cache) for Node, Time based cache for another entity types.
  - Attach your views to features.
  - Add CSS class to displays.

## Files

### [IMCE](https://www.drupal.org/project/imce)

  - Configure default IMCE profile for uploading files to non-root directory.