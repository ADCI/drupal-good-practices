# Utilities

## Table of Contents

  - [Chaos tool suite (ctools)](#chaos-tool-suite-ctools)
  - [Token](#token)
  - [jQuery Update](#jquery-update)
  - [Libraries API](#libraries-api)
  
### [Chaos tool suite (ctools)](https://www.drupal.org/project/ctools)

  - A set of APIs and tools to improve the developer experience.
  - Requirement for a lot of modules.
  - Plugins -- tools to make it easy for modules to let other modules implement plugins from.
  - Exportables -- tools to make it easier for modules to have objects that live in database or live in code, such as 'default views'.
  - Modal dialog -- tool to make it simple to put a form in a modal dialog.
  - Additional AJAX commands.
  - A lot lot more.

### [Token](https://www.drupal.org/project/token)

  - Extends Drupal 7 tokens system by adding some UI components, defining more tokens and other.

### [jQuery Update](https://www.drupal.org/project/jquery_update)

  - Set default jQuery version to at least **1.7** which is safe option for most of sites, newer is better.
  - Override default jQuery version for your admin theme - set **1.5** or even **1.4** (shipped with Drupal core). With newer versions issues in admin UI are possible.

### [Libraries API](https://www.drupal.org/project/libraries)

  - Attach all external libraries by Libraries API.
  - Exceptions are not acceptable.
  
### [Variable](https://www.drupal.org/project/variable)
  - Provides a registry for meta-data about Drupal variables and some extended Variable API and administration interface.
  - Other modules can know about your module's variables and they can be translated, exported, used in views, etc.
  - You'll get automatic variable edit forms, tokens, access control and uninstall for free.
  - Your module's variables will be allowed for Variable Realms being able to get values for each language (Internationalization) or Domain (Variable Domain).
  - Sometimes you'll have it just as dependency for other modules.
  