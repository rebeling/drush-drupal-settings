# drush-drupal-settings
 Allows you to get values for read only settings that are stored in settings.php (drush 9.3 and newer)

## Installation

```
composer require nymedia/drupal_settings
```

## Usage

Imagine we have a settings.local.php that includes this:

```php
$settings['environment'] = 'development';
```

Now maybe we want to get ahold of this value in a bash script, or a composer script. We could just go ahead and use this package:

```
drush setting:get environment
```
