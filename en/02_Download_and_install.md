[Download the latest wallabag version](http://www.wallabag.org/download) and extract it. Copy all the files on your web server.

## Requirements for your webserver
* [PHP needs to be a minimum version of PHP 5.3.3](http://php.net/manual/en/install.php)
* [SQLite](http://php.net/manual/en/book.sqlite.php) or [MySQL](http://php.net/manual/fr/book.mysql.php) or [PostgreSQL](http://php.net/manual/en/book.pgsql.php)
* [XML for PHP](http://php.net/xml)
* [PCRE](http://php.net/pcre)
* [Data filtering](http://php.net/manual/book.filter.php)
* [Tidy for PHP](http://php.net/tidy)
* [cURL](http://php.net/curl)
* [allow_url_fopen](http://www.php.net/manual/en/filesystem.configuration.php#ini.allow-url-fopen)
* [gettext](http://php.net/manual/en/book.gettext.php)

To be sure that your webserver can run wallabag, you can execute `wallabag_compatibility_test.php` which is located into the `install` folder of wallabag.

## Dependencies installation 
wallabag needs some dependencies. To install them, you have to use `composer`. In the wallabag folder, run these commands:

    curl -s http://getcomposer.org/installer | php
    php composer.phar install

If you can't install `composer` (if you have a shared hosting for example), you can download [vendor.zip](http://wllbg.org/vendor) and unzip it into the wallabag folder. 

## Permissions
The webserver needs write access on `assets`, `cache` and `db` folders. 

## wallabag installation
Access to wallabag with your browser. If your webserver is well configured, you will see an install screen.  

Give your database information (`sqlite`, `mysql` ou `postgresql`) and user information. 

wallabag is now installed. 

## Connection 

On the login screen, type your user information and you are now logged. 