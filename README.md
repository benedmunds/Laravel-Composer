#Composer bundle for Laravel

This bundle will cause your Composer packages to load automatically.


##Composer Setup
Install composer inside your project directory  

	$ curl -s http://getcomposer.org/installer | php

Create a composer.json file at the root of your project
  
	{
	    "require": {
	        "php": ">=5.3.0",
	        "doctrine/mongodb": ">=0.0.0"
	    }
	}
  
Install your composer packages
	php composer.phar install  

  

##Bundle Setup
Install the composer bundle  

	$ php artisan bundle:install composer

Include it in application/bundles.php  

	return array(
		'composer' => array('auto' => true),
	);


Bundle created by [Ben Edmunds](http://benedmunds.com).