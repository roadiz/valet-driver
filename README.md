# Laravel Valet driver for Roadiz


Copy `RoadizValetDriver.php` to your `~/.valet/Drivers` folder after having setup *Laravel/Valet*

For Laravel Valet setup, see:
https://laravel.com/docs/5.4/valet

## Requirements

- **Mysql 5.7**: `brew install mysql`
    - Create a database for your website: `mysql -uroot -p`, then type `create database mysite;` and `exit`
    - *Warning:* you must disable `ONLY_FULL_GROUP_BY` mysql mode which is incompatible with Roadiz at the moment. Edit `/usr/local/etc/my.cnf` and add `sql_mode = ''`. Then restart *mysql*: `brew services restart mysql`
- **PHP 7.1** with OpCache, APCU and Intl extensions: `brew install homebrew/php/php71-intl homebrew/php/php71-opcache homebrew/php/php71-apcu`
