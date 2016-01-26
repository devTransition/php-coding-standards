PHP Coding Standard
===================

This repository contains settings for [PHP coding style](https://github.com/devTransition/php-coding-standards/blob/master/doc/code-style.md)
for various tools.

Getting code
------------

You can get code style definition using one of the following methods.

* Clone `devtransition/php-coding-standards` repository:

```
$ git clone git://github.com/devtransition/php-coding-standardss.git
```

* Install `composer.phar` distribution:

```
$ curl -sS https://getcomposer.org/installer | php
```

Or if your system doesn't have CURL installed:

```
$ php -r "eval('?>'.file_get_contents('https://getcomposer.org/installer'));"
```

* Set up all dependencies declared in `composer.json`:

```
$ php composer.phar install
```

PHP_Codesniffer
---------------

[PHP_CodeSniffer](https://github.com/squizlabs/PHP_CodeSniffer) coding standard, rule set
and sniff token parsing classes. Overally rules
are based on PSR-2 standard with some minor exceptions and changes. Rules derived from PSR-2 standard and excluded
were implemented as sniff classes.


### Using code style

After CodeSniffer is installed you can launch it with custom code style using the following syntax:

```
$ ./vendor/bin/phpcs --extensions=php --standard=devtransition /home/resurtm/work/YourApp/
```

If you're using PhpStorm you can configure it to use CodeSniffer using Settings → PHP → Code Sniffer.
Yii2 code style can be specified at Inspections → PHP → PHP Code Sniffer validation.

### Useful links

* [Configuration options](http://pear.php.net/manual/en/package.php.php-codesniffer.config-options.php)
* [Manual and guide](http://pear.php.net/manual/en/package.php.php-codesniffer.php)
* [GitHub repository](https://github.com/squizlabs/PHP_CodeSniffer)

PhpStorm
--------

Yii uses PSR-1 and PSR-2 as code style standards. You can choose these via `Settings` → `Code Style` → `PHP` → `Set from...` → `Predefined Style` → `PSR1/PSR2`.

ADDITIONAL NOTES
----------------

Feel free to request additional features, submit bugs and problems.