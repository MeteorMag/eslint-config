# Verse Eslint Configuration

In an effort to keep the codebase consistent and easy to read, Verse projects should use a shared linting configuration. This repository exposes a shared configuration for the eslint tool. [eslint docs](http://eslint.org/)


## Using the configuration file
Assuming you have followed the getting started instructions on the eslint website and have a basic linting setup, follow the instructions to use the Verse version of the eslint configuration.

* Install verse eslint configuration using npm 
```
$ npm install git://github.com/MeteorMag/eslint-config.git --save-dev
```
* If there are errors you may need to install the peer dependencies listed in the error output. EX: 
```
$ npm install eslint-plugin-babel@^3.0.0 --save-dev
```
* Update your local .eslintrc file to extend the verse configuration.
Example .eslintrc
```
{
	"extends": [
		"./node_modules/verse-eslint-config/.eslintrc"
	],
	"env": {
		"browser": true
	}
}
```
* Run your lint command!