HAML View Renderer for Yii Framework
====================================

*yii-haml* is extension for [Yii Framework](http://www.yiiframework.com/) that brings [HAML](http://wikipedia.org/wiki/Haml) power to your views. 
Based on forks of [phamlp](http://code.google.com/p/phamlp/) project. 


## Installation with Composer

* Add this to your *composer.json* :

```json
"repositories": [
  {
    "type":"composer",
    "url": "http://packages.phundament.com"
    },
    {
      "type": "package",
      "package": {
        "name": "delfit/phamlp",
        "version": "dev-master",
        "source": {
          "type": "git",
          "url": "https://github.com/delfit/phamlp",
          "reference": "master"
        }
      }
    }
],
"require": {
  "delfit/phamlp": "*",
  "delfit/yii-haml": "*"
}
```

* Run `composer update` for your project




## Usage

* Add *component* to your `config/main.php` : 

```php
return array(
	'components' => array(
		'viewRenderer' => array(
			'class' => 'application.vendor.delfit.yii-haml.HamlViewRenderer',
		),
	),
);
```

* Write your views in HAML and name them with _*.haml_ extension




## Documentation

As far as `yii-haml` is just a Composer-powered wrapper around `phamlp`, you should read this docs : 

* [Options](http://code.google.com/p/phamlp/wiki/HamlOptions)
* [Conventions](http://code.google.com/p/phamlp/wiki/HamlConventions)
* [Indentation](http://code.google.com/p/phamlp/wiki/InstallationAndUsage#Indentation)
* [Predefined Filters](http://code.google.com/p/phamlp/wiki/PredefinedFilters)
* [Helpers](http://code.google.com/p/phamlp/wiki/HelperMethods)
* [Enhancements](http://code.google.com/p/phamlp/wiki/HamlEnhancements)
* [Debugging](http://code.google.com/p/phamlp/wiki/DebuggingHaml)




## Tools

There is a plugin for PHP HAML syntax for [Sublime Text 2](http://www.sublimetext.com/2) : [sublimetext-php-haml](https://github.com/xt99/sublimetext-php-haml)
