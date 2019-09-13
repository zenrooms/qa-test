# QA test

Welcome to our QA test.

Here are some hints for people not familiar with PHP, Laravel, Databases and package management.

/!\ The packages have been added to the repository for your convenience.
    We have also added an `.env` file and, exceptionally, the Laravel encryption key as well.

To begin, start a database server. We recommend a docker container.
Then, create a database following the configuration found the `.env` file.

By default, for Postgres, it looks like this:
```
create database forge;
create user forge with password 'forge';
grant all privileges on database forge to forge;
```

Install the basic tables and data with:
```php artisan migrate:refresh --seed```

Now, start the embedded server with `php artisan serve`. At this point your app is running and you can open it in your web browser.

You can also try to run the test suite with `./vendor/phpunit/phpunit/phpunit`.

You'll get something like:
```▶ ./vendor/phpunit/phpunit/phpunit
   PHPUnit 6.5.2 by Sebastian Bergmann and contributors.
   
   ..........     10 / 10 (100%)
   
   Time: 342 ms, Memory: 18.00MB
   
   OK (10 tests, 18 assertions)
```
Please note that you may need to install PHP, Docker and Postgres clients for all this.

For any question, please contact jeremy.lamit@zenrooms.com
