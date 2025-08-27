

# Laravel Starter (based on Laravel 12.x)
**Laravel Starter** is a Laravel 12.x based simple starter project. Most of the commonly needed features of an application like `Authentication`, `Authorisation`, `Users` and `Role management`, `Application Backend`, `Backup`, `Log viewer` are available here. It is modular, so you may use this project as a base and build your own modules. A module can be used in any `Laravel Starter` based project.
Here Frontend and Backend are completely separated with separate routes, controllers, and themes as well.

***Please let me know your feedback and comments.***

(https://packagist.org/packages/nasirkhan/laravel-starter) [![StyleCI Build](https://github.styleci.io/repos/105638882/shield?style=flat)](https://packagist.org/packages/nasirkhan/laravel-starter) [![License](http://poser.pugx.org/nasirkhan/laravel-starter/license)](https://packagist.org/packages/nasirkhan/laravel-starter) [![PHP Version Require](http://poser.pugx.org/nasirkhan/laravel-starter/require/php)](https://packagist.org/packages/nasirkhan/laravel-starter)


# Reporting a Vulnerability
If you discover any security-related issues, please send an e-mail to Nasir Khan Saikat via nasir8891@gmail.com instead of using the issue tracker.

# Appplication Demo
Check the following demo project. It is just a straight installation of the project without any modification.

Demo URL: https://laravel.nasirkhn.com

You may use the following account credentials to access the application backend.

```
User: super@admin.com
Pass: secret

User: user@user.com
Pass: secret

```

## Installation
If you want to test the application on your local machine with additional demo data you may use the following command.
```php

composer install

```
```php

yarn

```

```php

php artisan migrate

```

```php

php artisan db:seed

```

```php

php artisan laravel-starter:insert-demo-data

```

There are options to truncate the `posts, categories, tags, and comments` tables and insert new demo data.

`--fresh` option will truncate the tables, without this command a new set of data will be inserted.

```php

php artisan laravel-starter:insert-demo-data --fresh

```

# Custom Commands

We have created a number of custom commands for the project. The commands are listed below with a brief about their use of it.

## Create New module

To create a project use the following command, you have to replace the MODULE_NAME with the name of the module.

```php
php artisan module:build MODULE_NAME
```

You may want to use `--force` option to overwrite the existing module. if you use this option, it will replace all the existing files with the default stub files.

```php
php artisan module:build MODULE_NAME --force
```

## Clear All Cache

```bash
composer clear-all
```

this is a shortcut command to clear all cache including config, route, and more

## Code Style Fix

We are now using `Laravel Pint` to make the code style stay as clean and consistent as the Laravel Framework. Use the following command to apply CS-Fix.

```bash
composer pint
```

Along with Laravel Pint, we are using `prettier` to format the blade templates. You can install the `prettier` extension in your favorite editor.
The following command will format the blade templates.

```bash
npm run format
```

or if you are using `yarn` then you can use the following command.

```bash
yarn format
```


## Role - Permissions

Several custom commands are available to add and update `role-permissions`. Please read the [Role - Permission Wiki page](https://github.com/nasirkhan/laravel-starter/wiki/Role-Permission), where you will find the list of commands with examples.


# Features

The `Laravel Starter Admin` comes with several features which are the most common in almost all applications. It is a template project which means it is intended to be built in a way that it can be used for other projects.

It is a modular application, and some modules are installed by default. It will be helpful to use it as a base for future applications.



## Core Features

* User Authentication
* Social Login
  * Google
  * Facebook
  * Github
  * Build in a way adding more is much easier now
* User Profile with Avatar
* Role-Permissions for Users
* Dynamic Menu System
* Language Switcher
* Localization enabled across the project
* Backend Theme
  * Bootstrap 5, CoreUI
  * Fontawesome 6
  * Dark Mode
* Frontend Theme
  * Tailwind
  * Fontawesome 6
  * Dark Mode
* Article Module
  * Posts
  * Categories
  * Tags
  * Comments
  * wysiwyg editor
  * File browser
* Application Settings
* External Libraries
  * Bootstrap 5
  * Fontawesome 6
  * CoreUI
  * Tailwind
  * Datatables
  * Select2
  * Date Time Picker
* Backup (Source, Files, Database as Zip)
* Log Viewer
* Notification
  * Dashboard and details view












