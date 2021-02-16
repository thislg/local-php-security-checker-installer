# local-php-security-checker-installer
Composer integration for local PHP security check using fabpot/local-php-security-checker

## Install:

```
composer require thibautselingue/local-php-security-checker-installer
```

Binary will be downloaded to your project's bin directory (`vendor/bin` by default, see [documentation](https://getcomposer.org/doc/articles/vendor-binaries.md#can-vendor-binaries-be-installed-somewhere-other-than-vendor-bin-)).

## Usage:

```
vendor/bin/local-php-security-checker-installer && vendor/bin/local-php-security-checker
```

Example passing path to Composer binary:
```
COMPOSER_BIN=./composer.phar vendor/bin/local-php-security-checker-installer && vendor/bin/local-php-security-checker
```

Example in `composer.json` to run it after install:

```
"scripts": {
    "post-install-cmd": {
        "local-php-security-checker-installer && local-php-security-checker"
    }
}
```
