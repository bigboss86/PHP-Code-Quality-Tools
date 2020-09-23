<h1>PHP Code Quality Tools</h1>

# Installation

```bash
$ export PATH="$PATH:$HOME/.composer/vendor/bin"
```

## PHP_CodeSniffer (https://github.com/squizlabs/PHP_CodeSniffer)

```bash
$ composer global require "squizlabs/php_codesniffer=*"
```

Now you can run `phpcs` to check the code.

### Integrate with PHPStorm (https://www.jetbrains.com/help/phpstorm/using-php-code-sniffer.html)

Define the local path:

<img src="https://github.com/bigboss86/PHP-Code-Quality-Tools/blob/master/phpcs_1.png" alt="phpcs_1">

and enable it:

<img src="https://github.com/bigboss86/PHP-Code-Quality-Tools/blob/master/phpcs_2.png" alt="phpcs_2">

## PHP Mess Detector (https://github.com/squizlabs/PHP_CodeSniffer)

```bash
$ composer global require phpmd/phpmd
```

Now you can run `phpmd src/ ansi codesize,unusedcode,naming` to check the code.

### Integrate with PHPStorm (https://www.jetbrains.com/help/phpstorm/using-php-mess-detector.html)

Define the local path:

<img src="https://github.com/bigboss86/PHP-Code-Quality-Tools/blob/master/phpmd_1.png" alt="phpmd_1">

and enable it:

<img src="https://github.com/bigboss86/PHP-Code-Quality-Tools/blob/master/phpmd_2.png" alt="phpmd_2">
