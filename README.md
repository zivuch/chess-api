## PHP Chess API

API using [PHP Chess](https://github.com/chesslablab/php-chess).

### Documentation

Read the [reference guide](https://www.chesslablab.com/documentation/).

### Installation

Install the Composer packages:

    $ composer install

Create an `.env` file:

    $ cp .env.example .env

The Chess API goes hand in hand with [Chess Data](https://github.com/chesslablab/chess-data) which is a database, data science and machine learning repository.

However, there is an easy quick way to get the API up and running without an SSL certificate for when testing endpoints that don't require a database connection, e.g., `api/download_image` or `api/download_mp4`. In such cases you may want to use [PHP's built-in web server](https://www.php.net/manual/en/features.commandline.webserver.php) as described next.

```
$ cd public
$ php -S localhost:8000
```

### File Permissions Setup

Make sure the `var` directory exists:

```
$ mkdir var
```

And set up the following permissions:

```
$ sudo chown www-data:standard -R var
$ sudo chmod 775 -R var
```

Finally, set up the following permissions for the `storage` directory:

```
$ sudo chown www-data:standard -R storage
$ sudo chmod 775 -R storage
```

### Contributions

See the [contributing guidelines](https://github.com/chesslablab/chess-api/blob/main/CONTRIBUTING.md).

Happy learning and coding! Thank you, and keep it up.
