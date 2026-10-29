composer require wareon/rakuten-rms

## Requirements
This package runs inside a Laravel application and uses Laravel's configuration, service provider, facade, and application helpers.
It does not require `encore/laravel-admin`.

## config/app.php  providers  add line:
Wareon\RakutenRms\RakutenRmsServiceProvider::class,

## config/app.php aliases  add line:
'RakutenRms' => Wareon\RakutenRms\Facades\RakutenRms::class,

##publish command
php artisan vendor:publish --provider="Wareon\RakutenRms\RakutenRmsServiceProvider" 

##How to use?
use Wareon\RakutenRms\Facades\RakutenRms;
$msg = RakutenRms::getItem('123456');
