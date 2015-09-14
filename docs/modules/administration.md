# Administration

## Table of Contents

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

## [Administration menu](https://www.drupal.org/project/admin_menu)

  - Fast navigation through administration pages, administration and development tools and more.
  - Looks nice with Toolbar Style.

## [Module Filter](https://www.drupal.org/project/module_filter)

  - Greatly improves modules administration page.

## [Fast Permissions Administration](https://www.drupal.org/project/fpa)

  - Greatly improves permissions administration page.

## [Features](https://www.drupal.org/project/features)

  - Try to understand meaning of the "Feature" word.
  - Start machine names of your features with **feature_** prefix.
  - Place your features to **sites/all/modules/features** or **sites/[site]/modules/features** directory.
  - Set another modules package for your features (ex "Custom Features")
  - Remember: each feature is Drupal module so you can have some custom in it.
  - For complex custom code it's preferred to place it to separate custom module and set dependency on feature instead of having a lot of custom code in the feature.

## [Administration Views](https://www.drupal.org/project/admin_views)

  - Replaces number of core's administrative overview/listing pages with views making it possible to customize, extend these pages and add more similar pages for different purposes.

## [Views Bulk Operations (VBO)](https://www.drupal.org/project/views_bulk_operations)

  - Augments [Views](#views) by allowing bulk operations to be executed on the displayed rows.
  - Extendable by code and [Rules](#rules).
  - Requirement for the [Administration Views](#administration-views).

## [Backup and Migrate](https://www.drupal.org/project/backup_migrate)

  - Excellent and easy to use backup solution for small and middle projects.
  - Do not use this module on biggest projects. CLI solutions (like the Drush) more preferred.
  - Do not save backup to public access directories.

## [ThemeKey](https://www.drupal.org/project/themekey)

  - Allows to define simple or sophisticated theme-switching rules which allow automatic selection of a theme depending on current path, taxonomy terms, language, node-type, and many, many other properties.

## [Workbench Moderation](https://www.drupal.org/project/workbench_moderation)

  - Adds arbitrary moderation states to Drupal core's "unpublished" and "published" node states, and affects the behavior of node revisions when nodes are published.

## [Schema](https://www.drupal.org/project/schema)

  - Compares the live database structure with the schema structure declared by all enabled modules, reporting on any missing or incorrect tables.
  - Provides hyperlinked display of the schema's embedded documentation explaining what each table and field is for.
  - Examines the live database and creates Schema API data structures for all tables that match the live database.

## [Flood control](https://www.drupal.org/project/flood_control)

  - Adds an administration interface for hidden flood control variables in Drupal 7, like the login attempt limiters and any future hidden variables.

## [Rabbit Hole](https://www.drupal.org/project/rabbit_hole)

  - Adds the ability to control what should happen when an entity is being viewed at its own page.
  - Useful if you have a content type that never should be displayed on its own page, like an image content type that's displayed in a carousel.
  - This is not an access control module!
  - In most cases you will not need to override Rabbit Hole bundle settings on entity level.
  - If you often need to override bundle settings on entity level, make sure this module fits your needs and you do not need true access control for example.

## TODO items

### [Override Node Options](https://www.drupal.org/project/override_node_options)

  **@todo Is it really helpful?**

### [Views data export](https://www.drupal.org/project/views_data_export)

  **@todo TBD**

### [Diff](https://www.drupal.org/project/diff)

  **@todo TBD**

### [Ultimate Cron](https://www.drupal.org/project/ultimate_cron)

  **@todo TBD**
  
### @todo Weight vs. Nodequeue (vs. other?)

### @todo https://www.drupal.org/project/total_control ?