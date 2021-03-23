# Laravel
Laravel Codes And Commands


1. Installing Laravel

Via Laravel Installer :-
composer global require "laravel/installer"
laravel new blog
Via Composer Create-Project :-
composer create-project --prefer-dist laravel/laravel blog

2. Composer :

composer install
composer update
composer dump-autoload [--optimize]
composer self-update

3. Local Development Server :

php artisan serve

4. List Artisan commands :

php artisan list
php artisan help
php artisan tinker
php artisan make
php artisan –version
php artisan routes

5.  Key generate :

php artisan key:generate
php artisan make commnd list

6. create a new middleware :
php artisan make:middleware CheckAge

7. create Controller :
php artisan make:controller PhotoController
php artisan make:controller PhotoController --resource (with resource module)

8. create a model :
php artisan make:model User
php artisan make:model User --migration (or -m ) (with migration)

9. migrations :
php artisan make:migration create_users_table
php artisan make:migration create_users_table --create=users
php artisan make:migration add_votes_to_users_table --table=users
php artisan migrate
php artisan migrate:rollback
php artisan migrate:rollback --step=5
php artisan migrate:reset (roll back all migrations)
php artisan migrate:refresh (roll back & migrate)
php artisan migrate:refresh --step=5
php artisan migrate:fresh (drop all tables)

10.  test cases
php artisan make:test UserTest (Feature test cases)
php artisan make:test UserTest --unit (unit test cases)

11. Factory
php artisan make:factory PostFactory
