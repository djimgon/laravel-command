# sql удаление пользователей кроме админа
DELETE FROM users WHERE id <> 1;

# создание контроллера в каталоге
php artisan make:controller Admin\\Hostings\\CategoryController

# запуск php кода в консоли
php artisan tinker

# создания моделей, но без их сохранения в базе данных используя tinker
$users = User::factory()->count(3)->make();

# Генерация фабрик
php artisan make:factory PostFactory --model=Post

# автоматическое добавление данных в таблицы Laravel, использование сидоров
php artisan make:seeder UsersTableSeeder

# как запустить Seeder
php artisan db:seed --class=UsersTableSeeder
php artisan db:seed - если указали в DatabaseSeeder модели, которые нужно заполнить

# очистка таблицы
php artisan migrate:refresh

# активация админа через консольную команду
php artisan user:verify mail@mail.ru - запрограммировать свою консольную программу
