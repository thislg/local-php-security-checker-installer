# local-php-security-checker-installer
Composer integration for local PHP security check using fabpot/local-php-security-checker

Install:

```
composer require thibautselingue/local-php-security-checker-installer
```

Usage:

```
vendor/bin/local-php-security-checker-installer && vendor/bin/php-security-checker
```

Example in composer.json auto-scripts:

```
"scripts": {
    "auto-scripts": {
        "local-php-security-checker-installer && local-php-security-checker": "script"
    }
}
```