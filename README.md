<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

- [Simple, fast routing engine](https://laravel.com/docs/routing).
- [Powerful dependency injection container](https://laravel.com/docs/container).
- Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
- Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
- Database agnostic [schema migrations](https://laravel.com/docs/migrations).
- [Robust background job processing](https://laravel.com/docs/queues).
- [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

## Learning Laravel

Laravel has the most extensive and thorough [documentation](https://laravel.com/docs) and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework.

If you don't feel like reading, [Laracasts](https://laracasts.com) can help. Laracasts contains over 2000 video tutorials on a range of topics including Laravel, modern PHP, unit testing, and JavaScript. Boost your skills by digging into our comprehensive video library.

## Laravel Sponsors

We would like to extend our thanks to the following sponsors for funding Laravel development. If you are interested in becoming a sponsor, please visit the Laravel [Patreon page](https://patreon.com/taylorotwell).

### Premium Partners

- **[Vehikl](https://vehikl.com/)**
- **[Tighten Co.](https://tighten.co)**
- **[Kirschbaum Development Group](https://kirschbaumdevelopment.com)**
- **[64 Robots](https://64robots.com)**
- **[Cubet Techno Labs](https://cubettech.com)**
- **[Cyber-Duck](https://cyber-duck.co.uk)**
- **[Many](https://www.many.co.uk)**
- **[Webdock, Fast VPS Hosting](https://www.webdock.io/en)**
- **[DevSquad](https://devsquad.com)**
- **[Curotec](https://www.curotec.com/services/technologies/laravel/)**
- **[OP.GG](https://op.gg)**
- **[WebReinvent](https://webreinvent.com/?utm_source=laravel&utm_medium=github&utm_campaign=patreon-sponsors)**
- **[Lendio](https://lendio.com)**

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).

## ePetitions
composer create-project laravel/laravel example-app
 
cd example-app
 
php artisan serve
---------------------------------------
////////////---------PHP artisan migrate error in Laravel 8, illuminate\Database\QueryException.----------//////////////
AppServiceProvider.php
Schema::defaultStringLength(191);
/////////////////////////////
-------------------------------------

Laravel Database
------------------------
php artisan make:migration create_posts_table --create=posts
php artisan migrate				// database create lote tar
php artisan migrate:rollback    /// ko lote kae tae database ko rollback pyan lote tar
php artisan migrate:rollback --step=2 // nouk sone ka nay two ku ko rollback lote hmar
php artisan migrate:refresh		// shi tae database akone ko rollback lote pee migrate pyan lote tar
php artisan migrate:fresh		//	drop all table and migrate all
php artisan migrate:reset		// roll back all tables
php artisan migrate:rollback --path=database/migrations/2022_04_10_054826_add_is_active_column_into_table.php  // custom rollback table

php artisan migrate --path=/database/migrations/full_migration_file_name_migration.php

--------------------------------------
php artisan make:model Petition -mfs
php artisan make:controller PetitionController --api --model=Petition
php artisan make:resource PetitionResource
php artisan make:resource PetitionCollection

composer require doctrine/dbal
php artisan make:migration change_category_type --table=petitions
php artisan make:migration change_category_type_in_petitions
php artisan migrate

php artisan db:seed
php artisan db:seed --class=PetitionSeeder

php artisan route:list
---------------------------------
> php artisan make:model Author -mfs
> php artisan make:controller AuthorController --api --model=Author
> php artisan make:resource AuthorResource
> php artisan make:resource AuthorCollection
-----------------------------
php artisan migrate
php artisan db:seed --class=AuthorSeeder
--------------------------------------------

----------------------
Clone And Run Any Laravel Project From GitHub
> composer install
> npm install
> cp .env.example .env
> php artisan key:generate
