# RESTing with Symfony


## Setup the Project

Ok, cool - this will be easy!

1. Make sure you have [Composer installed](https://getcomposer.org/).

2. Install the composer dependencies:

```bash
composer install
```

Or you may need to run `php composer.phar install` - depending on *how*
you installed Composer. This will probably ask you some questions
about your database (answer for your system) and other settings
(just hit enter for these).

3. Load up your database

Make sure `app/config/parameters.yml` is correct for your database
credentials. Then:

```bash
php bin/console doctrine:database:create
php bin/console doctrine:schema:update --force
php bin/console doctrine:fixtures:load
```

4. Start up the built-in PHP web server:

```bash
php bin/console server:run
```

Then find the site at http://localhost:8000.

You can login with:

user: weaverryan
pass: foo

Have fun!
