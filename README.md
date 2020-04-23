This is a composer based installer for the [Drutopia distribution](http://www.drupal.org/project/drutopia).

# Prerequisites

1. [Prepare a local server for Drupal](https://www.drupal.org/docs/develop/local-server-setup)
2. [Install Composer](https://getcomposer.org/download/)


## Installation of Drutopia basic

```
composer create-project drutopia/drutopia_template:dev-master --no-interaction DIRECTORY
```

Composer will create a new directory called DIRECTORY (change to whatever presumably lower-case name you would like). Inside you will find the web directory with the entire code base of [Drutopia distribution](http://www.drupal.org/project/drutopia). You should be able to install it like any other Drupal site.

## Updating

Drutopia manages the version of Drupal core, so you should not require the `drupal/core` project. To update to a new version of core, update to the version of Drutopia that includes the new core version. For example:

```
composer require --no-update drutopia/drutopia:~1.0-rc2
composer update
```

## Making and managing custom changes

You will likely want to add the contents of this directory to git version control, including the `composer.lock` file that was created when you ran `composer create-project`.

You can `composer require` any packages such as Drupal modules you wish to add to your site.
