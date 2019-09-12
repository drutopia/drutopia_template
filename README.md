This is a composer based installer for the [Drutopia distribution](http://www.drupal.org/project/drutopia).

# Prerequisites

1. [Prepare a local server for Drupal](https://www.drupal.org/docs/develop/local-server-setup)
2. [Install Composer](https://getcomposer.org/download/)


## Installation of Drutopia basic

```
composer create-project drutopia/drutopia_template:dev-master --keep-vcs --no-interaction DIRECTORY
```

Composer will create a new directory called DIRECTORY (change to whatever presumably lower-case name you would like). Inside you will find the web directory with the entire code base of [Drutopia distribution](http://www.drupal.org/project/drutopia). You should be able to install it like any other Drupal site.
