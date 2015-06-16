# Drupal Good Practices
* * *

## Table of Contents
* * *

- [Modules](#modules)
    - [IMCE](#imce)
    - [jQuery Update](#jquery_update)
    - [Libraries API](#libraries)
    - [Features](#features)
    - [Pathauto](#pathauto)
    
## Modules
* * *

### [IMCE](https://www.drupal.org/project/imce)

  * Configure default IMCE profile for uploading files to non-root directory
 
### [jQuery Update](https://www.drupal.org/project/jquery_update)

  * Use jQuery version 1.5 for admin theme
    
### [Libraries](https://www.drupal.org/project/libraries)

  * Attach all external libraries by Libraries API
  * Exceptions are not acceptable
  
### [Features](https://www.drupal.org/project/features)

  * Try to understand the meaning of word "Feature"
  * Naming your features with "feature-" prefix
  * You can place your features in "custom" modules folder or you can create additional folder "features"
  * You can place some simple code to the feature files but if your code is more complex than a simple alter then best variant is create another custom module and set dependency to the feature module
  
### [Pathauto](https://www.drupal.org/project/pathauto)

  * Do not use default "content" path for Node.
  
