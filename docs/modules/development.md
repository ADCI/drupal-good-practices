# Development

## Table of Contents

  - [Devel](#devel)
  - [Masquerade](#masquarade)
  - [Entity API](#entity-api)

### [Devel](https://www.drupal.org/project/devel)

  - A set of development helper tools for debugging, content generation, etc.

### [Masquerade](https://www.drupal.org/project/masquerade)

  - allows site administrators to switch users and surf the site as that user (no password required).
  - Helpful for site developers when trying to determine what a client, logged in as themselves, might see when logged into the site.
  - **@todo Do not use on production?**

### [Entity API](https://www.drupal.org/project/entity)

  - Extends the entity API of Drupal core in order to provide a unified way to deal with entities and their properties.
  - It's very probable that you'll have it as dependency of other modules.
  - Very helpful in dealing with nodes and other entities in your code, or if you define your own entity types.
  - Entity Token module defines tokens for defined entity types (not only for core's node, user, etc.).