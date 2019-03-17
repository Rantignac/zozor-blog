Zozor's Blog
============

Symfony 4 course at OpenClassrooms

Requirements
------------

  * PHP 7.1.3 or higher;
  * PDO-SQLite PHP extension enabled;
  * and the [usual Symfony application requirements][1].

Installation
------------

Clone the project to download its contents :

```bash
$ git clone https://github.com/Rantignac/Zozor-blog.git
$ cd zozor-blog/
```
Installing the dependancies: 

```bash
$ composer install
```
Create the database:

```bash
$ php bin/console doctrine:database:create
$ php bin/console doctrine:schema:create
```
Load demo info into database:

```bash
$ php bin/console doctrine:fixtures:load
```

There's no need to configure anything to run the application. Just execute this
command to run the built-in web server and access the application in your
browser at <http://localhost:8000>:

```bash
$ php bin/console server:run
```

Alternatively, you can [configure a fully-featured web server][2] like Nginx
or Apache to run the application.

Tests
-----

Execute this command to run tests:

```bash
$ ./vendor/bin/simple-phpunit
```

[1]: https://symfony.com/doc/current/reference/requirements.html
[2]: https://symfony.com/doc/current/cookbook/configuration/web_server_configuration.html
