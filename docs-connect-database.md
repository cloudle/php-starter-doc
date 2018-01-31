Connect DB



======Install MySQL on macOS======

-Enter the following command : $ brew info mysql
-To install MySQL enter : $ brew install mysql

====== Additional configuration======

* Homebrew
	-Install brew services first : $ brew tap homebrew/services

	-Load and start the MySQL service : $ brew services start mysql.
	-Expected output : Successfully started mysql (label: homebrew.mxcl.mysql)

	-Check of the MySQL service has been loaded : $ brew services list 1

	-Verify the installed MySQL instance : $ mysql -V.
	-Expected output : Ver 14.14 Distrib 5.7.15, for osx10.12 (x86_64)

* MySQL
	-Open Terminal and execute the following command to set the root password:
		mysqladmin -u root password 'yourpassword'

*Database Management
	-To manage your databases, I recommend using Sequel Pro, a MySQL management tool designed for macOS. Current version available: 1.1.2

====== Install Sequel Pro======
-Download and install Sequel Pro



====== Config with Toml=====

Install Tool by adding to the require or require section of your project's composer.json configuration file, and running 'composer install':

	
"require": {
        "rooxim/phalcon-toml-ini":"dev-master",

    },
