# Layout building

## Table of Contents

  - [Core blocks](#core-blocks)
  - [Display Suite](#display-suite)
  - [Panels](#panels)
  - [Context](#context)
  - [Summary](#summary)
  - [Links](#links)

## Core blocks

There are many blocks defined by Drupal core modules and contributed modules, you can also create blocks with content via UI using core's Block module.
Drupal core provides simple enough blocks visibility system: blocks are assigned to (theme) regions, block visibility can be based on paths patterns or content-types.
When using Drupal core blocks system, site's pages are built from blocks using visibility rules.
This way is simple but also less flexible - it's limited to regions (you can't configure smaller parts), one block can be assigned to only one region and in one particular order.
Because of such limitations Drupal core blocks visibility system will not fit your needs often.

## Display Suite

[Display Suite](https://www.drupal.org/project/ds) module provides possibility to create new displays for entities via UI and many options to deal with them.
This module operates an entity content, allows to use different layouts for different displays, add special fields to displays (add block as field, clone existing field, define new field by code, etc.) - these features and core's visibility settings for fields make this module very powerful.
Module contains a lot of predefined layouts which can be overriden via Drupal templating/theming system, new layouts may be defined as well.
As it was mentioned above, the **Display Suite** module is limited to entity content.

If you only need to add more display modes to entities and other features are not needed (so Drupal core's fields formatting and visibility settings are enough) - check the [Entity view modes](https://www.drupal.org/project/entity_view_mode) module then.

Read the [module's documentation](https://www.drupal.org/node/644662) for more details.

## Panels

[Panels](https://www.drupal.org/project/panels) module gives you absolute freedom in content region layouts configuration.
Powered by the [Chaos tool suite (ctools)](https://www.drupal.org/project/ctools) - one of the most popular Drupal contributed module - it provides tons of features and options.
You can create any layout for content of any page, output needed blocks in regions (sub-regions of the content region) which you also can define.

In combination with **Page manager** module (part of the **ctools**) you can create any pages with any content layout you need.

Read the [module's documentation](https://www.drupal.org/node/496278) for (much more) details.

## Context

The [Context](https://www.drupal.org/project/context) module name is self-explaining - it allows to perform different actions on pages depending on pages' contexts (or number of met conditions).
Probably most used reaction on contexts is blocks visibility settings - because of many kinds of contexts which can be checked and a lot of contrinuted modules which extend its functionality it provides much more flexibility in blocks visibility configuration than Drupal core's visibility system.
But blocks visibility is limited to regions like Drupal core's system.

There are actually many other reactions of different kinds available. Check the [project's page](https://www.drupal.org/project/context) for more info.

## Summary

There is no single solution which fits all possible needs. Each of mentioned solution has its pros and cons.

Layouts building may be divided into 3 levels:

 1. Entities (usually nodes) content management (rendering of entities using display modes).
 2. Content region layout management (which is "main" region and is always here).
 3. Page's layout management (header, footer, etc.).

Depending on site's complexity (number of kinds of content and its layout complexity) different solutions may be applied:

 1. On small/simple sites Drupal core's blocks visibility system and entities/fields display system should be enough.
 2. If content region part becomes complex - try building layouts and assigning blocks via **Panels**, and **display modes** for nodes and other entities.
 3. If other pages' regions like header and footer becomes dynamic - try adding **context** to previous point.

Just to summarize:

- First of all try to leverage entities display modes for better layouts and styling (re)use.
- Different situations need different solution, but in cases of really complex sites it's possible to use them all in combination - don't much afraid to try this.

## Links

 - [Panels, Display Suite, and Context - oh my! What to use when, why, and how](https://www.youtube.com/watch?v=Hc1ujlWlA0c)
