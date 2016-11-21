# phulp-angular-template-cache

The angular-template-cache addon for [PHULP](https://github.com/reisraff/phulp).

It's like [gulp-angular-templatecache](https://github.com/miickel/gulp-angular-templatecache) with some modifications.

## Install

```bash
$ composer require reisraff/phulp-angular-template-cache
```

## Usage

```php
<?php

use Phulp\AngularTemplateCache\AngularTemplateCache;

$phulp->task('angular-template-cache', function ($phulp) {
    $phulp->src(['src/'], '/html$/')
        ->pipe(new AngularTemplateCache('templateCacheHtml.js', ['module' => 'app', 'root' => 'app']))
});

```