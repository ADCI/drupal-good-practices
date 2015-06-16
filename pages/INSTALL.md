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
  - [Administration menu](https://www.drupal.org/project/admin_menu)  
    A time-saver for site administrators, and useful for developers and site builders.
  - [jQuery Update](https://www.drupal.org/project/jquery_update)  
    Upgrades the version of jQuery in Drupal core (from 1.4.2) to a newer version of jQuery.
  - [Module Filter](https://www.drupal.org/project/module_filter)  
    Greatly improves modules administration page.
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

## Good-to-have modules
*You will need to have these modules installed very often.*

## Basic configuration
