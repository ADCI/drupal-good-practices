# Basic installation and configuration.

## Table of Contents

  - [Installation](#installation)
  - [Not used modules](#not-used-modules)
  - [Must-have modules](#must-have-modules)
  - [Good-to-have modules](#good-to-have-modules)
  - [Basic configuration](#basic-configuration)

## Installation
*Basic Drupal installation.*

There are 2 installation profiles options available by default:

  - Standard
  - Minimal

*Standard* is recommended option, it pre-configures misc things like *Article* and *Basic page* content-types, a few useful text formats and so on.

## Not used modules
*In most cases you will not need these modules*

  - Color
  - Dashboard
  - Overlay
  - Shortcut
  - Toolbar

Often you will not need to have *Comment* module installed.

You may uninstall listed modules via [Drush](DRUSH.md) using following commands:  
*drush dis -y color, comment, dashboard, overlay, shortcut, toolbar*  
*drush pmu -y color, comment, dashboard, overlay, shortcut, toolbar*

## Must-have modules
*In most cases you should have these modules installed.*

  - [Chaos tool suite (ctools)](https://www.drupal.org/project/ctools)  
    At least you'll need it as dependency for some of other must-have modules.
  - [Views](https://www.drupal.org/project/views)  
    Most of listings on the site like blog, news archive, related articles, front page slideshow, etc. will be built using this module.
  - [Token](https://www.drupal.org/project/token)  
    Adds more tokens and enhances UI for core's tokens.
  - [Pathauto](https://www.drupal.org/project/pathauto)  
    Automatically generates URL/path aliases for various kinds of content.
  - [Global Redirect](https://www.drupal.org/project/globalredirect)  
    Checks the current URL for an alias and does a 301 redirect to it if it is not being used. And not only.
  - [Administration menu](https://www.drupal.org/project/admin_menu)  
    A time-saver for site administrators, and useful for developers and site builders.
  - [jQuery Update](https://www.drupal.org/project/jquery_update)  
    Upgrades the version of jQuery in Drupal core (from 1.4.2) to a newer version of jQuery.
  - [Module Filter](https://www.drupal.org/project/module_filter)  
    Greatly improves modules administration page.
  - [Fast Permissions Administration](https://www.drupal.org/project/fpa)  
    Similar to **Module Filter** but for permissions administration page.
  - [Features](https://www.drupal.org/project/features)  
    Exports different site building components and bundling them together in a single feature module.
  - [Transliteration](https://www.drupal.org/project/transliteration)  
    Provides one-way string transliteration (romanization) and cleans file names during upload by replacing unwanted characters.
  - [Devel](https://www.drupal.org/project/devel)  
    A suite of developer helper modules.
  - [Strongarm](https://www.drupal.org/project/strongarm)  
    Usually used with **Features** to export Drupal variable values.
  - [Block Class](https://www.drupal.org/project/block_class)  
    Allows users to add classes to any block through the block's configuration interface.
  - [Title](https://www.drupal.org/project/title)  
    Convert node titles to the Field API in order to make nodes fully translatable.
  - [Delta](https://www.drupal.org/project/delta)  
    Delta Blocks submodule exposes a number of core Drupal elements as blocks.

## Good-to-have modules
*You will need to have these modules installed very often.*

  - [Libraries API](https://www.drupal.org/project/libraries)  
    The common denominator for all Drupal modules/profiles/themes that integrate with external libraries.  
    It's most likely that you'll have it as dependency for some other modules.
  - [CKEditor - WYSIWYG HTML editor](https://www.drupal.org/project/ckeditor)  
    Allows to replace textarea fields with the CKEditor WYSIWYG editor.  
    If you have rich text textarea fields then you need it.
  - [IMCE](https://www.drupal.org/project/imce)  
    Image/file uploader and browser that supports personal directories and quota.  
    If you have **CKEditor** then you probably should have it as well.
  - [IMCE Mkdir](https://www.drupal.org/project/imce_mkdir)  
    Allows users to create and delete sub-directories under directories assigned by IMCE.  
    If you have **IMCE** then you should have this one as well.
  - [Elysia Cron](https://www.drupal.org/project/elysia_cron)  
    Extends Drupal standard cron, allowing a fine grain control over each task.  
    Almost must-have.
  - [Entity API](https://www.drupal.org/project/entity)  
    Extends the entity API of Drupal core in order to provide a unified way to deal with entities and their properties.  
    It's very probable that you'll have it as dependency of other modules.  
    Must-have if you deal with nodes and other entities in your code, or if you define your own entity types.
  - [Entity cache](https://www.drupal.org/project/entitycache)  
    Puts core entities into Drupal's cache API.  
    Use with [Memcache API and Integration](https://www.drupal.org/project/memcache) or [Redis](https://www.drupal.org/project/redis) - so if your server allows to use one of these modules then **Entity cache** is must-have.
  - [Entity reference](https://www.drupal.org/project/entityreference)  
    Provides a field type that can reference arbitrary entities.  
    Create relations between entities (nodes, users and other). Similar [References](https://www.drupal.org/project/references) module is **not recommended for use**.
  - [Rabbit Hole](https://www.drupal.org/project/rabbit_hole)  
    Adds the ability to control what should happen when an entity is being viewed at its own page.  
    Useful if you have a content type that never should be displayed on its own page, like an image content type that's displayed in a carousel.
  - [Entity view modes](https://www.drupal.org/project/entity_view_mode)  
    Allows administrators to define custom view modes for entities.
  - [Better Formats](https://www.drupal.org/project/better_formats)  
    Adds more flexibility to Drupal's core input format system.
  - [Field Group](https://www.drupal.org/project/field_group)  
    All fieldable entities will have the possibility to add groups to wrap their fields together. Comes with default HTML wrappers like vertical tabs, horizontal tabs, accordions, fieldsets or div wrappers.
  - [Rules](https://www.drupal.org/project/rules)  
    Allows site administrators to define conditionally executed actions based on occurring events.
  - [Diff](https://www.drupal.org/project/diff)  
    Basically shows differencies between revisions. But also very helpful for developers when dealing with **Features**, particularly with overriden features exports.
  - [CAPTCHA](https://www.drupal.org/project/captcha)  
    A challenge-response test most often placed within web forms to determine whether the user is human.
  - [Views Bulk Operations (VBO)](https://www.drupal.org/project/views_bulk_operations)  
    Augments **Views** by allowing bulk operations to be executed on the displayed rows.
  - [Administration Views](https://www.drupal.org/project/admin_views)  
    Replaces administrative overview/listing pages with actual views for superior usability.  
    Requires **Views Bulk Operations (VBO)** be installed.
  - [Search API](https://www.drupal.org/project/search_api)  
    Provides a framework for easily creating searches on any entity known to Drupal, using any kind of search engine. Integrated well with **Views**.  
    Recommended for building of any kind of searches on the site. Recommended for use with [Search API Solr Search](https://www.drupal.org/project/search_api_solr). [Search API Database Search](https://www.drupal.org/project/search_api_db) backed may be used as starter option.
  - [ImageCache Actions](https://www.drupal.org/project/imagecache_actions)  
    Provides a suite of additional image effects that can be added to image styles (watermarking, file format switcher, rounded corners, etc.). Also adds the 'duplicate', 'export' and 'import' actions to image styles administration.

*See [Modules](MODULES.md) documentation page for more info on contrib modules.*

## Basic configuration

### Title settings

In the **Node** group check "Title" under **Automatic field replacement**.

**@todo Label replacement and Taxonomy term settings?**

*admin/config/content/title*

### jQuery Update

Set default jQuery version to at least **1.7** which is safe option for most of sites, newer is better.  
Override default jQuery version for your admin theme - set **1.5** or even **1.4** (shipped with Drupal core). With newer versions issues in admin UI are possible.

*admin/config/development/jquery_update*

### File system

Set some **Private file system path**. Make sure that **Transliteration** options are switched on.

**@todo Disable "Transliterate the displayed file name." option?**

*admin/config/media/file-system*

### Account settings

Un-tick "Enable user pictures." option under **PERSONALIZATION** - in most cases you will not need it, use profiles with fields instead.

*admin/config/people/accounts*

**@todo Is it easy enough to show pictures from profiles in comments for example?**

### Regional settings

Set **Default country** to "- None -" - initially it's safiest value, then the setting may be adjusted.  
Set appropriate **First day of week**.  
Set **Default time zone** to UTC.  
Un-tick "Users may set their own time zone." - in most cases you will not need this.

*admin/config/regional/settings*

### URL aliases

Empty **Default path pattern** in **CONTENT PATHS** and never set it to non-empty value.  
Set appropriate **Default path pattern** in **TAXONOMY TERM PATHS** or make it empty.  
Set appropriate **Pattern for user account page paths** in **USER PATHS** or make it empty.  
Set empty patterns for content-types if nodes of these types should not be visible for regular users on their own pages (slidshow elements for example).  
Patterns should consist of several parts separated by */* sign, for example for nodes *\[node:content-type\]/\[node:title\]* is good candidate. Try to avoid one-part aliases, for nodes of *Basic Page* content-type one-part aliases are ok (about-us, contact-us, etc.).

*/admin/config/search/path/settings*

**@todo Transliterate aliases?**

*admin/config/search/path/settings*

### Site information

Set appropriate **Site name** and **admin@localhost.com** if were not set on installation.

*admin/config/system/site-information*

### Cron

**@todo Set to "Never" on development?**

*admin/config/system/cron*

### Delta blocks

**@todo TBD**

### People

**@todo administrator/developer role**

### Content types

Edit **Article** and **Basic page** content types created during installation. Remove **Article** content-type if you don't need it. On content-type edit pages un-tick "Promoted to front page" checkbox in **Publishing options** group. Set other settings as needed. Give attention to **Comment settings** if you left the Comment module enabled because of needs and to **Menu settings**.

*admin/structure/types*  
*admin/structure/types/manage/article*  
*admin/structure/types/manage/page*

Replace Title property by Title field instance on the **MANAGE FIELDS** pages. Remove **Image** and **Tags** fields from **Article** content-type if needed. Adjust display settings on the **MANAGE DISPLAY** pages if needed.

*admin/structure/types/manage/article/fields*  
*admin/structure/types/manage/page/fields*

### Features

On the Features settings page set **Default export path** under **GENERAL SETTINGS** to "sites/all/modules/features".

*admin/structure/features/settings*

### Taxonomy

Delete "Tags" vocabulary if it's not needed for you.

*admin/structure/taxonomy*

### Views

On the Views settings page make sure the following settings are set:

  - Show filters on the list of views
  - Show advanced help warning
  - Always show the master display
  - Always show advanced display settings
  - Show information and statistics about the view during live preview
    - Above the preview
    - Show the SQL query
    - Show performance statistics
    - Show other queries run during render during live preview

Un-tick "Automatically update preview on changes".

*admin/structure/views/settings*

Development Views settings may be also set by executing of the following **drush** command:  
*drush vd*

### Update manager

On the Available updates settings page check the **Check for updates of disabled modules and themes**.

*admin/reports/updates/settings*
