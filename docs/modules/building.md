# Site building

## Table of Contents

  - [Views](#views)
  - [Date](#date)
  - [Webform](#webform)
  - [link](#link)
  - [Views Slideshow](#views-slideshow)
  - [Colorbox](#colorbox)
  - [Entity reference](#entity-reference)
  
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
