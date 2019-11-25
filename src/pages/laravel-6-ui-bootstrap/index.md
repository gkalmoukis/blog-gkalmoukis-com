---
title: Laravel 6.0 with Bootstrap 4
date: "2019-11-25T22:40:32.169Z"
language: en
translations:
---
## Create project
First, create a new project using Laravel CLI with the command
```bash
$ laravel new bootstrap-app
```
or by using the composer 
```bash
$ composer create-project --prefer-dist laravel/laravel bootstrap-app
```
in the source, go into the project directory and open it using an editor, i use vscode so
```bash
$ cd bootstrap-app && code .
```
check the files `/resources/js/bootstrap.js` and `/resources/js/app.js`, as you can see apart from lodash and axios there is nothing configured and event app.js file has nothing like vue , react components or anything. And your `devDependencies` should be like 
```json
"devDependencies": {
        "axios": "^0.19",
        "cross-env": "^5.1",
        "laravel-mix": "^4.0.7",
        "lodash": "^4.17.13",
        "resolve-url-loader": "^2.3.1",
        "sass": "^1.15.2",
        "sass-loader": "^7.1.0"
    }
```



## Install Laravel UI Package

Install the first-party package [Laravel Ui](https://github.com/laravel/ui) by executing the command
```bash
$ composer require laravel/ui
```

> You can always use the help option
> ```bash
> $ php artisan ui --help 
> ```
> for more info about usage, arguments and options.
## Install bootstrap 
Laravel does not a specific JavaScript or CSS pre-processor, it does provide a basic starting point using Bootstrap ,Vue or React. To install bootstrap execute 
```bash
$ php artisan ui bootstrap
```

After executing the above command you can check again the files  `/resources/js/bootstrap.js` and `/resources/js/app.js` and the new `_variables.scss` file that created under the `resources/sass/` directory. Also, your `devDependencies` now should be like this.
```json
 "devDependencies": {
        "axios": "^0.19",
        "bootstrap": "^4.0.0",
        "cross-env": "^5.1",
        "jquery": "^3.2",
        "laravel-mix": "^4.0.7",
        "lodash": "^4.17.13",
        "popper.js": "^1.12",
        "resolve-url-loader": "^2.3.1",
        "sass": "^1.15.2",
        "sass-loader": "^7.1.0"
    }
```
These changes are the basic scaffolding for a bootstrap project.

## Install dependencies
Install the required npm dependencies and compile bootstrap scaffolding using 
```bash
$ npm install && npm run dev
```