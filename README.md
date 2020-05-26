# Laravel Paysera
Package that helps to use Paysera API in laravel application.

## Installation
First require package with composer:
```sh
$ composer require dedo/laravel-paysera
```
Then add service provider to config/app.php:
```php
'providers' => [
    ...
    Dedo\Paysera\PayseraServiceProvider::class,
],
```
Facede to aliases:
```php
'aliases' => [
    ...
    'Paysera' => Dedo\Paysera\Facades\Paysera::class,
],
```
And last is to publish config, migrations and view:
```sh
$ php artisan vendor:publish --provider="Dedo\Paysera\PayseraServiceProvider"
```
