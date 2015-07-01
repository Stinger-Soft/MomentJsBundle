# Moment.js Bundle for Symfony2
Moment.js Bundle for Symfony2

## Current Version

Moment.js v2.10.3

## Installation

### Add bundle to your composer.json file

``` js
// composer.json

{
    "require": {
		// ...
        "stinger/momentjs-bundle": "~2.10"
    }
}
```

### Add bundle to your application kernel

``` php
// app/AppKernel.php

public function registerBundles()
{
    $bundles = array(
        // ...
        new Stinger\MomentJsBundle\StingerMomentJsBundle(),
        // ...
    );
}
```

### Download the bundle using Composer

``` bash
$ php composer.phar update stinger/momentjs-bundle
```

### Install assets

Given your server's public directory is named "web", install the public vendor resources

``` bash
$ php app/console assets:install web
```

Optionally, use the --symlink attribute to create links rather than copies of the resources 

``` bash
$ php app/console assets:install --symlink web
```

### Usage

Add the css and js file where needed:

``` html
{% javascripts
	'bundles/stingermomentjs/js/moment-with-locales.min.js'
%}
	<script src="{{ asset_url }}" ></script>
{% endjavascripts %}
```


# Licenses

Refer to the source code of the included files for license information

# References

1. http://momentjs.com
2. http://symfony.com
