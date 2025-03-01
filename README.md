![logo](assets/logo.png)

# Youtube Frame Generator
Laravel package allows you to generate an iframe tag with a video player depending on a youtube URL.

##### 1 - Dependency
The first step is using composer to install the package and automatically update your composer.json file, you can do this by running:

```shell
composer require syrian-open-source/laravel-youtube-iframe-generator
```

##### 2 - Copy the package providers to your local config with the publish command, this will publish the config:
```shell
php artisan yframe:install
```

Features
-----------
basic usage:

```php
{!! \SOS\LaravelYoutubeFrameGenerator\Facades\YFrameFacade::generate('https://www.youtube.com/watch?v=35JzR2ymxJE')!!}
```

If you want to set your css, attributes, height, width or fullscreen allowed:
```php

{!! \SOS\LaravelYoutubeFrameGenerator\Facades\YFrameFacade::width('100%')
        ->height('400px')
        ->isFullscreen(true)
        ->generate('https://www.youtube.com/watch?v=35JzR2ymxJE'); !!}

```

Changelog
---------
Please see the [CHANGELOG](https://github.com/syrian-open-source/laravel-youtube-iframe-generator/blob/master/CHANGELOG.md) for more information about what has changed or updated or added recently.

Security
--------
If you discover any security related issues, please email them first to "your email", 
if we do not fix it within a short period of time please open a new issue describing your problem. 

Credits
-------
* [Abdussalam M. Al-Ali](https://www.linkedin.com/in/abdussalam-alali/)
* [All contributors](https://github.com/syrian-open-source/laravel-youtube-iframe-generator/graphs/contributors)
