# QA test application

Welcome to our QA test application. 

Your task is to setup this application so you can test it.

The packages have been added to the repository for your convenience. We have also added an `.env` file and exceptionally, the Laravel encryption key as well.

## Instructions
1. Install PHP 7
2. Create PostgreSQL database (Docker container is preferred) following the configuration found the `.env` file. By default, for Postgres, it looks like this:

```
create database forge;
create user forge with password 'forge';
grant all privileges on database forge to forge;
```

If your database has different username and password, update the `DB_USERNAME` and `DB_PASSWORD` of the `.env` file accordingly.

3. Install the basic tables and data with `php artisan migrate:refresh --seed`
4. Start the server in cmd `php artisan serve` and access the application from your favorite browser at http://localhost:8000
5. Update the `.env.testing` DB variables if necessary, and run test suite in cmd: `./vendor/phpunit/phpunit/phpunit`

You'll get something like:

```▶ ./vendor/phpunit/phpunit/phpunit
   PHPUnit 6.5.2 by Sebastian Bergmann and contributors.
   
   ..........     10 / 10 (100%)
   
   Time: 342 ms, Memory: 18.00MB
   
   OK (10 tests, 18 assertions)
```


For any questions, please contact karlo.abapo@zenrooms.com
