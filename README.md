# Fis3 Smarty Extension for Yii 2

This extension provides a `ViewRender` that would allow you to use [Smarty](http://www.smarty.net/) view template engine
with [Yii framework 2.0](http://www.yiiframework.com).

For license information check the [LICENSE](LICENSE.md)-file.

Documentation is at [docs/guide/README.md](docs/guide/README.md).

[![Latest Stable Version](https://poser.pugx.org/yiiplus/yii2-fis-smarty/v/stable.png)](https://packagist.org/packages/yiiplus/yii2-fis-smarty)
[![Total Downloads](https://poser.pugx.org/yiiplus/yii2-fis-smarty/downloads.png)](https://packagist.org/packages/yiiplus/yii2-fis-smarty)
[![Build Status](https://travis-ci.org/yiiplus/yii2-fis-smarty.svg?branch=master)](https://travis-ci.org/yiiplus/yii2-fis-smarty)


Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
composer require "yiiplus/yii2-fis-smarty:^2.0.0"
```

or add

```json
"yiiplus/yii2-fis-smarty": "^2.0.0"
```

to the require section of your composer.json.

Note that the smarty composer package is distributed using subversion so you may need to install subversion.

Usage
-----

To use this extension, simply add the following code in your application configuration:

```php
return [
    //....
    'components' => [
        'view' => [
            'renderers' => [
                'tpl' => [
                    'class' => 'yiiplus\fis\smarty\ViewRenderer',
                    'configDirs' => ['@app/config/fis'],
                ],
            ],
        ],
    ],
];
```