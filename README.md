# A Blade directive to export variables to JavaScript

[![Latest Version on Packagist](https://img.shields.io/packagist/v/spatie/laravel-blade-javascript.svg?style=flat-square)](https://packagist.org/packages/spatie/laravel-blade-javascript)
[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](LICENSE.md)
[![Build Status](https://img.shields.io/travis/spatie/laravel-blade-javascript/master.svg?style=flat-square)](https://travis-ci.org/spatie/laravel-blade-javascript)
[![SensioLabsInsight](https://img.shields.io/sensiolabs/i/07458966-b1a2-4cef-8020-02b03f0dd240.svg?style=flat-square)](https://insight.sensiolabs.com/projects/07458966-b1a2-4cef-8020-02b03f0dd240)
[![Quality Score](https://img.shields.io/scrutinizer/g/spatie/laravel-blade-javascript.svg?style=flat-square)](https://scrutinizer-ci.com/g/spatie/laravel-blade-javascript)
[![Total Downloads](https://img.shields.io/packagist/dt/spatie/laravel-blade-javascript.svg?style=flat-square)](https://packagist.org/packages/spatie/laravel-blade-javascript)

This package contains a Blade directive to expofg values to JavaScript.

Here's an example of how it can be used:

```php
@javascript('key', 'value')
```

The rendered view will output:
```html
<script type="text/javascript">window['js'] = window['js'] || {};js['key'] = 'value';</script>
```

You can also use a single argument:
```php
@javascript(['key' => 'value])
```

Which will output the same as the first example.

Spatie is a webdesign agency based in Antwerp, Belgium. You'll find an overview of all our open source projects [on our website](https://spatie.be/opensource).

## Installation

You can install the package via composer:

``` bash
composer require spatie/laravel-blade-javascript
```

## Usage

``` php
$skeleton = new Spatie\Skeleton();
echo $skeleton->echoPhrase('Hello, Spatie!');
```

## Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information what has changed recently.

## Testing

``` bash
$ composer test
```

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

## Security

If you discover any security related issues, please email freek@spatie.be instead of using the issue tracker.

## Credits

- [Freek Van der Herten](https://github.com/freekmurze)
- [Sebastian De Deyne](https://github.com/seb)
- [All Contributors](../../contributors)

This repository contains some code from the [laracasts/PHP-Vars-To-Js-Transformer](https://github.com/laracasts/PHP-Vars-To-Js-Transformer) package written by [Jeffrey Way](https://github.com/JeffreyWay).

## About Spatie
Spatie is a webdesign agency based in Antwerp, Belgium. You'll find an overview of all our open source projects [on our website](https://spatie.be/opensource).

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
