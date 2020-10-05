<h1>PHP Code Quality Tools</h1>

## PHPCodeSniffer

### Installation

```bash
$ composer require --dev "squizlabs/php_codesniffer"
```

Now you can run `vendor/bin/phpcs` to check the code.

[More details](https://github.com/squizlabs/PHP_CodeSniffer)

### Integrate with PHPStorm

The above command configures the PHPStorm inspector automatically, but you can do it manually:

1. Configure path in `File->Settings->Languages->Frameworks->PHP->Quality Tools`
2. Enable it in `File->Settings->Editor->Inspections`

[More details](https://www.jetbrains.com/help/phpstorm/using-php-code-sniffer.html)

## PHPMessDetector

### Installation

```bash
$ composer require --dev "phpmd/phpmd"
```

Now you can run `vendor/bin/phpmd src/ ansi ruleset.xml` to check the code.

[More details](https://phpmd.org/)

### Integrate with PHPStorm

The above command configures the PHPStorm inspector automatically, but you can do it manually:

1. Configure path in `File->Settings->Languages->Frameworks->PHP->Quality Tools`
2. Enable it in `File->Settings->Editor->Inspections`

[More details](https://www.jetbrains.com/help/phpstorm/using-php-mess-detector.html)

## PHPStan

### Installation

[More details](https://github.com/phpstan/phpstan)

```bash
$ composer require --dev "phpstan/phpstan"
$ composer require --dev "phpstan/phpstan-doctrine"
$ composer require --dev "phpstan/phpstan-webmozart-assert"
```

Now you can run `vendor/bin/phpstan analyse -c phpstan.neon -l max src/` to check the code.

### Integrate with PHPStorm

The above command configures the PHPStorm inspector automatically, but you can do it manually:

1. Configure path in `File->Settings->Languages->Frameworks->PHP->Quality Tools`
2. Enable it in `File->Settings->Editor->Inspections`

## Configuration Files

Include the configuration files in the root directory of your project:

PHPCodeSniffer: phpcs.xml

PHPMessDetector: ruleset.xml

PHPStan: phpstan.neon

## Git Validation

Include the pre-push file into `.git/hooks` in your project.

## TODO

### TwigCS
### JSCS
### CSFIXER
