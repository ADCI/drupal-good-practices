# Main

## Table of Contents

- [Users](#users)
- [Content Display](#content)
- [Revisions and Moderation](#revision)
- [Multilanguage](#multilanguage)
- [Forms](#forms)
- [Search](#search)
- [Cache](#cache)
- [Security](#security)
- [Debug](#debug)
- [Theming](#theming)
- [Test](#testing)
- [Deploy](#deployment)

## Users

### User #1

[Securing user #1](https://www.drupal.org/node/947312)

## Content Display

**@todo TBD**

## Revisions and Moderation

**@todo TBD**

## Multilanguage

**@todo TBD**

## Forms

**@todo TBD**

## Search

**@todo TBD**

## Cache

**@todo TBD**

## Security

**@todo TBD**

## Debug

**@todo TBD**

## Theming

Inherit your site's theme from some base theme. Most popular base themes:

  - [Zen](https://www.drupal.org/project/zen)
  - [Omega](https://www.drupal.org/project/omega)
  - [Bootstrap](https://www.drupal.org/project/bootstrap)
  - [AdaptiveTheme](https://www.drupal.org/project/adaptivetheme)

Follow [CSS formatting guidelines](https://www.drupal.org/node/1887862).
Also see 
[CSS architecture](https://www.drupal.org/coding-standards/css/architecture), 
[CSS file organization](https://www.drupal.org/node/1887922) and 
[SMACSS](https://smacss.com/).

Make sure your theme adds **block-[module]-[delta]** class to blocks to avoid usage of IDs in CSS selectors.  
For styling needs also add more classes to blocks via **Block Class** module, add more classes and customize markup in Views via Views UI.  
For more info on modules configuration and usage see [Modules](/docs/MODULES.md/) page.

**@todo CSS preprocessors, postprocessor, etc.**

## Test

**@todo TBD**

## Deploy

**@todo TBD**
