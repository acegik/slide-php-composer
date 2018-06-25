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

### `composer search`

* searches for packages by its name, for example:
```bash
composer search monolog
```

--

### `composer init`

* creates a basic `composer.json` file in the current directory:
```bash
composer init
```

--

### `composer require`

* adds required packages to your composer.json and installs them:
```bash
composer require vendor-1/package-x:0.2.* \
        vendor-2/package-y:0.1.*
```

--

### `composer remove`

* removes a package from the current list of installed packages, for example:
```bash
composer remove monolog/monolog
```

--

### `composer info`

* displays detailed information about a package, or lists all packages available:
```bash
composer info
```

--

### `composer install`

* reads the composer.lock file from
  the current directory, processes it, and downloads and installs all the
  libraries and dependencies outlined in that file. If the file does not
  exist it will look for composer.json and do the same:
```bash
composer install
```

--

### `composer update`

* reads the composer.json file from the current directory, processes it, and updates, removes or installs all the dependencies:
```bash
composer update
```
* list the package(s) you want to update to limit the update operation to a few packages as such:
```bash
composer update vendor1/package1 vendor2/*
```

--

### `composer validate`

* validates a given composer.json and composer.lock:
```bash
composer validate [options] [--] [<file>]
```
__Arguments__:
  * file: path to composer.json file (default: "./composer.json")