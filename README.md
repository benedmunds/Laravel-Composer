#Composer bundle for Laravel

This bundle will autoload your Composer packages.


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
  

Now you can use Composer packages and they will be loaded automatically.  
  
See [Packagist.org](http://packagist.org) for Composer packages.  
  
Bundle created by [Ben Edmunds](http://benedmunds.com).