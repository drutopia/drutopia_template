This is a composer based installer for the [Drutopia distribution](http://www.drupal.org/project/drutopia).

# Prerequisites

1. [Prepare a local server for Drupal](https://www.drupal.org/docs/develop/local-server-setup)
2. [Install Composer](https://getcomposer.org/download/)


## Installation of Drutopia basic

```
composer create-project drutopia/drutopia_template:dev-master --keep-vcs --no-interaction DIRECTORY
```

Composer will create a new directory called DIRECTORY (change to whatever presumably lower-case name you would like). Inside you will find the web directory with the entire code base of [Drutopia distribution](http://www.drupal.org/project/drutopia). You should be able to install it like any other Drupal site.

## Updating

You can `git pull` to get updates to Drutopia's project template including `composer.lock` files for official releases of Drutopia.

You can then `composer install` to update.

## Making custom changes

If you are extending Drutopia with your own chosen modules or themes, you can delete the `.git` directory and `git init` to start your own version control, or change `gitlab.com:drutopia/drutopia_template.git` as [a separate upstream repository](https://happygitwithr.com/upstream-changes.html) for your project.

You can `composer require` a module without changing any versions.

If you only run `composer update` when Drutopia provides a new release, overall you will very closely track Drutopia stable releases.
