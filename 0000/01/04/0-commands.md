## Composer's commands

* list all of commands (default command)):
```bash
composer
```
* `help` command:
  * displays common help:
```bash
composer --help
```
  * displays help for a given command:
```bash
composer help init
```

--

## `composer search`

* searches for packages by its name, example:
```bash
composer search monolog
```

--

## `composer init`

* creates a basic `composer.json` file in the current directory:
```bash
composer init
```

--

## `composer require`

* adds required packages to your composer.json and installs them:
```bash
composer require vendor-1/package-x:0.2.* \
        vendor-2/package-y:0.1.*
```

