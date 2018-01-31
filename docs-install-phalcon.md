


INSTALL PHALCON PHP ON MAC


======Requirements======

-Install brew 
	ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

-PHP 5.5.x/5.6.x/7.0.x/7.1.x development resources
	# brew
	brew tap homebrew/homebrew-php
	brew install php55-phalcon
	brew install php56-phalcon
	brew install php70-phalcon
	brew install php71-phalcon

======File structure======

┗ project-name
   ┣ app
   ┇ ┣ controllers
   ┇ ┇ ┣ IndexController.php
   ┇ ┇ ┗ SignupController.php
   ┇ ┣ models
   ┇ ┇ ┗ Users.php
   ┇ ┗ views
   ┣ public.  
   ┇ ┣ css
   ┇ ┣ img
   ┇ ┣ js
   ┇ ┗ index.php
   ┗ composer.json  

======Install Composer======

-Project Setup: To start using Composer in your project, all you need is a composer.json file. This file describes the dependencies of your project and may contain other metadata as well.
-To install the defined dependencies for your project, just run the install command.

	composer install

- After install 

┗ project-name
   ┣ app
   ┇ ┣ config
   ┇ ┇ ┣ config.dev.toml
   ┇ ┇ ┣ config.local.toml
   ┇ ┇ ┣ config.php
   ┇ ┇ ┣ config.toml
   ┇ ┇ ┣ config_tool.php
   ┇ ┇ ┣ routing.toml
   ┇ ┣ controllers
   ┇ ┇ ┣ IndexController.php
   ┇ ┇ ┗ SignupController.php
   ┇ ┣ models
   ┇ ┇ ┗ Users.php
   ┇ ┗ views
   ┣ public.
   ┣ vendor
   ┇ ┣ css
   ┇ ┣ img
   ┇ ┣ js
   ┇ ┗ index.php
   ┣ composer.json 
   ┇ composer.lock
   ┣ composer.phar
  


======Install Phing======

-Install Phing by adding a dependency to ​phing/phing to the require-dev or require section of your project's composer.json configuration file, and running 'composer install':

{
    "require-dev": {
        "phing/phing": "2.*"
    }
}
- Run
	./phing server

==>  start server: http://0.0.0.0:8082

======Postman test======
Enter request url: http://0.0.0.0:8082

----------------END-----------------


Continue -> Connect Database 




