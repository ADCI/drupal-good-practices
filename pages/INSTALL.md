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

## Good-to-have modules
*You will need to have these modules very often.*

## Basic configuration
