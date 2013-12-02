PG4WP
=====

PostgreSQL for WordPress (PG4WP) gives you the possibility to install and use WordPress with a PostgreSQL database as a backend.

Fork from initial WordPress plugin PG4WP develop by Hawk__ (http://www.hawkix.net/)
http://wordpress.org/plugins/postgresql-for-wordpress/

## Installation

You have to install PG4WP *before* configuring your WordPress installation for things to work properly. 
This is because the database needs to be up and running before any plugin can be loaded.

1.  Place your WordPress files in the right place on your web server.

1.	Unzip the files from PG4WP and put the `pg4wp` directory in your `/wp-content` directory.

1.	Copy the `db.php` from the `pg4wp` directory to `wp-content`
	
	You can modify this file to configure the database driver you wish to use
	Currently you can set `DB_DRIVER` to `pgsql` or `mysql`
	
	You can also activate DEBUG and/or ERROR logs

1.	Point your Web Browser to your WordPress installation and go through the traditional WordPress installation routine.

## Config
If you want to install wp on a different schema than `public`, change the value of `PG4WP_SCHEMA` in your `db.php`