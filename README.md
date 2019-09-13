# QA test

Welcome to our QA test.

Here are some hints for people not familiar with PHP, Laravel, Databases and package management.

You need to start a database server, we recommend to start a docker container.
Then you will need to create a database following the configuration found in `config/database.php`
By default, for Postgres, it looks like this:
```
create database forge;
create user forge with password 'forge';
grant all privileges on database forge to forge;
```

The packages have been added to the repository for your convenience.
We have also added an `.env` file and, exceptionally, the Laravel encryption key as well.


You can now install the basic tables and data with:
```php artisan migrate:refresh --seed```

Please note that you may need to install PHP, Docker and Postgres client for all this.

For any question, please contact jeremy.lamit@zenrooms.com
