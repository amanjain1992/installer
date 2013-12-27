# Application installer


Speedwork composer application installer. Aids in automatic installation of Speedwork applications through Composer.

## Usage

You can use this to install Speedwork applications using composer. The installer will make sure the composer package containing
your application will be installed in the correct location.

This is an example of an application composer.json file:

````
{
  "name": "speedwork/demo-application",
    "type": "speedwork-component",
    "description": "Speedwork demo application",
    "keywords": ["framework"],
    "license": "MIT",
	"authors": [
		{
			"name": "sankar",
			"email": "sankar.suda@gmail.com"
		}
	],
	"require": {
		"php": ">=5.4",
		"speedwork/app-installer": "dev-master"
	},
    "minimum-stability": "dev"
}
````

Make sure you use the type "speed-***", and require the installer.

Once this is done, just require your application in your projects main composer.json file
(in the root of your Speedwork installation) and run a composer update to have it installed.
