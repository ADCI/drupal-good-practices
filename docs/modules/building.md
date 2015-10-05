# Site building

## Table of Contents

  - [Views](#views)
  - [Date](#date)
  - [Webform](#webform)
  - [link](#link)
  - [Views Slideshow](#views-slideshow)
  - [Colorbox](#colorbox)
  - [Entity reference](#entity-reference)
  - [Field Group](#field-group)
  - [Menu block](#menu-block)
  - [Context](#context)
  - [Internationalization](#internationalization)
  - [Strongarm](#strongarm)
  - [Display Suite](#display-suite)
  - [Menu attributes](#menu-attributes)
  - [Superfish](#superfish)
  - [Metatag](#metatag)
  - [Field collection](#field-collection)
  - [Block Class](#block-class)
  
### [Views](https://www.drupal.org/project/views)

  - Adequate machine names for your views and displays.
  - View and displays names should talk about where and how they will be used.
  - Write a little descriptions for view and displays.
  - [Content cache](https://www.drupal.org/project/views_content_cache) for Node, Time based cache for another entity types.
  - Attach your views to features.
  - Add CSS class to displays.

### [Date](https://www.drupal.org/project/date)

  - Flexible date/time field type Date field.
  - Date API that other modules can use.
  
### [Webform](https://www.drupal.org/project/webform)

  - The module for making forms and surveys. Often used for misc contact forms.
  - After a submission, users may be sent an e-mail "receipt" as well as sending a notification to administrators.
  - Results can be exported into Excel or other spreadsheet applications.
  - Also provides some basic statistical review and has an extensive API for expanding its features.
  - Does not use Drupal 7 Fields and Entities, has its own API, implementations and integrations - so it may be more lightweight solution, but sometimes it creates limitations on extendability.

### [Link](https://www.drupal.org/project/link)

  - Field type for links.
  
### [Views Slideshow](https://www.drupal.org/project/views_slideshow)

  - Can be used to create a slideshow of any content (not just images) that can appear in a View.
  - Heavily customizable.
  - Many contributes modules extend its functionality and provide more kinds of slideshow.
  
### [Colorbox](https://www.drupal.org/project/colorbox)

  - Probides Colorbox - light-weight customizable lightbox plugin for jQuery - integration into Drupal.
  - Images, iframed or inline content etc. can be displayed in a overlay above the current page.
  - Most installed Drupal 7 lightbox module.
  - There are many modules which support Colorbox or extend its functionality.  
    ex. [Colorbox node](https://www.drupal.org/project/colorbox_node) which provides an ability to display any page inside a colorbox modal without the header and footer.

### [Entity reference](https://www.drupal.org/project/entityreference)
  
  - Provides a field type that can reference arbitrary entities.  
  - Create relations between entities (nodes, users and other). Similar [References](https://www.drupal.org/project/references) module is **not recommended for use**.

### [Field Group](https://www.drupal.org/project/field_group)

  - All fieldable entities will have the possibility to add groups to wrap their fields together.
  - Comes with default HTML wrappers like vertical tabs, horizontal tabs, accordions, fieldsets or div wrappers.
  - May be used on both entity forms and displays.
  - Helps noticeable improve administrion UI, especially for entities with many fields.
  
### [Menu block](https://www.drupal.org/project/menu_block)

  - Configurable blocks of menu trees starting with any level of any menu.
  - And more!
  
### [Context](https://www.drupal.org/project/context)

  - Allows you to manage contextual conditions and reactions for different portions of your site.
  - Think of conditions as a set of rules that are checked during page load to see what context is active. Any reactions that are associated with active contexts are then fired.
  - Often used to manage blocks visibility depending on complex conditions when it's not possible to use core's blocks visibility.

### [Internationalization](https://www.drupal.org/project/i18n)

  - aka i18n.
  - Collection of modules to extend Drupal core multilingual capabilities.
  - Taxonomy translation (both, per language terms and translatable terms).
  - Multilingual variables.
  - Multilingual blocks (control visibility per language and translate title and content).
  - Language selection (when you switch the site language you'll see only the content for that language).
  
### [Strongarm](https://www.drupal.org/project/strongarm)

  - Gives site builders a way to override the default variable values that Drupal core and contributed modules ship with.
  - Mostly used with the [Features](https://www.drupal.org/project/features) module to export Drupal variable values.
  
### [Display Suite](https://www.drupal.org/project/ds)

  - Allows you to take full control over how your content is displayed using a drag and drop interface.
  - Arrange your nodes, views, comments, user data etc.
  - Dozens of template files.
  - A predefined list of layouts.
  - Possibility to add your own custom fields in the backend or in your code.
  - Possibility to add custom layouts in your theme.
  - Overrides layouts for rendered entities.
  - Has own templates so theme's node.tpl.php and similar are not used when Display Suite layout is used.
  
### [Menu attributes](https://www.drupal.org/project/menu_attributes)

  - Allows you to specify some additional attributes for menu items such as id, name, class, style, and rel.
  - Very useful when some of menu items need for individual styling (for example, links to social networks).

### [Superfish](https://www.drupal.org/project/superfish)

  - Integrates jQuery Superfish plugin with your Drupal menus.
  - Dropdown menus in blocks.
  
### [Metatag](https://www.drupal.org/project/metatag)

  - Allows you to automatically provide structured metadata, aka "meta tags", about a website.
  - Description and keywords metadata.
  - [Open Graph](http://ogp.me/) support  allow control of how content appears when shared on social networks (for example Facebook).
  - And more.
  - Most installed Drupal 7 module for metatags.
  
### [Field collection](https://www.drupal.org/project/field_collection)

  - Provides a field-collection field, to which any number of fields can be attached.
  - In other words it provides field type which is actually combination of several fields of any type.
  - Internally represented as an entity, which is embedded in the host entity.
  - Helpful in building complex fields, for example image with link.
  
### [Block Class](https://www.drupal.org/project/block_class)

  - Allows users to add classes to any block through the block's configuration interface.
  - Must-have. Blocks should not be styled using IDs in CSS selectors - classes much more preferred.
